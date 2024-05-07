# Comparing `tmp/pysigma_backend_opensearch-1.0.1.tar.gz` & `tmp/pysigma_backend_opensearch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_opensearch-1.0.1.tar", max compression
+gzip compressed data, was "pysigma_backend_opensearch-1.0.2.tar", max compression
```

## Comparing `pysigma_backend_opensearch-1.0.1.tar` & `pysigma_backend_opensearch-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7653 2023-08-30 20:39:57.212940 pysigma_backend_opensearch-1.0.1/LICENSE
--rw-r--r--   0        0        0     6098 2023-08-30 20:39:57.212940 pysigma_backend_opensearch-1.0.1/README.md
--rw-r--r--   0        0        0      979 2023-08-30 20:39:57.212940 pysigma_backend_opensearch-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      107 2023-08-30 20:39:57.212940 pysigma_backend_opensearch-1.0.1/sigma/backends/opensearch/__init__.py
--rw-r--r--   0        0        0     4304 2023-08-30 20:39:57.212940 pysigma_backend_opensearch-1.0.1/sigma/backends/opensearch/opensearch.py
--rw-r--r--   0        0        0     6942 1970-01-01 00:00:00.000000 pysigma_backend_opensearch-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7653 2024-05-07 09:15:04.686481 pysigma_backend_opensearch-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6098 2024-05-07 09:15:04.686481 pysigma_backend_opensearch-1.0.2/README.md
+-rw-r--r--   0        0        0      989 2024-05-07 09:15:04.686481 pysigma_backend_opensearch-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-07 09:15:04.686481 pysigma_backend_opensearch-1.0.2/sigma/backends/opensearch/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-07 09:15:04.690481 pysigma_backend_opensearch-1.0.2/sigma/backends/opensearch/opensearch.py
+-rw-r--r--   0        0        0     6993 1970-01-01 00:00:00.000000 pysigma_backend_opensearch-1.0.2/PKG-INFO
```

### Comparing `pysigma_backend_opensearch-1.0.1/LICENSE` & `pysigma_backend_opensearch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_opensearch-1.0.1/README.md` & `pysigma_backend_opensearch-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysigma_backend_opensearch-1.0.1/pyproject.toml` & `pysigma_backend_opensearch-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pySigma-backend-opensearch"
-version = "1.0.1"
+version = "1.0.2"
 description = "pySigma OpenSearch backend"
 readme = "README.md"
 authors = ["Hendrik Baecker <hendrik.baecker@dcso.de>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/SigmaHQ/pySigma-backend-opensearch"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pysigma-backend-elasticsearch = "^1.0.6"
-pysigma = "^0.10.2"
+pysigma = ">=0.10.2, <0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 coverage = "^6.4.1"
 requests = "^2.28.1"
 autopep8 = "^2.0.2"
```

### Comparing `pysigma_backend_opensearch-1.0.1/sigma/backends/opensearch/opensearch.py` & `pysigma_backend_opensearch-1.0.2/sigma/backends/opensearch/opensearch.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_opensearch-1.0.1/PKG-INFO` & `pysigma_backend_opensearch-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pySigma-backend-opensearch
-Version: 1.0.1
+Version: 1.0.2
 Summary: pySigma OpenSearch backend
 Home-page: https://github.com/SigmaHQ/pySigma-backend-opensearch
 License: LGPL-3.0-only
 Author: Hendrik Baecker
 Author-email: hendrik.baecker@dcso.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pysigma (>=0.10.2,<0.11.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pysigma (>=0.10.2,<0.12.0)
 Requires-Dist: pysigma-backend-elasticsearch (>=1.0.6,<2.0.0)
 Project-URL: Repository, https://github.com/SigmaHQ/pySigma-backend-opensearch
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/SigmaHQ/pySigma-backend-opensearch/actions/workflows/test.yml/badge.svg)
 ![Coverage
 Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/andurin/e95ff0904786bd5883f19105b6a3a1ee/raw/SigmaHQ-pySigma-backend-opensearch.json)
```

