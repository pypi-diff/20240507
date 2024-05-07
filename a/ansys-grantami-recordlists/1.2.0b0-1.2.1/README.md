# Comparing `tmp/ansys_grantami_recordlists-1.2.0b0.tar.gz` & `tmp/ansys_grantami_recordlists-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_grantami_recordlists-1.2.0b0.tar", max compression
+gzip compressed data, was "ansys_grantami_recordlists-1.2.1.tar", max compression
```

## Comparing `ansys_grantami_recordlists-1.2.0b0.tar` & `ansys_grantami_recordlists-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      629 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/AUTHORS
--rw-r--r--   0        0        0     1089 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/LICENSE
--rw-r--r--   0        0        0     3897 2024-04-22 16:38:11.243311 ansys_grantami_recordlists-1.2.0b0/README.rst
--rw-r--r--   0        0        0     2416 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/pyproject.toml
--rw-r--r--   0        0        0     1746 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/__init__.py
--rw-r--r--   0        0        0    32212 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_connection.py
--rw-r--r--   0        0        0     1268 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_logger.py
--rw-r--r--   0        0        0    28762 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_models.py
--rw-r--r--   0        0        0        0 2024-04-22 16:38:11.247310 ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/py.typed
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0      629 2024-05-07 12:49:10.473659 ansys_grantami_recordlists-1.2.1/AUTHORS
+-rw-r--r--   0        0        0     1089 2024-05-07 12:49:10.473659 ansys_grantami_recordlists-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3897 2024-05-07 12:49:10.473659 ansys_grantami_recordlists-1.2.1/README.rst
+-rw-r--r--   0        0        0     2425 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1746 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/__init__.py
+-rw-r--r--   0        0        0    32212 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_connection.py
+-rw-r--r--   0        0        0     1268 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_logger.py
+-rw-r--r--   0        0        0    28762 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_models.py
+-rw-r--r--   0        0        0        0 2024-05-07 12:49:10.477659 ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/py.typed
+-rw-r--r--   0        0        0     4985 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.2.1/PKG-INFO
```

### Comparing `ansys_grantami_recordlists-1.2.0b0/AUTHORS` & `ansys_grantami_recordlists-1.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/LICENSE` & `ansys_grantami_recordlists-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/README.rst` & `ansys_grantami_recordlists-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/pyproject.toml` & `ansys_grantami_recordlists-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-grantami-recordlists"
-version = "1.2.0b0"
+version = "1.2.1"
 description = "A python wrapper for the Granta MI RecordLists API"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/grantami-recordlists"
 documentation = "https://recordlists.grantami.docs.pyansys.com"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -26,15 +26,15 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 ansys-openapi-common = "^2.0.0"
-ansys-grantami-serverapi-openapi = "3.0.0b0"
+ansys-grantami-serverapi-openapi = "3.0.0"
 requests = "^2.26"
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/__init__.py` & `ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_connection.py` & `ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_connection.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_logger.py` & `ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/src/ansys/grantami/recordlists/_models.py` & `ansys_grantami_recordlists-1.2.1/src/ansys/grantami/recordlists/_models.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.2.0b0/PKG-INFO` & `ansys_grantami_recordlists-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ansys-grantami-recordlists
-Version: 1.2.0b0
+Version: 1.2.1
 Summary: A python wrapper for the Granta MI RecordLists API
 Home-page: https://github.com/ansys/grantami-recordlists
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ansys-grantami-serverapi-openapi (==3.0.0b0)
+Requires-Dist: ansys-grantami-serverapi-openapi (==3.0.0)
 Requires-Dist: ansys-openapi-common (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Project-URL: Documentation, https://recordlists.grantami.docs.pyansys.com
 Project-URL: Repository, https://github.com/ansys/grantami-recordlists
 Description-Content-Type: text/x-rst
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black| |pre-commit-ci|
```

