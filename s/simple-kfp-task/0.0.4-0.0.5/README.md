# Comparing `tmp/simple_kfp_task-0.0.4.tar.gz` & `tmp/simple_kfp_task-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task-0.0.4.tar", last modified: Tue May  7 16:03:49 2024, max compression
+gzip compressed data, was "simple_kfp_task-0.0.5.tar", last modified: Tue May  7 16:16:06 2024, max compression
```

## Comparing `simple_kfp_task-0.0.4.tar` & `simple_kfp_task-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.674924 simple_kfp_task-0.0.4/
--rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/LICENSE
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:03:49.674335 simple_kfp_task-0.0.4/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:02:29.000000 simple_kfp_task-0.0.4/pyproject.toml
--rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/requirements.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:03:49.675088 simple_kfp_task-0.0.4/setup.cfg
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.669930 simple_kfp_task-0.0.4/simple_kfp_task/
--rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.4/simple_kfp_task/__init__.py
--rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.4/simple_kfp_task/cli.py
--rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/simple_kfp_task/deploykf.py
--rw-r--r--   0 sebastian   (501) staff       (20)     5077 2024-05-07 08:30:55.000000 simple_kfp_task-0.0.4/simple_kfp_task/git_helper.py
--rw-r--r--   0 sebastian   (501) staff       (20)     8675 2024-05-07 15:59:06.000000 simple_kfp_task-0.0.4/simple_kfp_task/pipeline.py
--rw-r--r--   0 sebastian   (501) staff       (20)     7408 2024-05-07 16:00:04.000000 simple_kfp_task-0.0.4/simple_kfp_task/task.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1157 2024-05-07 09:18:59.000000 simple_kfp_task-0.0.4/simple_kfp_task/utils.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.673524 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/entry_points.txt
--rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/requires.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/top_level.txt
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:16:06.606355 simple_kfp_task-0.0.5/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.5/LICENSE
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:16:06.605581 simple_kfp_task-0.0.5/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:15:13.000000 simple_kfp_task-0.0.5/pyproject.toml
+-rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.5/requirements.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:16:06.606525 simple_kfp_task-0.0.5/setup.cfg
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:16:06.600763 simple_kfp_task-0.0.5/simple_kfp_task/
+-rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.5/simple_kfp_task/__init__.py
+-rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.5/simple_kfp_task/cli.py
+-rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.5/simple_kfp_task/deploykf.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     5077 2024-05-07 08:30:55.000000 simple_kfp_task-0.0.5/simple_kfp_task/git_helper.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     8727 2024-05-07 16:07:33.000000 simple_kfp_task-0.0.5/simple_kfp_task/pipeline.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     7468 2024-05-07 16:14:30.000000 simple_kfp_task-0.0.5/simple_kfp_task/task.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1157 2024-05-07 09:18:59.000000 simple_kfp_task-0.0.5/simple_kfp_task/utils.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:16:06.604229 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/entry_points.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/requires.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:16:06.000000 simple_kfp_task-0.0.5/simple_kfp_task.egg-info/top_level.txt
```

### Comparing `simple_kfp_task-0.0.4/LICENSE` & `simple_kfp_task-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.4/PKG-INFO` & `simple_kfp_task-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task-0.0.4/pyproject.toml` & `simple_kfp_task-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/cli.py` & `simple_kfp_task-0.0.5/simple_kfp_task/cli.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/deploykf.py` & `simple_kfp_task-0.0.5/simple_kfp_task/deploykf.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/git_helper.py` & `simple_kfp_task-0.0.5/simple_kfp_task/git_helper.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/pipeline.py` & `simple_kfp_task-0.0.5/simple_kfp_task/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,20 @@
     exit 1
 fi
 
 #
 # Wait for the git apply to finish
 #
 
-until [ -f /ipc/git-apply ]; do sleep 1; done
-while read -r line; do echo $line; done < /ipc/git-apply.log
-if [ $(cat /ipc/git-apply) -ne 0 ]; then
-    exit 1
+if [ -n "{git_diff}" ]; then
+    until [ -f /ipc/git-apply ]; do sleep 1; done
+    while read -r line; do echo $line; done < /ipc/git-apply.log
+    if [ $(cat /ipc/git-apply) -ne 0 ]; then
+        exit 1
+    fi
 fi
 
 cd {cwd} && \
 if [ -n "{requirements}" ]; then pip install -r {requirements}; fi && \
 if [ -n "{packages}" ]; then echo "{packages}" | xargs pip install; fi && \
 python {command} {args}
             """
```

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/task.py` & `simple_kfp_task-0.0.5/simple_kfp_task/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
         self.gpu_vendor = gpu_vendor
         self.cpu_limit = cpu_limit
         self.cpu_request = cpu_request
         self.memory_limit = memory_limit
         self.memory_request = memory_request
         self.volume_name = volume_name
 
+        if os.environ.get('INSIDE_KFP_FUNC_CONTAINER'):
+            return
+
         git_helper = GitHelper()
 
         if self.func:
             self.command = os.path.relpath(get_caller_filename(), os.getcwd())
             if self.packages is None:
                 self.packages = [PIP_PACKAGE_NAME]
             else:
@@ -147,15 +150,15 @@
         Returns:
             kfp_client.create_run_from_pipeline_func: The KFP run created for the task.
 
         """
         if os.environ.get('INSIDE_KFP_FUNC_CONTAINER'):
             if self.func:
                 self.func()
-                
+
         kfp_client = create_kfp_client(namespace=self.namespace)
         return kfp_client.create_run_from_pipeline_func(
             pipeline_func=simple_task_pipeline,
             experiment_name=self.experiment_name,
             run_name=self.run_name,
             arguments={
                 "command": self.command if self.command else "",
```

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task/utils.py` & `simple_kfp_task-0.0.5/simple_kfp_task/utils.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.4/simple_kfp_task.egg-info/PKG-INFO` & `simple_kfp_task-0.0.5/simple_kfp_task.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

