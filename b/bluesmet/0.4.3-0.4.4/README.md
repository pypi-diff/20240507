# Comparing `tmp/bluesmet-0.4.3.tar.gz` & `tmp/bluesmet-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluesmet-0.4.3.tar", last modified: Thu Mar 21 12:12:55 2024, max compression
+gzip compressed data, was "bluesmet-0.4.4.tar", last modified: Tue May  7 07:17:11 2024, max compression
```

## Comparing `bluesmet-0.4.3.tar` & `bluesmet-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.427098 bluesmet-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-21 12:11:35.000000 bluesmet-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-21 12:12:55.427098 bluesmet-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-21 12:11:35.000000 bluesmet-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-21 12:11:35.000000 bluesmet-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-21 12:12:55.427098 bluesmet-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-21 12:11:35.000000 bluesmet-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.423098 bluesmet-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.423098 bluesmet-0.4.3/src/bluesmet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.423098 bluesmet-0.4.3/src/bluesmet/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/common/latlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/common/scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.427098 bluesmet-0.4.3/src/bluesmet/normet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/combine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.427098 bluesmet-0.4.3/src/bluesmet/normet/metengine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/metengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/metengine/extreme_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.427098 bluesmet-0.4.3/src/bluesmet/normet/nora3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/nora3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/nora3/arome3km_3hr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/nora3/mywavewam3km.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/nora3/wave_sub_time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.427098 bluesmet-0.4.3/src/bluesmet/normet/norkyst/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/norkyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-21 12:11:35.000000 bluesmet-0.4.3/src/bluesmet/normet/norkyst/zdepths_his.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:12:55.423098 bluesmet-0.4.3/src/bluesmet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-21 12:12:55.000000 bluesmet-0.4.3/src/bluesmet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-21 12:12:55.000000 bluesmet-0.4.3/src/bluesmet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 12:12:55.000000 bluesmet-0.4.3/src/bluesmet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 12:12:55.000000 bluesmet-0.4.3/src/bluesmet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.971500 bluesmet-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 07:16:17.000000 bluesmet-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-07 07:17:11.971500 bluesmet-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 07:16:17.000000 bluesmet-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 07:16:17.000000 bluesmet-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 07:17:11.971500 bluesmet-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 07:16:17.000000 bluesmet-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/common/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/common/scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/normet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/normet/metengine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/metengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/metengine/extreme_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/normet/nora3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/nora3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/nora3/arome3km_3hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/nora3/mywavewam3km.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/nora3/wave_sub_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet/normet/norkyst/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/norkyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 07:16:17.000000 bluesmet-0.4.4/src/bluesmet/normet/norkyst/zdepths_his.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:17:11.967500 bluesmet-0.4.4/src/bluesmet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-07 07:17:11.000000 bluesmet-0.4.4/src/bluesmet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 07:17:11.000000 bluesmet-0.4.4/src/bluesmet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:17:11.000000 bluesmet-0.4.4/src/bluesmet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 07:17:11.000000 bluesmet-0.4.4/src/bluesmet.egg-info/top_level.txt
```

### Comparing `bluesmet-0.4.3/LICENSE` & `bluesmet-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/PKG-INFO` & `bluesmet-0.4.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluesmet
-Version: 0.4.3
+Version: 0.4.4
 Summary: SFI Blues Metocean Library
 Author: SINTEF Ocean
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `bluesmet-0.4.3/README.md` & `bluesmet-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/common/latlon.py` & `bluesmet-0.4.4/src/bluesmet/common/latlon.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/common/scatter.py` & `bluesmet-0.4.4/src/bluesmet/common/scatter.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/cache.py` & `bluesmet-0.4.4/src/bluesmet/normet/cache.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/combine.py` & `bluesmet-0.4.4/src/bluesmet/normet/combine.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/dataset.py` & `bluesmet-0.4.4/src/bluesmet/normet/dataset.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/metengine/extreme_stats.py` & `bluesmet-0.4.4/src/bluesmet/normet/metengine/extreme_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Sequence
 import xarray as xr
 import numpy as np
 import matplotlib.pyplot as plt
 from virocon import get_OMAE2020_Hs_Tz, GlobalHierarchicalModel,IFORMContour
 from xclim.indices.stats import frequency_analysis
 """
-Temporarily copied from https://github.com/MET-OM/metocean_engine/blob/dev/metocean_engine/extreme_stats.py with permissions until the library is made public
+Temporarily copied from https://github.com/MET-OM/metocean-stats/blob/main/metocean_stats/stats/extreme_stats.py with permissions
 
 """
 
 def return_value(hs: xr.DataArray,return_periods=[50,100], month=[1,2,3,4,5, 6, 7, 8, 9, 10,11,12], image_path=None) -> xr.DataArray:
     time = hs.time
     r_val = frequency_analysis(hs, t=return_periods, dist="genextreme", mode="max", freq="YS", month=month)
     if image_path:
@@ -78,16 +78,16 @@
             y.extend(contour['y'])
             y.append(y[0])
 
             rp = contour['return_period']
             ax.plot(x, y, color=color[i],label=str(rp)+'y')
 
         if hs.name and tp.name:
-            ax.set_xlabel(hs.name)
-            ax.set_ylabel(tp.name)
+            ax.set_xlabel(tp.name)
+            ax.set_ylabel(hs.name)
         plt.grid()
         if image_title:
             plt.title(image_title)
         plt.legend()
         plt.savefig(image_path)
 
     return contours
```

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/nora3/arome3km_3hr.py` & `bluesmet-0.4.4/src/bluesmet/normet/nora3/arome3km_3hr.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/nora3/mywavewam3km.py` & `bluesmet-0.4.4/src/bluesmet/normet/nora3/mywavewam3km.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/nora3/wave_sub_time.py` & `bluesmet-0.4.4/src/bluesmet/normet/nora3/wave_sub_time.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet/normet/norkyst/zdepths_his.py` & `bluesmet-0.4.4/src/bluesmet/normet/norkyst/zdepths_his.py`

 * *Files identical despite different names*

### Comparing `bluesmet-0.4.3/src/bluesmet.egg-info/PKG-INFO` & `bluesmet-0.4.4/src/bluesmet.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluesmet
-Version: 0.4.3
+Version: 0.4.4
 Summary: SFI Blues Metocean Library
 Author: SINTEF Ocean
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `bluesmet-0.4.3/src/bluesmet.egg-info/SOURCES.txt` & `bluesmet-0.4.4/src/bluesmet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

