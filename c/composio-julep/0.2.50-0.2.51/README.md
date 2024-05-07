# Comparing `tmp/composio_julep-0.2.50.tar.gz` & `tmp/composio_julep-0.2.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.50.tar", last modified: Mon May  6 11:15:03 2024, max compression
+gzip compressed data, was "composio_julep-0.2.51.tar", last modified: Mon May  6 16:45:15 2024, max compression
```

## Comparing `composio_julep-0.2.50.tar` & `composio_julep-0.2.51.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 11:15:03.347524 composio_julep-0.2.50/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-06 11:15:03.347298 composio_julep-0.2.50/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3933 2024-05-02 07:58:37.000000 composio_julep-0.2.50/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 11:15:03.346100 composio_julep-0.2.50/composio_julep/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      157 2024-05-02 07:58:37.000000 composio_julep-0.2.50/composio_julep/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1619 2024-05-02 07:58:37.000000 composio_julep-0.2.50/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 11:15:03.347016 composio_julep-0.2.50/composio_julep.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-06 11:15:03.000000 composio_julep-0.2.50/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      267 2024-05-06 11:15:03.000000 composio_julep-0.2.50/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-06 11:15:03.000000 composio_julep-0.2.50/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-06 11:15:03.000000 composio_julep-0.2.50/composio_julep.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-05-06 11:15:03.000000 composio_julep-0.2.50/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-06 11:15:03.347574 composio_julep-0.2.50/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      842 2024-05-06 11:14:43.000000 composio_julep-0.2.50/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 16:45:15.760025 composio_julep-0.2.51/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-06 16:45:15.759770 composio_julep-0.2.51/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3933 2024-05-02 07:58:37.000000 composio_julep-0.2.51/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 16:45:15.758404 composio_julep-0.2.51/composio_julep/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      157 2024-05-02 07:58:37.000000 composio_julep-0.2.51/composio_julep/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1619 2024-05-02 07:58:37.000000 composio_julep-0.2.51/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-05-06 16:45:15.759363 composio_julep-0.2.51/composio_julep.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     4463 2024-05-06 16:45:15.000000 composio_julep-0.2.51/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      267 2024-05-06 16:45:15.000000 composio_julep-0.2.51/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-05-06 16:45:15.000000 composio_julep-0.2.51/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-06 16:45:15.000000 composio_julep-0.2.51/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       15 2024-05-06 16:45:15.000000 composio_julep-0.2.51/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-05-06 16:45:15.760075 composio_julep-0.2.51/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      842 2024-05-06 16:44:48.000000 composio_julep-0.2.51/setup.py
```

### Comparing `composio_julep-0.2.50/PKG-INFO` & `composio_julep-0.2.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.50
+Version: 0.2.51
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.50
+Requires-Dist: composio_openai===0.2.51
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.50/README.md` & `composio_julep-0.2.51/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.50/composio_julep/julep_toolspec.py` & `composio_julep-0.2.51/composio_julep/julep_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.50/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.51/composio_julep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.50
+Version: 0.2.51
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.50
+Requires-Dist: composio_openai===0.2.51
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.50/setup.py` & `composio_julep-0.2.51/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.50",
+    version="0.2.51",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_openai===0.2.50",
+        "composio_openai===0.2.51",
         "julep>=0.3.2"
     ],
     include_package_data=True,
 )
```
