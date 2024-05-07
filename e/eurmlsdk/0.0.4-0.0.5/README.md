# Comparing `tmp/eurmlsdk-0.0.4.tar.gz` & `tmp/eurmlsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.4.tar", last modified: Tue May  7 09:32:44 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.5.tar", last modified: Tue May  7 09:37:39 2024, max compression
```

## Comparing `eurmlsdk-0.0.4.tar` & `eurmlsdk-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.4/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.4/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.4/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.884478 eurmlsdk-0.0.4/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.4/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     4628 2024-05-07 09:18:30.000000 eurmlsdk-0.0.4/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.4/eurmlsdk/base_class.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.884478 eurmlsdk-0.0.4/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 09:32:32.000000 eurmlsdk-0.0.4/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:37:39.974474 eurmlsdk-0.0.5/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.5/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.5/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 09:37:39.974474 eurmlsdk-0.0.5/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.5/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:37:39.974474 eurmlsdk-0.0.5/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.5/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     4628 2024-05-07 09:18:30.000000 eurmlsdk-0.0.5/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.5/eurmlsdk/base_class.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:37:39.974474 eurmlsdk-0.0.5/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       41 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 09:37:39.000000 eurmlsdk-0.0.5/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 09:37:39.974474 eurmlsdk-0.0.5/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      718 2024-05-07 09:37:27.000000 eurmlsdk-0.0.5/setup.py
```

### Comparing `eurmlsdk-0.0.4/eurmlsdk/__main__.py` & `eurmlsdk-0.0.5/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.4/eurmlsdk/base_class.py` & `eurmlsdk-0.0.5/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.4/setup.py` & `eurmlsdk-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
-        'paramiko'
+        'paramiko',
+        'ultralytics'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
             "eurmlsdk = eurmlsdk.__main__:main"
```

