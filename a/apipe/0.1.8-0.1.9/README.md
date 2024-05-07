# Comparing `tmp/apipe-0.1.8.tar.gz` & `tmp/apipe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apipe-0.1.8.tar", max compression
+gzip compressed data, was "apipe-0.1.9.tar", max compression
```

## Comparing `apipe-0.1.8.tar` & `apipe-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-24 10:28:19.017484 apipe-0.1.8/LICENSE
--rw-r--r--   0        0        0     2369 2024-04-24 10:28:19.017484 apipe-0.1.8/README.md
--rw-r--r--   0        0        0      273 2024-04-24 10:28:19.017484 apipe-0.1.8/apipe/__init__.py
--rw-r--r--   0        0        0    15864 2024-04-24 10:28:19.021484 apipe-0.1.8/apipe/_cached.py
--rw-r--r--   0        0        0     5203 2024-04-24 10:28:19.021484 apipe-0.1.8/apipe/_dask.py
--rw-r--r--   0        0        0     2403 2024-04-24 10:28:38.413587 apipe-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 apipe-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 07:39:18.975547 apipe-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2369 2024-05-07 07:39:18.975547 apipe-0.1.9/README.md
+-rw-r--r--   0        0        0      273 2024-05-07 07:39:18.975547 apipe-0.1.9/apipe/__init__.py
+-rw-r--r--   0        0        0    15864 2024-05-07 07:39:18.975547 apipe-0.1.9/apipe/_cached.py
+-rw-r--r--   0        0        0     5203 2024-05-07 07:39:18.975547 apipe-0.1.9/apipe/_dask.py
+-rw-r--r--   0        0        0     2403 2024-05-07 07:39:35.039441 apipe-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 apipe-0.1.9/PKG-INFO
```

### Comparing `apipe-0.1.8/LICENSE` & `apipe-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apipe-0.1.8/README.md` & `apipe-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `apipe-0.1.8/apipe/_cached.py` & `apipe-0.1.9/apipe/_cached.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.8/apipe/_dask.py` & `apipe-0.1.9/apipe/_dask.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.8/pyproject.toml` & `apipe-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apipe"
-version = "0.1.8"
+version = "0.1.9"
 description = "Data pipelines with lazy computation and caching"
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 keywords = ["python", "pipeline", "dask", "pandas"]
 readme = "README.md"
 license = "Apache License, Version 2.0"
 homepage = "https://github.com/mysterious-ben/apipe"
 repository = "https://github.com/mysterious-ben/apipe"
@@ -12,17 +12,17 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.25"
 pandas = {extras = ["pyarrow"], version = "^2.1"}
-dask = {extras = ["delayed"], version = "^2022"}
+dask = {extras = ["delayed"], version = ">=2023"}
 xxhash = "^3.4"
-cloudpickle = "^2.0"
+cloudpickle = ">=2"
 loguru = ">=0.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8"
 ruff = ">=0.4"
 black = "^24.4"
 pylint = "^3.1"
```

### Comparing `apipe-0.1.8/PKG-INFO` & `apipe-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: apipe
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data pipelines with lazy computation and caching
 Home-page: https://github.com/mysterious-ben/apipe
 License: Apache License, Version 2.0
 Keywords: python,pipeline,dask,pandas
 Author: Mysterious Ben
 Author-email: datascience@tuta.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cloudpickle (>=2.0,<3.0)
-Requires-Dist: dask[delayed] (>=2022,<2023)
+Requires-Dist: cloudpickle (>=2)
+Requires-Dist: dask[delayed] (>=2023)
 Requires-Dist: loguru (>=0.5)
 Requires-Dist: numpy (>=1.25,<2.0)
 Requires-Dist: pandas[pyarrow] (>=2.1,<3.0)
 Requires-Dist: xxhash (>=3.4,<4.0)
 Project-URL: Repository, https://github.com/mysterious-ben/apipe
 Description-Content-Type: text/markdown
```

