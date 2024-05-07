# Comparing `tmp/eurmlsdk-0.0.3.tar.gz` & `tmp/eurmlsdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.3.tar", last modified: Tue May  7 09:15:08 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.4.tar", last modified: Tue May  7 09:32:44 2024, max compression
```

## Comparing `eurmlsdk-0.0.3.tar` & `eurmlsdk-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.3/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.3/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.3/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.3/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     4616 2024-05-07 08:16:01.000000 eurmlsdk-0.0.3/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)    10376 2024-05-07 08:21:30.000000 eurmlsdk-0.0.3/eurmlsdk/base_class.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 09:15:08.000000 eurmlsdk-0.0.3/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 09:15:08.754494 eurmlsdk-0.0.3/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 09:15:03.000000 eurmlsdk-0.0.3/setup.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-04-29 05:37:24.000000 eurmlsdk-0.0.4/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-04-29 05:37:24.000000 eurmlsdk-0.0.4/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-07 07:43:41.000000 eurmlsdk-0.0.4/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.884478 eurmlsdk-0.0.4/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-07 07:30:15.000000 eurmlsdk-0.0.4/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     4628 2024-05-07 09:18:30.000000 eurmlsdk-0.0.4/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)    10466 2024-05-07 09:25:59.000000 eurmlsdk-0.0.4/eurmlsdk/base_class.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-07 09:32:44.884478 eurmlsdk-0.0.4/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      433 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      301 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       29 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-07 09:32:44.000000 eurmlsdk-0.0.4/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-07 09:32:44.894478 eurmlsdk-0.0.4/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      695 2024-05-07 09:32:32.000000 eurmlsdk-0.0.4/setup.py
```

### Comparing `eurmlsdk-0.0.3/eurmlsdk/__main__.py` & `eurmlsdk-0.0.4/eurmlsdk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             print("Usage: eurmlsdk deploy <local path> <hostname> <username> <password>")
         else:
             localPath = argv[2]
             remotePath = "/home/embeduradmin/" + localPath.split("/")[-1]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
-            modelBase = ModelBase(s3_bucket, model_key, model_ouput_path)
+            modelBase = ModelBase(s3_bucket, model_key, model_ouput_path ,None ,None)
             script_path = "/home/embeduradmin/hello.py"
             modelBase.deployModel(localPath, remotePath, hostname, username, password ,script_path)
         exit(1)
         
     else:
         print("Unknown command. Please find the list of commands")
         list_commands()
```

### Comparing `eurmlsdk-0.0.3/eurmlsdk/base_class.py` & `eurmlsdk-0.0.4/eurmlsdk/base_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sys import argv,exit
 from abc import abstractmethod
 import os
 import boto3
-from mltk.core import profile_model
+#from mltk.core import profile_model
 import json
 import matplotlib.pyplot as plt
 from ultralytics import YOLO
 import paramiko
 
 class ModelBase:
     """
@@ -70,69 +70,69 @@
         s3client = boto3.client('s3')
         s3client.download_file(Bucket, Key, Filename)
         filePath = self.model_output_path
         return filePath
 
     def getProfileInfo(self , model_file)->None:
         print("Profiling for "+ model_file)
-        profiling_results = profile_model(model_file,return_estimates=True).to_json(indent=2, format_units=True, exclude_null=True, full_summary=False)
-        return profiling_results
+        #profiling_results = profile_model(model_file,return_estimates=True).to_json(indent=2, format_units=True, exclude_null=True, full_summary=False)
+        #return profiling_results
     
     def compareMetrics(self , unQuantizedModel , quantizedModel)->None:
         print("Metrics Comparison")
-        metrics_uq = self.getProfileInfo(unQuantizedModel)
-        metrics_q = self.getProfileInfo(quantizedModel)
-        prof_1 = json.loads(metrics_uq)
-        prof_2 = json.loads(metrics_q)
-
-        data1 = prof_1['summary']
-        data2 = prof_2['summary']
-        keys_to_drop = ["name", "accelerator" , "input_shape" , "input_dtype" , "output_shape" , "output_dtype"]
-        val1 = data1['name']
-        val2 = data2['name']
-        # Drop the keys
-        for key in keys_to_drop:
-            if key in data1:
-                del data1[key]
+        # metrics_uq = self.getProfileInfo(unQuantizedModel)
+        # metrics_q = self.getProfileInfo(quantizedModel)
+        # prof_1 = json.loads(metrics_uq)
+        # prof_2 = json.loads(metrics_q)
+
+        # data1 = prof_1['summary']
+        # data2 = prof_2['summary']
+        # keys_to_drop = ["name", "accelerator" , "input_shape" , "input_dtype" , "output_shape" , "output_dtype"]
+        # val1 = data1['name']
+        # val2 = data2['name']
+        # # Drop the keys
+        # for key in keys_to_drop:
+        #     if key in data1:
+        #         del data1[key]
                 
-        for key in keys_to_drop:
-            if key in data2:
-                del data2[key]
-
-        # Get the keys (assuming they are the same in both JSON objects)
-        keys = list(data1.keys())
-
-        # Calculate the number of rows and columns for the subplots
-        n = len(keys)
-        ncols = 4
-        nrows = n // ncols + (n % ncols > 0)
-
-        # Create a figure and a grid of subplots
-        fig, axs = plt.subplots(nrows, ncols, figsize=(20, 5*nrows))
-
-        # Flatten the array of axes
-        axs = axs.flatten()
-
-
-        # Generate a subplot for each key
-        for i, key in enumerate(keys):
-            values1 = data1[key]
-            values2 = data2[key]
-            axs[i].bar([val1 , val2], [values1, values2])  # Plot the values
-            axs[i].set_title(f'Comparison of {key}')
-            axs[i].set_ylim(0,20)
-
-        # Remove unused subplots
-        for j in range(i+1, len(axs)):
-            fig.delaxes(axs[j])
+        # for key in keys_to_drop:
+        #     if key in data2:
+        #         del data2[key]
+
+        # # Get the keys (assuming they are the same in both JSON objects)
+        # keys = list(data1.keys())
+
+        # # Calculate the number of rows and columns for the subplots
+        # n = len(keys)
+        # ncols = 4
+        # nrows = n // ncols + (n % ncols > 0)
+
+        # # Create a figure and a grid of subplots
+        # fig, axs = plt.subplots(nrows, ncols, figsize=(20, 5*nrows))
+
+        # # Flatten the array of axes
+        # axs = axs.flatten()
+
+
+        # # Generate a subplot for each key
+        # for i, key in enumerate(keys):
+        #     values1 = data1[key]
+        #     values2 = data2[key]
+        #     axs[i].bar([val1 , val2], [values1, values2])  # Plot the values
+        #     axs[i].set_title(f'Comparison of {key}')
+        #     axs[i].set_ylim(0,20)
+
+        # # Remove unused subplots
+        # for j in range(i+1, len(axs)):
+        #     fig.delaxes(axs[j])
 
-        plt.tight_layout()
-        plt.savefig("metrics_comparison_chart.png")
+        # plt.tight_layout()
+        # plt.savefig("metrics_comparison_chart.png")
         
-    def connect_ssh_client(hostname , username, password):
+    def connect_ssh_client(self ,hostname , username, password):
         ssh = paramiko.SSHClient()
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         ssh.connect(hostname, username=username, password=password)
         return ssh
     
     def uploadModel(self, local_path, remote_path, hostname, username, password):
         # Establish SSH connection
@@ -146,15 +146,15 @@
 
         # Close SSH connection
         ssh_client.close()
         
     def execute_script(self, hostname, username, password , script_path):
         ssh_client = self.connect_ssh_client(hostname, username, password)
         
-        stdin, stdout, stderr = ssh_client.exec_command('python3 -m mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {}'.format(script_path))
+        stdin, stdout, stderr = ssh_client.exec_command('python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {}'.format(script_path))
         #python3 {}'.format(script_path)
         op = stdout.read().decode('utf-8')
         err = stderr.read().decode('utf-8')
         if op:
                 print(op)
         if err:
                 print("Error:")
```

### Comparing `eurmlsdk-0.0.3/setup.py` & `eurmlsdk-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko'
```

