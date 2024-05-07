# Comparing `tmp/iext-1.0.0.tar.gz` & `tmp/iext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iext-1.0.0.tar", last modified: Tue Jan  9 21:11:49 2024, max compression
+gzip compressed data, was "iext-1.1.0.tar", last modified: Tue May  7 03:01:51 2024, max compression
```

## Comparing `iext-1.0.0.tar` & `iext-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-01-09 21:11:37.372739 iext-1.0.0/LICENSE
--rw-r--r--   0        0        0     1409 2024-01-09 21:11:37.372739 iext-1.0.0/README.md
--rw-r--r--   0        0        0      940 2024-01-09 21:11:49.528714 iext-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       43 2024-01-09 21:11:37.376739 iext-1.0.0/src/iext/__init__.py
--rw-r--r--   0        0        0     1837 2024-01-09 21:11:37.376739 iext-1.0.0/src/iext/importextension.py
--rw-r--r--   0        0        0        0 2024-01-09 21:11:37.376739 iext-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      436 2024-01-09 21:11:37.376739 iext-1.0.0/tests/test_iext.py
--rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 iext-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 03:01:35.085814 iext-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1409 2024-05-07 03:01:35.085814 iext-1.1.0/README.md
+-rw-r--r--   0        0        0      935 2024-05-07 03:01:51.361935 iext-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-05-07 03:01:35.085814 iext-1.1.0/src/iext/__init__.py
+-rw-r--r--   0        0        0     2659 2024-05-07 03:01:35.085814 iext-1.1.0/src/iext/importextension.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:01:35.085814 iext-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 03:01:35.085814 iext-1.1.0/tests/module_dummy.py
+-rw-r--r--   0        0        0       44 2024-05-07 03:01:35.085814 iext-1.1.0/tests/module_throw_exception.py
+-rw-r--r--   0        0        0     3910 2024-05-07 03:01:35.085814 iext-1.1.0/tests/test_iext.py
+-rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 iext-1.1.0/PKG-INFO
```

### Comparing `iext-1.0.0/LICENSE` & `iext-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iext-1.0.0/README.md` & `iext-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iext-1.0.0/pyproject.toml` & `iext-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iext"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python import extension metaclass."
 authors = [
     { name = "ilikecubesnstuff", email = "25328250+ilikecubesnstuff@users.noreply.github.com" },
 ]
 dependencies = []
 classifiers = [
     "Intended Audience :: Developers",
@@ -27,14 +27,14 @@
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
-package-type = "library"
+distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.4",
     "tox>=4.11.4",
 ]
```

### Comparing `iext-1.0.0/src/iext/importextension.py` & `iext-1.1.0/src/iext/importextension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import textwrap
+import warnings
 
 
 def _unavailable(e):
     """
     Creates a placeholder type that raises the provided exception on instantiation.
     """
 
@@ -14,42 +15,68 @@
 
         def __init__(self):
             raise e
 
     return Unavailable
 
 
+class ImportExtensionError(Exception):
+    """
+    Base class for all exceptions raised by the import extension module.
+    """
+
+    pass
+
+
 class ExtendImportsMeta(type):
     """
     A metaclass that dynamically extends classes with additional imports.
 
     This metaclass allows classes to extend their functionality by providing extra
     imports that might not be present in the environment. It attempts the specified
     imports and injects them into the class's namespace, enabling the class to use them.
     If any import fails, the class becomes unavailable and raises an exception on
     instantiation.
     """
 
-    def __imports__():
-        """
-        This method name must be used to define additional imports.
-        """
-        pass
-
     def __new__(metacls, name, bases, namespace):
         """
         Create a new class with dynamically injected imports.
         """
-        imports = namespace.pop("__imports__", metacls.__imports__)
-        src = inspect.getsource(imports)
-        *_, body = src.partition("\n")
+        if "__imports__" not in namespace:
+            return super().__new__(metacls, name, bases, namespace)
+
+        __imports__ = namespace.pop("__imports__")
+
+        src_file = inspect.getsourcefile(__imports__)
+        src_lines, line_number = inspect.getsourcelines(__imports__)
+        src = "".join(src_lines)
+
+        _, _, src = src.partition("\n")
+        line_number += 1
+        src = textwrap.dedent(src)
+
         try:
-            exec(textwrap.dedent(body), {}, namespace)
+            for line in src.split("\n"):
+                exec(line, {}, namespace)
+                line_number += 1
         except ModuleNotFoundError as e:
             return _unavailable(e)
+        except SyntaxError as e:
+            raise ImportExtensionError(
+                f"the __imports__ body must contain no docstrings or multi-line expressions."
+            )
+        except Exception as e:
+            warnings.warn_explicit(
+                f"failed to create {name} due to {e.__class__.__name__}: {e}",
+                UserWarning,
+                src_file,
+                line_number,
+            )
+            return _unavailable(e)
         return super().__new__(metacls, name, bases, namespace)
 
 
 class ExtendImports(metaclass=ExtendImportsMeta):
     """
     A base class that allows extending functionality with additional imports.
```

### Comparing `iext-1.0.0/PKG-INFO` & `iext-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iext
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python import extension metaclass.
 Author-Email: ilikecubesnstuff <25328250+ilikecubesnstuff@users.noreply.github.com>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

