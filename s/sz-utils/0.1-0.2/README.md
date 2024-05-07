# Comparing `tmp/sz_utils-0.1.tar.gz` & `tmp/sz_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sz_utils-0.1.tar", last modified: Tue May  7 02:02:19 2024, max compression
+gzip compressed data, was "sz_utils-0.2.tar", last modified: Tue May  7 02:09:02 2024, max compression
```

## Comparing `sz_utils-0.1.tar` & `sz_utils-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:02:19.385759 sz_utils-0.1/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.1/LICENSE
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:02:19.385759 sz_utils-0.1/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      232 2024-05-07 01:53:10.000000 sz_utils-0.1/README.md
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:02:19.385759 sz_utils-0.1/setup.cfg
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      588 2024-05-07 02:02:04.000000 sz_utils-0.1/setup.py
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:02:19.385759 sz_utils-0.1/sz/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 01:15:56.000000 sz_utils-0.1/sz/__init__.py
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.1/sz/sz_utils.py
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:02:19.385759 sz_utils-0.1/sz_utils.egg-info/
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:02:19.000000 sz_utils-0.1/sz_utils.egg-info/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      215 2024-05-07 02:02:19.000000 sz_utils-0.1/sz_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:02:19.000000 sz_utils-0.1/sz_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:02:19.000000 sz_utils-0.1/sz_utils.egg-info/requires.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        3 2024-05-07 02:02:19.000000 sz_utils-0.1/sz_utils.egg-info/top_level.txt
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:09:02.108225 sz_utils-0.2/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.2/LICENSE
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:09:02.108225 sz_utils-0.2/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      232 2024-05-07 01:53:10.000000 sz_utils-0.2/README.md
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:09:02.108225 sz_utils-0.2/setup.cfg
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      588 2024-05-07 02:08:57.000000 sz_utils-0.2/setup.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:09:02.108225 sz_utils-0.2/sz/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 01:15:56.000000 sz_utils-0.2/sz/__init__.py
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.2/sz/sz_utils.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:09:02.108225 sz_utils-0.2/sz_utils.egg-info/
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:09:02.000000 sz_utils-0.2/sz_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      215 2024-05-07 02:09:02.000000 sz_utils-0.2/sz_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:09:02.000000 sz_utils-0.2/sz_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:09:02.000000 sz_utils-0.2/sz_utils.egg-info/requires.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        3 2024-05-07 02:09:02.000000 sz_utils-0.2/sz_utils.egg-info/top_level.txt
```

### Comparing `sz_utils-0.1/LICENSE` & `sz_utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sz_utils-0.1/PKG-INFO` & `sz_utils-0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.1
+Version: 0.2
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sz_utils-0.1/setup.py` & `sz_utils-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sz-utils',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         "numpy",
     ],
     author='Peng Zhou',
     author_email='zhoupeng23@nuaa.edu.cn',
     description='A simple example library',
```

### Comparing `sz_utils-0.1/sz_utils.egg-info/PKG-INFO` & `sz_utils-0.2/sz_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.1
+Version: 0.2
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

