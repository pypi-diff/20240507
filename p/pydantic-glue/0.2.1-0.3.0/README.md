# Comparing `tmp/pydantic_glue-0.2.1.tar.gz` & `tmp/pydantic_glue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_glue-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_glue-0.3.0.tar", max compression
```

## Comparing `pydantic_glue-0.2.1.tar` & `pydantic_glue-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/LICENSE
--rw-r--r--   0        0        0     2574 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/README.md
--rw-r--r--   0        0        0       65 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/pydantic_glue/__init__.py
--rw-r--r--   0        0        0      771 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/pydantic_glue/cli.py
--rw-r--r--   0        0        0     1556 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/pydantic_glue/handler.py
--rw-r--r--   0        0        0     1591 2024-05-02 08:59:10.062561 pydantic_glue-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pydantic_glue-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2574 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/README.md
+-rw-r--r--   0        0        0       65 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/cli.py
+-rw-r--r--   0        0        0     1694 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/handler.py
+-rw-r--r--   0        0        0     1591 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pydantic_glue-0.3.0/PKG-INFO
```

### Comparing `pydantic_glue-0.2.1/LICENSE` & `pydantic_glue-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.2.1/README.md` & `pydantic_glue-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.2.1/pydantic_glue/cli.py` & `pydantic_glue-0.3.0/pydantic_glue/cli.py`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.2.1/pydantic_glue/handler.py` & `pydantic_glue-0.3.0/pydantic_glue/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
             return handle_map(v)
         return handle_object(v)
 
     if t == "array":
         return handle_array(v)
 
     if t == "string":
+        if v.get("format") == "date-time":
+            return "timestamp"
+        if v.get("format") == "date":
+            return "date"
         return "string"
 
     if t == "boolean":
         return "boolean"
 
     if t == "integer":
         return "int"
```

### Comparing `pydantic_glue-0.2.1/pyproject.toml` & `pydantic_glue-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pydantic-glue"
 keywords = ["pydantic", "glue", "athena", "types", "convert"]
-version = "0.2.1"
+version = "0.3.0"
 description = "Convert pydantic model to aws glue schema for terraform"
 authors = ["Serhii Dimchenko <svdimchenko@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/svdimchenko/pydantic-glue"
 
 [tool.poetry.urls]
```

### Comparing `pydantic_glue-0.2.1/PKG-INFO` & `pydantic_glue-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-glue
-Version: 0.2.1
+Version: 0.3.0
 Summary: Convert pydantic model to aws glue schema for terraform
 Home-page: https://github.com/svdimchenko/pydantic-glue
 License: MIT
 Keywords: pydantic,glue,athena,types,convert
 Author: Serhii Dimchenko
 Author-email: svdimchenko@gmail.com
 Requires-Python: >=3.9,<4.0
```

