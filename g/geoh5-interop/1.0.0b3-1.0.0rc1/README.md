# Comparing `tmp/geoh5_interop-1.0.0b3.tar.gz` & `tmp/geoh5_interop-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5_interop-1.0.0b3.tar", max compression
+gzip compressed data, was "geoh5_interop-1.0.0rc1.tar", max compression
```

## Comparing `geoh5_interop-1.0.0b3.tar` & `geoh5_interop-1.0.0rc1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      712 2024-05-06 21:41:55.411027 geoh5_interop-1.0.0b3/geoh5_interop/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 geoh5_interop-1.0.0b3/LICENSE
--rw-r--r--   0        0        0     2022 2024-05-06 21:41:55.386644 geoh5_interop-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     2348 2024-05-06 20:54:07.468238 geoh5_interop-1.0.0b3/README.rst
--rw-r--r--   0        0        0     3559 1970-01-01 00:00:00.000000 geoh5_interop-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      710 2024-05-07 21:39:19.350815 geoh5_interop-1.0.0rc1/geoh5_interop/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-27 22:59:02.102762 geoh5_interop-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2020 2024-05-07 21:39:19.330814 geoh5_interop-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2348 2024-05-06 20:54:07.468238 geoh5_interop-1.0.0rc1/README.rst
+-rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 geoh5_interop-1.0.0rc1/PKG-INFO
```

### Comparing `geoh5_interop-1.0.0b3/geoh5_interop/__init__.py` & `geoh5_interop-1.0.0rc1/geoh5_interop/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 #                                                                                 '
 #  This file is part of geoh5-interop meta-package.                               '
 #                                                                                 '
 #  geoh5-interop is distributed under the terms and conditions of the MIT License '
 #  (see LICENSE file at the root of this source code package).                    '
 # '''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
-__version__ = "1.0.0-beta.3"
+__version__ = "1.0.0-rc.1"
```

### Comparing `geoh5_interop-1.0.0b3/LICENSE` & `geoh5_interop-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `geoh5_interop-1.0.0b3/pyproject.toml` & `geoh5_interop-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5-interop"
-version = "1.0.0-beta.3"
+version = "1.0.0-rc.1"
 license = "MIT"
 description = "A meta-package that groups together packages for interoperability between GEOH5 and other file formats."
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 homepage = "https://www.mirageoscience.com/mining-industry-software/python-integration/"
 readme = "README.rst"
 keywords = ["geology", "geophysics", "data", "interoperability"]
 classifiers = [
```

### Comparing `geoh5_interop-1.0.0b3/README.rst` & `geoh5_interop-1.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `geoh5_interop-1.0.0b3/PKG-INFO` & `geoh5_interop-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5-interop
-Version: 1.0.0b3
+Version: 1.0.0rc1
 Summary: A meta-package that groups together packages for interoperability between GEOH5 and other file formats.
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.10,<4.0
```

