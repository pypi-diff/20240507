# Comparing `tmp/eurmlsdk-0.0.6.tar.gz` & `tmp/eurmlsdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.6.tar", last modified: Tue May  7 11:10:41 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.7.tar", last modified: Tue May  7 11:16:21 2024, max compression
```

## Comparing `eurmlsdk-0.0.6.tar` & `eurmlsdk-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:10:41.064392 eurmlsdk-0.0.6/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.6/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.6/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 11:10:41.064392 eurmlsdk-0.0.6/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.6/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:10:41.054392 eurmlsdk-0.0.6/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       31 2024-05-07 10:58:56.000000 eurmlsdk-0.0.6/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     3155 2024-05-07 11:03:15.000000 eurmlsdk-0.0.6/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.6/eurmlsdk/base_class.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     3321 2024-05-07 11:02:43.000000 eurmlsdk-0.0.6/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:10:41.064392 eurmlsdk-0.0.6/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      321 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       41 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 11:10:40.000000 eurmlsdk-0.0.6/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 11:10:41.064392 eurmlsdk-0.0.6/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      718 2024-05-07 11:10:35.000000 eurmlsdk-0.0.6/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:16:21.894387 eurmlsdk-0.0.7/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.7/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.7/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 11:16:21.894387 eurmlsdk-0.0.7/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.7/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:16:21.894387 eurmlsdk-0.0.7/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       31 2024-05-07 10:58:56.000000 eurmlsdk-0.0.7/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     3155 2024-05-07 11:03:15.000000 eurmlsdk-0.0.7/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.7/eurmlsdk/base_class.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     3315 2024-05-07 11:15:44.000000 eurmlsdk-0.0.7/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 11:16:21.894387 eurmlsdk-0.0.7/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      460 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      321 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       41 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 11:16:21.000000 eurmlsdk-0.0.7/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 11:16:21.894387 eurmlsdk-0.0.7/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      718 2024-05-07 11:16:09.000000 eurmlsdk-0.0.7/setup.py
```

### Comparing `eurmlsdk-0.0.6/eurmlsdk/__main__.py` & `eurmlsdk-0.0.7/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.6/eurmlsdk/base_class.py` & `eurmlsdk-0.0.7/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.6/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.7/eurmlsdk/eur_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         sftp.close()
         # Close SSH connection
         ssh_client.close()
 
      def execute_script(self, hostname, username, password , script_path , modelFile):
         ssh_client = self.connect_ssh_client(hostname, username, password)
         
-        stdin, stdout, stderr = ssh_client.exec_command('python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {} {}'.format(script_path).format(modelFile))
+        stdin, stdout, stderr = ssh_client.exec_command('python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {} {}'.format(script_path , modelFile))
         #python3 {}'.format(script_path)
         op = stdout.read().decode('utf-8')
         err = stderr.read().decode('utf-8')
         if op:
                 print(op)
         if err:
                 print("Error:")
```

### Comparing `eurmlsdk-0.0.6/setup.py` & `eurmlsdk-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
```

