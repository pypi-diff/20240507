# Comparing `tmp/pychute-0.0.1.tar.gz` & `tmp/pychute-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychute-0.0.1.tar", last modified: Tue May  7 17:02:28 2024, max compression
+gzip compressed data, was "pychute-0.0.2.tar", last modified: Tue May  7 17:18:29 2024, max compression
```

## Comparing `pychute-0.0.1.tar` & `pychute-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:02:28.118494 pychute-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4259 2024-05-07 17:02:28.116494 pychute-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2390 2024-05-07 13:31:13.000000 pychute-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:02:28.097412 pychute-0.0.1/pychute/
--rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.1/pychute/__init__.py
--rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.1/pychute/config.py
--rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.1/pychute/helpers.py
--rw-rw-rw-   0        0        0     3759 2024-05-07 16:42:55.000000 pychute-0.0.1/pychute/main.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:02:28.113496 pychute-0.0.1/pychute.egg-info/
--rw-rw-rw-   0        0        0     4259 2024-05-07 17:02:28.000000 pychute-0.0.1/pychute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-07 17:02:28.000000 pychute-0.0.1/pychute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:02:28.000000 pychute-0.0.1/pychute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 17:02:28.000000 pychute-0.0.1/pychute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2024-05-07 17:02:15.000000 pychute-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 17:02:28.119493 pychute-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-07 17:02:15.000000 pychute-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:02:28.110506 pychute-0.0.1/tests/
--rw-rw-rw-   0        0        0      937 2024-05-07 16:42:56.000000 pychute-0.0.1/tests/test_functionality.py
--rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.1/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:18:29.164168 pychute-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4336 2024-05-07 17:18:29.162172 pychute-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2024-05-07 13:31:13.000000 pychute-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 17:18:29.143648 pychute-0.0.2/pychute/
+-rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.2/pychute/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.2/pychute/config.py
+-rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.2/pychute/helpers.py
+-rw-rw-rw-   0        0        0     3759 2024-05-07 16:42:55.000000 pychute-0.0.2/pychute/main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:18:29.160163 pychute-0.0.2/pychute.egg-info/
+-rw-rw-rw-   0        0        0     4336 2024-05-07 17:18:29.000000 pychute-0.0.2/pychute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-07 17:18:29.000000 pychute-0.0.2/pychute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:18:29.000000 pychute-0.0.2/pychute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-07 17:18:29.000000 pychute-0.0.2/pychute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 17:18:29.000000 pychute-0.0.2/pychute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      786 2024-05-07 17:17:57.000000 pychute-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:18:29.164168 pychute-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      643 2024-05-07 17:17:57.000000 pychute-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:18:29.156659 pychute-0.0.2/tests/
+-rw-rw-rw-   0        0        0      937 2024-05-07 16:42:56.000000 pychute-0.0.2/tests/test_functionality.py
+-rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.2/tests/test_helpers.py
```

### Comparing `pychute-0.0.1/LICENSE` & `pychute-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pychute-0.0.1/PKG-INFO` & `pychute-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -30,14 +30,17 @@
 Project-URL: Issues, https://github.com/paichiwo/pychute/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: selenium
+Requires-Dist: beautifulsoup4
 
 # pychute
 
 
 ### A library that helps download videos from BitChute website
 ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/paichiwo/pychute/total)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/t/paichiwo/pychute)
```

### Comparing `pychute-0.0.1/README.md` & `pychute-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pychute-0.0.1/pychute/helpers.py` & `pychute-0.0.2/pychute/helpers.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.1/pychute/main.py` & `pychute-0.0.2/pychute/main.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.1/pychute.egg-info/PKG-INFO` & `pychute-0.0.2/pychute.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
@@ -30,14 +30,17 @@
 Project-URL: Issues, https://github.com/paichiwo/pychute/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: selenium
+Requires-Dist: beautifulsoup4
 
 # pychute
 
 
 ### A library that helps download videos from BitChute website
 ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/paichiwo/pychute/total)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/t/paichiwo/pychute)
```

### Comparing `pychute-0.0.1/pyproject.toml` & `pychute-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [project]
 name = "pychute"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lukasz Zerucha", email="lzerucha@gmail.com" },
 ]
 description = "A library that helps downloading videos from bitchute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license={file="LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "lxml",
+    "selenium",
+    "beautifulsoup4"
+]
 
 [project.urls]
 Homepage = "https://github.com/paichiwo/pychute"
 Issues = "https://github.com/paichiwo/pychute/issues"
 
 [build-system]
 requires = [
```

### Comparing `pychute-0.0.1/setup.py` & `pychute-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 setup(
     name='pychute',
-    version='0.0.1',
+    version='0.0.2',
     packages=setuptools.find_packages(),
     url='http://github.com/paichiwo/pychute',
     author='Lukasz Zerucha',
     author_email='lzerucha@gmail.com',
     description='A library that helps downloading videos from bitchute.com',
     long_description=long_desc,
     long_description_content_type='text/markdown',
```

### Comparing `pychute-0.0.1/tests/test_functionality.py` & `pychute-0.0.2/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.1/tests/test_helpers.py` & `pychute-0.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

