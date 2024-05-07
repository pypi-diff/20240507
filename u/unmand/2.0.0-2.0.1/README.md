# Comparing `tmp/unmand-2.0.0.tar.gz` & `tmp/unmand-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unmand-2.0.0.tar", last modified: Wed May  1 00:56:15 2024, max compression
+gzip compressed data, was "unmand-2.0.1.tar", last modified: Wed May  1 03:08:28 2024, max compression
```

## Comparing `unmand-2.0.0.tar` & `unmand-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.073983 unmand-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 00:56:08.000000 unmand-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 00:56:15.073983 unmand-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-01 00:56:08.000000 unmand-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 00:56:08.000000 unmand-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:56:15.073983 unmand-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-01 00:56:08.000000 unmand-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.069983 unmand-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.069983 unmand-2.0.0/src/unmand/
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-01 00:56:08.000000 unmand-2.0.0/src/unmand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:56:15.073983 unmand-2.0.0/src/unmand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:56:14.000000 unmand-2.0.0/src/unmand.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 00:56:15.000000 unmand-2.0.0/src/unmand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:08:28.528980 unmand-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 03:08:24.000000 unmand-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 03:08:28.528980 unmand-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-01 03:08:24.000000 unmand-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 03:08:24.000000 unmand-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 03:08:28.528980 unmand-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-01 03:08:24.000000 unmand-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:08:28.528980 unmand-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:08:28.528980 unmand-2.0.1/src/unmand/
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-01 03:08:24.000000 unmand-2.0.1/src/unmand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 03:08:28.528980 unmand-2.0.1/src/unmand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 03:08:28.000000 unmand-2.0.1/src/unmand.egg-info/top_level.txt
```

### Comparing `unmand-2.0.0/LICENSE` & `unmand-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unmand-2.0.0/PKG-INFO` & `unmand-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmand
-Version: 2.0.0
+Version: 2.0.1
 Summary: Helper library for consuming the Unmand API
 Home-page: https://github.com/unmand-systems/unmand-python
 Author: Josiah Khor
 Author-email: josiah.khor@unmand.com
 Project-URL: Bug Tracker, https://github.com/unmand-systems/unmand-python/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unmand-2.0.0/README.md` & `unmand-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unmand-2.0.0/setup.py` & `unmand-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def readme():
     """Pull README file for long documentation string"""
     with open("README.md", "r") as f:
         return f.read()
 
 setuptools.setup(name='unmand',
-    version='2.0.0',
+    version='2.0.1',
     description='Helper library for consuming the Unmand API',
     url='https://github.com/unmand-systems/unmand-python',
     author='Josiah Khor',
     author_email='josiah.khor@unmand.com',
     long_description=readme(),
     long_description_content_type="text/markdown",
     project_urls={
```

### Comparing `unmand-2.0.0/src/unmand/__init__.py` & `unmand-2.0.1/src/unmand/__init__.py`

 * *Files identical despite different names*

### Comparing `unmand-2.0.0/src/unmand.egg-info/PKG-INFO` & `unmand-2.0.1/src/unmand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmand
-Version: 2.0.0
+Version: 2.0.1
 Summary: Helper library for consuming the Unmand API
 Home-page: https://github.com/unmand-systems/unmand-python
 Author: Josiah Khor
 Author-email: josiah.khor@unmand.com
 Project-URL: Bug Tracker, https://github.com/unmand-systems/unmand-python/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

