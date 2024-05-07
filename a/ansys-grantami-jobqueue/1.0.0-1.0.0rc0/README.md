# Comparing `tmp/ansys_grantami_jobqueue-1.0.0.tar.gz` & `tmp/ansys_grantami_jobqueue-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_grantami_jobqueue-1.0.0.tar", max compression
+gzip compressed data, was "ansys_grantami_jobqueue-1.0.0rc0.tar", max compression
```

## Comparing `ansys_grantami_jobqueue-1.0.0.tar` & `ansys_grantami_jobqueue-1.0.0rc0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      358 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/AUTHORS
--rw-r--r--   0        0        0     1089 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/LICENSE
--rw-r--r--   0        0        0     3209 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/README.rst
--rw-r--r--   0        0        0     3309 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1864 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/__init__.py
--rw-r--r--   0        0        0    20557 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_connection.py
--rw-r--r--   0        0        0     1278 2024-05-07 13:13:13.574248 ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_logger.py
--rw-r--r--   0        0        0    41237 2024-05-07 13:13:13.578248 ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_models.py
--rw-r--r--   0        0        0        0 2024-05-07 13:13:13.578248 ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/py.typed
--rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 ansys_grantami_jobqueue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-05-07 07:46:06.162448 ansys_grantami_jobqueue-1.0.0rc0/AUTHORS
+-rw-r--r--   0        0        0     1089 2024-05-07 07:46:06.162448 ansys_grantami_jobqueue-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     3209 2024-05-07 07:46:06.162448 ansys_grantami_jobqueue-1.0.0rc0/README.rst
+-rw-r--r--   0        0        0     3304 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1864 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/__init__.py
+-rw-r--r--   0        0        0    20557 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_connection.py
+-rw-r--r--   0        0        0     1278 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_logger.py
+-rw-r--r--   0        0        0    41237 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_models.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:46:06.166447 ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/py.typed
+-rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 ansys_grantami_jobqueue-1.0.0rc0/PKG-INFO
```

### Comparing `ansys_grantami_jobqueue-1.0.0/LICENSE` & `ansys_grantami_jobqueue-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/README.rst` & `ansys_grantami_jobqueue-1.0.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/pyproject.toml` & `ansys_grantami_jobqueue-1.0.0rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-grantami-jobqueue"
-version = "1.0.0"
+version = "1.0.0rc0"
 description = "A python wrapper for the Granta MI Job Queue API"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/grantami-jobqueue"
 documentation = "https://jobqueue.grantami.docs.pyansys.com"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/__init__.py` & `ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_connection.py` & `ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_connection.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_logger.py` & `ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/src/ansys/grantami/jobqueue/_models.py` & `ansys_grantami_jobqueue-1.0.0rc0/src/ansys/grantami/jobqueue/_models.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_jobqueue-1.0.0/PKG-INFO` & `ansys_grantami_jobqueue-1.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ansys-grantami-jobqueue
-Version: 1.0.0
+Version: 1.0.0rc0
 Summary: A python wrapper for the Granta MI Job Queue API
 Home-page: https://github.com/ansys/grantami-jobqueue
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

