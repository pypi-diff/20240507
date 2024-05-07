# Comparing `tmp/python_sdk_remote-0.0.92.tar.gz` & `tmp/python_sdk_remote-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sdk_remote-0.0.92.tar", last modified: Sun May  5 08:19:47 2024, max compression
+gzip compressed data, was "python_sdk_remote-0.0.93.tar", last modified: Tue May  7 04:52:27 2024, max compression
```

## Comparing `python_sdk_remote-0.0.92.tar` & `python_sdk_remote-0.0.93.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.062531 python_sdk_remote-0.0.92/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/http_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 08:19:47.000000 python_sdk_remote-0.0.92/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:19:47.066531 python_sdk_remote-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-05 08:19:34.000000 python_sdk_remote-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.756741 python_sdk_remote-0.0.93/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/get_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 04:52:27.000000 python_sdk_remote-0.0.93/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 04:52:27.760741 python_sdk_remote-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-07 04:52:17.000000 python_sdk_remote-0.0.93/setup.py
```

### Comparing `python_sdk_remote-0.0.92/PKG-INFO` & `python_sdk_remote-0.0.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.92
+Version: 0.0.93
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.92/README.md` & `python_sdk_remote-0.0.93/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# python-package-backend-template
+# python-sdk-package
+
+https://github.com/grosser/repo_dependency_graph Ruby, Graph the dependencies of your repositories
+https://github.com/thebjorn/pydeps Python
 
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 #database Python scripts in /db folder
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
```

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/constants.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 PYTHON_SDK_LOCAL_COMPONENT_ID = 184
-PYTHON_SDK_LOCAL_COMPONENT_NAME = 'python_sdk_local'
+PYTHON_SDK_LOCAL_COMPONENT_NAME = 'python_sdk_remote'
 
 ENVIRONMENT_NAME = os.getenv("ENVIRONMENT_NAME")
 BRAND_NAME = os.getenv("BRAND_NAME")
 LOGZIO_TOKEN = os.getenv("LOGZIO_TOKEN")
 # TODO Shall Can we use python-sdk function to get the value from Environment?
 # TODO Shall we get the value from environment here of send the value to the function as @akiva-skolnik did?
 GOOGLE_PORT_FOR_AUTHENTICATION = os.getenv("PORT_FOR_AUTHENTICATION")
```

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/http_response.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/http_response.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/mini_logger.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/our_object.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/unified_json.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/utilities.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/utilities.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote/src/validate_environment.py` & `python_sdk_remote-0.0.93/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote.egg-info/PKG-INFO` & `python_sdk_remote-0.0.93/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.92
+Version: 0.0.93
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_sdk_remote-0.0.92/python_sdk_remote.egg-info/SOURCES.txt` & `python_sdk_remote-0.0.93/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 python_sdk_remote.egg-info/PKG-INFO
 python_sdk_remote.egg-info/SOURCES.txt
 python_sdk_remote.egg-info/dependency_links.txt
 python_sdk_remote.egg-info/requires.txt
 python_sdk_remote.egg-info/top_level.txt
 python_sdk_remote/src/__init__.py
 python_sdk_remote/src/constants.py
+python_sdk_remote/src/get_dependencies.py
 python_sdk_remote/src/http_response.py
 python_sdk_remote/src/item.py
 python_sdk_remote/src/mini_logger.py
 python_sdk_remote/src/our_object.py
 python_sdk_remote/src/unified_json.py
 python_sdk_remote/src/utilities.py
 python_sdk_remote/src/valid_json_versions.py
```

### Comparing `python_sdk_remote-0.0.92/setup.py` & `python_sdk_remote-0.0.93/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.92',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.93',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

