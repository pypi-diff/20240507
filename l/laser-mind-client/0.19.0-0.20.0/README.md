# Comparing `tmp/laser_mind_client-0.19.0.tar.gz` & `tmp/laser_mind_client-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laser_mind_client-0.19.0.tar", last modified: Tue May  7 12:42:20 2024, max compression
+gzip compressed data, was "laser_mind_client-0.20.0.tar", last modified: Tue May  7 13:23:51 2024, max compression
```

## Comparing `laser_mind_client-0.19.0.tar` & `laser_mind_client-0.20.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 12:42:20.778959 laser_mind_client-0.19.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-05-07 12:40:56.000000 laser_mind_client-0.19.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8760 2024-05-07 12:42:20.778959 laser_mind_client-0.19.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2024-05-07 12:40:56.000000 laser_mind_client-0.19.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 12:42:20.778959 laser_mind_client-0.19.0/laser_mind_client/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-07 12:40:56.000000 laser_mind_client-0.19.0/laser_mind_client/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2024-05-07 12:40:56.000000 laser_mind_client-0.19.0/laser_mind_client/laser_mind_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 12:42:20.778959 laser_mind_client-0.19.0/laser_mind_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8760 2024-05-07 12:42:20.000000 laser_mind_client-0.19.0/laser_mind_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      305 2024-05-07 12:42:20.000000 laser_mind_client-0.19.0/laser_mind_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 12:42:20.000000 laser_mind_client-0.19.0/laser_mind_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-07 12:42:20.000000 laser_mind_client-0.19.0/laser_mind_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-07 12:42:20.000000 laser_mind_client-0.19.0/laser_mind_client.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      710 2024-05-07 12:42:17.000000 laser_mind_client-0.19.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 12:42:20.778959 laser_mind_client-0.19.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 13:23:51.958324 laser_mind_client-0.20.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-07 12:59:06.000000 laser_mind_client-0.20.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-07 13:23:51.958324 laser_mind_client-0.20.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8152 2024-05-07 12:40:56.000000 laser_mind_client-0.20.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 13:23:51.958324 laser_mind_client-0.20.0/laser_mind_client/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2024-05-07 12:40:56.000000 laser_mind_client-0.20.0/laser_mind_client/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2024-05-07 12:40:56.000000 laser_mind_client-0.20.0/laser_mind_client/laser_mind_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 13:23:51.958324 laser_mind_client-0.20.0/laser_mind_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8772 2024-05-07 13:23:51.000000 laser_mind_client-0.20.0/laser_mind_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      305 2024-05-07 13:23:51.000000 laser_mind_client-0.20.0/laser_mind_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 13:23:51.000000 laser_mind_client-0.20.0/laser_mind_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-05-07 13:23:51.000000 laser_mind_client-0.20.0/laser_mind_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-07 13:23:51.000000 laser_mind_client-0.20.0/laser_mind_client.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      722 2024-05-07 13:23:49.000000 laser_mind_client-0.20.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 13:23:51.958324 laser_mind_client-0.20.0/setup.cfg
```

### Comparing `laser_mind_client-0.19.0/LICENSE` & `laser_mind_client-0.20.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 LightSolver Internal
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `laser_mind_client-0.19.0/PKG-INFO` & `laser_mind_client-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.19.0
+Version: 0.20.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: laser-mind-client-meta>=0.0.9
 Requires-Dist: ls_api_clients>=0.4.6
```

### Comparing `laser_mind_client-0.19.0/README.md` & `laser_mind_client-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.19.0/laser_mind_client/laser_mind_client.py` & `laser_mind_client-0.20.0/laser_mind_client/laser_mind_client.py`

 * *Files identical despite different names*

### Comparing `laser_mind_client-0.19.0/laser_mind_client.egg-info/PKG-INFO` & `laser_mind_client-0.20.0/laser_mind_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: laser-mind-client
-Version: 0.19.0
+Version: 0.20.0
 Summary: A client python API for accessing LightSolver's capabilities
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: laser-mind-client-meta>=0.0.9
 Requires-Dist: ls_api_clients>=0.4.6
```

### Comparing `laser_mind_client-0.19.0/pyproject.toml` & `laser_mind_client-0.20.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "laser-mind-client"
-version = "0.19.0"
+version = "0.20.0"
 description = "A client python API for accessing LightSolver's capabilities"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "numpy>=1.21.5", "laser-mind-client-meta>=0.0.9", "ls_api_clients>=0.4.6", "ls-packers>=0.2.0",]
-classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
 email = "assaf@lightsolver.com"
 
 [project.urls]
 Homepage = "https://lightsolver.com"
```

