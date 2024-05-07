# Comparing `tmp/cogflow-1.9.7.tar.gz` & `tmp/cogflow-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.9.7.tar", last modified: Mon May  6 13:37:55 2024, max compression
+gzip compressed data, was "cogflow-1.9.8.tar", last modified: Tue May  7 07:24:58 2024, max compression
```

## Comparing `cogflow-1.9.7.tar` & `cogflow-1.9.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:37:55.191490 cogflow-1.9.7/
--rw-rw-rw-   0        0        0     3230 2024-05-06 13:37:55.185668 cogflow-1.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:37:54.905184 cogflow-1.9.7/cogflow/
--rw-rw-rw-   0        0        0     5489 2024-05-03 11:06:52.000000 cogflow-1.9.7/cogflow/__init__.py
--rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.7/cogflow/cogflow_config.ini
--rw-rw-rw-   0        0        0     6159 2024-05-03 11:09:50.000000 cogflow-1.9.7/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.7/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    15647 2024-05-06 12:36:42.000000 cogflow-1.9.7/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0     3116 2024-05-03 11:02:35.000000 cogflow-1.9.7/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.7/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.7/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.7/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:37:55.076536 cogflow-1.9.7/cogflow.egg-info/
--rw-rw-rw-   0        0        0     3230 2024-05-06 13:37:54.000000 cogflow-1.9.7/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-05-06 13:37:54.000000 cogflow-1.9.7/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:37:54.000000 cogflow-1.9.7/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-05-06 13:37:54.000000 cogflow-1.9.7/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-06 13:37:54.000000 cogflow-1.9.7/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 13:37:55.191490 cogflow-1.9.7/setup.cfg
--rw-rw-rw-   0        0        0     1940 2024-05-06 13:37:31.000000 cogflow-1.9.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:37:55.179233 cogflow-1.9.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.7/tests/__init__.py
--rw-rw-rw-   0        0        0    11566 2024-05-03 11:09:50.000000 cogflow-1.9.7/tests/test_dataset_plugin.py
--rw-rw-rw-   0        0        0     6614 2024-05-03 11:09:50.000000 cogflow-1.9.7/tests/test_kubeflowplugin.py
--rw-rw-rw-   0        0        0    18889 2024-05-06 13:32:38.000000 cogflow-1.9.7/tests/test_mlflowplugin.py
--rw-rw-rw-   0        0        0     4363 2024-05-03 11:09:50.000000 cogflow-1.9.7/tests/test_plugin_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.966848 cogflow-1.9.8/
+-rw-rw-rw-   0        0        0     3230 2024-05-07 07:24:57.934664 cogflow-1.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2339 2024-04-29 16:43:23.000000 cogflow-1.9.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.715655 cogflow-1.9.8/cogflow/
+-rw-rw-rw-   0        0        0     5551 2024-05-06 13:50:23.000000 cogflow-1.9.8/cogflow/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-29 15:44:21.000000 cogflow-1.9.8/cogflow/cogflow_config.ini
+-rw-rw-rw-   0        0        0     6159 2024-05-03 11:09:50.000000 cogflow-1.9.8/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     9770 2024-04-29 09:33:07.000000 cogflow-1.9.8/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    15647 2024-05-06 12:36:42.000000 cogflow-1.9.8/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0     3116 2024-05-03 11:02:35.000000 cogflow-1.9.8/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.9.8/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.9.8/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     9654 2024-04-29 16:16:34.000000 cogflow-1.9.8/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.794737 cogflow-1.9.8/cogflow.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-07 07:24:56.000000 cogflow-1.9.8/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 07:24:57.966848 cogflow-1.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1940 2024-05-07 07:24:47.000000 cogflow-1.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:24:57.925433 cogflow-1.9.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.9.8/tests/__init__.py
+-rw-rw-rw-   0        0        0    11566 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     6614 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    18889 2024-05-06 13:32:38.000000 cogflow-1.9.8/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     4363 2024-05-03 11:09:50.000000 cogflow-1.9.8/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.9.7/PKG-INFO` & `cogflow-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.7
+Version: 1.9.8
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.7/README.md` & `cogflow-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/__init__.py` & `cogflow-1.9.8/cogflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 pyfunc = MlflowPlugin().pyfunc
 mlflow = MlflowPlugin().mlflow
 sklearn = MlflowPlugin().sklearn
 cogclient = MlflowPlugin().cogclient
 tensorflow = MlflowPlugin().tensorflow
 pytorch = MlflowPlugin().pytorch
 models = MlflowPlugin().models
+search_model_versions = MlflowPlugin().search_model_versions
 
 
 add_model_access = CogContainer().add_model_access
 pipeline = KubeflowPlugin().pipeline
 create_component_from_func = KubeflowPlugin().create_component_from_func
 client = KubeflowPlugin().client
 load_component_from_url = KubeflowPlugin().load_component_from_url
```

### Comparing `cogflow-1.9.7/cogflow/dataset_plugin.py` & `cogflow-1.9.8/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/kubeflowplugin.py` & `cogflow-1.9.8/cogflow/kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/mlflowplugin.py` & `cogflow-1.9.8/cogflow/mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/plugin_config.py` & `cogflow-1.9.8/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/plugin_status.py` & `cogflow-1.9.8/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow/pluginmanager.py` & `cogflow-1.9.8/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/cogflow.egg-info/PKG-INFO` & `cogflow-1.9.8/cogflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogflow
-Version: 1.9.7
+Version: 1.9.8
 Summary: cog modules
 Home-page: UNKNOWN
 Author: Sai_kireeti
 Author-email: sai.kireeti@hiro-microdatacenters.nl
 License: UNKNOWN
 Description: 
         # CogFlow
```

### Comparing `cogflow-1.9.7/cogflow.egg-info/SOURCES.txt` & `cogflow-1.9.8/cogflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/setup.py` & `cogflow-1.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Read the content of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cogflow",
-    version="1.9.7",
+    version="1.9.8",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `cogflow-1.9.7/tests/test_dataset_plugin.py` & `cogflow-1.9.8/tests/test_dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/tests/test_kubeflowplugin.py` & `cogflow-1.9.8/tests/test_kubeflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/tests/test_mlflowplugin.py` & `cogflow-1.9.8/tests/test_mlflowplugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.9.7/tests/test_plugin_manager.py` & `cogflow-1.9.8/tests/test_plugin_manager.py`

 * *Files identical despite different names*

