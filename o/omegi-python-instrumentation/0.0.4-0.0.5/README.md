# Comparing `tmp/omegi_python_instrumentation-0.0.4.tar.gz` & `tmp/omegi_python_instrumentation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omegi_python_instrumentation-0.0.4.tar", last modified: Tue May  7 07:10:45 2024, max compression
+gzip compressed data, was "omegi_python_instrumentation-0.0.5.tar", last modified: Tue May  7 07:32:23 2024, max compression
```

## Comparing `omegi_python_instrumentation-0.0.4.tar` & `omegi_python_instrumentation-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:10:45.305667 omegi_python_instrumentation-0.0.4/
--rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.4/LICENSE.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:10:45.305457 omegi_python_instrumentation-0.0.4/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.4/README.md
--rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.4/pyproject.toml
--rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-07 07:10:45.305713 omegi_python_instrumentation-0.0.4/setup.cfg
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2167 2024-05-07 07:10:35.000000 omegi_python_instrumentation-0.0.4/setup.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:10:45.303194 omegi_python_instrumentation-0.0.4/src/
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:10:45.304329 omegi_python_instrumentation-0.0.4/src/omegi/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2809 2024-05-06 19:38:23.000000 omegi_python_instrumentation-0.0.4/src/omegi/KafkaSpanExporter.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     1350 2024-05-07 07:10:24.000000 omegi_python_instrumentation-0.0.4/src/omegi/OmegHandler.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2722 2024-05-07 07:10:24.000000 omegi_python_instrumentation-0.0.4/src/omegi/OmegiTracer.py
--rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:14:19.000000 omegi_python_instrumentation-0.0.4/src/omegi/__init__.py
-drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:10:45.305151 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/
--rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:10:45.000000 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 whisenlantern   (501) staff       (20)      427 2024-05-07 07:10:45.000000 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-07 07:10:45.000000 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-07 07:10:45.000000 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/requires.txt
--rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-07 07:10:45.000000 omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:32:23.420271 omegi_python_instrumentation-0.0.5/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       13 2024-05-07 06:22:05.000000 omegi_python_instrumentation-0.0.5/LICENSE.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:32:23.420075 omegi_python_instrumentation-0.0.5/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       44 2024-05-07 06:21:19.000000 omegi_python_instrumentation-0.0.5/README.md
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      103 2024-05-07 06:17:54.000000 omegi_python_instrumentation-0.0.5/pyproject.toml
+-rw-r--r--   0 whisenlantern   (501) staff       (20)       38 2024-05-07 07:32:23.420315 omegi_python_instrumentation-0.0.5/setup.cfg
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2167 2024-05-07 07:32:19.000000 omegi_python_instrumentation-0.0.5/setup.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:32:23.417494 omegi_python_instrumentation-0.0.5/src/
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:32:23.418981 omegi_python_instrumentation-0.0.5/src/omegi/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2809 2024-05-06 19:38:23.000000 omegi_python_instrumentation-0.0.5/src/omegi/KafkaSpanExporter.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     1350 2024-05-07 07:10:24.000000 omegi_python_instrumentation-0.0.5/src/omegi/OmegHandler.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2877 2024-05-07 07:31:46.000000 omegi_python_instrumentation-0.0.5/src/omegi/OmegiTracer.py
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        0 2024-05-07 06:14:19.000000 omegi_python_instrumentation-0.0.5/src/omegi/__init__.py
+drwxr-xr-x   0 whisenlantern   (501) staff       (20)        0 2024-05-07 07:32:23.419792 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/
+-rw-r--r--   0 whisenlantern   (501) staff       (20)     2065 2024-05-07 07:32:23.000000 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      427 2024-05-07 07:32:23.000000 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        1 2024-05-07 07:32:23.000000 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)      840 2024-05-07 07:32:23.000000 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 whisenlantern   (501) staff       (20)        6 2024-05-07 07:32:23.000000 omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/top_level.txt
```

### Comparing `omegi_python_instrumentation-0.0.4/PKG-INFO` & `omegi_python_instrumentation-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.4/setup.py` & `omegi_python_instrumentation-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="omegi-python-instrumentation",
-    version="0.0.4",
+    version="0.0.5",
     author="Omegi",
     author_email="canon1107@naver.com",
     description="Python Instrumentation for Automatic Error Logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TeamOmegi/Instrumentation-Python",
     project_urls={
```

### Comparing `omegi_python_instrumentation-0.0.4/src/omegi/KafkaSpanExporter.py` & `omegi_python_instrumentation-0.0.5/src/omegi/KafkaSpanExporter.py`

 * *Files identical despite different names*

### Comparing `omegi_python_instrumentation-0.0.4/src/omegi/OmegHandler.py` & `omegi_python_instrumentation-0.0.5/src/omegi/OmegHandler.py`

 * *Files identical despite different names*

### Comparing `omegi_python_instrumentation-0.0.4/src/omegi/OmegiTracer.py` & `omegi_python_instrumentation-0.0.5/src/omegi/OmegiTracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,22 +50,27 @@
         args = []
         for i, arg_name in enumerate(raw):
             arg_value = frame.f_locals[arg_name]
             args.append(f"{arg_name} : {arg_value}")
         return args
 
     def __find_project_root__(self):
-        current_path = os.path.abspath(__file__)
-        while True:
-            if os.path.exists(os.path.join(current_path, 'requirements.txt')) or os.path.exists(os.path.join(current_path, 'setup.py')):
-                return current_path
-            parent_path = os.path.dirname(current_path)
-            if parent_path == current_path:
-                raise Exception("Project root not found.")
-            current_path = parent_path
+        try:
+            main_file_path = sys.modules['__main__'].__file__
+            current_path = os.path.dirname(os.path.abspath(main_file_path))
+
+            while True:
+                if os.path.exists(os.path.join(current_path, 'requirements.txt')) or os.path.exists(os.path.join(current_path, 'setup.py')):
+                    return current_path
+                parent_path = os.path.dirname(current_path)
+                if parent_path == current_path:
+                    return current_path
+                current_path = parent_path
+        except:
+            return os.getcwd()
 
     def start_tracing(self):
         sys.setprofile(self.trace_function)
 
     def stop_tracing(self):
         sys.setprofile(None)
```

### Comparing `omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/PKG-INFO` & `omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omegi-python-instrumentation
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Instrumentation for Automatic Error Logging
 Home-page: https://github.com/TeamOmegi/Instrumentation-Python
 Author: Omegi
 Author-email: canon1107@naver.com
 Project-URL: Source Code, https://github.com/TeamOmegi/Instrumentation-Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `omegi_python_instrumentation-0.0.4/src/omegi_python_instrumentation.egg-info/requires.txt` & `omegi_python_instrumentation-0.0.5/src/omegi_python_instrumentation.egg-info/requires.txt`

 * *Files identical despite different names*

