# Comparing `tmp/pynamodb_encoder-0.1.2.tar.gz` & `tmp/pynamodb_encoder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb_encoder-0.1.2.tar", max compression
+gzip compressed data, was "pynamodb_encoder-0.2.0.tar", max compression
```

## Comparing `pynamodb_encoder-0.1.2.tar` & `pynamodb_encoder-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-03-23 18:10:06.176708 pynamodb_encoder-0.1.2/LICENSE
--rw-r--r--   0        0        0     2797 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/README.md
--rw-r--r--   0        0        0     2546 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/pynamodb_encoder/decoder.py
--rw-r--r--   0        0        0     2024 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/pynamodb_encoder/encoder.py
--rw-r--r--   0        0        0      852 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/pynamodb_encoder/primitive_attribute_decoder.py
--rw-r--r--   0        0        0      737 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/pynamodb_encoder/primitive_attribute_encoder.py
--rw-r--r--   0        0        0     1375 2023-03-23 18:10:06.180708 pynamodb_encoder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 pynamodb_encoder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2797 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/README.md
+-rw-r--r--   0        0        0     2546 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/pynamodb_encoder/decoder.py
+-rw-r--r--   0        0        0     2024 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/pynamodb_encoder/encoder.py
+-rw-r--r--   0        0        0      852 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/pynamodb_encoder/primitive_attribute_decoder.py
+-rw-r--r--   0        0        0      737 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/pynamodb_encoder/primitive_attribute_encoder.py
+-rw-r--r--   0        0        0     1383 2024-05-07 00:00:36.914220 pynamodb_encoder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 pynamodb_encoder-0.2.0/PKG-INFO
```

### Comparing `pynamodb_encoder-0.1.2/LICENSE` & `pynamodb_encoder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/README.md` & `pynamodb_encoder-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/pynamodb_encoder/decoder.py` & `pynamodb_encoder-0.2.0/pynamodb_encoder/decoder.py`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/pynamodb_encoder/encoder.py` & `pynamodb_encoder-0.2.0/pynamodb_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/pynamodb_encoder/primitive_attribute_decoder.py` & `pynamodb_encoder-0.2.0/pynamodb_encoder/primitive_attribute_decoder.py`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/pynamodb_encoder/primitive_attribute_encoder.py` & `pynamodb_encoder-0.2.0/pynamodb_encoder/primitive_attribute_encoder.py`

 * *Files identical despite different names*

### Comparing `pynamodb_encoder-0.1.2/pyproject.toml` & `pynamodb_encoder-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,30 +28,31 @@
 authors = ["Lin Yang <github@linyang.me>"]
 keywords = ["dynamodb", "pynamodb", "json", "encode", "decode"]
 homepage = "https://github.com/lyang/pynamodb-encoder"
 repository = "https://github.com/lyang/pynamodb-encoder"
 license = "MIT"
 include = ["LICENSE"]
 readme = "README.md"
-version = "0.1.2"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pynamodb = "^5.1.0"
+python = "^3.8"
+pynamodb = "^6.0.0"
 
-[tool.poetry.dev-dependencies]
-black = "^23.1"
-coverage = {extras = ["toml"], version = "^7.2"}
+[tool.poetry.group.dev.dependencies]
+black = "^24.3"
 flake8 = "^5.0.4"
 isort = "^5.11.5"
-pyright = "^1.1.300"
-pytest = "^7.2"
-pytest-cov = "^4.0.0"
-typed-ast = {version = "^1.5.4", python = "< 3.8"}
-pre-commit = "^2.21.0"
+pre-commit = ">=2.21,<4.0"
+pyright = "^1.1.360"
+
+[tool.poetry.group.test.dependencies]
+coverage = {extras = ["toml"], version = "^7.2"}
+pytest = ">=7.4,<9.0"
+pytest-cov = ">=4.1,<6.0"
 
 [tool.pytest.ini_options]
 addopts = [
   "--cov-report=html",
   "--cov-report=term",
   "--cov-report=xml",
   "--cov=pynamodb_encoder",
```

### Comparing `pynamodb_encoder-0.1.2/PKG-INFO` & `pynamodb_encoder-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pynamodb-encoder
-Version: 0.1.2
+Version: 0.2.0
 Summary: Helper classes that encode/decode pynamodb models to/from JSON serializable dict
 Home-page: https://github.com/lyang/pynamodb-encoder
 License: MIT
 Keywords: dynamodb,pynamodb,json,encode,decode
 Author: Lin Yang
 Author-email: github@linyang.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pynamodb (>=5.1.0,<6.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pynamodb (>=6.0.0,<7.0.0)
 Project-URL: Repository, https://github.com/lyang/pynamodb-encoder
 Description-Content-Type: text/markdown
 
 # pynamodb-encoder
 ![Build](https://github.com/lyang/pynamodb-encoder/actions/workflows/build.yml/badge.svg) ![CodeQL](https://github.com/lyang/pynamodb-encoder/actions/workflows/codeql-analysis.yml/badge.svg) [![codecov](https://codecov.io/gh/lyang/pynamodb-encoder/branch/main/graph/badge.svg?token=P51YVL86N8)](https://codecov.io/gh/lyang/pynamodb-encoder) [![Maintainability](https://api.codeclimate.com/v1/badges/1e5c3b615dedb2bffb0c/maintainability)](https://codeclimate.com/github/lyang/pynamodb-encoder/maintainability) [![PyPI version](https://badge.fury.io/py/pynamodb-encoder.svg)](https://badge.fury.io/py/pynamodb-encoder)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/pynamodb-encoder.svg)](https://pypi.python.org/pypi/pynamodb-encoder/)
```

