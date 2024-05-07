# Comparing `tmp/sorcerun-0.3.4.tar.gz` & `tmp/sorcerun-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.3.4.tar", last modified: Thu Mar 14 18:33:22 2024, max compression
+gzip compressed data, was "sorcerun-0.4.0.tar", last modified: Tue May  7 17:03:15 2024, max compression
```

## Comparing `sorcerun-0.3.4.tar` & `sorcerun-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:33:22.069420 sorcerun-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-14 18:33:17.000000 sorcerun-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-14 18:33:22.069420 sorcerun-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-14 18:33:17.000000 sorcerun-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 18:33:22.069420 sorcerun-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-14 18:33:17.000000 sorcerun-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:33:22.069420 sorcerun-0.3.4/sorcerun/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/grid_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/incense_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-14 18:33:17.000000 sorcerun-0.3.4/sorcerun/sacred_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 18:33:22.069420 sorcerun-0.3.4/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 18:33:22.000000 sorcerun-0.3.4/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 17:03:11.000000 sorcerun-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:03:15.666714 sorcerun-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-07 17:03:11.000000 sorcerun-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:03:15.666714 sorcerun-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-07 17:03:11.000000 sorcerun-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/sorcerun/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/grid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/grid_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/incense_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/top_level.txt
```

### Comparing `sorcerun-0.3.4/LICENSE` & `sorcerun-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.3.4/PKG-INFO` & `sorcerun-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.3.4
+Version: 0.4.0
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: sacred==0.8.4
+Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
 Requires-Dist: xarray
 Requires-Dist: tqdm
 Requires-Dist: streamlit
```

### Comparing `sorcerun-0.3.4/README.md` & `sorcerun-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,16 +12,13 @@
 
 Sorcerun also offers a CLI to help setup and manage a MongoDB observer for sacred.
 
 It also has tools to run **grids** of experiments and then analyze results from experiment grids.
 
 # TODO
 
--   [ ] Add example and documentation (top priority)
--   [x] Grid run utilities via CLI
--   [ ] More template adapters and generate them via CLI
-    -   Specifically something that can track STDOUT and log metrics from STDOUT?
--   [ ] Cleaner source file and other meta info tracking
--   [x] General utilities with `incense` -- maybe build `streamlit` app separately?
--   [x] Better logging for the mongod server
--   [x] Change description to be simpler -- logged function calls
+-   [x] Add example and documentation (top priority)
+    -   [ ] Document the JL example
+-   [ ] Add ability to add and edit tags to `grid_plotter` to filter experiments
 -   [ ] Improve `grid_plotter` with more features for plot customization
+-   [ ] Fix the incense version dependency for `FileStorageObserver`
+-   [ ] Cleaner source file and other meta info tracking
```

### Comparing `sorcerun-0.3.4/setup.py` & `sorcerun-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.3.4",
+    version="0.4.0",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
-        "sacred==0.8.4",
+        "sacred",
         "pymongo",
         "pyyaml",
         "scikit-learn",
         "incense",
         "xarray",
         "tqdm",
         "streamlit",
```

### Comparing `sorcerun-0.3.4/sorcerun/auth_mongodb_option.py` & `sorcerun-0.4.0/sorcerun/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.3.4/sorcerun/cli.py` & `sorcerun-0.4.0/sorcerun/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import os
 import subprocess
 import json, yaml
 from contextlib import ExitStack
 from .mongodb_utils import mongodb_server, init_mongodb
 from .sacred_utils import load_python_module, run_sacred_experiment
 from .incense_utils import squish_dict, unsquish_dict, process_and_save_grid_to_netcdf
-from .globals import AUTH_FILE, TEMP_CONFIGS_DIR, FILE_STORAGE_ROOT, RUNS_DIR
+from .globals import (
+    AUTH_FILE,
+    TEMP_CONFIGS_DIR,
+    FILE_STORAGE_ROOT,
+    RUNS_DIR,
+    TEMPLATE_FILES,
+)
 
 import sys, ipdb, traceback
 
 
 def info(type, value, tb):
     traceback.print_exception(type, value, tb)
     ipdb.pm()
@@ -27,14 +33,32 @@
 )
 def sorcerun(debug):
     if debug:
         sys.excepthook = info
 
 
 @sorcerun.command()
+def template():
+    this_file_path = os.path.abspath(__file__)
+    this_dir = os.path.dirname(this_file_path)
+
+    for file in TEMPLATE_FILES:
+        # check if file already exists in current directory
+        if os.path.exists(file):
+            click.echo(f"File {file} already exists. Skipping creation.")
+            continue
+
+        path_to_template_file = os.path.join(this_dir, file)
+        with open(path_to_template_file, "r") as f:
+            click.echo(f"Creating file: {file}")
+            with open(file, "w") as new_f:
+                new_f.write(f.read())
+
+
+@sorcerun.command()
 @click.argument("python_file", type=click.Path(exists=True, dir_okay=False))
 @click.argument("config_file", type=click.Path(exists=True, dir_okay=False))
 @click.option(
     "--file_root",
     "-f",
     default=FILE_STORAGE_ROOT,
     type=click.Path(file_okay=False),
```

### Comparing `sorcerun-0.3.4/sorcerun/grid_plotter.py` & `sorcerun-0.4.0/sorcerun/grid_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from globals import GRID_OUTPUTS
 import itertools
 import os
 import xarray as xr
 import matplotlib.pyplot as plt
 import streamlit as st
+import scipy.stats
 
 st.title("Grid Plotter")
 # show current working directory
 working_dir = os.getcwd()
 st.write(f"Current working directory: `{working_dir}`")
 
 st.title("Settings")
@@ -183,35 +184,50 @@
         # use itertools product to iterate over all coordinate combinations of dims_used_in_plot
         for coord in itertools.product(
             *[xarr.coords[dim].values for dim in dims_used_in_plot]
         ):
             d = {dim: coord[i] for i, dim in enumerate(dims_used_in_plot)}
             ys = xarr.loc[d]
             for y_axis in y_axes:
-                y = ys.loc[dict(metric=y_axis)].squeeze()
+                y = ys.loc[dict(metric=y_axis)].squeeze().to_numpy()
                 label = " ".join(
                     [f"{y_axis}", ", ".join([f"{k}={v}" for k, v in d.items()])]
                 )
 
                 # check if y is all nans or infs, if so, don't plot
+                good_inds = np.isfinite(y)
 
-                dont_plot = (
-                    y.isnull().all().item() or (y == float("inf")).all().item()
-                )
+                # dont_plot = y.isnull().all().item() or (y == float("inf")).all().item()
+                dont_plot = not np.any(good_inds)
                 if not dont_plot:
-                    plt.plot(x, y, label=label)
+                    plt.plot(x, y, "-o", label=label)
                     # add regression line slope
                     if len(x) > 1 and show_slope:
                         x_to_regress = np.log(x) if log_x else x
                         y_to_regress = np.log(y) if log_y else y
-                        slope, intercept = np.polyfit(x_to_regress, y_to_regress, 1)
+
+                        # remove nans and infs
+                        keep_inds = np.isfinite(x_to_regress) & np.isfinite(
+                            y_to_regress
+                        )
+                        x_to_regress = x_to_regress[np.where(keep_inds)]
+                        y_to_regress = y_to_regress[np.where(keep_inds)]
+
+                        # slope, intercept = np.polyfit(x_to_regress, y_to_regress, 1)
+                        (
+                            slope,
+                            intercept,
+                            r_value,
+                            p_value,
+                            std_err,
+                        ) = scipy.stats.linregress(x_to_regress, y_to_regress)
                         plt.text(
                             x[-1],
                             y[-1],
-                            f"Slope: {slope:.7f}",
+                            f"Slope: {slope:.7f}, $r^2$: {r_value**2:.7f}",
                             horizontalalignment="right",
                             verticalalignment="top",
                         )
 
         if log_x:
             plt.xscale("log")
         if log_y:
```

### Comparing `sorcerun-0.3.4/sorcerun/incense_utils.py` & `sorcerun-0.4.0/sorcerun/incense_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.3.4/sorcerun/mongodb_utils.py` & `sorcerun-0.4.0/sorcerun/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.3.4/sorcerun/sacred_utils.py` & `sorcerun-0.4.0/sorcerun/sacred_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from sacred import Experiment
+from sacred import Experiment, SETTINGS
 import pymongo
 import traceback
 from sacred.observers import MongoObserver, FileStorageObserver
+from sacred.utils import apply_backspaces_and_linefeeds
 import importlib
 import json
 from .globals import AUTH_FILE, RUNS_DIR
 import sys
 import os
 
+SETTINGS.CAPTURE_MODE = "sys"
 
 def load_python_module(python_file):
     file_dir = os.path.dirname(os.path.abspath(python_file))
     file_name = os.path.basename(python_file).replace(".py", "")
 
     sys.path.insert(0, file_dir)
     module = importlib.import_module(file_name)
@@ -25,14 +27,15 @@
     config,
     auth_path=AUTH_FILE,
     use_mongo=True,
     file_storage_root=".",
 ):
     experiment_name = getattr(adapter_func, "experiment_name", "sorcerun_experiment")
     ex = Experiment(experiment_name)
+    ex.captured_out_filter = apply_backspaces_and_linefeeds
 
     # Read auth_data from auth_path
     if use_mongo:
         if os.path.exists(auth_path):
             with open(auth_path, "r") as f:
                 auth_data = json.load(f)
 
@@ -71,11 +74,23 @@
 
     @ex.main
     def run_experiment(_config, _run):
         _run.info["info"] = "info-entry"
         result = adapter_func(_config, _run)
         return result
 
-    try:
-        ex.run()
-    except:
-        traceback.print_exc()
+    ex.run()
+
+
+class DummyRun():
+    def __init__(self):
+        pass
+
+    def to_dict(self):
+        pass
+
+    def log_scalar(self, key, value, step=0):
+        pass
+
+    def add_artifact(self, filename, name):
+        pass
+
```

### Comparing `sorcerun-0.3.4/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.4.0/sorcerun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.3.4
+Version: 0.4.0
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: sacred==0.8.4
+Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
 Requires-Dist: xarray
 Requires-Dist: tqdm
 Requires-Dist: streamlit
```

