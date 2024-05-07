# Comparing `tmp/galaxy_web_framework-24.0.1.tar.gz` & `tmp/galaxy_web_framework-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_web_framework-24.0.1.tar", last modified: Thu May  2 13:49:22 2024, max compression
+gzip compressed data, was "galaxy_web_framework-24.0.2.tar", last modified: Tue May  7 14:34:29 2024, max compression
```

## Comparing `galaxy_web_framework-24.0.1.tar` & `galaxy_web_framework-24.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/form_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.534112 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38863 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.538112 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/proxy/js/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/galaxy/web/statsd_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:49:22.000000 galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-02 13:49:22.542112 galaxy_web_framework-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_web_framework-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.176555 galaxy_web_framework-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_web_framework-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-07 14:34:29.176555 galaxy_web_framework-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.168556 galaxy_web_framework-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.168556 galaxy_web_framework-24.0.2/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.168556 galaxy_web_framework-24.0.2/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21864 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.168556 galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38863 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/proxy/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:34:29.172556 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-07 14:34:29.000000 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-07 14:34:29.000000 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:34:29.000000 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 14:34:29.000000 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:34:29.000000 galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-07 14:34:29.176555 galaxy_web_framework-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_web_framework-24.0.2/test-requirements.txt
```

### Comparing `galaxy_web_framework-24.0.1/HISTORY.rst` & `galaxy_web_framework-24.0.2/HISTORY.rst`

 * *Files 1% similar despite different names*

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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_web_framework-24.0.1/LICENSE` & `galaxy_web_framework-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/PKG-INFO` & `galaxy_web_framework-24.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,20 @@
 
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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/__init__.py` & `galaxy_web_framework-24.0.2/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/__init__.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/base.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/base.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/decorators.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/__init__.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/grids.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/helpers/tags.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/error.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/error.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/profile.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/remoteuser.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/remoteuser.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/sqldebug.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/sqldebug.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/static.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/static.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/statsd.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/statsd.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/translogger.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/translogger.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy_web_framework-24.0.2/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/legacy_framework/grids.py` & `galaxy_web_framework-24.0.2/galaxy/web/legacy_framework/grids.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/proxy/__init__.py` & `galaxy_web_framework-24.0.2/galaxy/web/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/Dockerfile` & `galaxy_web_framework-24.0.2/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/main.js` & `galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/mapper.js` & `galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/proxy/js/lib/proxy.js` & `galaxy_web_framework-24.0.2/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy/web/statsd_client.py` & `galaxy_web_framework-24.0.2/galaxy/web/statsd_client.py`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,20 @@
 
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
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_web_framework-24.0.1/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy_web_framework-24.0.2/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_web_framework-24.0.1/setup.cfg` & `galaxy_web_framework-24.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-framework
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 	babel
```

