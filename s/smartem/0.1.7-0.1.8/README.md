# Comparing `tmp/smartem-0.1.7.tar.gz` & `tmp/smartem-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartem-0.1.7.tar", last modified: Tue May  7 12:50:21 2024, max compression
+gzip compressed data, was "smartem-0.1.8.tar", last modified: Tue May  7 13:22:49 2024, max compression
```

## Comparing `smartem-0.1.7.tar` & `smartem-0.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.747363 smartem-0.1.7/
--rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.7/LICENSE
--rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 12:50:21.746528 smartem-0.1.7/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.7/README.rst
--rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.7/pyproject.toml
--rw-r--r--   0 kif41228   (504) staff       (20)     1224 2024-05-07 12:50:21.749876 smartem-0.1.7/setup.cfg
--rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.7/setup.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.639594 smartem-0.1.7/src/
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.646987 smartem-0.1.7/src/smartem/
--rw-r--r--   0 kif41228   (504) staff       (20)      212 2024-05-07 12:48:41.000000 smartem-0.1.7/src/smartem/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.659927 smartem-0.1.7/src/smartem/cli/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/change_epu_directory.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/initialise.py
--rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/launch.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/missing.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1577 2023-07-11 12:47:43.000000 smartem-0.1.7/src/smartem/cli/quick_epu_viewer.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/start.py
--rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/cli/stop.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.663539 smartem-0.1.7/src/smartem/data_model/
--rw-r--r--   0 kif41228   (504) staff       (20)     7267 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/data_model/construct.py
--rw-r--r--   0 kif41228   (504) staff       (20)    37096 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/extract.py
--rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/data_model/structure.py
--rw-r--r--   0 kif41228   (504) staff       (20)    23224 2024-02-05 10:53:08.000000 smartem-0.1.7/src/smartem/data_model/torch.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.664131 smartem-0.1.7/src/smartem/gui/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/__init__.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.731578 smartem-0.1.7/src/smartem/gui/qt/
--rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/component_tab.py
--rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/display.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/image_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/loader.py
--rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/loader_csv.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/plotting_utils.py
--rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/gui/qt/qt_style.css
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.743826 smartem-0.1.7/src/smartem/parsing/
--rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/parsing/__init__.py
--rw-r--r--   0 kif41228   (504) staff       (20)    19626 2024-05-07 12:47:34.000000 smartem-0.1.7/src/smartem/parsing/epu.py
--rw-r--r--   0 kif41228   (504) staff       (20)    15129 2024-01-05 11:06:15.000000 smartem-0.1.7/src/smartem/parsing/epu_vis.py
--rw-r--r--   0 kif41228   (504) staff       (20)    15154 2024-05-07 12:46:26.000000 smartem-0.1.7/src/smartem/parsing/export.py
--rw-r--r--   0 kif41228   (504) staff       (20)     7093 2024-01-05 11:20:56.000000 smartem-0.1.7/src/smartem/parsing/relion_default.py
--rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/parsing/star.py
--rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.7/src/smartem/stage_model.py
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.745636 smartem-0.1.7/src/smartem.egg-info/
--rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/PKG-INFO
--rw-r--r--   0 kif41228   (504) staff       (20)     1286 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/SOURCES.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/dependency_links.txt
--rw-r--r--   0 kif41228   (504) staff       (20)      372 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/entry_points.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.7/src/smartem.egg-info/not-zip-safe
--rw-r--r--   0 kif41228   (504) staff       (20)       95 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/requires.txt
--rw-r--r--   0 kif41228   (504) staff       (20)        8 2024-05-07 12:50:21.000000 smartem-0.1.7/src/smartem.egg-info/top_level.txt
-drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 12:50:21.744589 smartem-0.1.7/tests/
--rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.7/tests/test_stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.468296 smartem-0.1.8/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.8/LICENSE
+-rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 13:22:49.468063 smartem-0.1.8/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.8/README.rst
+-rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.8/pyproject.toml
+-rw-r--r--   0 kif41228   (504) staff       (20)     1224 2024-05-07 13:22:49.469801 smartem-0.1.8/setup.cfg
+-rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.8/setup.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.326335 smartem-0.1.8/src/
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.339156 smartem-0.1.8/src/smartem/
+-rw-r--r--   0 kif41228   (504) staff       (20)      212 2024-05-07 13:22:03.000000 smartem-0.1.8/src/smartem/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.380934 smartem-0.1.8/src/smartem/cli/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/change_epu_directory.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/initialise.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/launch.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/missing.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1577 2023-07-11 12:47:43.000000 smartem-0.1.8/src/smartem/cli/quick_epu_viewer.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/start.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/cli/stop.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.409578 smartem-0.1.8/src/smartem/data_model/
+-rw-r--r--   0 kif41228   (504) staff       (20)     7267 2024-02-05 10:53:08.000000 smartem-0.1.8/src/smartem/data_model/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/data_model/construct.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    37096 2024-02-05 10:53:08.000000 smartem-0.1.8/src/smartem/data_model/extract.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/data_model/structure.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    23224 2024-02-05 10:53:08.000000 smartem-0.1.8/src/smartem/data_model/torch.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.410228 smartem-0.1.8/src/smartem/gui/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.443682 smartem-0.1.8/src/smartem/gui/qt/
+-rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/component_tab.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/display.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/image_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/loader.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/loader_csv.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/plotting_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/gui/qt/qt_style.css
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.464133 smartem-0.1.8/src/smartem/parsing/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/parsing/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    19750 2024-05-07 13:21:32.000000 smartem-0.1.8/src/smartem/parsing/epu.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    15129 2024-01-05 11:06:15.000000 smartem-0.1.8/src/smartem/parsing/epu_vis.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    15154 2024-05-07 12:46:26.000000 smartem-0.1.8/src/smartem/parsing/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     7093 2024-01-05 11:20:56.000000 smartem-0.1.8/src/smartem/parsing/relion_default.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/parsing/star.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.8/src/smartem/stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.467571 smartem-0.1.8/src/smartem.egg-info/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1508 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1286 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/SOURCES.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/dependency_links.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)      372 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/entry_points.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.8/src/smartem.egg-info/not-zip-safe
+-rw-r--r--   0 kif41228   (504) staff       (20)       95 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/requires.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        8 2024-05-07 13:22:49.000000 smartem-0.1.8/src/smartem.egg-info/top_level.txt
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2024-05-07 13:22:49.466979 smartem-0.1.8/tests/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.8/tests/test_stage_model.py
```

### Comparing `smartem-0.1.7/LICENSE` & `smartem-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/PKG-INFO` & `smartem-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: gemmi
 Requires-Dist: matplotlib
 Requires-Dist: xmltodict
 Requires-Dist: mrcfile
```

### Comparing `smartem-0.1.7/README.rst` & `smartem-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/setup.cfg` & `smartem-0.1.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smartem
-version = 0.1.7
+version = 0.1.8
 description = Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 long_description = file: README.rst
 license_file = LICENSE
 
 [options]
 include_package_data = True
 install_requires =
```

### Comparing `smartem-0.1.7/src/smartem/cli/change_epu_directory.py` & `smartem-0.1.8/src/smartem/cli/change_epu_directory.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/export.py` & `smartem-0.1.8/src/smartem/cli/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/initialise.py` & `smartem-0.1.8/src/smartem/cli/initialise.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/missing.py` & `smartem-0.1.8/src/smartem/cli/missing.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/quick_epu_viewer.py` & `smartem-0.1.8/src/smartem/cli/quick_epu_viewer.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/start.py` & `smartem-0.1.8/src/smartem/cli/start.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/cli/stop.py` & `smartem-0.1.8/src/smartem/cli/stop.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/data_model/__init__.py` & `smartem-0.1.8/src/smartem/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/data_model/construct.py` & `smartem-0.1.8/src/smartem/data_model/construct.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/data_model/extract.py` & `smartem-0.1.8/src/smartem/data_model/extract.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/data_model/structure.py` & `smartem-0.1.8/src/smartem/data_model/structure.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/data_model/torch.py` & `smartem-0.1.8/src/smartem/data_model/torch.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/__init__.py` & `smartem-0.1.8/src/smartem/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/component_tab.py` & `smartem-0.1.8/src/smartem/gui/qt/component_tab.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/display.py` & `smartem-0.1.8/src/smartem/gui/qt/display.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/image_utils.py` & `smartem-0.1.8/src/smartem/gui/qt/image_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/loader.py` & `smartem-0.1.8/src/smartem/gui/qt/loader.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/loader_csv.py` & `smartem-0.1.8/src/smartem/gui/qt/loader_csv.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/plotting_utils.py` & `smartem-0.1.8/src/smartem/gui/qt/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/gui/qt/qt_style.css` & `smartem-0.1.8/src/smartem/gui/qt/qt_style.css`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/parsing/epu.py` & `smartem-0.1.8/src/smartem/parsing/epu.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,23 @@
         for key in nodes.keys():
             if key.startswith("KeyValuePairOfintNodeXml"):
                 required_key = key
                 break
         if not required_key:
             continue
         for gs in nodes[required_key]:
-            gs_stage_positions[gs["key"]] = (
-                float(gs["value"]["b:PositionOnTheAtlas"]["c:Physical"]["d:x"]) * 1e9,
-                float(gs["value"]["b:PositionOnTheAtlas"]["c:Physical"]["d:y"]) * 1e9,
-            )
+            try:
+                gs_stage_positions[gs["key"]] = (
+                    float(gs["value"]["b:PositionOnTheAtlas"]["c:Physical"]["d:x"])
+                    * 1e9,
+                    float(gs["value"]["b:PositionOnTheAtlas"]["c:Physical"]["d:y"])
+                    * 1e9,
+                )
+            except TypeError:
+                pass
     return gs_stage_positions
 
 
 def mask_foil_hole_positions(
     xml_path: Path, image_size: Tuple[int, int], diameter: float | None = None
 ):
     with open(xml_path, "r") as xml:
```

### Comparing `smartem-0.1.7/src/smartem/parsing/epu_vis.py` & `smartem-0.1.8/src/smartem/parsing/epu_vis.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/parsing/export.py` & `smartem-0.1.8/src/smartem/parsing/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/parsing/relion_default.py` & `smartem-0.1.8/src/smartem/parsing/relion_default.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/parsing/star.py` & `smartem-0.1.8/src/smartem/parsing/star.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem/stage_model.py` & `smartem-0.1.8/src/smartem/stage_model.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/src/smartem.egg-info/PKG-INFO` & `smartem-0.1.8/src/smartem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: gemmi
 Requires-Dist: matplotlib
 Requires-Dist: xmltodict
 Requires-Dist: mrcfile
```

### Comparing `smartem-0.1.7/src/smartem.egg-info/SOURCES.txt` & `smartem-0.1.8/src/smartem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartem-0.1.7/tests/test_stage_model.py` & `smartem-0.1.8/tests/test_stage_model.py`

 * *Files identical despite different names*

