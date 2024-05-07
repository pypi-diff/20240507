# Comparing `tmp/galaxy_tours-24.0.1.tar.gz` & `tmp/galaxy_tours-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_tours-24.0.1.tar", last modified: Thu May  2 13:48:37 2024, max compression
+gzip compressed data, was "galaxy_tours-24.0.2.tar", last modified: Tue May  7 14:33:42 2024, max compression
```

## Comparing `galaxy_tours-24.0.1.tar` & `galaxy_tours-24.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/galaxy/tours/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/tours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/tours/_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/tours/_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/tours/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/galaxy/tours/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/galaxy_tours.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:37.000000 galaxy_tours-24.0.1/galaxy_tours.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 13:48:37.029835 galaxy_tours-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_tours-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:42.852895 galaxy_tours-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_tours-24.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-07 14:33:42.852895 galaxy_tours-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:42.848895 galaxy_tours-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:42.848895 galaxy_tours-24.0.2/galaxy/tours/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/tours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/tours/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/tours/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/tours/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/galaxy/tours/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:42.852895 galaxy_tours-24.0.2/galaxy_tours.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:33:42.000000 galaxy_tours-24.0.2/galaxy_tours.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-07 14:33:42.852895 galaxy_tours-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_tours-24.0.2/test-requirements.txt
```

### Comparing `galaxy_tours-24.0.1/HISTORY.rst` & `galaxy_tours-24.0.2/HISTORY.rst`

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

### Comparing `galaxy_tours-24.0.1/LICENSE.txt` & `galaxy_tours-24.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy_tours-24.0.1/PKG-INFO` & `galaxy_tours-24.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,20 @@
 
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

### Comparing `galaxy_tours-24.0.1/galaxy/tours/_impl.py` & `galaxy_tours-24.0.2/galaxy/tours/_impl.py`

 * *Files identical despite different names*

### Comparing `galaxy_tours-24.0.1/galaxy/tours/_schema.py` & `galaxy_tours-24.0.2/galaxy/tours/_schema.py`

 * *Files identical despite different names*

### Comparing `galaxy_tours-24.0.1/galaxy/tours/validate.py` & `galaxy_tours-24.0.2/galaxy/tours/validate.py`

 * *Files identical despite different names*

### Comparing `galaxy_tours-24.0.1/galaxy_tours.egg-info/PKG-INFO` & `galaxy_tours-24.0.2/galaxy_tours.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,20 @@
 
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

### Comparing `galaxy_tours-24.0.1/setup.cfg` & `galaxy_tours-24.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tours
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	pydantic>=2,!=2.6.0,!=2.6.1
 	PyYAML
```

