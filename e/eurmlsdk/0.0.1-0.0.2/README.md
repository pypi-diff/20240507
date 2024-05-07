# Comparing `tmp/eurmlsdk-0.0.1.tar.gz` & `tmp/eurmlsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.1.tar", last modified: Tue May  7 08:12:20 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.2.tar", last modified: Tue May  7 08:16:50 2024, max compression
```

## Comparing `eurmlsdk-0.0.1.tar` & `eurmlsdk-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:12:20.864549 eurmlsdk-0.0.1/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.1/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.1/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:12:20.864549 eurmlsdk-0.0.1/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.1/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:12:20.864549 eurmlsdk-0.0.1/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.1/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     4604 2024-05-07 08:10:40.000000 eurmlsdk-0.0.1/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10366 2024-05-07 08:11:05.000000 eurmlsdk-0.0.1/eurmlsdk/base_class.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:12:20.864549 eurmlsdk-0.0.1/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       46 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 08:12:20.000000 eurmlsdk-0.0.1/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 08:12:20.864549 eurmlsdk-0.0.1/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      689 2024-05-07 07:43:31.000000 eurmlsdk-0.0.1/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.2/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.954545 eurmlsdk-0.0.2/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.2/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     4616 2024-05-07 08:16:01.000000 eurmlsdk-0.0.2/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)    10366 2024-05-07 08:11:05.000000 eurmlsdk-0.0.2/eurmlsdk/base_class.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 08:16:50.000000 eurmlsdk-0.0.2/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 08:16:50.964545 eurmlsdk-0.0.2/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 08:16:35.000000 eurmlsdk-0.0.2/setup.py
```

### Comparing `eurmlsdk-0.0.1/eurmlsdk/__main__.py` & `eurmlsdk-0.0.2/eurmlsdk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     model_key = os.getenv("MLSDK_S3_MODEL_KEY")
     model_ouput_path = os.getenv("MLSDK_MODEL_OUTPUT_PATH")
     # print("Bucket: %s" % s3_bucket)
     # print("Model key: %s" % model_key)
     
     if len(argv) == 1:
         print("Model Zoo SDK")
-        print("Package name: mlsdk")
+        print("Package name: eurmlsdk")
         print("Version: 0.0.1")
-        print("Run 'mlsdk help' or mlsdk --h to find the list of commands.")
+        print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
         exit(1)
 
     command = argv[1]
     if command == "help" or command == "--h":
         list_commands()
         exit(1)
     elif command == "get":
@@ -86,15 +86,15 @@
                                                                                                                                              
             modelBase.compareMetrics(unQuantizedModel , quantizedModel)
             exit(1)
     
     elif command == "deploy":
         if len(argv) < 6:
             print("Missing required arguments")
-            print("Usage: mlsdk deploy <local path> <hostname> <username> <password>")
+            print("Usage: eurmlsdk deploy <local path> <hostname> <username> <password>")
         else:
             localPath = argv[2]
             remotePath = "/home/embeduradmin/" + localPath.split("/")[-1]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
             modelBase = ModelBase(s3_bucket, model_key, model_ouput_path)
```

### Comparing `eurmlsdk-0.0.1/eurmlsdk/base_class.py` & `eurmlsdk-0.0.2/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.1/setup.py` & `eurmlsdk-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
-            "mlsdk = mlsdk.__main__:main"
+            "eurmlsdk = eurmlsdk.__main__:main"
         ]
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

