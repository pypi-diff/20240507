# Comparing `tmp/sz_utils-0.5.tar.gz` & `tmp/sz_utils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sz_utils-0.5.tar", last modified: Tue May  7 02:28:36 2024, max compression
+gzip compressed data, was "sz_utils-0.6.tar", last modified: Tue May  7 02:42:14 2024, max compression
```

## Comparing `sz_utils-0.5.tar` & `sz_utils-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:28:36.524921 sz_utils-0.5/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.5/LICENSE
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:28:36.524921 sz_utils-0.5/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      242 2024-05-07 02:21:27.000000 sz_utils-0.5/README.md
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:28:36.524921 sz_utils-0.5/setup.cfg
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      653 2024-05-07 02:28:30.000000 sz_utils-0.5/setup.py
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:28:36.524921 sz_utils-0.5/sz_utils.egg-info/
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:28:36.000000 sz_utils-0.5/sz_utils.egg-info/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      225 2024-05-07 02:28:36.000000 sz_utils-0.5/sz_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:28:36.000000 sz_utils-0.5/sz_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:28:36.000000 sz_utils-0.5/sz_utils.egg-info/requires.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        8 2024-05-07 02:28:36.000000 sz_utils-0.5/sz_utils.egg-info/top_level.txt
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:28:36.524921 sz_utils-0.5/szutils/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       19 2024-05-07 02:28:23.000000 sz_utils-0.5/szutils/__init__.py
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.5/szutils/sz_utils.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:42:14.309474 sz_utils-0.6/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.6/LICENSE
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:42:14.309474 sz_utils-0.6/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      242 2024-05-07 02:21:27.000000 sz_utils-0.6/README.md
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:42:14.309474 sz_utils-0.6/setup.cfg
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      653 2024-05-07 02:41:18.000000 sz_utils-0.6/setup.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:42:14.309474 sz_utils-0.6/sz1/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       29 2024-05-07 02:41:05.000000 sz_utils-0.6/sz1/__init__.py
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.6/sz1/sz_utils.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:42:14.309474 sz_utils-0.6/sz_utils.egg-info/
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:42:14.000000 sz_utils-0.6/sz_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      217 2024-05-07 02:42:14.000000 sz_utils-0.6/sz_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:42:14.000000 sz_utils-0.6/sz_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:42:14.000000 sz_utils-0.6/sz_utils.egg-info/requires.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        4 2024-05-07 02:42:14.000000 sz_utils-0.6/sz_utils.egg-info/top_level.txt
```

### Comparing `sz_utils-0.5/LICENSE` & `sz_utils-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sz_utils-0.5/PKG-INFO` & `sz_utils-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.5
+Version: 0.6
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sz_utils-0.5/setup.py` & `sz_utils-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='sz-utils',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
     ],
     author='Peng Zhou',
     author_email='zhoupeng23@nuaa.edu.cn',
     description='A simple example library',
```

### Comparing `sz_utils-0.5/sz_utils.egg-info/PKG-INFO` & `sz_utils-0.6/sz_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.5
+Version: 0.6
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

