# Comparing `tmp/eurmlsdk-0.0.2.tar.gz` & `tmp/eurmlsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.2.tar", last modified: Tue May  7 08:16:50 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.3.tar", last modified: Tue May  7 09:15:08 2024, max compression
```

## Comparing `eurmlsdk-0.0.2.tar` & `eurmlsdk-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.2/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.2/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.2/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.954545 eurmlsdk-0.0.2/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.2/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     4616 2024-05-07 08:16:01.000000 eurmlsdk-0.0.2/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10366 2024-05-07 08:11:05.000000 eurmlsdk-0.0.2/eurmlsdk/base_class.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 08:16:35.000000 eurmlsdk-0.0.2/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.3/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.3/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.3/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.3/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     4616 2024-05-07 08:16:01.000000 eurmlsdk-0.0.3/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)    10376 2024-05-07 08:21:30.000000 eurmlsdk-0.0.3/eurmlsdk/base_class.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 09:15:03.000000 eurmlsdk-0.0.3/setup.py
```

### Comparing `eurmlsdk-0.0.2/eurmlsdk/__main__.py` & `eurmlsdk-0.0.3/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.2/eurmlsdk/base_class.py` & `eurmlsdk-0.0.3/eurmlsdk/base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     and abstract methods that need to be implemented in the sub classes
     """
 
     """
     Below mentioned methods are defined methods that are used in the template methods
     and these methods logic remanins the same
     """
-    def __init__(self, s3_bucket, model_key, model_ouput_path, trained_model, dataset):
+    def __init__(self, s3_bucket, model_key, model_ouput_path, trained_model=None, dataset=None):
         self.s3_bucket = s3_bucket
         self.model_key = model_key
         self.model_output_path = model_ouput_path
         self.trained_model = trained_model
         self.dataset = dataset
         # print("Bucket: %s" % self.s3_bucket)
         # print("Model key: %s" % self.model_key)
```

### Comparing `eurmlsdk-0.0.2/setup.py` & `eurmlsdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko'
```

