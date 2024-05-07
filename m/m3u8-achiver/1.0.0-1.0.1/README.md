# Comparing `tmp/m3u8_achiver-1.0.0.tar.gz` & `tmp/m3u8_achiver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u8_achiver-1.0.0.tar", last modified: Mon May  6 14:15:57 2024, max compression
+gzip compressed data, was "m3u8_achiver-1.0.1.tar", last modified: Tue May  7 01:45:18 2024, max compression
```

## Comparing `m3u8_achiver-1.0.0.tar` & `m3u8_achiver-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 benedictchen   (501) staff       (20)        0 2024-05-06 14:15:57.825759 m3u8_achiver-1.0.0/
--rw-r--r--   0 benedictchen   (501) staff       (20)     1069 2024-05-06 13:43:41.000000 m3u8_achiver-1.0.0/LICENSE.md
--rw-r--r--   0 benedictchen   (501) staff       (20)       14 2024-05-06 14:12:55.000000 m3u8_achiver-1.0.0/MANIFEST.in
--rw-r--r--   0 benedictchen   (501) staff       (20)     1028 2024-05-06 14:15:57.825502 m3u8_achiver-1.0.0/PKG-INFO
--rw-r--r--   0 benedictchen   (501) staff       (20)      307 2024-05-06 13:51:22.000000 m3u8_achiver-1.0.0/README.md
-drwxr-xr-x   0 benedictchen   (501) staff       (20)        0 2024-05-06 14:15:57.825033 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/
--rw-r--r--   0 benedictchen   (501) staff       (20)     1028 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/PKG-INFO
--rw-r--r--   0 benedictchen   (501) staff       (20)      274 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/SOURCES.txt
--rw-r--r--   0 benedictchen   (501) staff       (20)        1 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/dependency_links.txt
--rw-r--r--   0 benedictchen   (501) staff       (20)       56 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/entry_points.txt
--rw-r--r--   0 benedictchen   (501) staff       (20)       61 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/requires.txt
--rw-r--r--   0 benedictchen   (501) staff       (20)        7 2024-05-06 14:15:57.000000 m3u8_achiver-1.0.0/m3u8_achiver.egg-info/top_level.txt
--rw-r--r--   0 benedictchen   (501) staff       (20)     1238 2024-05-06 14:10:15.000000 m3u8_achiver-1.0.0/pyproject.toml
--rw-r--r--   0 benedictchen   (501) staff       (20)       38 2024-05-06 14:15:57.825806 m3u8_achiver-1.0.0/setup.cfg
--rw-r--r--   0 benedictchen   (501) staff       (20)       37 2024-05-06 14:14:09.000000 m3u8_achiver-1.0.0/setup.py
+drwxr-xr-x   0 benedictchen   (501) staff       (20)        0 2024-05-07 01:45:18.554189 m3u8_achiver-1.0.1/
+-rw-r--r--   0 benedictchen   (501) staff       (20)     1069 2024-05-06 13:43:41.000000 m3u8_achiver-1.0.1/LICENSE.md
+-rw-r--r--   0 benedictchen   (501) staff       (20)       14 2024-05-06 14:12:55.000000 m3u8_achiver-1.0.1/MANIFEST.in
+-rw-r--r--   0 benedictchen   (501) staff       (20)     1270 2024-05-07 01:45:18.553986 m3u8_achiver-1.0.1/PKG-INFO
+-rw-r--r--   0 benedictchen   (501) staff       (20)      548 2024-05-07 01:24:32.000000 m3u8_achiver-1.0.1/README.md
+drwxr-xr-x   0 benedictchen   (501) staff       (20)        0 2024-05-07 01:45:18.553544 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/
+-rw-r--r--   0 benedictchen   (501) staff       (20)     1270 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/PKG-INFO
+-rw-r--r--   0 benedictchen   (501) staff       (20)      274 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/SOURCES.txt
+-rw-r--r--   0 benedictchen   (501) staff       (20)        1 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/dependency_links.txt
+-rw-r--r--   0 benedictchen   (501) staff       (20)       56 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/entry_points.txt
+-rw-r--r--   0 benedictchen   (501) staff       (20)       61 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/requires.txt
+-rw-r--r--   0 benedictchen   (501) staff       (20)        7 2024-05-07 01:45:18.000000 m3u8_achiver-1.0.1/m3u8_achiver.egg-info/top_level.txt
+-rw-r--r--   0 benedictchen   (501) staff       (20)     1237 2024-05-07 01:42:54.000000 m3u8_achiver-1.0.1/pyproject.toml
+-rw-r--r--   0 benedictchen   (501) staff       (20)       38 2024-05-07 01:45:18.554232 m3u8_achiver-1.0.1/setup.cfg
+-rw-r--r--   0 benedictchen   (501) staff       (20)       37 2024-05-06 14:14:09.000000 m3u8_achiver-1.0.1/setup.py
```

### Comparing `m3u8_achiver-1.0.0/LICENSE.md` & `m3u8_achiver-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `m3u8_achiver-1.0.0/PKG-INFO` & `m3u8_achiver-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u8-achiver
-Version: 1.0.0
+Version: 1.0.1
 Summary: Download m3u8 files as-is
 Author-email: Benedict Chen <benedict@benedictchen.com>
 Project-URL: Homepage, https://github.com/benedictchen/m3u8-downloader-py
 Keywords: hls,m3u8,video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,19 +17,29 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 M3U8 Python Archiver
 ====================
+
+- Homepage: [Github](https://github.com/benedictchen/m3u8-archiver-py)
+
 Given an m3u8 URL, will download ALL variable bitrate m3u8 children and all associated
 `.ts` files, any encryption keys.
 
 This is open, MIT licensed.  Please feel free to use.
 
 Usage:
 ------
 
 ```
-pip3 install -r requirements.txt 
+pip3 install -r requirements.txt
 python3 download.py <M3U8_URL>
 ```
+
+
+Contributing
+------------
+- Publishing
+  - https://packaging.python.org/en/latest/tutorials/packaging-projects/
+  - https://realpython.com/pypi-publish-python-package/
```

### Comparing `m3u8_achiver-1.0.0/m3u8_achiver.egg-info/PKG-INFO` & `m3u8_achiver-1.0.1/m3u8_achiver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u8-achiver
-Version: 1.0.0
+Version: 1.0.1
 Summary: Download m3u8 files as-is
 Author-email: Benedict Chen <benedict@benedictchen.com>
 Project-URL: Homepage, https://github.com/benedictchen/m3u8-downloader-py
 Keywords: hls,m3u8,video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,19 +17,29 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 M3U8 Python Archiver
 ====================
+
+- Homepage: [Github](https://github.com/benedictchen/m3u8-archiver-py)
+
 Given an m3u8 URL, will download ALL variable bitrate m3u8 children and all associated
 `.ts` files, any encryption keys.
 
 This is open, MIT licensed.  Please feel free to use.
 
 Usage:
 ------
 
 ```
-pip3 install -r requirements.txt 
+pip3 install -r requirements.txt
 python3 download.py <M3U8_URL>
 ```
+
+
+Contributing
+------------
+- Publishing
+  - https://packaging.python.org/en/latest/tutorials/packaging-projects/
+  - https://realpython.com/pypi-publish-python-package/
```

### Comparing `m3u8_achiver-1.0.0/pyproject.toml` & `m3u8_achiver-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "m3u8-achiver"
-version = "1.0.0"
+version = "1.0.1"
 description = "Download m3u8 files as-is"
 readme = "README.md"
 authors = [{ name = "Benedict Chen", email = "benedict@benedictchen.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -44,8 +44,7 @@
 "pyproject.toml" = [
     'current_version = "{version}"',
 ]
 "README.md" = [
     "{version}",
     "{pep440_version}",
 ]
-
```

