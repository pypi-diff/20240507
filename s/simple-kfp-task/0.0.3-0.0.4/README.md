# Comparing `tmp/simple_kfp_task-0.0.3.tar.gz` & `tmp/simple_kfp_task-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task-0.0.3.tar", last modified: Fri May  3 09:00:48 2024, max compression
+gzip compressed data, was "simple_kfp_task-0.0.4.tar", last modified: Tue May  7 16:03:49 2024, max compression
```

## Comparing `simple_kfp_task-0.0.3.tar` & `simple_kfp_task-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 09:00:48.553953 simple_kfp_task-0.0.3/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     1077 2024-05-03 07:11:12.000000 simple_kfp_task-0.0.3/LICENSE
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      852 2024-05-03 09:00:48.553376 simple_kfp_task-0.0.3/PKG-INFO
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:10:43.000000 simple_kfp_task-0.0.3/README.md
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      788 2024-05-03 08:58:27.000000 simple_kfp_task-0.0.3/pyproject.toml
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      161 2024-05-03 07:19:04.000000 simple_kfp_task-0.0.3/requirements.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       38 2024-05-03 09:00:48.554081 simple_kfp_task-0.0.3/setup.cfg
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 09:00:48.549657 simple_kfp_task-0.0.3/simple_kfp_task/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      169 2024-05-03 08:48:23.000000 simple_kfp_task-0.0.3/simple_kfp_task/__init__.py
--rwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)     1607 2024-05-02 20:55:36.000000 simple_kfp_task-0.0.3/simple_kfp_task/cli.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)    10826 2024-05-02 20:55:39.000000 simple_kfp_task-0.0.3/simple_kfp_task/deploykf.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3855 2024-05-02 20:55:47.000000 simple_kfp_task-0.0.3/simple_kfp_task/git.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     9711 2024-05-03 07:38:07.000000 simple_kfp_task-0.0.3/simple_kfp_task/pipeline.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3102 2024-05-03 08:58:48.000000 simple_kfp_task-0.0.3/simple_kfp_task/task.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      614 2024-05-03 08:46:02.000000 simple_kfp_task-0.0.3/simple_kfp_task/utils.py
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 09:00:48.552716 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      852 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/PKG-INFO
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      464 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/SOURCES.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        1 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/dependency_links.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       61 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/entry_points.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      162 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/requires.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       16 2024-05-03 09:00:48.000000 simple_kfp_task-0.0.3/simple_kfp_task.egg-info/top_level.txt
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.674924 simple_kfp_task-0.0.4/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/LICENSE
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:03:49.674335 simple_kfp_task-0.0.4/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:02:29.000000 simple_kfp_task-0.0.4/pyproject.toml
+-rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/requirements.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:03:49.675088 simple_kfp_task-0.0.4/setup.cfg
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.669930 simple_kfp_task-0.0.4/simple_kfp_task/
+-rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.4/simple_kfp_task/__init__.py
+-rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.4/simple_kfp_task/cli.py
+-rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.4/simple_kfp_task/deploykf.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     5077 2024-05-07 08:30:55.000000 simple_kfp_task-0.0.4/simple_kfp_task/git_helper.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     8675 2024-05-07 15:59:06.000000 simple_kfp_task-0.0.4/simple_kfp_task/pipeline.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     7408 2024-05-07 16:00:04.000000 simple_kfp_task-0.0.4/simple_kfp_task/task.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1157 2024-05-07 09:18:59.000000 simple_kfp_task-0.0.4/simple_kfp_task/utils.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:03:49.673524 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/entry_points.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/requires.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:03:49.000000 simple_kfp_task-0.0.4/simple_kfp_task.egg-info/top_level.txt
```

### Comparing `simple_kfp_task-0.0.3/LICENSE` & `simple_kfp_task-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.3/PKG-INFO` & `simple_kfp_task-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task-0.0.3/pyproject.toml` & `simple_kfp_task-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_kfp_task-0.0.3/simple_kfp_task/cli.py` & `simple_kfp_task-0.0.4/simple_kfp_task/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 #!/usr/bin/env python
-from simple_kfp_task.task import run
+from simple_kfp_task.task import Task
 from argparse import ArgumentParser
 
 
 def main():
+    """
+    Entry point of the program.
+    
+    Parses command line arguments and calls the `run` function with the parsed arguments.
+    """
+    
     parser = ArgumentParser()
     parser.add_argument('command')
-    # kfp
     parser.add_argument("--namespace", required=True)
     parser.add_argument("--experiment-name")
     parser.add_argument("--run-name")
-    # git
     parser.add_argument("--remote", default="origin")
     parser.add_argument("--remote-url")
     parser.add_argument("--branch")
     parser.add_argument("--commit")
     parser.add_argument("--ignore-ssh-error")
-    # pip
     parser.add_argument("--requirements")
     parser.add_argument("--packages", nargs='+', default=[])
-    parser.add_argument("--volume-size", default="1Gi")
-    # container
     parser.add_argument("--gpu-limit", default=0)
+    parser.add_argument("--cpu-limit", default="1")
+    parser.add_argument("--cpu-request", default="0.5")
+    parser.add_argument("--memory-limit", default="2Gi")
+    parser.add_argument("--memory-request", default="1Gi")
     parser.add_argument("--gpu-vendor", default="nvidia.com/gpu")
     parser.add_argument("--container-image", default="python:3.12.3-slim")
+    parser.add_argument("--volume-name", default=None)
+    parser.add_argument("--disable-git-detection", action="store_true", default=False)
+    parser.add_argument("--dry-run", action="store_true", default=False)
+    parser.add_argument("--wait-for-run", action="store_true", default=False)
 
     args, command_args = parser.parse_known_args()
 
-    run(
-        # kfp
+    task = Task.init(
         run_name=args.run_name,
         experiment_name=args.experiment_name,
         namespace=args.namespace,
-        # command
         command=args.command,
-        command_args=command_args,
-        # git
+        args=command_args,
         remote=args.remote,
         remote_url=args.remote_url,
         branch=args.branch,
         commit=args.commit,
-        # pip
         requirements=args.requirements,
         packages=args.packages,
-        # volume
-        volume_size=args.volume_size,
-        # container
         gpu_limit=args.gpu_limit,
         gpu_vendor=args.gpu_vendor,
-        container_image=args.container_image,
+        cpu_limit=args.cpu_limit,
+        cpu_request=args.cpu_request,
+        memory_limit=args.memory_limit,
+        memory_request=args.memory_request,
+        volume_name=args.volume_name,
+        container_image=args.container_image
     )
+
+    if not args.dry_run:
+        run = task.run()
+        if args.wait_for_run:
+            run_response = run.wait_for_run_completion()
+            run = run_response.run.id
+            print(run_response)
```

### Comparing `simple_kfp_task-0.0.3/simple_kfp_task/deploykf.py` & `simple_kfp_task-0.0.4/simple_kfp_task/deploykf.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.3/simple_kfp_task.egg-info/PKG-INFO` & `simple_kfp_task-0.0.4/simple_kfp_task.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

