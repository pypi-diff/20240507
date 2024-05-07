# Comparing `tmp/simple_kfp_task-0.0.6.tar.gz` & `tmp/simple_kfp_task-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task-0.0.6.tar", last modified: Tue May  7 16:26:16 2024, max compression
+gzip compressed data, was "simple_kfp_task-0.0.7.tar", last modified: Tue May  7 16:30:15 2024, max compression
```

## Comparing `simple_kfp_task-0.0.6.tar` & `simple_kfp_task-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:26:16.368480 simple_kfp_task-0.0.6/
--rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.6/LICENSE
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:26:16.367733 simple_kfp_task-0.0.6/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:25:58.000000 simple_kfp_task-0.0.6/pyproject.toml
--rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.6/requirements.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:26:16.368636 simple_kfp_task-0.0.6/setup.cfg
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:26:16.363264 simple_kfp_task-0.0.6/simple_kfp_task/
--rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.6/simple_kfp_task/__init__.py
--rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.6/simple_kfp_task/cli.py
--rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.6/simple_kfp_task/deploykf.py
--rw-r--r--   0 sebastian   (501) staff       (20)     5077 2024-05-07 08:30:55.000000 simple_kfp_task-0.0.6/simple_kfp_task/git_helper.py
--rw-r--r--   0 sebastian   (501) staff       (20)     8727 2024-05-07 16:07:33.000000 simple_kfp_task-0.0.6/simple_kfp_task/pipeline.py
--rw-r--r--   0 sebastian   (501) staff       (20)     7479 2024-05-07 16:25:45.000000 simple_kfp_task-0.0.6/simple_kfp_task/task.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1410 2024-05-07 16:24:19.000000 simple_kfp_task-0.0.6/simple_kfp_task/utils.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:26:16.366774 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/entry_points.txt
--rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/requires.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:26:16.000000 simple_kfp_task-0.0.6/simple_kfp_task.egg-info/top_level.txt
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:30:15.991930 simple_kfp_task-0.0.7/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.7/LICENSE
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:30:15.991388 simple_kfp_task-0.0.7/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:30:04.000000 simple_kfp_task-0.0.7/pyproject.toml
+-rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.7/requirements.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:30:15.992083 simple_kfp_task-0.0.7/setup.cfg
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:30:15.987228 simple_kfp_task-0.0.7/simple_kfp_task/
+-rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.7/simple_kfp_task/__init__.py
+-rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.7/simple_kfp_task/cli.py
+-rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.7/simple_kfp_task/deploykf.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     5166 2024-05-07 16:29:26.000000 simple_kfp_task-0.0.7/simple_kfp_task/git_helper.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     8727 2024-05-07 16:07:33.000000 simple_kfp_task-0.0.7/simple_kfp_task/pipeline.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     7479 2024-05-07 16:25:45.000000 simple_kfp_task-0.0.7/simple_kfp_task/task.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     1410 2024-05-07 16:24:19.000000 simple_kfp_task-0.0.7/simple_kfp_task/utils.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:30:15.990636 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/
+-rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/entry_points.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/requires.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:30:15.000000 simple_kfp_task-0.0.7/simple_kfp_task.egg-info/top_level.txt
```

### Comparing `simple_kfp_task-0.0.6/LICENSE` & `simple_kfp_task-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/PKG-INFO` & `simple_kfp_task-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task-0.0.6/pyproject.toml` & `simple_kfp_task-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/cli.py` & `simple_kfp_task-0.0.7/simple_kfp_task/cli.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/deploykf.py` & `simple_kfp_task-0.0.7/simple_kfp_task/deploykf.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/git_helper.py` & `simple_kfp_task-0.0.7/simple_kfp_task/git_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from git import Repo
 import os
 import sys
+from simple_kfp_task.utils import is_remote_execution
+
+if not is_remote_execution():
+    from git import Repo
 
 class GitHelper:
     """
     A helper class for interacting with Git repositories.
     """
 
     def __init__(self):
```

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/pipeline.py` & `simple_kfp_task-0.0.7/simple_kfp_task/pipeline.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/task.py` & `simple_kfp_task-0.0.7/simple_kfp_task/task.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task/utils.py` & `simple_kfp_task-0.0.7/simple_kfp_task/utils.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.6/simple_kfp_task.egg-info/PKG-INFO` & `simple_kfp_task-0.0.7/simple_kfp_task.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

