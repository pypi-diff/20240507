# Comparing `tmp/io_collection-0.8.0.tar.gz` & `tmp/io_collection-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_collection-0.8.0.tar", max compression
+gzip compressed data, was "io_collection-0.9.0.tar", max compression
```

## Comparing `io_collection-0.8.0.tar` & `io_collection-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1540 2023-07-14 21:37:39.031324 io_collection-0.8.0/LICENSE
--rw-r--r--   0        0        0     2506 2023-07-14 21:37:39.031324 io_collection-0.8.0/README.md
--rw-r--r--   0        0        0     1915 2023-07-14 21:37:39.035325 io_collection-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/__main__.py
--rw-r--r--   0        0        0      389 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/__init__.py
--rw-r--r--   0        0        0      709 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/change_key.py
--rw-r--r--   0        0        0      525 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/check_key.py
--rw-r--r--   0        0        0      726 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/copy_key.py
--rw-r--r--   0        0        0     1365 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/get_keys.py
--rw-r--r--   0        0        0      297 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/make_key.py
--rw-r--r--   0        0        0      461 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/remove_key.py
--rw-r--r--   0        0        0      429 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/__init__.py
--rw-r--r--   0        0        0     1028 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_buffer.py
--rw-r--r--   0        0        0      705 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_dataframe.py
--rw-r--r--   0        0        0      953 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_image.py
--rw-r--r--   0        0        0      223 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_pickle.py
--rw-r--r--   0        0        0      606 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_tar.py
--rw-r--r--   0        0        0      561 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_text.py
--rw-r--r--   0        0        0        0 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/py.typed
--rw-r--r--   0        0        0      209 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/quilt/__init__.py
--rw-r--r--   0        0        0      185 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/quilt/load_quilt_package.py
--rw-r--r--   0        0        0      287 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/quilt/save_quilt_item.py
--rw-r--r--   0        0        0      616 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/__init__.py
--rw-r--r--   0        0        0      745 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_buffer.py
--rw-r--r--   0        0        0      920 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_dataframe.py
--rw-r--r--   0        0        0      889 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_figure.py
--rw-r--r--   0        0        0      514 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_gif.py
--rw-r--r--   0        0        0     1404 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_image.py
--rw-r--r--   0        0        0      590 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_json.py
--rw-r--r--   0        0        0      274 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_pickle.py
--rw-r--r--   0        0        0     1018 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_tar.py
--rw-r--r--   0        0        0      712 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_text.py
--rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 io_collection-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-08-18 23:38:43.565616 io_collection-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2769 2023-08-18 23:38:43.565616 io_collection-0.9.0/README.md
+-rw-r--r--   0        0        0     1915 2023-08-18 23:38:43.569616 io_collection-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/__main__.py
+-rw-r--r--   0        0        0      432 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/__init__.py
+-rw-r--r--   0        0        0      709 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/change_key.py
+-rw-r--r--   0        0        0      525 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/check_key.py
+-rw-r--r--   0        0        0      726 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/copy_key.py
+-rw-r--r--   0        0        0     1365 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/get_keys.py
+-rw-r--r--   0        0        0      297 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/make_key.py
+-rw-r--r--   0        0        0      461 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/keys/remove_key.py
+-rw-r--r--   0        0        0      577 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/__init__.py
+-rw-r--r--   0        0        0     1028 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_buffer.py
+-rw-r--r--   0        0        0      705 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_dataframe.py
+-rw-r--r--   0        0        0      953 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_image.py
+-rw-r--r--   0        0        0      664 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_json.py
+-rw-r--r--   0        0        0      223 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_pickle.py
+-rw-r--r--   0        0        0      606 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_tar.py
+-rw-r--r--   0        0        0      561 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/load/load_text.py
+-rw-r--r--   0        0        0        0 2023-08-18 23:38:43.569616 io_collection-0.9.0/src/io_collection/py.typed
+-rw-r--r--   0        0        0      264 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/quilt/__init__.py
+-rw-r--r--   0        0        0      185 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/quilt/load_quilt_package.py
+-rw-r--r--   0        0        0      287 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/quilt/save_quilt_item.py
+-rw-r--r--   0        0        0      700 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/__init__.py
+-rw-r--r--   0        0        0      745 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_buffer.py
+-rw-r--r--   0        0        0      920 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_dataframe.py
+-rw-r--r--   0        0        0      889 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_figure.py
+-rw-r--r--   0        0        0      514 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_gif.py
+-rw-r--r--   0        0        0     1404 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_image.py
+-rw-r--r--   0        0        0      590 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_json.py
+-rw-r--r--   0        0        0      274 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_pickle.py
+-rw-r--r--   0        0        0     1018 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_tar.py
+-rw-r--r--   0        0        0      712 2023-08-18 23:38:43.573617 io_collection-0.9.0/src/io_collection/save/save_text.py
+-rw-r--r--   0        0        0     3583 1970-01-01 00:00:00.000000 io_collection-0.9.0/PKG-INFO
```

### Comparing `io_collection-0.8.0/LICENSE` & `io_collection-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/README.md` & `io_collection-0.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-[![Build Status](https://github.com/allen-cell-animated/io-collection/workflows/build/badge.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Abuild)
-[![Codecov](https://img.shields.io/codecov/c/gh/allen-cell-animated/io-collection?token=KQTGXCOLLU)](https://codecov.io/gh/allen-cell-animated/io-collection)
-[![Lint Status](https://github.com/allen-cell-animated/io-collection/workflows/lint/badge.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Alint)
-[![Documentation](https://github.com/allen-cell-animated/io-collection/workflows/documentation/badge.svg)](https://allen-cell-animated.github.io/io-collection/)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](https://allen-cell-animated.github.io/io-collection/_badges/build.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Abuild)
+[![Lint Status](https://allen-cell-animated.github.io/io-collection/_badges/lint.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Alint)
+[![Documentation](https://allen-cell-animated.github.io/io-collection/_badges/documentation.svg)](https://allen-cell-animated.github.io/io-collection/)
+[![Coverage](https://allen-cell-animated.github.io/io-collection/_badges/coverage.svg)](https://allen-cell-animated.github.io/io-collection/_coverage/)
+[![Code style](https://allen-cell-animated.github.io/io-collection/_badges/style.svg)](https://github.com/psf/black)
+[![Version](https://allen-cell-animated.github.io/io-collection/_badges/version.svg)](https://pypi.org/project/io-collection/)
+[![License](https://allen-cell-animated.github.io/io-collection/_badges/license.svg)](https://github.com/allen-cell-animated/io-collection/blob/main/LICENSE)
 
 Collection of tasks for I/O.
 Designed to be used both in [Prefect](https://docs.prefect.io/latest/) workflows and as modular, useful pieces of code.
 
 # Installation
 
 The collection can be installed using:
```

### Comparing `io_collection-0.8.0/pyproject.toml` & `io_collection-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "io-collection"
-version = "0.8.0"
+version = "0.9.0"
 description = "Collection of tasks for I/O."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `io_collection-0.8.0/src/io_collection/keys/change_key.py` & `io_collection-0.9.0/src/io_collection/keys/change_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/keys/check_key.py` & `io_collection-0.9.0/src/io_collection/keys/check_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/keys/copy_key.py` & `io_collection-0.9.0/src/io_collection/keys/copy_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/keys/get_keys.py` & `io_collection-0.9.0/src/io_collection/keys/get_keys.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/load/load_buffer.py` & `io_collection-0.9.0/src/io_collection/load/load_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/load/load_dataframe.py` & `io_collection-0.9.0/src/io_collection/load/load_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/load/load_image.py` & `io_collection-0.9.0/src/io_collection/load/load_image.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/load/load_tar.py` & `io_collection-0.9.0/src/io_collection/load/load_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/load/load_text.py` & `io_collection-0.9.0/src/io_collection/load/load_text.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/__init__.py` & `io_collection-0.9.0/src/io_collection/save/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Tasks for saving different object types to local file systems or S3 buckets."""
+
 from prefect import task
 
 from .save_buffer import save_buffer
 from .save_dataframe import save_dataframe
 from .save_figure import save_figure
 from .save_gif import save_gif
 from .save_image import save_image
```

### Comparing `io_collection-0.8.0/src/io_collection/save/save_buffer.py` & `io_collection-0.9.0/src/io_collection/save/save_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_dataframe.py` & `io_collection-0.9.0/src/io_collection/save/save_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_figure.py` & `io_collection-0.9.0/src/io_collection/save/save_figure.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_gif.py` & `io_collection-0.9.0/src/io_collection/save/save_gif.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_image.py` & `io_collection-0.9.0/src/io_collection/save/save_image.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_json.py` & `io_collection-0.9.0/src/io_collection/save/save_json.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_tar.py` & `io_collection-0.9.0/src/io_collection/save/save_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/src/io_collection/save/save_text.py` & `io_collection-0.9.0/src/io_collection/save/save_text.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.8.0/PKG-INFO` & `io_collection-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: io-collection
-Version: 0.8.0
+Version: 0.9.0
 Summary: Collection of tasks for I/O.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -17,19 +17,21 @@
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: prefect (>=2.8.2,<3.0.0)
 Requires-Dist: quilt3 (>=5.0.0,<6.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
 Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/allen-cell-animated/io-collection/workflows/build/badge.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Abuild)
-[![Codecov](https://img.shields.io/codecov/c/gh/allen-cell-animated/io-collection?token=KQTGXCOLLU)](https://codecov.io/gh/allen-cell-animated/io-collection)
-[![Lint Status](https://github.com/allen-cell-animated/io-collection/workflows/lint/badge.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Alint)
-[![Documentation](https://github.com/allen-cell-animated/io-collection/workflows/documentation/badge.svg)](https://allen-cell-animated.github.io/io-collection/)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Build Status](https://allen-cell-animated.github.io/io-collection/_badges/build.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Abuild)
+[![Lint Status](https://allen-cell-animated.github.io/io-collection/_badges/lint.svg)](https://github.com/allen-cell-animated/io-collection/actions?query=workflow%3Alint)
+[![Documentation](https://allen-cell-animated.github.io/io-collection/_badges/documentation.svg)](https://allen-cell-animated.github.io/io-collection/)
+[![Coverage](https://allen-cell-animated.github.io/io-collection/_badges/coverage.svg)](https://allen-cell-animated.github.io/io-collection/_coverage/)
+[![Code style](https://allen-cell-animated.github.io/io-collection/_badges/style.svg)](https://github.com/psf/black)
+[![Version](https://allen-cell-animated.github.io/io-collection/_badges/version.svg)](https://pypi.org/project/io-collection/)
+[![License](https://allen-cell-animated.github.io/io-collection/_badges/license.svg)](https://github.com/allen-cell-animated/io-collection/blob/main/LICENSE)
 
 Collection of tasks for I/O.
 Designed to be used both in [Prefect](https://docs.prefect.io/latest/) workflows and as modular, useful pieces of code.
 
 # Installation
 
 The collection can be installed using:
```

