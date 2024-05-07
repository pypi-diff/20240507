# Comparing `tmp/avocado-framework-plugin-spawner-remote-104.0.tar.gz` & `tmp/avocado_framework_plugin_spawner_remote-105.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocado-framework-plugin-spawner-remote-104.0.tar", last modified: Tue Mar 19 14:44:20 2024, max compression
+gzip compressed data, was "avocado_framework_plugin_spawner_remote-105.0.tar", last modified: Tue May  7 18:46:16 2024, max compression
```

## Comparing `avocado-framework-plugin-spawner-remote-104.0.tar` & `avocado_framework_plugin_spawner_remote-105.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-03-19 14:44:20.535662 avocado-framework-plugin-spawner-remote-104.0/
--rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2024-02-05 17:51:31.000000 avocado-framework-plugin-spawner-remote-104.0/MANIFEST.in
--rw-r--r--   0 cleber    (1000) cleber    (1000)     1514 2024-03-19 14:44:20.534662 avocado-framework-plugin-spawner-remote-104.0/PKG-INFO
--rw-r--r--   0 cleber    (1000) cleber    (1000)     1173 2024-02-05 17:51:31.000000 avocado-framework-plugin-spawner-remote-104.0/README.rst
--rw-r--r--   0 cleber    (1000) cleber    (1000)        6 2024-03-19 14:12:03.000000 avocado-framework-plugin-spawner-remote-104.0/VERSION
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-03-19 14:44:20.534662 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/
--rw-r--r--   0 cleber    (1000) cleber    (1000)     1514 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/PKG-INFO
--rw-r--r--   0 cleber    (1000) cleber    (1000)      454 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/SOURCES.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/dependency_links.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)      146 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/entry_points.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)       40 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/requires.txt
--rw-r--r--   0 cleber    (1000) cleber    (1000)       23 2024-03-19 14:44:20.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/top_level.txt
-drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-03-19 14:44:20.534662 avocado-framework-plugin-spawner-remote-104.0/avocado_spawner_remote/
--rw-r--r--   0 cleber    (1000) cleber    (1000)     8144 2024-02-07 13:51:39.000000 avocado-framework-plugin-spawner-remote-104.0/avocado_spawner_remote/__init__.py
--rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2024-03-19 14:44:20.535662 avocado-framework-plugin-spawner-remote-104.0/setup.cfg
--rw-r--r--   0 cleber    (1000) cleber    (1000)     1894 2024-02-05 17:51:31.000000 avocado-framework-plugin-spawner-remote-104.0/setup.py
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:16.676699 avocado_framework_plugin_spawner_remote-105.0/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       16 2024-05-03 14:13:15.000000 avocado_framework_plugin_spawner_remote-105.0/MANIFEST.in
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1514 2024-05-07 18:46:16.676699 avocado_framework_plugin_spawner_remote-105.0/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1173 2024-05-03 14:13:15.000000 avocado_framework_plugin_spawner_remote-105.0/README.rst
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        6 2024-05-07 18:43:50.000000 avocado_framework_plugin_spawner_remote-105.0/VERSION
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:16.676699 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1514 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/PKG-INFO
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      454 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)        1 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)      146 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/entry_points.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       40 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/requires.txt
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       23 2024-05-07 18:46:16.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/top_level.txt
+drwxr-xr-x   0 cleber    (1000) cleber    (1000)        0 2024-05-07 18:46:16.676699 avocado_framework_plugin_spawner_remote-105.0/avocado_spawner_remote/
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     8144 2024-05-03 14:13:15.000000 avocado_framework_plugin_spawner_remote-105.0/avocado_spawner_remote/__init__.py
+-rw-r--r--   0 cleber    (1000) cleber    (1000)       38 2024-05-07 18:46:16.676699 avocado_framework_plugin_spawner_remote-105.0/setup.cfg
+-rw-r--r--   0 cleber    (1000) cleber    (1000)     1894 2024-05-03 14:13:15.000000 avocado_framework_plugin_spawner_remote-105.0/setup.py
```

### Comparing `avocado-framework-plugin-spawner-remote-104.0/PKG-INFO` & `avocado_framework_plugin_spawner_remote-105.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: avocado-framework-plugin-spawner-remote
-Version: 104.0
+Version: 105.0
 Summary: Remote (host) based spawner
 Home-page: http://avocado-framework.github.io/
 Author: Avocado Developers
 Author-email: avocado-devel@redhat.com
 Description-Content-Type: text/x-rst
-Requires-Dist: avocado-framework==104.0
+Requires-Dist: avocado-framework==105.0
 Requires-Dist: aexpect>=1.6.2
 
 =====================
 Remote Spawner Plugin
 =====================
 
 This plugin makes use of remote `aexpect
```

### Comparing `avocado-framework-plugin-spawner-remote-104.0/README.rst` & `avocado_framework_plugin_spawner_remote-105.0/README.rst`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-spawner-remote-104.0/avocado_framework_plugin_spawner_remote.egg-info/PKG-INFO` & `avocado_framework_plugin_spawner_remote-105.0/avocado_framework_plugin_spawner_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: avocado-framework-plugin-spawner-remote
-Version: 104.0
+Version: 105.0
 Summary: Remote (host) based spawner
 Home-page: http://avocado-framework.github.io/
 Author: Avocado Developers
 Author-email: avocado-devel@redhat.com
 Description-Content-Type: text/x-rst
-Requires-Dist: avocado-framework==104.0
+Requires-Dist: avocado-framework==105.0
 Requires-Dist: aexpect>=1.6.2
 
 =====================
 Remote Spawner Plugin
 =====================
 
 This plugin makes use of remote `aexpect
```

### Comparing `avocado-framework-plugin-spawner-remote-104.0/avocado_spawner_remote/__init__.py` & `avocado_framework_plugin_spawner_remote-105.0/avocado_spawner_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `avocado-framework-plugin-spawner-remote-104.0/setup.py` & `avocado_framework_plugin_spawner_remote-105.0/setup.py`

 * *Files identical despite different names*

