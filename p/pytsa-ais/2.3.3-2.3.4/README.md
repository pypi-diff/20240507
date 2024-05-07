# Comparing `tmp/pytsa_ais-2.3.3.tar.gz` & `tmp/pytsa_ais-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsa_ais-2.3.3.tar", max compression
+gzip compressed data, was "pytsa_ais-2.3.4.tar", max compression
```

## Comparing `pytsa_ais-2.3.3.tar` & `pytsa_ais-2.3.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.3/LICENSE
--rw-r--r--   0        0        0    15713 2024-04-12 09:18:41.000000 pytsa_ais-2.3.3/README.md
--rw-r--r--   0        0        0      952 2024-04-23 08:26:33.511946 pytsa_ais-2.3.3/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-23 08:26:38.695946 pytsa_ais-2.3.3/pytsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.3/pytsa/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.3/pytsa/data/geometry/__init__.py
--rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/denmark.json
--rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/germany.json
--rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/netherlands_detailed.json
--rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/norway.json
--rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/sweden.json
--rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/__init__.py
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/diffquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/dquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/squants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/tquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/trquants.pkl
--rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.3/pytsa/decoder/__init__.py
--rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.3/pytsa/decoder/ais_decoder.py
--rw-r--r--   0        0        0     1548 2024-04-19 11:16:21.000000 pytsa_ais-2.3.3/pytsa/decoder/filedescriptor.py
--rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.3/pytsa/logger.py
--rw-r--r--   0        0        0     6472 2024-04-19 11:52:30.000000 pytsa_ais-2.3.3/pytsa/structs.py
--rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.3/pytsa/trajectories/__init__.py
--rw-r--r--   0        0        0     9694 2024-04-19 08:41:02.000000 pytsa_ais-2.3.3/pytsa/trajectories/inspect.py
--rw-r--r--   0        0        0     5813 2024-04-15 11:06:38.000000 pytsa_ais-2.3.3/pytsa/trajectories/rules.py
--rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.3/pytsa/tsea/__init__.py
--rw-r--r--   0        0        0    29053 2024-04-23 07:39:41.352004 pytsa_ais-2.3.3/pytsa/tsea/search_agent.py
--rw-r--r--   0        0        0     8323 2024-04-23 08:23:14.755950 pytsa_ais-2.3.3/pytsa/tsea/split.py
--rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.3/pytsa/tsea/targetship.py
--rw-r--r--   0        0        0    14189 2024-04-19 11:22:56.000000 pytsa_ais-2.3.3/pytsa/utils.py
--rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.3/pytsa/visualization/__init__.py
--rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.3/pytsa/visualization/ecdf.py
--rw-r--r--   0        0        0    15336 2024-04-15 13:35:43.000000 pytsa_ais-2.3.3/pytsa/visualization/misc.py
--rw-r--r--   0        0        0    16726 1970-01-01 00:00:00.000000 pytsa_ais-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.4/LICENSE
+-rw-r--r--   0        0        0    15713 2024-04-12 09:18:41.000000 pytsa_ais-2.3.4/README.md
+-rw-r--r--   0        0        0      951 2024-05-07 08:48:09.760058 pytsa_ais-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0      721 2024-05-07 08:48:20.500058 pytsa_ais-2.3.4/pytsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.4/pytsa/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.4/pytsa/data/geometry/__init__.py
+-rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.4/pytsa/data/geometry/denmark.json
+-rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.4/pytsa/data/geometry/germany.json
+-rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.4/pytsa/data/geometry/netherlands_detailed.json
+-rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.4/pytsa/data/geometry/norway.json
+-rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.4/pytsa/data/geometry/sweden.json
+-rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/__init__.py
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/diffquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/dquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/squants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/tquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.4/pytsa/data/quantiles/trquants.pkl
+-rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.4/pytsa/decoder/__init__.py
+-rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.4/pytsa/decoder/ais_decoder.py
+-rw-r--r--   0        0        0     1548 2024-04-19 11:16:21.000000 pytsa_ais-2.3.4/pytsa/decoder/filedescriptor.py
+-rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.4/pytsa/logger.py
+-rwxr-xr-x   0        0        0   532504 2024-04-23 12:13:08.835665 pytsa_ais-2.3.4/pytsa/shared/rhaversine.so
+-rw-r--r--   0        0        0     6472 2024-04-19 11:52:30.000000 pytsa_ais-2.3.4/pytsa/structs.py
+-rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.4/pytsa/trajectories/__init__.py
+-rw-r--r--   0        0        0     9694 2024-04-19 08:41:02.000000 pytsa_ais-2.3.4/pytsa/trajectories/inspect.py
+-rw-r--r--   0        0        0     5813 2024-04-15 11:06:38.000000 pytsa_ais-2.3.4/pytsa/trajectories/rules.py
+-rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.4/pytsa/tsea/__init__.py
+-rw-r--r--   0        0        0    29828 2024-04-26 05:43:51.000000 pytsa_ais-2.3.4/pytsa/tsea/search_agent.py
+-rw-r--r--   0        0        0     8323 2024-04-23 08:23:14.755950 pytsa_ais-2.3.4/pytsa/tsea/split.py
+-rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.4/pytsa/tsea/targetship.py
+-rw-r--r--   0        0        0    14618 2024-04-26 05:48:13.000000 pytsa_ais-2.3.4/pytsa/utils.py
+-rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.4/pytsa/visualization/__init__.py
+-rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.4/pytsa/visualization/ecdf.py
+-rw-r--r--   0        0        0    15336 2024-04-15 13:35:43.000000 pytsa_ais-2.3.4/pytsa/visualization/misc.py
+-rw-r--r--   0        0        0    16726 1970-01-01 00:00:00.000000 pytsa_ais-2.3.4/PKG-INFO
```

### Comparing `pytsa_ais-2.3.3/LICENSE` & `pytsa_ais-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/README.md` & `pytsa_ais-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pyproject.toml` & `pytsa_ais-2.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytsa-ais"
-version = "2.3.3"
+version = "2.3.4"
 description = "Toolbox for extracting trajectories and monitoring vessels from raw AIS records."
 authors = ["Niklas Paulig <niklas.paulig@tu-dresden.de>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
@@ -30,8 +30,8 @@
 tomli = "^2.0.1"
 
 [tool.setuptools.package-data]
 "pytsa.data.geometry" = ["*.json"]
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pytsa_ais-2.3.3/pytsa/data/geometry/denmark.json` & `pytsa_ais-2.3.4/pytsa/data/geometry/denmark.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/geometry/germany.json` & `pytsa_ais-2.3.4/pytsa/data/geometry/germany.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/geometry/netherlands_detailed.json` & `pytsa_ais-2.3.4/pytsa/data/geometry/netherlands_detailed.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/geometry/norway.json` & `pytsa_ais-2.3.4/pytsa/data/geometry/norway.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/geometry/sweden.json` & `pytsa_ais-2.3.4/pytsa/data/geometry/sweden.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/quantiles/diffquants.pkl` & `pytsa_ais-2.3.4/pytsa/data/quantiles/diffquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/quantiles/dquants.pkl` & `pytsa_ais-2.3.4/pytsa/data/quantiles/dquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/quantiles/squants.pkl` & `pytsa_ais-2.3.4/pytsa/data/quantiles/squants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/quantiles/tquants.pkl` & `pytsa_ais-2.3.4/pytsa/data/quantiles/tquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/data/quantiles/trquants.pkl` & `pytsa_ais-2.3.4/pytsa/data/quantiles/trquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/decoder/ais_decoder.py` & `pytsa_ais-2.3.4/pytsa/decoder/ais_decoder.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/decoder/filedescriptor.py` & `pytsa_ais-2.3.4/pytsa/decoder/filedescriptor.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/logger.py` & `pytsa_ais-2.3.4/pytsa/logger.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/structs.py` & `pytsa_ais-2.3.4/pytsa/structs.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/trajectories/inspect.py` & `pytsa_ais-2.3.4/pytsa/trajectories/inspect.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/trajectories/rules.py` & `pytsa_ais-2.3.4/pytsa/trajectories/rules.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/tsea/__init__.py` & `pytsa_ais-2.3.4/pytsa/tsea/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/tsea/search_agent.py` & `pytsa_ais-2.3.4/pytsa/tsea/search_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -371,23 +371,43 @@
         # Statistics
         self._n_split_points = 0
         self._n_rejoined_tracks = 0
         self._n_duplicates = 0
         self._n_obs_raw = 0
         self._n_trajectories = 0
 
-
-    def _distribute(self, df: pd.DataFrame) -> list[pd.DataFrame]:
-        """
-        Distribute a given dataframe into smaller
-        dataframes, each containing only messages
-        from a single MMSI.
+    def _distribute(self, df: pd.DataFrame, nparts: int) -> list[pd.DataFrame]:
         """
-        mmsis = df[Msg12318Columns.MMSI.value].unique()
-        return [df[df[Msg12318Columns.MMSI.value] == mmsi] for mmsi in mmsis]
+        Distribute a given dataframe into `nparts`
+        equally sized smaller data frames.
+        
+        Parameters:
+        -----------------
+        df (pd.DataFrame): Pandas DataFrame containing the
+            data to be split
+        nparts (int): number of parts into which `df` is
+            going to be split.
+    
+        Returns:
+        -----------------
+        List of DataFrames: A list of DataFrames, 
+        each being a part of the original DataFrame.
+        """
+        # Check if the DataFrame can be split 
+        # into the desired number of parts
+        if nparts <= 0 or df is None:
+            raise ValueError(
+                "Number of parts must be a positive"
+                "integer and DataFrame must not be None."
+            )
+
+        # Use numpy.array_split to split the 
+        # DataFrame into nearly equal parts
+        return list(np.array_split(df, nparts))
+        
     
     def _impl_construct_target_vessel(self, 
                                       dyn: pd.DataFrame,
                                       stat: pd.DataFrame) -> Targets:
         """
         Construct a single TargetVessel object from a given dataframe.
         """
@@ -440,22 +460,25 @@
         The initial dataframe is split into smaller dataframes, each
         containing only messages from a single MMSI. These dataframes
         are then processed in parallel and the results are merged.
         """
         self.reset_stats()
         singles: list[Targets] = []
         with mp.Pool(njobs) as pool:
+            results = []
             for dyn, stat in self.data_loader.iterate_chunks():
                 self._n_obs_raw += len(dyn)
-                single_frames = self._distribute(dyn)
-                res = pool.starmap(
+                single_frames = self._distribute(dyn,njobs)
+                res = pool.starmap_async(
                     self._impl_construct_target_vessel,
                     [(dframe,stat) for dframe in single_frames]
                 )
-                singles.extend(res)
+                results.append(res)
+            for result in results:
+                singles.extend(result.get())
         targets = self._merge_targets(*singles)
         targets = self._remove_duplicates(targets)
         if not skip_tsplit:
             targets = self._rejoin_tracks(
                 self._determine_split_points(targets)
             )
         self._n_trajectories = sum([len(tgt.tracks) for tgt in targets.values()])
```

### Comparing `pytsa_ais-2.3.3/pytsa/tsea/split.py` & `pytsa_ais-2.3.4/pytsa/tsea/split.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/tsea/targetship.py` & `pytsa_ais-2.3.4/pytsa/tsea/targetship.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/utils.py` & `pytsa_ais-2.3.4/pytsa/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,54 @@
 """
 Utility functions for pytsa
 """
 from __future__ import annotations
 
 from datetime import datetime
 from itertools import cycle
-import math
+import numpy as np
 from pathlib import Path
 from threading import Thread
 import time
 from typing import Callable, Generator
 import pandas as pd
 import psutil
 import vincenty as _vincenty
 import ciso8601
 from .logger import logger
 from .decoder import decode_from_file
 from .decoder.filedescriptor import (
     BaseColumns, Msg12318Columns, Msg5Columns
 )
+try:
+    import rhaversine
+    haversine: Callable = rhaversine.haversine
+except ImportError:
+    logger.warning(
+        "Shared library 'rhaversine.so' not found. "
+        "Using numpy implementation."
+    )
+    def haversine(lon1, lat1, lon2, lat2, miles = True):
+        """
+        Calculate the great circle distance in kilometers between two points 
+        on the earth (specified in decimal degrees)
+        """
+        # convert decimal degrees to radians 
+        lon1, lat1, lon2, lat2 = map(np.radians, [lon1, lat1, lon2, lat2])
+
+        # haversine formula 
+        dlon = lon2 - lon1 
+        dlat = lat2 - lat1 
+        a = (
+            np.sin(dlat/2)**2 + np.cos(lat1) * 
+            np.cos(lat2) * np.sin(dlon/2)**2
+            )
+        c = 2 * np.arcsin(np.sqrt(a)) 
+        r = 3956 if miles else 6371 # Radius of earth in kilometers or miles
+        return c * r
 
 def m2nm(m: float) -> float:
     """Convert meters to nautical miles"""
     return m/1852
 
 def nm2m(nm: float) -> float:
     """Convert nautical miles to meters"""
@@ -41,33 +67,14 @@
     Calculate the great circle distance in kilometers between two points 
     on the earth (specified in decimal degrees)
     """
     p1 = (lat1,lon1)
     p2 = (lat2,lon2)
     return _vincenty.vincenty_inverse(p1,p2,miles=miles)
 
-def haversine(lon1, lat1, lon2, lat2, miles = True):
-    """
-    Calculate the great circle distance in kilometers between two points 
-    on the earth (specified in decimal degrees)
-    """
-    # convert decimal degrees to radians 
-    lon1, lat1, lon2, lat2 = map(math.radians, [lon1, lat1, lon2, lat2])
-
-    # haversine formula 
-    dlon = lon2 - lon1 
-    dlat = lat2 - lat1 
-    a = (
-        math.sin(dlat/2)**2 + math.cos(lat1) * 
-        math.cos(lat2) * math.sin(dlon/2)**2
-        )
-    c = 2 * math.asin(math.sqrt(a)) 
-    r = 3956 if miles else 6371 # Radius of earth in kilometers or miles
-    return c * r
-
 def greater_circle_distance(lon1, lat1, lon2, lat2, miles = True, method = "haversine"):
     """
     Calculate the great circle distance in kilometers between two points 
     on the earth (specified in decimal degrees)
     """
     assert method in ["haversine", "vincenty"], "Invalid method: {}".format(method)
     if method == "haversine":
@@ -102,14 +109,17 @@
     
     Takes a list of paths to static and dynamic data files
     provides utilities to decode and load the data.
     """
     
     # Fraction of the file to load
     chunkfrac = 1/3
+
+    #Engine to use for decoding
+    ENGINE = "pyarrow"
     
     dynamic_columns = [
         BaseColumns.TIMESTAMP.value,
         Msg12318Columns.MMSI.value,
         Msg12318Columns.LAT.value,
         Msg12318Columns.LON.value,
         Msg12318Columns.SPEED.value,
@@ -270,17 +280,17 @@
         """
         Loads all data into memory.
         """
         self.dynamic_data = pd.DataFrame()
         self.static_data = pd.DataFrame()
         for dyn_path, stat_path in zip(self.sdyn,self.sstat):
             logger.info(f"Loading {stat_path.stem} and {dyn_path.stem}")
-            d = pd.read_csv(dyn_path,sep=",",usecols=self.dynamic_columns)
+            d = pd.read_csv(dyn_path,sep=",",usecols=self.dynamic_columns,engine=DataLoader.ENGINE)
             d = self._dynamic_preprocessor(d)
-            s = pd.read_csv(stat_path,sep=",",usecols=self.static_columns)
+            s = pd.read_csv(stat_path,sep=",",usecols=self.static_columns,engine=DataLoader.ENGINE)
             s = self._static_preprocessor(s)
             self.dynamic_data = pd.concat([self.dynamic_data,d])
             self.static_data = pd.concat([self.static_data,s])
         logger.info("Done.")
         
         self.loaded = True
     
@@ -321,16 +331,16 @@
             stat_options["chunksize"] = chunksize_stat
             
             if decode:
                 # Decode dynamic data
                 yield self.from_raw(dyn_path, stat_path)
             else:
                 # Create a generator of pandas DataFrames
-                dyniter = pd.read_csv(dyn_path,**dyn_options)
-                statiter = pd.read_csv(stat_path,**stat_options)
+                dyniter = pd.read_csv(dyn_path,**dyn_options,engine=DataLoader.ENGINE)
+                statiter = pd.read_csv(stat_path,**stat_options,engine=DataLoader.ENGINE)
                 
                 for i, (dc,sc) in enumerate(zip(dyniter,statiter)):
                     logger.info(
                         f"Processing chunk {i+1} of file "
                         f"{dyn_path.stem}"
                     )
                     dc = self._dynamic_preprocessor(dc)
```

### Comparing `pytsa_ais-2.3.3/pytsa/visualization/__init__.py` & `pytsa_ais-2.3.4/pytsa/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/visualization/ecdf.py` & `pytsa_ais-2.3.4/pytsa/visualization/ecdf.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/pytsa/visualization/misc.py` & `pytsa_ais-2.3.4/pytsa/visualization/misc.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.3/PKG-INFO` & `pytsa_ais-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytsa-ais
-Version: 2.3.3
+Version: 2.3.4
 Summary: Toolbox for extracting trajectories and monitoring vessels from raw AIS records.
 Author: Niklas Paulig
 Author-email: niklas.paulig@tu-dresden.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

