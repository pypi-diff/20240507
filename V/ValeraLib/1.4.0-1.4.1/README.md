# Comparing `tmp/valeralib-1.4.0.tar.gz` & `tmp/valeralib-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valeralib-1.4.0.tar", last modified: Thu Mar 14 01:58:57 2024, max compression
+gzip compressed data, was "valeralib-1.4.1.tar", last modified: Tue May  7 13:06:52 2024, max compression
```

## Comparing `valeralib-1.4.0.tar` & `valeralib-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0      411 2023-08-23 20:42:10.000000 valeralib-1.4.0/README.md
--rwxr-xr-x   0        0        0     6524 2023-10-24 22:19:30.534392 valeralib-1.4.0/ValeraLib/Binance.py
--rwxr-xr-x   0        0        0     3720 2023-08-15 12:26:40.000000 valeralib-1.4.0/ValeraLib/DataScience.py
--rwxr-xr-x   0        0        0     7251 2023-10-27 19:22:08.113453 valeralib-1.4.0/ValeraLib/Valera.py
--rwxr-xr-x   0        0        0      402 2024-03-13 20:16:05.523601 valeralib-1.4.0/ValeraLib/__init__.py
--rw-r--r--   0        0        0      216 2024-03-13 22:50:35.900945 valeralib-1.4.0/ValeraLib/prelude.py
--rwxr-xr-x   0        0        0     7883 2024-03-12 13:13:57.313243 valeralib-1.4.0/ValeraLib/utils/DuckTypes.py
--rwxr-xr-x   0        0        0     6587 2022-03-26 20:22:20.000000 valeralib-1.4.0/ValeraLib/utils/Notification.mp3
--rwxr-xr-x   0        0        0        0 2024-03-12 13:12:13.224838 valeralib-1.4.0/ValeraLib/utils/__init__.py
--rw-r--r--   0        0        0     8688 2024-03-14 01:55:28.089609 valeralib-1.4.0/ValeraLib/utils/rust_types.py
--rw-r--r--   0        0        0     1460 2024-03-14 01:58:57.437003 valeralib-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-03-14 01:58:18.400205 valeralib-1.4.0/tests/rust_types/test_option.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 valeralib-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0      411 2023-08-23 20:42:10.000000 valeralib-1.4.1/README.md
+-rwxr-xr-x   0        0        0     6524 2023-10-24 22:19:30.534392 valeralib-1.4.1/ValeraLib/Binance.py
+-rwxr-xr-x   0        0        0     3720 2023-08-15 12:26:40.000000 valeralib-1.4.1/ValeraLib/DataScience.py
+-rwxr-xr-x   0        0        0     7251 2023-10-27 19:22:08.113453 valeralib-1.4.1/ValeraLib/Valera.py
+-rwxr-xr-x   0        0        0      402 2024-03-13 20:16:05.523601 valeralib-1.4.1/ValeraLib/__init__.py
+-rw-r--r--   0        0        0      216 2024-03-13 22:50:35.900945 valeralib-1.4.1/ValeraLib/prelude.py
+-rwxr-xr-x   0        0        0     7883 2024-03-12 13:13:57.313243 valeralib-1.4.1/ValeraLib/utils/DuckTypes.py
+-rwxr-xr-x   0        0        0     6587 2022-03-26 20:22:20.000000 valeralib-1.4.1/ValeraLib/utils/Notification.mp3
+-rwxr-xr-x   0        0        0        0 2024-03-12 13:12:13.224838 valeralib-1.4.1/ValeraLib/utils/__init__.py
+-rw-r--r--   0        0        0     8688 2024-03-14 02:04:55.644812 valeralib-1.4.1/ValeraLib/utils/rust_types.py
+-rw-r--r--   0        0        0     1460 2024-05-07 13:06:52.456505 valeralib-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-03-14 01:59:46.813834 valeralib-1.4.1/tests/rust_types/test_option.py
+-rw-r--r--   0        0        0     1622 2024-03-14 02:05:09.954856 valeralib-1.4.1/tests/rust_types/test_result.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 valeralib-1.4.1/PKG-INFO
```

### Comparing `valeralib-1.4.0/ValeraLib/Binance.py` & `valeralib-1.4.1/ValeraLib/Binance.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/ValeraLib/DataScience.py` & `valeralib-1.4.1/ValeraLib/DataScience.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/ValeraLib/Valera.py` & `valeralib-1.4.1/ValeraLib/Valera.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/ValeraLib/utils/DuckTypes.py` & `valeralib-1.4.1/ValeraLib/utils/DuckTypes.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/ValeraLib/utils/Notification.mp3` & `valeralib-1.4.1/ValeraLib/utils/Notification.mp3`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/ValeraLib/utils/rust_types.py` & `valeralib-1.4.1/ValeraLib/utils/rust_types.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/pyproject.toml` & `valeralib-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ValeraLib"
-version = "1.4.0"
+version = "1.4.1"
 description = "The library goes brrrrrr"
 keywords = [
     "The greatest package to ever exist",
 ]
 readme = "README.md"
 authors = [
     { name = "Valera", email = "v79166789533@gmail.com" },
```

### Comparing `valeralib-1.4.0/tests/rust_types/test_option.py` & `valeralib-1.4.1/tests/rust_types/test_option.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.0/PKG-INFO` & `valeralib-1.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValeraLib
-Version: 1.4.0
+Version: 1.4.1
 Summary: The library goes brrrrrr
 Keywords: The greatest package to ever exist
 Author-Email: Valera <v79166789533@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

