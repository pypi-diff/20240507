# Comparing `tmp/pisahkan_ktp-0.0.2.tar.gz` & `tmp/pisahkan_ktp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisahkan_ktp-0.0.2.tar", max compression
+gzip compressed data, was "pisahkan_ktp-0.0.3.tar", max compression
```

## Comparing `pisahkan_ktp-0.0.2.tar` & `pisahkan_ktp-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     1996 2024-05-07 06:53:15.180845 pisahkan_ktp-0.0.2/README.md
--rwxr-xr-x   0        0        0      690 2024-05-07 06:59:22.709325 pisahkan_ktp-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.2/src/pisahkan_ktp/__init__.py
--rwxr-xr-x   0        0        0    10785 2024-05-07 06:57:16.481480 pisahkan_ktp-0.0.2/src/pisahkan_ktp/ktp_segmenter.py
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1097 2024-05-07 03:55:25.046040 pisahkan_ktp-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1996 2024-05-07 06:53:15.180845 pisahkan_ktp-0.0.3/README.md
+-rwxr-xr-x   0        0        0      690 2024-05-07 07:03:40.580569 pisahkan_ktp-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-05-07 03:58:19.125178 pisahkan_ktp-0.0.3/src/pisahkan_ktp/__init__.py
+-rwxr-xr-x   0        0        0    10785 2024-05-07 06:57:16.481480 pisahkan_ktp-0.0.3/src/pisahkan_ktp/ktp_segmenter.py
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 pisahkan_ktp-0.0.3/PKG-INFO
```

### Comparing `pisahkan_ktp-0.0.2/LICENSE` & `pisahkan_ktp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.2/README.md` & `pisahkan_ktp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.2/pyproject.toml` & `pisahkan_ktp-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pisahkan-ktp"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Hanif Yuli Abdillah P <hanifabd23@gmail.com>"]
 description = "Python package for detecting entities in text based on a dictionary and fuzzy similarity"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pisahkan_ktp-0.0.2/src/pisahkan_ktp/ktp_segmenter.py` & `pisahkan_ktp-0.0.3/src/pisahkan_ktp/ktp_segmenter.py`

 * *Files identical despite different names*

### Comparing `pisahkan_ktp-0.0.2/PKG-INFO` & `pisahkan_ktp-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisahkan-ktp
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for detecting entities in text based on a dictionary and fuzzy similarity
 Author: Hanif Yuli Abdillah P
 Author-email: hanifabd23@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

