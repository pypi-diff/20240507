# Comparing `tmp/pyscopedstorage-0.0.1.tar.gz` & `tmp/pyscopedstorage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscopedstorage-0.0.1.tar", max compression
+gzip compressed data, was "pyscopedstorage-0.0.2.tar", max compression
```

## Comparing `pyscopedstorage-0.0.1.tar` & `pyscopedstorage-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.1/LICENSE
--rw-r--r--   0        0        0     3200 2024-04-29 18:22:12.715575 pyscopedstorage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       55 2024-04-13 11:35:51.639971 pyscopedstorage-0.0.1/src/PyScopedStorage/__init__.py
--rw-r--r--   0        0        0      389 2024-04-13 13:30:59.138107 pyscopedstorage-0.0.1/src/PyScopedStorage/android_objects.py
--rw-r--r--   0        0        0     2870 2024-04-29 16:44:18.965900 pyscopedstorage-0.0.1/src/PyScopedStorage/filechooser.py
--rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.1/src/PyScopedStorage/io.py
--rw-r--r--   0        0        0     1821 2024-04-13 16:32:52.260323 pyscopedstorage-0.0.1/src/PyScopedStorage/tools.py
--rw-r--r--   0        0        0     1271 2024-04-13 13:39:51.636118 pyscopedstorage-0.0.1/src/PyScopedStorage/utils.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3200 2024-05-07 15:43:20.841694 pyscopedstorage-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-08 00:56:10.748860 pyscopedstorage-0.0.2/src/PyScopedStorage/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-07 16:10:47.864603 pyscopedstorage-0.0.2/src/PyScopedStorage/android_objects.py
+-rw-r--r--   0        0        0     2870 2024-04-29 16:44:18.965900 pyscopedstorage-0.0.2/src/PyScopedStorage/filechooser.py
+-rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.2/src/PyScopedStorage/io.py
+-rw-r--r--   0        0        0     2617 2024-05-07 23:46:46.622090 pyscopedstorage-0.0.2/src/PyScopedStorage/tools.py
+-rw-r--r--   0        0        0     3436 2024-05-08 01:13:30.867802 pyscopedstorage-0.0.2/src/PyScopedStorage/utils.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.2/PKG-INFO
```

### Comparing `pyscopedstorage-0.0.1/LICENSE` & `pyscopedstorage-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.1/pyproject.toml` & `pyscopedstorage-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyScopedStorage"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library to simplify storage interaction in Android apps."
 # readme = "README.md"  # TODO..
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `pyscopedstorage-0.0.1/src/PyScopedStorage/filechooser.py` & `pyscopedstorage-0.0.2/src/PyScopedStorage/filechooser.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.1/PKG-INFO` & `pyscopedstorage-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScopedStorage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to simplify storage interaction in Android apps.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

