# Comparing `tmp/byuimage-0.1.6.tar.gz` & `tmp/byuimage-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byuimage-0.1.6.tar", max compression
+gzip compressed data, was "byuimage-0.1.7.tar", max compression
```

## Comparing `byuimage-0.1.6.tar` & `byuimage-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5079 2024-05-01 18:25:29.000000 byuimage-0.1.6/byuimage.py
--rw-r--r--   0        0        0     1087 2024-04-30 17:21:43.000000 byuimage-0.1.6/LICENSE
--rw-r--r--   0        0        0      455 2024-05-01 18:40:43.000000 byuimage-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 byuimage-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5079 2024-05-01 18:25:29.000000 byuimage-0.1.7/byuimage.py
+-rw-r--r--   0        0        0     1087 2024-04-30 17:21:43.000000 byuimage-0.1.7/LICENSE
+-rw-r--r--   0        0        0      455 2024-05-07 20:20:42.000000 byuimage-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 byuimage-0.1.7/PKG-INFO
```

### Comparing `byuimage-0.1.6/byuimage.py` & `byuimage-0.1.7/byuimage.py`

 * *Files identical despite different names*

### Comparing `byuimage-0.1.6/LICENSE` & `byuimage-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `byuimage-0.1.6/PKG-INFO` & `byuimage-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byuimage
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple Image processing library, used for teaching people how to program
 License: MIT
 Author: Daniel Zappala
 Author-email: daniel.zappala@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

