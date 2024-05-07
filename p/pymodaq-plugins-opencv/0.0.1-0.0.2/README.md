# Comparing `tmp/pymodaq_plugins_opencv-0.0.1.tar.gz` & `tmp/pymodaq_plugins_opencv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_opencv-0.0.1.tar", last modified: Fri Oct  6 11:11:50 2023, max compression
+gzip compressed data, was "pymodaq_plugins_opencv-0.0.2.tar", last modified: Tue May  7 14:07:49 2024, max compression
```

## Comparing `pymodaq_plugins_opencv-0.0.1.tar` & `pymodaq_plugins_opencv-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.254091 pymodaq_plugins_opencv-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 11:11:50.254091 pymodaq_plugins_opencv-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.242091 pymodaq_plugins_opencv-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.246091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.246091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_move_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.246091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.246091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/daq_2Dviewer_OpenCV.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/extensions/myextension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/hardware/opencv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/models/PIDModelTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.250091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/resources/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/resources/config_template.toml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-06 11:11:37.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 11:11:50.246091 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-06 11:11:50.000000 pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.644291 pymodaq_plugins_opencv-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-07 14:07:49.644291 pymodaq_plugins_opencv-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:07:49.644291 pymodaq_plugins_opencv-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.636292 pymodaq_plugins_opencv-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_move_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/daq_2Dviewer_OpenCV.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/extensions/myextension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/hardware/opencv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/models/PIDModelTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.640292 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/resources/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/resources/config_template.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 14:07:42.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:07:49.644291 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 14:07:49.000000 pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_opencv-0.0.1/LICENSE` & `pymodaq_plugins_opencv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_opencv-0.0.1/PKG-INFO` & `pymodaq_plugins_opencv-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_opencv
-Version: 0.0.1
+Version: 0.0.2
 Summary: plugin to use camera instrumented using the opencv library
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_opencv
 Author: Sebastien J. Weber
 Author-email: sebastien.weber@cnrs.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,17 @@
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: pymodaq>=4.0.0
+Requires-Dist: opencv-python
 
 pymodaq_plugins_opencv
 ######################
 
 .. the following must be adapted to your developped package, links to pypi, github  description...
 
 .. image:: https://img.shields.io/pypi/v/pymodaq_plugins_opencv.svg
@@ -39,26 +42,14 @@
 
 
 Authors
 =======
 
 * Sebastien J. Weber  (sebastien.weber@cnrs.fr)
 
-.. if needed use this field
-
-    Contributors
-    ============
-
-    * First Contributor
-    * Other Contributors
-
-.. if needed use this field
-
-  Depending on the plugin type, delete/complete the fields below
-
 
 Instruments
 ===========
 
 Below is the list of instruments included in this plugin
 
 Viewer2D
```

### Comparing `pymodaq_plugins_opencv-0.0.1/README.rst` & `pymodaq_plugins_opencv-0.0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -19,26 +19,14 @@
 
 
 Authors
 =======
 
 * Sebastien J. Weber  (sebastien.weber@cnrs.fr)
 
-.. if needed use this field
-
-    Contributors
-    ============
-
-    * First Contributor
-    * Other Contributors
-
-.. if needed use this field
-
-  Depending on the plugin type, delete/complete the fields below
-
 
 Instruments
 ===========
 
 Below is the list of instruments included in this plugin
 
 Viewer2D
```

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/daq_2Dviewer_OpenCV.py` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/daq_viewer_plugins/plugins_2D/daq_2Dviewer_OpenCV.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/extensions/myextension.py` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/extensions/myextension.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/hardware/opencv.py` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/hardware/opencv.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv/models/PIDModelTemplate.py` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv/models/PIDModelTemplate.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/PKG-INFO` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq-plugins-opencv
-Version: 0.0.1
+Name: pymodaq_plugins_opencv
+Version: 0.0.2
 Summary: plugin to use camera instrumented using the opencv library
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_opencv
 Author: Sebastien J. Weber
 Author-email: sebastien.weber@cnrs.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,17 @@
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 License-File: LICENSE
+Requires-Dist: toml
+Requires-Dist: pymodaq>=4.0.0
+Requires-Dist: opencv-python
 
 pymodaq_plugins_opencv
 ######################
 
 .. the following must be adapted to your developped package, links to pypi, github  description...
 
 .. image:: https://img.shields.io/pypi/v/pymodaq_plugins_opencv.svg
@@ -39,26 +42,14 @@
 
 
 Authors
 =======
 
 * Sebastien J. Weber  (sebastien.weber@cnrs.fr)
 
-.. if needed use this field
-
-    Contributors
-    ============
-
-    * First Contributor
-    * Other Contributors
-
-.. if needed use this field
-
-  Depending on the plugin type, delete/complete the fields below
-
 
 Instruments
 ===========
 
 Below is the list of instruments included in this plugin
 
 Viewer2D
```

### Comparing `pymodaq_plugins_opencv-0.0.1/src/pymodaq_plugins_opencv.egg-info/SOURCES.txt` & `pymodaq_plugins_opencv-0.0.2/src/pymodaq_plugins_opencv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

