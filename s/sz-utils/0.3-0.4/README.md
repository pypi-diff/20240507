# Comparing `tmp/sz_utils-0.3.tar.gz` & `tmp/sz_utils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sz_utils-0.3.tar", last modified: Tue May  7 02:18:13 2024, max compression
+gzip compressed data, was "sz_utils-0.4.tar", last modified: Tue May  7 02:23:07 2024, max compression
```

## Comparing `sz_utils-0.3.tar` & `sz_utils-0.4.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:18:13.257839 sz_utils-0.3/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.3/LICENSE
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:18:13.257839 sz_utils-0.3/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      232 2024-05-07 01:53:10.000000 sz_utils-0.3/README.md
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:18:13.257839 sz_utils-0.3/setup.cfg
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      653 2024-05-07 02:18:06.000000 sz_utils-0.3/setup.py
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:18:13.257839 sz_utils-0.3/sz/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 01:15:56.000000 sz_utils-0.3/sz/__init__.py
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.3/sz/sz_utils.py
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:18:13.257839 sz_utils-0.3/sz_utils.egg-info/
--rw-r--r--   0 y9000k    (1000) y9000k    (1000)      623 2024-05-07 02:18:13.000000 sz_utils-0.3/sz_utils.egg-info/PKG-INFO
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      235 2024-05-07 02:18:13.000000 sz_utils-0.3/sz_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:18:13.000000 sz_utils-0.3/sz_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:18:13.000000 sz_utils-0.3/sz_utils.egg-info/requires.txt
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       11 2024-05-07 02:18:13.000000 sz_utils-0.3/sz_utils.egg-info/top_level.txt
-drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:18:13.257839 sz_utils-0.3/szutils/
--rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       44 2024-05-07 02:17:57.000000 sz_utils-0.3/szutils/__init__.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:23:07.395913 sz_utils-0.4/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)     1066 2024-05-07 01:04:19.000000 sz_utils-0.4/LICENSE
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:23:07.395913 sz_utils-0.4/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      242 2024-05-07 02:21:27.000000 sz_utils-0.4/README.md
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       38 2024-05-07 02:23:07.395913 sz_utils-0.4/setup.cfg
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      653 2024-05-07 02:23:02.000000 sz_utils-0.4/setup.py
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:23:07.395913 sz_utils-0.4/sz_utils.egg-info/
+-rw-r--r--   0 y9000k    (1000) y9000k    (1000)      633 2024-05-07 02:23:07.000000 sz_utils-0.4/sz_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)      225 2024-05-07 02:23:07.000000 sz_utils-0.4/sz_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        1 2024-05-07 02:23:07.000000 sz_utils-0.4/sz_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        6 2024-05-07 02:23:07.000000 sz_utils-0.4/sz_utils.egg-info/requires.txt
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        8 2024-05-07 02:23:07.000000 sz_utils-0.4/sz_utils.egg-info/top_level.txt
+drwxrwxr-x   0 y9000k    (1000) y9000k    (1000)        0 2024-05-07 02:23:07.395913 sz_utils-0.4/szutils/
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)        3 2024-05-07 02:22:25.000000 sz_utils-0.4/szutils/__init__.py
+-rw-rw-r--   0 y9000k    (1000) y9000k    (1000)       72 2024-05-07 01:15:35.000000 sz_utils-0.4/szutils/sz_utils.py
```

### Comparing `sz_utils-0.3/LICENSE` & `sz_utils-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sz_utils-0.3/PKG-INFO` & `sz_utils-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.3
+Version: 0.4
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 ## PyPi
 
 ```bash
 # 安装打包工具
 pip install twine setuptools wheel
 
 # 构建包
-rm -rf dist build
+rm -rf dist build *egg-info
 python setup.py sdist bdist_wheel
 
 # 上传包 
 # 设置 $HOME/.pypirc  token
 twine upload dist/*
```

### Comparing `sz_utils-0.3/setup.py` & `sz_utils-0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='sz-utils',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
     ],
     author='Peng Zhou',
     author_email='zhoupeng23@nuaa.edu.cn',
     description='A simple example library',
```

### Comparing `sz_utils-0.3/sz_utils.egg-info/PKG-INFO` & `sz_utils-0.4/sz_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sz-utils
-Version: 0.3
+Version: 0.4
 Summary: A simple example library
 Home-page: https://github.com/PeterouZh
 Author: Peng Zhou
 Author-email: zhoupeng23@nuaa.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 ## PyPi
 
 ```bash
 # 安装打包工具
 pip install twine setuptools wheel
 
 # 构建包
-rm -rf dist build
+rm -rf dist build *egg-info
 python setup.py sdist bdist_wheel
 
 # 上传包 
 # 设置 $HOME/.pypirc  token
 twine upload dist/*
```

