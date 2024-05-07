# Comparing `tmp/pymodaq_plugins_bnc-0.0.4.tar.gz` & `tmp/pymodaq_plugins_bnc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_bnc-0.0.4.tar", last modified: Tue May  7 07:33:12 2024, max compression
+gzip compressed data, was "pymodaq_plugins_bnc-0.0.5.tar", last modified: Tue May  7 07:48:34 2024, max compression
```

## Comparing `pymodaq_plugins_bnc-0.0.4.tar` & `pymodaq_plugins_bnc-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/plugin_info.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.578198 pymodaq_plugins_bnc-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.582198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/bnc_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/models/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/resources/config_template.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/scanners/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:33:12.000000 pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:33:12.586198 pymodaq_plugins_bnc-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-07 07:32:41.000000 pymodaq_plugins_bnc-0.0.4/tests/test_plugin_package_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/plugin_info.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.703225 pymodaq_plugins_bnc-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.707225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/bnc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/resources/config_template.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 07:48:34.000000 pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:48:34.711225 pymodaq_plugins_bnc-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-07 07:48:04.000000 pymodaq_plugins_bnc-0.0.5/tests/test_plugin_package_structure.py
```

### Comparing `pymodaq_plugins_bnc-0.0.4/LICENSE` & `pymodaq_plugins_bnc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/PKG-INFO` & `pymodaq_plugins_bnc-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_bnc
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
+Home-page: https://github.com/ccabello99/pymodaq_plugins_bnc
 Author: Christian Cabello
 Author-email: christian.cabello@ip-paris.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymodaq_plugins_bnc-0.0.4/README.rst` & `pymodaq_plugins_bnc-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/plugin_info.toml` & `pymodaq_plugins_bnc-0.0.5/plugin_info.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## To modify by developer(s) of the plugin
 
 [plugin-info]
 SHORT_PLUGIN_NAME = 'bnc'
 
-package-url = 'https://github.com/PyMoDAQ/pymodaq_plugins_bnc' #to modify
+package-url = 'https://github.com/ccabello99/pymodaq_plugins_bnc' #to modify
 description = 'PyMoDAQ module for communication and readout from BNC575 delay/signal generator'
 
 author = 'Christian Cabello'
 author-email = 'christian.cabello@ip-paris.fr'
 license = 'MIT'
 
 [plugin-install]
```

### Comparing `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py` & `pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/daq_move_plugins/daq_move_bnc.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/bnc_commands.py` & `pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/bnc_commands.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc/hardware/device.py` & `pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc/hardware/device.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/PKG-INFO` & `pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_bnc
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyMoDAQ module for communication and readout from BNC575 delay/signal generator
-Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_bnc
+Home-page: https://github.com/ccabello99/pymodaq_plugins_bnc
 Author: Christian Cabello
 Author-email: christian.cabello@ip-paris.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymodaq_plugins_bnc-0.0.4/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt` & `pymodaq_plugins_bnc-0.0.5/src/pymodaq_plugins_bnc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_bnc-0.0.4/tests/test_plugin_package_structure.py` & `pymodaq_plugins_bnc-0.0.5/tests/test_plugin_package_structure.py`

 * *Files identical despite different names*

