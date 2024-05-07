# Comparing `tmp/statsnet_python_sdk-0.0.1.tar.gz` & `tmp/statsnet_python_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsnet_python_sdk-0.0.1.tar", max compression
+gzip compressed data, was "statsnet_python_sdk-0.0.2.tar", max compression
```

## Comparing `statsnet_python_sdk-0.0.1.tar` & `statsnet_python_sdk-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      162 2024-05-07 20:45:27.909886 statsnet_python_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      523 2024-05-07 20:48:39.775221 statsnet_python_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      180 2024-05-07 20:49:08.157727 statsnet_python_sdk-0.0.1/statsnet_python_sdk/__init__.py
--rw-r--r--   0        0        0     3711 2024-05-07 20:49:08.186603 statsnet_python_sdk-0.0.1/statsnet_python_sdk/client.py
--rw-r--r--   0        0        0     1162 2024-05-02 21:22:58.798994 statsnet_python_sdk-0.0.1/statsnet_python_sdk/exceptions.py
--rw-r--r--   0        0        0      869 2024-05-07 20:49:08.162071 statsnet_python_sdk-0.0.1/statsnet_python_sdk/validations.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 statsnet_python_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      162 2024-05-07 20:45:27.909886 statsnet_python_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      523 2024-05-07 20:53:10.573109 statsnet_python_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-05-07 20:53:15.188830 statsnet_python_sdk-0.0.2/statsnet_python_sdk/__init__.py
+-rw-r--r--   0        0        0     3711 2024-05-07 20:49:08.186603 statsnet_python_sdk-0.0.2/statsnet_python_sdk/client.py
+-rw-r--r--   0        0        0     1162 2024-05-02 21:22:58.798994 statsnet_python_sdk-0.0.2/statsnet_python_sdk/exceptions.py
+-rw-r--r--   0        0        0      870 2024-05-07 20:53:02.338913 statsnet_python_sdk-0.0.2/statsnet_python_sdk/validations.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 statsnet_python_sdk-0.0.2/PKG-INFO
```

### Comparing `statsnet_python_sdk-0.0.1/pyproject.toml` & `statsnet_python_sdk-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statsnet-python-sdk"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python SDK for statsnet.co"
 authors = ["statsnet <hi@statsnet.co>"]
 readme = "README.md"
 packages = [
     { include = "statsnet_python_sdk" },
 ]
```

### Comparing `statsnet_python_sdk-0.0.1/statsnet_python_sdk/client.py` & `statsnet_python_sdk-0.0.2/statsnet_python_sdk/client.py`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-0.0.1/statsnet_python_sdk/exceptions.py` & `statsnet_python_sdk-0.0.2/statsnet_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `statsnet_python_sdk-0.0.1/statsnet_python_sdk/validations.py` & `statsnet_python_sdk-0.0.2/statsnet_python_sdk/validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import NoReturn, Optional
 
-from exceptions import InvalidParamsException
+from .exceptions import InvalidParamsException
 
 
 def validate_id(value: int) -> NoReturn:
     if not type(value) is int:
         raise InvalidParamsException("id must be of type int", "id", id)
```

### Comparing `statsnet_python_sdk-0.0.1/PKG-INFO` & `statsnet_python_sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsnet-python-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for statsnet.co
 Author: statsnet
 Author-email: hi@statsnet.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

