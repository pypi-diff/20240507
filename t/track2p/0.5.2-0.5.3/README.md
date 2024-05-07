# Comparing `tmp/track2p-0.5.2.tar.gz` & `tmp/track2p-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.2.tar", last modified: Fri Apr 26 14:38:32 2024, max compression
+gzip compressed data, was "track2p-0.5.3.tar", last modified: Tue May  7 11:27:38 2024, max compression
```

## Comparing `track2p-0.5.2.tar` & `track2p-0.5.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.100858 track2p-0.5.2/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.2/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-04-26 14:38:32.100623 track2p-0.5.2/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.2/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-26 14:38:32.100897 track2p-0.5.2/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      583 2024-04-26 14:36:00.000000 track2p-0.5.2/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.094027 track2p-0.5.2/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.2/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.2/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.096680 track2p-0.5.2/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8309 2024-04-26 11:45:50.000000 track2p-0.5.2/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2063 2024-04-26 11:45:53.000000 track2p-0.5.2/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    24060 2024-04-26 14:35:38.000000 track2p-0.5.2/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10642 2024-04-26 11:45:43.000000 track2p-0.5.2/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.097801 track2p-0.5.2/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-26 14:30:23.000000 track2p-0.5.2/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.2/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.098398 track2p-0.5.2/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.098724 track2p-0.5.2/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3385 2024-04-24 13:38:09.000000 track2p-0.5.2/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.099492 track2p-0.5.2/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.2/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1008 2024-04-17 14:31:55.000000 track2p-0.5.2/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:32:00.000000 track2p-0.5.2/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.100242 track2p-0.5.2/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.2/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.2/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.2/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2391 2024-04-17 14:32:03.000000 track2p-0.5.2/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9781 2024-04-26 11:45:47.000000 track2p-0.5.2/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-26 14:38:32.094675 track2p-0.5.2/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      155 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-26 14:38:32.000000 track2p-0.5.2/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.062509 track2p-0.5.3/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.3/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-05-07 11:27:38.062258 track2p-0.5.3/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.3/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-05-07 11:27:38.062556 track2p-0.5.3/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      583 2024-05-07 11:27:05.000000 track2p-0.5.3/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.054922 track2p-0.5.3/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.3/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.3/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.057809 track2p-0.5.3/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8309 2024-04-26 11:45:50.000000 track2p-0.5.3/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2063 2024-05-03 10:45:47.000000 track2p-0.5.3/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    24543 2024-05-07 11:25:01.000000 track2p-0.5.3/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10513 2024-05-07 11:25:00.000000 track2p-0.5.3/track2p/gui/s2p_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10642 2024-04-26 11:45:43.000000 track2p-0.5.3/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.058811 track2p-0.5.3/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-26 14:30:23.000000 track2p-0.5.3/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.3/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.3/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.059418 track2p-0.5.3/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.3/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.059751 track2p-0.5.3/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3450 2024-05-03 09:53:49.000000 track2p-0.5.3/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.060800 track2p-0.5.3/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.3/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      914 2024-05-07 11:25:04.000000 track2p-0.5.3/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:32:00.000000 track2p-0.5.3/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.061753 track2p-0.5.3/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.3/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.3/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.3/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-05-07 11:25:03.000000 track2p-0.5.3/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9781 2024-05-07 11:24:59.000000 track2p-0.5.3/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-05-07 11:27:38.055472 track2p-0.5.3/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5065 2024-05-07 11:27:38.000000 track2p-0.5.3/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      883 2024-05-07 11:27:38.000000 track2p-0.5.3/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-05-07 11:27:38.000000 track2p-0.5.3/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      155 2024-05-07 11:27:38.000000 track2p-0.5.3/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-05-07 11:27:38.000000 track2p-0.5.3/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.2/LICENSE` & `track2p-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/PKG-INFO` & `track2p-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.2
+Version: 0.5.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.2/README.md` & `track2p-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/setup.py` & `track2p-0.5.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.2',
+    version='0.5.3',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk==5.4rc2',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.2/track2p/gui/cell_plot.py` & `track2p-0.5.3/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/gui/fluo_plot.py` & `track2p-0.5.3/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/gui/import_wd.py` & `track2p-0.5.3/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/gui/main_wd.py` & `track2p-0.5.3/track2p/gui/main_wd.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from types import SimpleNamespace
 from track2p.gui.cell_plot import CellPlotWidget
 from track2p.gui.fluo_plot import FluorescencePlotWidget
 from track2p.gui.roi_plot import ZoomPlotWidget
 from track2p.gui.t2p_wd import NewWindow
 from track2p.gui.import_wd import ImportWindow
 from track2p.gui.raster_wd import RasterWindow
+from track2p.gui.s2p_wd import Suite2pWindow
 import pandas as pd 
 
 
 class MainWindow(QMainWindow):
     """This class is used to create the main window of the application. QWidget is the base class for all user interface objects in PyQt5 """
     def __init__(self):
         """it initializes the class attributes and calls the initUI method to create the main window of the application. It also calls the init_cell method to display the first cell of the t2p_match_mat_allday and its fluorescence and zooms across days."""
@@ -61,14 +62,19 @@
         visualization_menu = QMenu( self)
         
         load_data_action = QAction("Load processed data (⌘L or Ctrl+L)", self)
         load_data_action.setShortcut("Ctrl+L")
         load_data_action.triggered.connect(self.runProcessedData)
         file_menu.addAction(load_data_action)
         
+        suite2p_action = QAction("Generate the outputs in suite2p format (⌘S or Ctrl+S)", self)
+        suite2p_action.setShortcut("Ctrl+S")
+        suite2p_action.triggered.connect(self.save_in_s2p_format)
+        file_menu.addAction(suite2p_action)
+        
         run_track_action = QAction("Run track2p alogorithm (⌘R or Ctrl+)", self)
         run_track_action.setShortcut("Ctrl+R")
         run_track_action.triggered.connect(self.runTrack2p)
         run_menu.addAction(run_track_action)
         
         generate_rasterplot_action = QAction("Generate raster plot (⌘G or Ctrl+G)", self)
         generate_rasterplot_action.setShortcut("Ctrl+G")
@@ -199,21 +205,23 @@
         data = {'cell_number': list(self.vector_curation_t2p.keys()), 'status_t2p': list(self.vector_curation_t2p.values()), 'status_s2p': status_suite2p}
         self.df = pd.DataFrame(data)
 
         nb_cells= f'number of cells present on all days : {len(self.t2p_match_mat_allday)}'  
         is_cell_prob=f'probability used in track2p algorithm : {self.iscell_thr}'
         num_zeros_t2p = f'number of cells deleted in track2p : {len([value for value in self.vector_curation_t2p.values() if value == 0])}'
         
+        #indexes_per_day = []
         info_string = ""
         for day in range(len(self.all_iscell_t2p) + 1):
             num_values_equal_to_day = len([value for value in self.num_ones.values() if value == day])
             info_string += f"Number of cells present {day} day out of {len(self.all_iscell_t2p)}: {num_values_equal_to_day}\n"
             keys_for_day = [key for key, value in self.num_ones.items() if value == day]
             info_string += f'Indexes: {keys_for_day}\n\n'
-    
+
+       # print(indexes_per_day)
 
         with open(os.path.join(self.t2p_folder_path, "track2p",'info.txt'), 'w') as f:
             f.write(nb_cells + "\n" + is_cell_prob + "\n\n" +info_string +"\n\n" + num_zeros_t2p +"\n\n" + self.df.to_string(index=False) + "\n")
         
 
     def spin_box_changed(self):
         current_value = self.spin_box.value() #selected ROI 
@@ -437,14 +445,18 @@
         self.importWindow.show()
         
     def generateRasterPlot(self):
         self.rasterWindow=RasterWindow(self)
         self.rasterWindow.show()
         
         
+    def save_in_s2p_format(self):
+        self.s2p_window=Suite2pWindow(self)
+        self.s2p_window.show()
+        
     def meanimage(self): 
         for i, (ops, stat_t2p) in enumerate(zip(self.all_ops, self.all_stat_t2p)):
             tab = QWidget()  
             cell_plot = CellPlotWidget(tab, ops=ops, stat_t2p=stat_t2p, f_t2p=self.all_f_t2p[i],
                                        colors=self.colors, update_selection_callback=self.update_selection,
                                        all_f_t2p=self.all_f_t2p, all_ops=self.all_ops,initial_colors=self.init_colors)
             layout = QVBoxLayout(tab)
```

### Comparing `track2p-0.5.2/track2p/gui/raster_wd.py` & `track2p-0.5.3/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/gui/roi_plot.py` & `track2p-0.5.3/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/gui/t2p_wd.py` & `track2p-0.5.3/track2p/gui/t2p_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/io/loaders.py` & `track2p-0.5.3/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/io/s2p_loaders.py` & `track2p-0.5.3/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/io/savers.py` & `track2p-0.5.3/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/match/loop.py` & `track2p-0.5.3/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/match/utils.py` & `track2p-0.5.3/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/ops/default.py` & `track2p-0.5.3/track2p/ops/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         # plotting parameters
         self.win_size = 48 # window size for visualising matched ROIs across days (crop of mean image)
         self.sat_perc = 99.9 # percentile to saturate image at (only affects visualisation not the registration/matching)
         
         self.colors = None # save color after curation
         self.vector_curation=None #save the status of the ROIs after curation
         self.curated_cells=None #save the index of the curated cells
-        
+        #self.indexes_per_day=None #save the indexes of the cells per day
         
         self.save_in_s2p_format = False # save the output in suite2p format (this is useful for downstream analysis with suite2p)
 
         # make the output directories when initialising the object
         
     def init_save_paths(self):
         self.save_path = os.path.join(self.save_path, 'track2p/')
```

### Comparing `track2p-0.5.2/track2p/plot/output.py` & `track2p-0.5.3/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/plot/progress.py` & `track2p-0.5.3/track2p/plot/progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from track2p.plot.utils import match_hist_all
 
 def plot_all_planes(all_ds_avg_ch, track_ops, sat_perc=99):
-    print("starting")
     nplanes = track_ops.nplanes
     fig, axs = plt.subplots(nplanes, len(track_ops.all_ds_path), figsize=(3 * len(track_ops.all_ds_path), 3 * nplanes), dpi=300)
     # add dummy dimension to axs if only one plane
     if nplanes==1:
         axs = np.expand_dims(axs, axis=0)
-    print("starting match hist all")
     all_ds_avg_ch_matched = match_hist_all(all_ds_avg_ch)
 
 
     for i in range(nplanes):
         for j in range(len(track_ops.all_ds_path)):
             img = all_ds_avg_ch_matched[j][i]
             axs[i, j].imshow(img, cmap='gray', vmin=0, vmax=np.percentile(img, sat_perc))
             axs[i, j].set_title('Plane ' + str(i) + ' in dataset ' + str(j))
             axs[i, j].axis('off')
-    print("done")
     plt.close(fig)
-    print("done")
+
```

### Comparing `track2p-0.5.2/track2p/plot/utils.py` & `track2p-0.5.3/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/register/elastix.py` & `track2p-0.5.3/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/register/loop.py` & `track2p-0.5.3/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p/register/utils.py` & `track2p-0.5.3/track2p/register/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 
 def get_all_ds_img_for_reg(all_ds_avg_ch1, all_ds_avg_ch2, track_ops): # chooses which channel to use for registration and returns all_ref_img and all_mov_img (shifted by one day to always register to previous day)
-    print("starting get_all_ds_img_for_reg ")
     if track_ops.reg_chan==0:
         all_ds_avg = all_ds_avg_ch1
     elif track_ops.reg_chan==1:
         all_ds_avg = all_ds_avg_ch2
         print('WARNING: using anatomical channel for registration (this is not always available)')
 
     all_ds_ref_img = []
```

### Comparing `track2p-0.5.2/track2p/t2p.py` & `track2p-0.5.3/track2p/t2p.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.2/track2p.egg-info/PKG-INFO` & `track2p-0.5.3/track2p.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.2
+Version: 0.5.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk==5.4rc2
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.2/track2p.egg-info/SOURCES.txt` & `track2p-0.5.3/track2p.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 track2p/gui/__init__.py
 track2p/gui/cell_plot.py
 track2p/gui/fluo_plot.py
 track2p/gui/import_wd.py
 track2p/gui/main_wd.py
 track2p/gui/raster_wd.py
 track2p/gui/roi_plot.py
+track2p/gui/s2p_wd.py
 track2p/gui/t2p_wd.py
 track2p/io/__init__.py
 track2p/io/loaders.py
 track2p/io/s2p_loaders.py
 track2p/io/savers.py
 track2p/io/utils.py
 track2p/match/__init__.py
```

