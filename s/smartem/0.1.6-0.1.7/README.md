# Comparing `tmp/smartem-0.1.6.tar.gz` & `tmp/smartem-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartem-0.1.6.tar", last modified: Wed Jun 21 13:19:57 2023, max compression
+gzip compressed data, was "smartem-0.1.7.tar", last modified: Tue May  7 12:50:21 2024, max compression
```

## Comparing `smartem-0.1.6.tar` & `smartem-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.934579 smartem-0.1.6/
--rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.6/LICENSE
--rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-21 13:19:57.934646 smartem-0.1.6/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.6/README.rst
--rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.6/pyproject.toml
--rw-r--r--   0 kif41228   (504) staff       (20)     1224 2023-06-21 13:19:57.935057 smartem-0.1.6/setup.cfg
--rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.6/setup.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.925536 smartem-0.1.6/src/
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.926955 smartem-0.1.6/src/smartem/
--rw-r--r--   0 kif41228   (504) staff       (20)      212 2023-06-21 13:19:25.000000 smartem-0.1.6/src/smartem/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.929983 smartem-0.1.6/src/smartem/cli/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/change_epu_directory.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/initialise.py
--rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/launch.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/missing.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1136 2023-06-15 15:34:04.000000 smartem-0.1.6/src/smartem/cli/quick_epu_viewer.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/start.py
--rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/cli/stop.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.930878 smartem-0.1.6/src/smartem/data_model/
--rw-r--r--   0 kif41228   (504) staff       (20)     7130 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/data_model/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/data_model/construct.py
--rw-r--r--   0 kif41228   (504) staff       (20)    35995 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/data_model/extract.py
--rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/data_model/structure.py
--rw-r--r--   0 kif41228   (504) staff       (20)    14708 2023-06-15 09:29:29.000000 smartem-0.1.6/src/smartem/data_model/torch.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.931183 smartem-0.1.6/src/smartem/gui/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.932859 smartem-0.1.6/src/smartem/gui/qt/
--rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/component_tab.py
--rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/display.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/image_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/loader.py
--rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/loader_csv.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/plotting_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/gui/qt/qt_style.css
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.934161 smartem-0.1.6/src/smartem/parsing/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/parsing/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)    19542 2023-06-15 09:29:29.000000 smartem-0.1.6/src/smartem/parsing/epu.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12836 2023-06-21 13:19:14.000000 smartem-0.1.6/src/smartem/parsing/epu_vis.py
--rw-r--r--   0 kif41228   (504) staff       (20)    13637 2023-05-15 12:06:59.000000 smartem-0.1.6/src/smartem/parsing/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     5608 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/parsing/relion_default.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/parsing/star.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.6/src/smartem/stage_model.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.928367 smartem-0.1.6/src/smartem.egg-info/
--rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1286 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/SOURCES.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/dependency_links.txt
--rw-r--r--   0 kif41228   (504) staff       (20)      372 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/entry_points.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.6/src/smartem.egg-info/not-zip-safe
--rw-r--r--   0 kif41228   (504) staff       (20)       95 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/requires.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        8 2023-06-21 13:19:57.000000 smartem-0.1.6/src/smartem.egg-info/top_level.txt
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-21 13:19:57.934340 smartem-0.1.6/tests/
--rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.6/tests/test_stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.747363 smartem-0.1.7/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.7/LICENSE
+-rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 12:50:21.746528 smartem-0.1.7/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.7/README.rst
+-rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.7/pyproject.toml
+-rw-r--r--   0 kif41228   (504) staff       (20)     1224 2024-05-07 12:50:21.749876 smartem-0.1.7/setup.cfg
+-rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.7/setup.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.639594 smartem-0.1.7/src/
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.646987 smartem-0.1.7/src/smartem/
+-rw-r--r--   0 kif41228   (504) staff       (20)      212 2024-05-07 12:48:41.000000 smartem-0.1.7/src/smartem/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.659927 smartem-0.1.7/src/smartem/cli/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/change_epu_directory.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/initialise.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/launch.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/missing.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1577 2023-07-11 12:47:43.000000 smartem-0.1.7/src/smartem/cli/quick_epu_viewer.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/start.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/stop.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.663539 smartem-0.1.7/src/smartem/data_model/
+-rw-r--r--   0 kif41228   (504) staff       (20)     7267 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/data_model/construct.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    37096 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/extract.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/data_model/structure.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    23224 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/torch.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.664131 smartem-0.1.7/src/smartem/gui/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.731578 smartem-0.1.7/src/smartem/gui/qt/
+-rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/component_tab.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/display.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/image_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/loader.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/loader_csv.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/plotting_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/qt_style.css
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.743826 smartem-0.1.7/src/smartem/parsing/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/parsing/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    19626 2024-05-07 12:47:34.000000 smartem-0.1.7/src/smartem/parsing/epu.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    15129 2024-01-05 11:06:15.000000 smartem-0.1.7/src/smartem/parsing/epu_vis.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    15154 2024-05-07 12:46:26.000000 smartem-0.1.7/src/smartem/parsing/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     7093 2024-01-05 11:20:56.000000 smartem-0.1.7/src/smartem/parsing/relion_default.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/parsing/star.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.745636 smartem-0.1.7/src/smartem.egg-info/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1286 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/SOURCES.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/dependency_links.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)      372 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/entry_points.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.7/src/smartem.egg-info/not-zip-safe
+-rw-r--r--   0 kif41228   (504) staff       (20)       95 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/requires.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        8 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/top_level.txt
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.744589 smartem-0.1.7/tests/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.7/tests/test_stage_model.py
```

### Comparing `smartem-0.1.6/LICENSE` & `smartem-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/PKG-INFO` & `smartem-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: gemmi
+Requires-Dist: matplotlib
+Requires-Dist: xmltodict
+Requires-Dist: mrcfile
+Requires-Dist: pyyaml
+Requires-Dist: psycopg2
+Requires-Dist: sqlalchemy<2.0
+Requires-Dist: PyQt5
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: tifffile
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
 
 
 Installation
```

### Comparing `smartem-0.1.6/README.rst` & `smartem-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/setup.cfg` & `smartem-0.1.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartem
-version = 0.1.6
+version = 0.1.7
 description = Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 long_description = file: README.rst
 license_file = LICENSE
 
 [options]
 include_package_data = True
 install_requires =
```

### Comparing `smartem-0.1.6/src/smartem/cli/change_epu_directory.py` & `smartem-0.1.7/src/smartem/cli/change_epu_directory.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/cli/export.py` & `smartem-0.1.7/src/smartem/cli/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/cli/initialise.py` & `smartem-0.1.7/src/smartem/cli/initialise.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/cli/missing.py` & `smartem-0.1.7/src/smartem/cli/missing.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/cli/quick_epu_viewer.py` & `smartem-0.1.7/src/smartem/cli/quick_epu_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,32 @@
     parser.add_argument(
         "--grid-square",
         type=int,
         help="Grid square EPU ID",
         dest="grid_square",
         default=0,
     )
+    parser.add_argument(
+        "--switch-xy",
+        help="Switch the x and y axes in display",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
+        "--flip-x",
+        help="Flip x axis in display",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
+        "--flip-y",
+        help="Flip y axis in display",
+        action="store_true",
+        default=False,
+    )
     args = parser.parse_args()
 
     if args.atlas_dir and args.sample is None:
         exit("If --atlas-dir is specified then --sample must also be specified")
 
     if args.atlas_dir:
         a = Atlas(Path(args.atlas_dir), args.sample, epu_data_dir=Path(args.epu_dir))
```

### Comparing `smartem-0.1.6/src/smartem/cli/start.py` & `smartem-0.1.7/src/smartem/cli/start.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/cli/stop.py` & `smartem-0.1.7/src/smartem/cli/stop.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/data_model/__init__.py` & `smartem-0.1.7/src/smartem/data_model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 from pathlib import Path
-from typing import Any, List, Optional, Type, Union, cast
+from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Type, Union, cast
 
 import yaml
 from sqlalchemy import Column
 from sqlalchemy import Float as Float_org
 from sqlalchemy import ForeignKey, Integer, Text, create_engine, inspect
 from sqlalchemy.exc import ProgrammingError
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.type_api import TypeEngine
 
+
+class PhysicalSubset(NamedTuple):
+    pixel_sizes: Dict[str, float]
+    sub_sample_size: Tuple[float, float]
+
+
 # this is a mypy workaround suggeted in https://github.com/dropbox/sqlalchemy-stubs/issues/178
 Float = cast(Type[TypeEngine[float]], Float_org)
 
 Base: Any = declarative_base()
 
 
 class EPUImage:
```

### Comparing `smartem-0.1.6/src/smartem/data_model/construct.py` & `smartem-0.1.7/src/smartem/data_model/construct.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/data_model/extract.py` & `smartem-0.1.7/src/smartem/data_model/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Any, List, Optional, Sequence, Set, Tuple, Type, Union
 
 from sqlalchemy import create_engine, delete, select
 from sqlalchemy.dialects.postgresql import insert
-from sqlalchemy.engine.row import LegacyRow
+from sqlalchemy.engine.row import LegacyRow, Row
 from sqlalchemy.orm import Load, load_only, sessionmaker
 
 from smartem.data_model import (
     Atlas,
     Base,
     Exposure,
     ExposureInfo,
     FoilHole,
     GridSquare,
     Particle,
     ParticleInfo,
     ParticleSet,
     ParticleSetInfo,
     ParticleSetLinker,
+    PhysicalSubset,
     Project,
     Tile,
     url,
 )
 from smartem.data_model.construct import linear_joins, table_chain
 
 
@@ -101,14 +102,41 @@
         if not updated_values:
             return
         self.session.query(Atlas).filter(Atlas.atlas_id == atlas_id).update(
             updated_values
         )
         self.session.commit()
 
+    def get_physical_subset(
+        self, project: str, subset_shape: Tuple[float, float]
+    ) -> PhysicalSubset:
+        end: Type[Base] = Tile
+        tables = table_chain(GridSquare, end)
+        tables.append(Project)
+        query = linear_joins(self.session, tables, skip=[Project])
+        query = query.join(Project, Project.atlas_id == Tile.atlas_id).filter(
+            Project.project_name == project
+        )
+        grid_square_res: Row = query.first()
+        grid_square = grid_square_res[0]
+        assert isinstance(grid_square, GridSquare)
+        end = FoilHole
+        primary_filter = grid_square.grid_square_name
+        tables = table_chain(FoilHole, end)
+        query = linear_joins(self.session, tables, primary_filter=primary_filter)
+        foil_hole = query.first()
+        assert isinstance(foil_hole, FoilHole)
+        return PhysicalSubset(
+            pixel_sizes={
+                "grid_square": grid_square.pixel_size,
+                "foil_hole": foil_hole.pixel_size,
+            },
+            sub_sample_size=subset_shape,
+        )
+
     def get_tile(
         self,
         stage_position: Tuple[float, float],
         atlas_id: Optional[int] = None,
         project: str = "",
     ) -> Optional[Tile]:
         if atlas_id is None and project:
```

### Comparing `smartem-0.1.6/src/smartem/data_model/structure.py` & `smartem-0.1.7/src/smartem/data_model/structure.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/data_model/torch.py` & `smartem-0.1.7/src/smartem/parsing/epu_vis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,365 +1,413 @@
-import functools
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple
+from typing import Tuple
 
+import matplotlib.pyplot as plt
 import mrcfile
 import numpy as np
-import pandas as pd
-import tifffile
-import yaml
-from PIL import Image
-from torch import Tensor, from_numpy, reshape
-from torch.utils.data import DataLoader
-from torchvision.io import read_image
-
-from smartem.data_model.extract import DataAPI
-from smartem.parsing.epu import calibrate_coordinate_system
-from smartem.parsing.export import get_dataframe
-from smartem.stage_model import StageCalibration, find_point_pixel
-
-
-@functools.lru_cache(maxsize=50)
-def mrc_to_tensor(mrc_file: Path) -> Tensor:
-    with mrcfile.open(mrc_file) as mrc:
-        data = mrc.data
-    shape = data.shape
-    if data.dtype.char in np.typecodes["AllInteger"]:
-        tensor_2d = Tensor(data.astype(np.int16))
-    else:
-        tensor_2d = Tensor(data.astype(np.float16))
-    return reshape(tensor_2d, (1, shape[0], shape[1]))
-
-
-@functools.lru_cache(maxsize=50)
-def tiff_to_tensor(tiff_file: Path) -> Tensor:
-    data = tifffile.imread(tiff_file)
-    shape = data.shape
-    if data.dtype.char in np.typecodes["AllInteger"]:
-        tensor_2d = Tensor(data.astype(np.int16))
-    else:
-        tensor_2d = Tensor(data.astype(np.float16))
-    return reshape(tensor_2d, (1, shape[0], shape[1]))
 
+from smartem.parsing.epu import (
+    metadata_foil_hole_positions,
+    metadata_foil_hole_stage,
+    metadata_grid_square_positions,
+    metadata_grid_square_stage,
+    parse_epu_xml,
+)
 
-class SmartEMDataLoader(DataLoader):
+
+class Atlas:
     def __init__(
         self,
-        level: str,
-        full_res: bool = False,
-        num_samples: int = 0,
-        sub_sample_size: Optional[Tuple[int, int]] = None,
-        allowed_labels: Optional[Dict[str, bool]] = None,
-        seed: int = 0,
+        atlas_epu_dir: Path,
+        sample: int,
+        epu_data_dir: Path | None = None,
+        flip: Tuple[bool, bool] = (False, False),
+        switch: bool = False,
     ):
-        np.random.seed(seed)
-        self._level = level
-        self._use_full_res = full_res
-        self._num_samples = num_samples
-        self._sub_sample_size = sub_sample_size or (256, 256)
-        self._allowed_labels = allowed_labels or list(_standard_labels.keys())
-        self._lower_better_label = (
-            [allowed_labels[k] for k in self._allowed_labels]
-            if allowed_labels
-            else [_standard_labels[k] for k in self._allowed_labels]
-        )
-        if self._level not in ("grid_square", "foil_hole"):
-            raise ValueError(
-                f"Unrecognised SmartEMDataLoader level {self._level}: accepted values are grid_square or foil_hole"
-            )
-
-        self._full_res_extension = ""
-        self._data_dir = Path("/")
-        self._df = pd.DataFrame()
-
-    def _determine_extension(self):
-        if Path(self._df.iloc[0]["grid_square"]).with_suffix(".mrc").exists():
-            self._full_res_extension = ".mrc"
-        elif Path(self._df.iloc[0]["grid_square"]).with_suffix(".tiff").exists():
-            self._full_res_extension = ".tiff"
-        elif Path(self._df.iloc[0]["grid_square"]).with_suffix(".tif").exists():
-            self._full_res_extension = ".tif"
+        atlas_epu_dir = Path(atlas_epu_dir)
+        self._epu_data_dir = epu_data_dir
+        self._atlas_location = atlas_epu_dir / f"Sample{sample}" / "Atlas"
+        if (self._atlas_location / "Atlas_1.xml").is_file():
+            epu_data = parse_epu_xml(self._atlas_location / "Atlas_1.xml")
         else:
-            self._full_res_extension = ""
-        if self._level == "foil_hole":
-            self._df = self._df[self._df["foil_hole"].notna()]
-        if self._full_res_extension in (".tiff", ".tif"):
-            tiff_file = (self._data_dir / self._df.iloc[0]["grid_square"]).with_suffix(
-                self._full_res_extension
-            )
-            self._gs_full_res_size = tifffile.imread(tiff_file).shape
-        else:
-            with mrcfile.open(
-                (self._data_dir / self._df.iloc[0]["grid_square"]).with_suffix(".mrc")
-            ) as _mrc:
-                self._gs_full_res_size = _mrc.data.shape
-        with Image.open(self._data_dir / self._df.iloc[0]["grid_square"]) as im:
-            self._gs_jpeg_size = im.size
-        if self._use_full_res:
-            self._boundary_points_x = np.random.randint(
-                self._gs_full_res_size[1] - self._sub_sample_size[0], size=len(self)
-            )
-            self._boundary_points_y = np.random.randint(
-                self._gs_full_res_size[0] - self._sub_sample_size[1], size=len(self)
-            )
+            epu_data = parse_epu_xml(list(self._atlas_location.glob("Atlas_*.xml"))[0])
+        self._pixel_size = epu_data["pixel_size"]
+        self._readout_area = epu_data["readout_area"]
+        self._grid_square_positions = metadata_grid_square_positions(
+            self._atlas_location / "Atlas.dm"
+        )
+        self._flip = flip
+        self._switch = switch
+        self._flip_powers = (1 if flip[0] else 2, 1 if flip[1] else 2)
+        self._switch_indices = (0 if switch else 1, 1 if switch else 0)
+
+    @property
+    def image(self) -> np.array:
+        if (self._atlas_location / "Atlas_1.mrc").is_file():
+            atlasf = self._atlas_location / "Atlas_1.mrc"
         else:
-            self._boundary_points_x = np.random.randint(
-                self._gs_jpeg_size[0] - self._sub_sample_size[0], size=len(self)
+            atlasf = list(self._atlas_location.glob("Atlas_*.mrc"))[0]
+        with mrcfile.open(atlasf) as mrc:
+            data = mrc.data
+        return data
+
+    @property
+    def _grid_square_stage_locations(self) -> dict:
+        return metadata_grid_square_stage(self._atlas_location / "Atlas.dm")
+
+    def stage_correction(self):
+        vals_x = []
+        vals_y = []
+        stage = self._grid_square_stage_locations
+        for gs, c in self._grid_square_positions.items():
+            stage_x = (
+                int((-stage[gs][0]) / self._pixel_size) + self._readout_area[0] // 2
             )
-            self._boundary_points_y = np.random.randint(
-                self._gs_jpeg_size[1] - self._sub_sample_size[1], size=len(self)
+            vals_x.append(stage_x - c[0])
+            stage_y = (
+                int((stage[gs][1]) / self._pixel_size) + self._readout_area[1] // 2
             )
+            vals_y.append(stage_y - c[1])
+        return ((np.mean(vals_x), np.std(vals_x)), (np.mean(vals_y), np.std(vals_y)))
+
+    def display(
+        self,
+        show_squares: bool = True,
+        show_stage_positions: bool = True,
+    ):
+
+        corrected_center = ((0, 0), (0, 0))
 
-    def __len__(self) -> int:
-        if self._level == "grid_square" and self._num_samples:
-            return self._df[self._level].nunique() * self._num_samples
-        return self._df[self._level].nunique()
-
-    def __getitem__(self, idx: int) -> Tuple[Tensor, List[float]]:
-        sub_sample_boundaries = (-1, -1)
-        if self._level == "grid_square" and self._num_samples:
-            sub_sample_boundaries = (
-                self._boundary_points_x[idx],
-                self._boundary_points_y[idx],
+        # fig, ax = plt.subplots(1, figsize=(12, 6))
+        fig = plt.figure(1)
+        ax = fig.gca()
+        ax.imshow(self.image)
+
+        self._readout_area = self.image.shape
+
+        annot = ax.annotate(
+            "Grid square ID: ", xy=(0, 0), xytext=(5, 5), textcoords="offset points"
+        )
+        annot.set_visible(False)
+
+        labels: dict = {}
+        scatters: dict = {}
+        lines: dict = {}
+        lines_list: list = []
+
+        def hover(event):
+            if event.inaxes == ax:
+                for sc, c in scatters.items():
+                    cont, ind = sc.contains(event)
+                    if cont:
+                        # annot.xy = (event.xdata, event.ydata)
+                        annot_text = f"Grid square ID: {', '.join([str(labels[sc][n]) for n in ind['ind']])}"
+                        annot.set_text(annot_text)
+                        annot.set_color(c)
+                        annot.set_visible(True)
+                        break
+                    else:
+                        annot.set_visible(False)
+                fig.canvas.draw()
+
+        def click(event):
+            if event.inaxes == ax:
+                for sc, c in scatters.items():
+                    cont, ind = sc.contains(event)
+                    if cont and self._epu_data_dir:
+                        try:
+                            gs = GridSquare(
+                                self._epu_data_dir,
+                                int(labels[sc][ind["ind"][0]]),
+                                flip=self._flip,
+                                switch=self._switch,
+                            )
+                        except IndexError:
+                            print(
+                                f"No grid square mag image found for {labels[sc][ind['ind'][0]]}"
+                            )
+                            return
+                        gs.display()
+
+        def on_pick(event):
+            legline = event.artist
+            origline = lines[legline]
+            visible = not origline.get_visible()
+            origline.set_visible(visible)
+            legline.set_alpha(1.0 if visible else 0.2)
+            fig.canvas.draw()
+
+        if show_squares:
+            squares_sc = ax.scatter(
+                [p[0] for p in self._grid_square_positions.values()],
+                [p[1] for p in self._grid_square_positions.values()],
+                marker="x",
+                color="green",
+                label="Pixel",
             )
-            grid_square_idx = idx // self._num_samples
-            _grid_squares = self._df["grid_square"].unique()
-            selected_df = self._df[
-                self._df["grid_square"] == _grid_squares[grid_square_idx]
-            ]
-            drop_indices = []
-            if self._use_full_res:
-                for ri, row in selected_df.iterrows():
-                    fh_centre = find_point_pixel(
-                        (
-                            row["foil_hole_x"],
-                            row["foil_hole_y"],
-                        ),
-                        (row["grid_square_x"], row["grid_square_y"]),
-                        row["grid_square_pixel_size"],
-                        (self._gs_full_res_size[1], self._gs_full_res_size[0]),
-                        xfactor=-1 if self._stage_calibration.x_flip else 1,
-                        yfactor=-1 if self._stage_calibration.y_flip else 1,
+            scatters[squares_sc] = "green"
+            labels[squares_sc] = list(self._grid_square_positions.keys())
+            lines_list.append(squares_sc)
+
+        if show_stage_positions:
+            stage_data = self._grid_square_stage_locations
+            keys = list(stage_data.keys())
+            gs = keys[0]
+            stage_sc = ax.scatter(
+                [
+                    int(
+                        (((-1) ** self._flip_powers[0]) * p[self._switch_indices[0]])
+                        / self._pixel_size
                     )
-                    if self._stage_calibration.inverted:
-                        fh_centre = (fh_centre[1], fh_centre[0])
-                    if (
-                        fh_centre[0] < sub_sample_boundaries[0]
-                        or fh_centre[1] < sub_sample_boundaries[1]
-                        or fh_centre[0]
-                        > sub_sample_boundaries[0] + self._sub_sample_size[0]
-                        or fh_centre[1]
-                        > sub_sample_boundaries[1] + self._sub_sample_size[1]
-                    ):
-                        drop_indices.append(ri)
-            else:
-                for ri, row in selected_df.iterrows():
-                    fh_centre = find_point_pixel(
-                        (
-                            row["foil_hole_x"],
-                            row["foil_hole_y"],
-                        ),
-                        (row["grid_square_x"], row["grid_square_y"]),
-                        row["grid_square_pixel_size"]
-                        * (self._gs_full_res_size[1] / self._gs_jpeg_size[0]),
-                        self._gs_jpeg_size,
-                        xfactor=-1 if self._stage_calibration.x_flip else 1,
-                        yfactor=-1 if self._stage_calibration.y_flip else 1,
+                    - corrected_center[0][0]
+                    + self._readout_area[1] // 2
+                    for p in stage_data.values()
+                ],
+                [
+                    int(
+                        ((-1) ** self._flip_powers[1])
+                        * p[self._switch_indices[1]]
+                        / self._pixel_size
                     )
-                    if self._stage_calibration.inverted:
-                        fh_centre = (fh_centre[1], fh_centre[0])
-                    if (
-                        fh_centre[0] < sub_sample_boundaries[0]
-                        or fh_centre[1] < sub_sample_boundaries[1]
-                        or fh_centre[0]
-                        > sub_sample_boundaries[0] + self._sub_sample_size[0]
-                        or fh_centre[1]
-                        > sub_sample_boundaries[1] + self._sub_sample_size[1]
-                    ):
-                        drop_indices.append(ri)
-            selected_df = selected_df.drop(drop_indices)
-            averaged_df = selected_df.groupby("grid_square").mean()
-            if len(averaged_df):
-                labels = [
-                    v
-                    for k, v in averaged_df.iloc[0].to_dict().items()
-                    if k in self._allowed_labels
-                ]
-            else:
-                labels = [np.inf if b else -np.inf for b in self._lower_better_label]
-            if self._use_full_res:
-                if self._full_res_extension == ".mrc":
-                    preimage = mrc_to_tensor(
-                        (self._data_dir / _grid_squares[grid_square_idx]).with_suffix(
-                            ".mrc"
-                        )
-                    )
-                elif self._full_res_extension in (".tiff", ".tif"):
-                    preimage = tiff_to_tensor(
-                        (self._data_dir / _grid_squares[grid_square_idx]).with_suffix(
-                            self._full_res_extension
+                    + corrected_center[1][0]
+                    + self._readout_area[0] // 2
+                    for p in stage_data.values()
+                ],
+                marker="x",
+                color="red",
+                label="Stage from atlas mag",
+            )
+            scatters[stage_sc] = "red"
+            labels[stage_sc] = keys
+            lines_list.append(stage_sc)
+        if self._epu_data_dir:
+            grid_squares = []
+            for gs in self._grid_square_positions.keys():
+                if GridSquare.found(self._epu_data_dir, int(gs)):
+                    grid_squares.append(
+                        GridSquare(
+                            self._epu_data_dir,
+                            int(gs),
+                            flip=self._flip,
+                            switch=self._switch,
                         )
                     )
-                image = preimage[
-                    :,
-                    sub_sample_boundaries[1] : sub_sample_boundaries[1]
-                    + self._sub_sample_size[1],
-                    sub_sample_boundaries[0] : sub_sample_boundaries[0]
-                    + self._sub_sample_size[0],
-                ]
-            else:
-                image = read_image(
-                    str(self._data_dir / _grid_squares[grid_square_idx])
-                )[
-                    :,
-                    sub_sample_boundaries[1] : sub_sample_boundaries[1]
-                    + self._sub_sample_size[1],
-                    sub_sample_boundaries[0] : sub_sample_boundaries[0]
-                    + self._sub_sample_size[0],
-                ]
-        elif self._level == "grid_square":
-            averaged_df = self._df.groupby("grid_square").mean()
-            labels = [
-                v
-                for k, v in averaged_df.iloc[idx].to_dict().items()
-                if k in self._allowed_labels
-            ]
-            if self._full_res_extension == ".mrc":
-                image = mrc_to_tensor(
-                    (self._data_dir / averaged_df.iloc[idx].name).with_suffix(".mrc")
-                )
-            else:
-                image = read_image(str(self._data_dir / averaged_df.iloc[idx].name))
-        else:
-            labels = [
-                v
-                for k, v in self._df.iloc[idx].to_dict().items()
-                if k in self._allowed_labels
-            ]
-            if self._use_full_res:
-                if self._full_res_extension == ".mrc":
-                    image = mrc_to_tensor(
-                        (self._data_dir / self._df.iloc[idx][self._level]).with_suffix(
-                            ".mrc"
+            gs_sc = ax.scatter(
+                [
+                    int(
+                        (
+                            ((-1) ** self._flip_powers[0])
+                            * p._stage_position[self._switch_indices[0]]
                         )
+                        / self._pixel_size
                     )
-                elif self._full_res_extension in (".tiff", ".tif"):
-                    image = tiff_to_tensor(
-                        (self._data_dir / self._df.iloc[idx][self._level]).with_suffix(
-                            self._full_res_extension
+                    - corrected_center[0][0]
+                    + self._readout_area[1] // 2
+                    for p in grid_squares
+                ],
+                [
+                    int(
+                        (
+                            ((-1) ** self._flip_powers[1])
+                            * p._stage_position[self._switch_indices[1]]
                         )
+                        / self._pixel_size
                     )
-            else:
-                image = read_image(
-                    str(self._data_dir / self._df.iloc[idx][self._level])
-                )
-        return image, labels
-
-    def thresholds(self, quantile: float = 0.7):
-        required_columns = (
-            [*_standard_labels, self._level]
-            if self._level == "grid_square"
-            else list(_standard_labels)
-        )
-        if self._level == "grid_square":
-            newdf = (
-                self._df[required_columns]
-                .groupby(self._level)
-                .mean()[list(_standard_labels)]
+                    + corrected_center[1][0]
+                    + self._readout_area[0] // 2
+                    for p in grid_squares
+                ],
+                marker="x",
+                color="blue",
+                label="Stage from grid square mag",
             )
-        else:
-            newdf = self._df[required_columns]
-        return newdf.quantile(q=quantile)
+            scatters[gs_sc] = "blue"
+            labels[gs_sc] = [gs._id for gs in grid_squares]
+            lines_list.append(gs_sc)
+
+        leg = ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+        for legline, origline in zip(leg.legendHandles, lines_list):
+            legline.set_picker(True)
+            lines[legline] = origline
+        fig.canvas.mpl_connect("motion_notify_event", hover)
+        fig.canvas.mpl_connect("button_press_event", click)
+        fig.canvas.mpl_connect("pick_event", on_pick)
+        plt.show()
 
 
-class SmartEMPostgresDataLoader(SmartEMDataLoader):
+class GridSquare:
     def __init__(
         self,
-        level: str,
-        projects: List[str],
-        data_api: Optional[DataAPI] = None,
-        **kwargs,
+        epu_dir: Path,
+        grid_square: int,
+        images_disc: int = 1,
+        flip: Tuple[bool, bool] = (False, False),
+        switch: bool = False,
     ):
-        super().__init__(level, **kwargs)
-        self._data_api: DataAPI = data_api or DataAPI()
-        self._df = get_dataframe(self._data_api, projects)
-        super()._determine_extension()
-
-        _project = self._data_api.get_project(project_name=projects[0])
-        for dm in (Path(_project.acquisition_directory).parent / "Metadata").glob(
-            "*.dm"
-        ):
-            self._stage_calibration = calibrate_coordinate_system(dm)
-            if self._stage_calibration:
-                break
-
-
-_standard_labels = {
-    "accummotiontotal": True,
-    "ctfmaxresolution": True,
-    "estimatedresolution": True,
-    "maxvalueprobdistribution": False,
-}
+        epu_dir = Path(epu_dir)
+        self._id = grid_square
+        self._epu_location = (
+            epu_dir / f"Images-Disc{images_disc}" / f"GridSquare_{grid_square}"
+        )
+        xml_file = list(self._epu_location.glob("*.xml"))[0]
+        epu_data = parse_epu_xml(xml_file)
+        self._pixel_size = epu_data["pixel_size"]
+        self._readout_area = epu_data["readout_area"]
+        self._stage_position = epu_data["stage_position"]
+        self._foil_hole_positions = metadata_foil_hole_positions(
+            epu_dir / "Metadata" / f"GridSquare_{grid_square}.dm"
+        )
+        self._foil_hole_stage_locations = metadata_foil_hole_stage(
+            epu_dir / "Metadata" / f"GridSquare_{grid_square}.dm"
+        )
+        self._flip_powers = (1 if flip[0] else 2, 1 if flip[1] else 2)
+        self._switch_indices = (0 if switch else 1, 1 if switch else 0)
 
+    @classmethod
+    def found(cls, epu_dir: Path, grid_square: int, images_disc: int = 1) -> bool:
+        epu_dir = Path(epu_dir)
+        return (
+            epu_dir / f"Images-Disc{images_disc}" / f"GridSquare_{grid_square}"
+        ).is_dir()
+
+    @property
+    def image(self) -> np.array:
+        img_file = list(self._epu_location.glob("*.mrc"))[0]
+        with mrcfile.open(img_file) as mrc:
+            return mrc.data
 
-class SmartEMDiskDataLoader(SmartEMDataLoader):
-    def __init__(
+    def display(
         self,
-        level: str,
-        data_dir: Path,
-        full_res: bool = False,
-        labels_csv: str = "labels.csv",
-        num_samples: int = 0,
-        sub_sample_size: Optional[Tuple[int, int]] = None,
-        allowed_labels: Optional[Dict[str, bool]] = None,
-        seed: int = 0,
+        show_holes: bool = True,
+        show_stage_positions: bool = True,
+        show_foil_hole_data: bool = True,
     ):
-        super().__init__(
-            level,
-            full_res=full_res,
-            num_samples=num_samples,
-            sub_sample_size=sub_sample_size,
-            allowed_labels=allowed_labels,
-            seed=seed,
-        )
-        self._data_dir = data_dir
-        self._df = pd.read_csv(self._data_dir / labels_csv)
-        super()._determine_extension()
-
-        try:
-            with open(self._data_dir / "coordinate_calibration.yaml", "r") as cal_in:
-                sc = yaml.safe_load(cal_in)
-        except FileNotFoundError:
-            sc = {"inverted": False, "x_flip": False, "y_flip": True}
-        self._stage_calibration = StageCalibration(**sc)
-
-
-class SmartEMMaskDataLoader(DataLoader):
-    def __init__(self, data_dir: Path, labels_csv: str = "labels.csv"):
-        self._data_dir = data_dir
-        self._df = (
-            pd.read_csv(self._data_dir / labels_csv).groupby("grid_square").mean()
-        )
-        if (self._data_dir / self._df.iloc[0].name).with_suffix(".mrc").exists():
-            self._full_res_extension = ".mrc"
-        elif (self._data_dir / self._df.iloc[0].name).with_suffix(".tiff").exists():
-            self._full_res_extension = ".tiff"
-        elif (self._data_dir / self._df.iloc[0].name).with_suffix(".tif").exists():
-            self._full_res_extension = ".tif"
-        else:
-            raise FileNotFoundError(
-                f"{self._data_dir / self._df.iloc[0].name} was not found with any of the following suffixes: .mrc, .tiff, .tif"
-            )
+        # fig, ax = plt.subplots(1, figsize=(12, 6))
+        fig = plt.figure(2)
+        ax = fig.gca()
+        ax.imshow(self.image)
 
-    def __len__(self) -> int:
-        return len(self._df.index)
+        self._readout_area = self.image.shape
 
-    def __getitem__(self, idx: int) -> Tuple[Tensor, Tensor]:
-        image_path = (self._data_dir / self._df.iloc[idx].name).with_suffix(
-            self._full_res_extension
+        annot = ax.annotate(
+            "Grid square ID: ", xy=(0, 0), xytext=(5, 5), textcoords="offset points"
         )
-        if self._full_res_extension == ".mrc":
-            image = mrc_to_tensor(image_path)
-        else:
-            image = tiff_to_tensor(image_path)
-        mask = from_numpy(np.load(image_path.with_suffix(".npy")))
-        return image, mask
+        annot.set_visible(False)
+
+        labels: dict = {}
+        scatters: dict = {}
+        lines: dict = {}
+        lines_list: list = []
+
+        def hover(event):
+            if event.inaxes == ax:
+                for sc, c in scatters.items():
+                    cont, ind = sc.contains(event)
+                    if cont:
+                        # annot.xy = (event.xdata, event.ydata)
+                        annot_text = f"Foil hole ID: {', '.join([str(labels[sc][n]) for n in ind['ind']])}"
+                        annot.set_text(annot_text)
+                        annot.set_color(c)
+                        annot.set_visible(True)
+                        break
+                    else:
+                        annot.set_visible(False)
+                fig.canvas.draw()
+
+        def on_pick(event):
+            legline = event.artist
+            origline = lines[legline]
+            visible = not origline.get_visible()
+            origline.set_visible(visible)
+            legline.set_alpha(1.0 if visible else 0.2)
+            fig.canvas.draw()
+
+        if show_holes:
+            holes_sc = ax.scatter(
+                [p[0] for p in self._foil_hole_positions.values()],
+                [p[1] for p in self._foil_hole_positions.values()],
+                marker="x",
+                color="green",
+                label="Pixel",
+            )
+            scatters[holes_sc] = "green"
+            labels[holes_sc] = list(self._foil_hole_positions.keys())
+            lines_list.append(holes_sc)
+
+        if show_stage_positions:
+            stage_sc = ax.scatter(
+                [
+                    int(
+                        (((-1) ** self._flip_powers[0]) * p[self._switch_indices[0]])
+                        / self._pixel_size
+                    )
+                    + int(self._stage_position[1] / self._pixel_size)
+                    + self._readout_area[0] // 2
+                    for p in self._foil_hole_stage_locations.values()
+                ],
+                [
+                    int(
+                        (((-1) ** self._flip_powers[1]) * p[self._switch_indices[1]])
+                        / self._pixel_size
+                    )
+                    + (self._stage_position[0] / self._pixel_size)
+                    + self._readout_area[1] // 2
+                    for p in self._foil_hole_stage_locations.values()
+                ],
+                marker="x",
+                color="red",
+                label="Stage from grid square mag",
+            )
+            scatters[stage_sc] = "red"
+            labels[stage_sc] = list(self._foil_hole_stage_locations.keys())
+            lines_list.append(stage_sc)
+
+        if show_foil_hole_data:
+            foil_holes = []
+            found_foil_holes = []
+            for fh in self._foil_hole_positions.keys():
+                fh_xmls = list(
+                    (self._epu_location / "FoilHoles").glob(f"FoilHole_{fh}*.xml")
+                )
+                if fh_xmls:
+                    foil_holes.append(parse_epu_xml(fh_xmls[0]))
+                    found_foil_holes.append(fh)
+            fh_sc = ax.scatter(
+                [
+                    int(
+                        (
+                            ((-1) ** self._flip_powers[0])
+                            * p["stage_position"][self._switch_indices[0]]
+                        )
+                        / self._pixel_size
+                    )
+                    + (self._stage_position[1] / self._pixel_size)
+                    + self._readout_area[0] // 2
+                    for p in foil_holes
+                ],
+                [
+                    int(
+                        (
+                            ((-1) ** self._flip_powers[1])
+                            * p["stage_position"][self._switch_indices[1]]
+                        )
+                        / self._pixel_size
+                    )
+                    + (self._stage_position[0] / self._pixel_size)
+                    + self._readout_area[1] // 2
+                    for p in foil_holes
+                ],
+                marker="x",
+                color="blue",
+                label="Stage from foil hole mag",
+            )
+            scatters[fh_sc] = "blue"
+            labels[fh_sc] = found_foil_holes
+            lines_list.append(fh_sc)
+
+        leg = ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+        for legline, origline in zip(leg.legendHandles, lines_list):
+            legline.set_picker(True)
+            lines[legline] = origline
+        fig.canvas.mpl_connect("motion_notify_event", hover)
+        fig.canvas.mpl_connect("pick_event", on_pick)
+        plt.show()
```

### Comparing `smartem-0.1.6/src/smartem/gui/qt/__init__.py` & `smartem-0.1.7/src/smartem/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/component_tab.py` & `smartem-0.1.7/src/smartem/gui/qt/component_tab.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/display.py` & `smartem-0.1.7/src/smartem/gui/qt/display.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/image_utils.py` & `smartem-0.1.7/src/smartem/gui/qt/image_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/loader.py` & `smartem-0.1.7/src/smartem/gui/qt/loader.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/loader_csv.py` & `smartem-0.1.7/src/smartem/gui/qt/loader_csv.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/plotting_utils.py` & `smartem-0.1.7/src/smartem/gui/qt/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/gui/qt/qt_style.css` & `smartem-0.1.7/src/smartem/gui/qt/qt_style.css`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/parsing/epu.py` & `smartem-0.1.7/src/smartem/parsing/epu.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,21 @@
         for key in nodes.keys():
             if key.startswith("KeyValuePairOfintNodeXml"):
                 required_key = key
                 break
         if not required_key:
             continue
         for gs in nodes[required_key]:
-            gs_pix_positions[gs["key"]] = (
-                int(float(gs["value"]["b:PositionOnTheAtlas"]["c:Center"]["d:x"])),
-                int(float(gs["value"]["b:PositionOnTheAtlas"]["c:Center"]["d:y"])),
-            )
+            try:
+                gs_pix_positions[gs["key"]] = (
+                    int(float(gs["value"]["b:PositionOnTheAtlas"]["c:Center"]["d:x"])),
+                    int(float(gs["value"]["b:PositionOnTheAtlas"]["c:Center"]["d:y"])),
+                )
+            except TypeError:
+                pass
     return gs_pix_positions
 
 
 def metadata_grid_square_stage(xml_path: Path) -> Dict[str, Tuple[float, float]]:
     with open(xml_path, "r") as xml:
         for_parsing = xml.read()
         data = xmltodict.parse(for_parsing)
```

### Comparing `smartem-0.1.6/src/smartem/parsing/export.py` & `smartem-0.1.7/src/smartem/parsing/export.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import shutil
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import numpy as np
+import xmltodict
 import yaml
 from pandas import DataFrame
 
 from smartem.data_model import GridSquare
 from smartem.data_model.extract import DataAPI
 from smartem.data_model.structure import extract_keys_with_foil_hole_averages
 from smartem.parsing.epu import calibrate_coordinate_system, mask_foil_hole_positions
@@ -30,41 +31,51 @@
         "grid_square_y": [],
         "foil_hole": [],
         "foil_hole_pixel_size": [],
         "foil_hole_x": [],
         "foil_hole_y": [],
         "accummotiontotal": [],
         "ctfmaxresolution": [],
+        "particlecount": [],
         "estimatedresolution": [],
         "maxvalueprobdistribution": [],
     }
     for project in projects:
         _grid_squares = grid_squares or data_api.get_grid_squares(project)
         foil_holes = data_api.get_foil_holes(project=project)
 
         _data_labels = data_labels or [
             "_rlnaccummotiontotal",
             "_rlnctfmaxresolution",
+            "_rlnmicrographparticlecount",
             "_rlnestimatedresolution",
             "_rlnmaxvalueprobdistribution",
         ]
 
         _project = data_api.get_project(project_name=project)
         atlas = data_api.get_atlas_from_project(_project)
         atlas_id = atlas.atlas_id
         atlas_info = data_api.get_atlas_info(
             atlas_id,
-            ["_rlnaccummotiontotal", "_rlnctfmaxresolution"],
+            [
+                "_rlnaccummotiontotal",
+                "_rlnctfmaxresolution",
+                "_rlnmicrographparticlecount",
+            ],
             ["_rlnmaxvalueprobdistribution"],
             ["_rlnestimatedresolution"],
         )
 
         fh_extracted = extract_keys_with_foil_hole_averages(
             atlas_info,
-            ["_rlnaccummotiontotal", "_rlnctfmaxresolution"],
+            [
+                "_rlnaccummotiontotal",
+                "_rlnctfmaxresolution",
+                "_rlnmicrographparticlecount",
+            ],
             ["_rlnmaxvalueprobdistribution"],
             ["_rlnestimatedresolution"],
         )
         epu_dir = Path(_project.acquisition_directory)
 
         gs_coordinates = {}
         gs_pixel_sizes = {}
@@ -124,14 +135,17 @@
                         data["foil_hole_y"].append(fh.stage_position_y)
                     data["accummotiontotal"].append(
                         fh_extracted["_rlnaccummotiontotal"].averages[fh.foil_hole_name]  # type: ignore
                     )
                     data["ctfmaxresolution"].append(
                         fh_extracted["_rlnctfmaxresolution"].averages[fh.foil_hole_name]  # type: ignore
                     )
+                    data["particlecount"].append(
+                        fh_extracted["_rlnmicrographparticlecount"].averages[fh.foil_hole_name]  # type: ignore
+                    )
                     data["estimatedresolution"].append(
                         fh_extracted["_rlnestimatedresolution"].averages[  # type: ignore
                             fh.foil_hole_name
                         ]
                     )
                     data["maxvalueprobdistribution"].append(
                         fh_extracted["_rlnmaxvalueprobdistribution"].averages[  # type: ignore
@@ -160,42 +174,53 @@
         "grid_square_y": [],
         "foil_hole": [],
         "foil_hole_pixel_size": [],
         "foil_hole_x": [],
         "foil_hole_y": [],
         "accummotiontotal": [],
         "ctfmaxresolution": [],
+        "particlecount": [],
         "estimatedresolution": [],
         "maxvalueprobdistribution": [],
+        "image_defocus": [],
     }
 
     for project in projects:
         grid_squares = data_api.get_grid_squares(project)
         foil_holes = data_api.get_foil_holes(project=project)
 
         data_labels = [
             "_rlnaccummotiontotal",
             "_rlnctfmaxresolution",
+            "_rlnmicrographparticlecount",
             "_rlnestimatedresolution",
             "_rlnmaxvalueprobdistribution",
         ]
 
         _project = data_api.get_project(project_name=project)
         atlas = data_api.get_atlas_from_project(_project)
         atlas_id = atlas.atlas_id
         atlas_info = data_api.get_atlas_info(
             atlas_id,
-            ["_rlnaccummotiontotal", "_rlnctfmaxresolution"],
+            [
+                "_rlnaccummotiontotal",
+                "_rlnctfmaxresolution",
+                "_rlnmicrographparticlecount",
+            ],
             ["_rlnmaxvalueprobdistribution"],
             ["_rlnestimatedresolution"],
         )
 
         fh_extracted = extract_keys_with_foil_hole_averages(
             atlas_info,
-            ["_rlnaccummotiontotal", "_rlnctfmaxresolution"],
+            [
+                "_rlnaccummotiontotal",
+                "_rlnctfmaxresolution",
+                "_rlnmicrographparticlecount",
+            ],
             ["_rlnmaxvalueprobdistribution"],
             ["_rlnestimatedresolution"],
         )
 
         epu_dir = Path(_project.acquisition_directory)
         metadata_path = epu_dir.parent / "Metadata"
 
@@ -208,27 +233,35 @@
             out_dir / atlas_image_path.with_suffix(".mrc").name,
         )
 
         gs_coordinates = {}
         gs_pixel_sizes = {}
 
         for gs in grid_squares:
+            grid_square_image_defocus = None
             if gs.thumbnail:
                 gs_dir = out_dir / gs.grid_square_name
                 gs_dir.mkdir()
                 thumbnail_path: Optional[Path] = epu_dir / gs.thumbnail
                 if thumbnail_path:
                     shutil.copy(thumbnail_path, gs_dir / thumbnail_path.name)
                     shutil.copy(
                         thumbnail_path.with_suffix(alternative_extension or ".mrc"),
                         gs_dir
                         / thumbnail_path.with_suffix(
                             alternative_extension or ".mrc"
                         ).name,
                     )
+                    with open(thumbnail_path.with_suffix(".xml")) as gs_xml:
+                        custom_data = xmltodict.parse(gs_xml.read())["MicroscopeImage"][
+                            "CustomData"
+                        ]["a:KeyValueOfstringanyType"]
+                        for elem in custom_data:
+                            if elem["a:Key"] == "AppliedDefocus":
+                                grid_square_image_defocus = elem["a:Value"]["#text"]
                     out_gs_paths[gs.grid_square_name] = (
                         gs_dir / thumbnail_path.name
                     ).relative_to(out_dir)
                 gs_coordinates[gs.grid_square_name] = (
                     gs.stage_position_x,
                     gs.stage_position_y,
                 )
@@ -297,24 +330,28 @@
                         data["foil_hole_y"].append(fh.stage_position_y)
                     data["accummotiontotal"].append(
                         fh_extracted["_rlnaccummotiontotal"].averages[fh.foil_hole_name]  # type: ignore
                     )
                     data["ctfmaxresolution"].append(
                         fh_extracted["_rlnctfmaxresolution"].averages[fh.foil_hole_name]  # type: ignore
                     )
+                    data["particlecount"].append(
+                        fh_extracted["_rlnmicrographparticlecount"].averages[fh.foil_hole_name]  # type: ignore
+                    )
                     data["estimatedresolution"].append(
                         fh_extracted["_rlnestimatedresolution"].averages[  # type: ignore
                             fh.foil_hole_name
                         ]
                     )
                     data["maxvalueprobdistribution"].append(
                         fh_extracted["_rlnmaxvalueprobdistribution"].averages[  # type: ignore
                             fh.foil_hole_name
                         ]
                     )
+                    data["image_defocus"].append(grid_square_image_defocus)
 
     df = DataFrame.from_dict(data)
     df.to_csv(out_dir / "labels.csv", index=False)
 
     if projects:
         _project = data_api.get_project(project_name=projects[0])
         for dm in (Path(_project.acquisition_directory).parent / "Metadata").glob(
```

### Comparing `smartem-0.1.6/src/smartem/parsing/relion_default.py` & `smartem-0.1.7/src/smartem/parsing/relion_default.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 from numpy import argmin
 
 from smartem.data_model.extract import DataAPI
 from smartem.parsing.star import (
     get_column_data,
     insert_exposure_data,
@@ -57,14 +57,52 @@
         "_rlnmicrographname",
         str(ctf_file_path),
         data_handler,
         project=project,
     )
 
 
+def _num_particles(relion_dir: Path, data_handler: DataAPI, project: str):
+    picking_base_path = relion_dir / "AutoPick"
+    picking_file_job_paths = picking_base_path.glob("job*")
+    job_numbers = [str(j.name).replace("job", "") for j in picking_file_job_paths]
+    first_job_idx = argmin([int(jn) for jn in job_numbers])
+    picking_file_path = (
+        relion_dir / "AutoPick" / f"job{job_numbers[first_job_idx]}" / "autopick.star"
+    )
+    star_file = open_star_file(picking_file_path)
+    column_data = get_column_data(
+        star_file,
+        ["_rlnmicrographname", "_rlnmicrographcoordinates"],
+        "coordinate_files",
+    )
+    count_data: Dict[str, list] = {
+        "_rlnmicrographname": [],
+        "_rlnmicrographparticlecount": [],
+    }
+    for mic, cfile in zip(
+        column_data["_rlnmicrographname"], column_data["_rlnmicrographcoordinates"]
+    ):
+        if not (relion_dir / cfile).is_file():
+            continue
+        coord_file = open_star_file(relion_dir / cfile)
+        coord_column_data = get_column_data(coord_file, ["_rlncoordinatex"], "#")
+        count_data["_rlnmicrographname"].append(mic)
+        count_data["_rlnmicrographparticlecount"].append(
+            len(coord_column_data["_rlncoordinatex"])
+        )
+    insert_exposure_data(
+        count_data,
+        "_rlnmicrographname",
+        str(picking_file_path),
+        data_handler,
+        project=project,
+    )
+
+
 def _prob_dist_max_class2d(
     relion_dir: Path,
     data_handler: DataAPI,
     project: str,
     excluded_directories: Optional[List[str]] = None,
 ):
     exclude = excluded_directories or []
@@ -155,11 +193,12 @@
     relion_dir: Path,
     data_handler: DataAPI,
     project: str,
     class_2d_excludes: Optional[List[str]] = None,
 ):
     _motion_corr(relion_dir, data_handler, project)
     _ctf(relion_dir, data_handler, project)
+    _num_particles(relion_dir, data_handler, project)
     _prob_dist_max_class2d(
         relion_dir, data_handler, project, excluded_directories=class_2d_excludes
     )
     _class2d(relion_dir, data_handler, project, excluded_directories=class_2d_excludes)
```

### Comparing `smartem-0.1.6/src/smartem/parsing/star.py` & `smartem-0.1.7/src/smartem/parsing/star.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem/stage_model.py` & `smartem-0.1.7/src/smartem/stage_model.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/src/smartem.egg-info/PKG-INFO` & `smartem-0.1.7/src/smartem.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: gemmi
+Requires-Dist: matplotlib
+Requires-Dist: xmltodict
+Requires-Dist: mrcfile
+Requires-Dist: pyyaml
+Requires-Dist: psycopg2
+Requires-Dist: sqlalchemy<2.0
+Requires-Dist: PyQt5
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: tifffile
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
 
 
 Installation
```

### Comparing `smartem-0.1.6/src/smartem.egg-info/SOURCES.txt` & `smartem-0.1.7/src/smartem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartem-0.1.6/tests/test_stage_model.py` & `smartem-0.1.7/tests/test_stage_model.py`

 * *Files identical despite different names*

