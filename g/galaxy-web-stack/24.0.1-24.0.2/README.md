# Comparing `tmp/galaxy_web_stack-24.0.1.tar.gz` & `tmp/galaxy_web_stack-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_web_stack-24.0.1.tar", last modified: Thu May  2 13:49:31 2024, max compression
+gzip compressed data, was "galaxy_web_stack-24.0.2.tar", last modified: Tue May  7 14:34:38 2024, max compression
```

## Comparing `galaxy_web_stack-24.0.1.tar` & `galaxy_web_stack-24.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:31.574156 galaxy_web_stack-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-02 13:49:31.574156 galaxy_web_stack-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:31.570156 galaxy_web_stack-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:31.570156 galaxy_web_stack-24.0.1/galaxy/web_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/web_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/web_stack/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/web_stack/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/web_stack/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/galaxy/web_stack/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:31.574156 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-02 13:49:31.000000 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-02 13:49:31.000000 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:31.000000 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 13:49:31.000000 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:49:31.000000 galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-02 13:49:31.574156 galaxy_web_stack-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 13:46:45.000000 galaxy_web_stack-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:38.400491 galaxy_web_stack-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_web_stack-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-07 14:34:38.400491 galaxy_web_stack-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:38.396491 galaxy_web_stack-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:38.400491 galaxy_web_stack-24.0.2/galaxy/web_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/web_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/web_stack/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/web_stack/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/web_stack/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/galaxy/web_stack/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:38.400491 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-07 14:34:38.000000 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 14:34:38.000000 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:34:38.000000 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 14:34:38.000000 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:34:38.000000 galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-07 14:34:38.400491 galaxy_web_stack-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:31:50.000000 galaxy_web_stack-24.0.2/test-requirements.txt
```

### Comparing `galaxy_web_stack-24.0.1/HISTORY.rst` & `galaxy_web_stack-24.0.2/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_web_stack-24.0.1/LICENSE` & `galaxy_web_stack-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/PKG-INFO` & `galaxy_web_stack-24.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_web_stack-24.0.1/galaxy/web_stack/__init__.py` & `galaxy_web_stack-24.0.2/galaxy/web_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/galaxy/web_stack/gunicorn_config.py` & `galaxy_web_stack-24.0.2/galaxy/web_stack/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/galaxy/web_stack/handlers.py` & `galaxy_web_stack-24.0.2/galaxy/web_stack/handlers.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/galaxy/web_stack/message.py` & `galaxy_web_stack-24.0.2/galaxy/web_stack/message.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/galaxy/web_stack/transport.py` & `galaxy_web_stack-24.0.2/galaxy/web_stack/transport.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_stack-24.0.1/galaxy_web_stack.egg-info/PKG-INFO` & `galaxy_web_stack-24.0.2/galaxy_web_stack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_web_stack-24.0.1/setup.cfg` & `galaxy_web_stack-24.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-stack
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	SQLAlchemy>=1.4.25,<2
```

