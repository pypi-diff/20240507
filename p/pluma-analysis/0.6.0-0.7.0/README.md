# Comparing `tmp/pluma_analysis-0.6.0.tar.gz` & `tmp/pluma_analysis-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluma_analysis-0.6.0.tar", last modified: Fri May  3 12:58:14 2024, max compression
+gzip compressed data, was "pluma_analysis-0.7.0.tar", last modified: Tue May  7 12:55:11 2024, max compression
```

## Comparing `pluma_analysis-0.6.0.tar` & `pluma_analysis-0.7.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.129819 pluma_analysis-0.6.0/
--rw-rw-rw-   0        0        0       78 2024-01-04 11:17:02.000000 pluma_analysis-0.6.0/.gitignore
--rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma_analysis-0.6.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma_analysis-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2554 2024-05-03 12:58:14.127819 pluma_analysis-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-03 12:56:42.000000 pluma_analysis-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.972980 pluma_analysis-0.6.0/pluma/
--rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma_analysis-0.6.0/pluma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.975485 pluma_analysis-0.6.0/pluma/export/
--rw-rw-rw-   0        0        0     2334 2024-05-03 12:20:23.000000 pluma_analysis-0.6.0/pluma/export/maps.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.979503 pluma_analysis-0.6.0/pluma/export/ogcapi/
--rw-rw-rw-   0        0        0     2988 2024-05-03 12:33:39.000000 pluma_analysis-0.6.0/pluma/export/ogcapi/features.py
--rw-rw-rw-   0        0        0     2465 2024-04-05 03:03:44.000000 pluma_analysis-0.6.0/pluma/export/ogcapi/records.py
--rw-rw-rw-   0        0        0     6426 2024-04-05 03:04:11.000000 pluma_analysis-0.6.0/pluma/export/streams.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:13.998071 pluma_analysis-0.6.0/pluma/io/
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.002069 pluma_analysis-0.6.0/pluma/io/_nepy/
--rw-rw-rw-   0        0        0    18315 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/_nepy/NedfReader.py
--rw-rw-rw-   0        0        0     2006 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/accelerometer.py
--rw-rw-rw-   0        0        0     4605 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/eeg.py
--rw-rw-rw-   0        0        0     3317 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/empatica.py
--rw-rw-rw-   0        0        0     3494 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/harp.py
--rw-rw-rw-   0        0        0     1442 2024-05-03 12:22:48.000000 pluma_analysis-0.6.0/pluma/io/microphone.py
--rw-rw-rw-   0        0        0     3777 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/path_helper.py
--rw-rw-rw-   0        0        0     6800 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/io/ubx.py
--rw-rw-rw-   0        0        0     1046 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/io/zeromq.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.013594 pluma_analysis-0.6.0/pluma/preprocessing/
--rw-rw-rw-   0        0        0     2107 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/ecg.py
--rw-rw-rw-   0        0        0     2401 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/resampling.py
--rw-rw-rw-   0        0        0      511 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/preprocessing/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.039152 pluma_analysis-0.6.0/pluma/schema/
--rw-rw-rw-   0        0        0    11227 2024-05-03 12:51:39.000000 pluma_analysis-0.6.0/pluma/schema/__init__.py
--rw-rw-rw-   0        0        0    11160 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/schema/outdoor.py
--rw-rw-rw-   0        0        0    12228 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/schema/vr.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.071719 pluma_analysis-0.6.0/pluma/stream/
--rw-rw-rw-   0        0        0     3076 2024-05-03 11:22:24.000000 pluma_analysis-0.6.0/pluma/stream/__init__.py
--rw-rw-rw-   0        0        0     1857 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/accelerometer.py
--rw-rw-rw-   0        0        0     1468 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/csv.py
--rw-rw-rw-   0        0        0     1733 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/eeg.py
--rw-rw-rw-   0        0        0      947 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/empatica.py
--rw-rw-rw-   0        0        0     6626 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/georeference.py
--rw-rw-rw-   0        0        0     2298 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/harp.py
--rw-rw-rw-   0        0        0     1097 2024-05-03 11:07:19.000000 pluma_analysis-0.6.0/pluma/stream/microphone.py
--rw-rw-rw-   0        0        0     1578 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/siconversion.py
--rw-rw-rw-   0        0        0     3023 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/stream/ubx.py
--rw-rw-rw-   0        0        0     6408 2024-05-02 08:42:57.000000 pluma_analysis-0.6.0/pluma/stream/zeromq.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.082241 pluma_analysis-0.6.0/pluma/sync/
--rw-rw-rw-   0        0        0     2049 2024-04-05 03:07:52.000000 pluma_analysis-0.6.0/pluma/sync/__init__.py
--rw-rw-rw-   0        0        0     1337 2024-05-02 13:12:29.000000 pluma_analysis-0.6.0/pluma/sync/plotting.py
--rw-rw-rw-   0        0        0     6918 2024-05-03 00:07:30.000000 pluma_analysis-0.6.0/pluma/sync/ubx2harp.py
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.085240 pluma_analysis-0.6.0/pluma/templates/
--rw-rw-rw-   0        0        0     2980 2024-01-04 11:17:02.000000 pluma_analysis-0.6.0/pluma/templates/metadata_template.j2
-drwxrwxrwx   0        0        0        0 2024-05-03 12:58:14.125810 pluma_analysis-0.6.0/pluma_analysis.egg-info/
--rw-rw-rw-   0        0        0     2554 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 12:58:13.000000 pluma_analysis-0.6.0/pluma_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1545 2024-05-02 08:55:22.000000 pluma_analysis-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 12:58:14.129819 pluma_analysis-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.460892 pluma_analysis-0.7.0/
+-rw-rw-rw-   0        0        0       78 2024-01-04 11:17:02.000000 pluma_analysis-0.7.0/.gitignore
+-rw-rw-rw-   0        0        0     1092 2022-11-21 15:02:54.000000 pluma_analysis-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-08-12 12:33:04.000000 pluma_analysis-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2605 2024-05-07 12:55:11.458888 pluma_analysis-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-07 12:54:30.000000 pluma_analysis-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.402112 pluma_analysis-0.7.0/pluma/
+-rw-rw-rw-   0        0        0        0 2023-08-12 12:33:04.000000 pluma_analysis-0.7.0/pluma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.405110 pluma_analysis-0.7.0/pluma/export/
+-rw-rw-rw-   0        0        0     3266 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/export/maps.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.407113 pluma_analysis-0.7.0/pluma/export/ogcapi/
+-rw-rw-rw-   0        0        0     3014 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/export/ogcapi/features.py
+-rw-rw-rw-   0        0        0     2465 2024-04-05 03:03:44.000000 pluma_analysis-0.7.0/pluma/export/ogcapi/records.py
+-rw-rw-rw-   0        0        0     6674 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/export/streams.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.416113 pluma_analysis-0.7.0/pluma/io/
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.417111 pluma_analysis-0.7.0/pluma/io/_nepy/
+-rw-rw-rw-   0        0        0    18315 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/_nepy/NedfReader.py
+-rw-rw-rw-   0        0        0     2006 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/accelerometer.py
+-rw-rw-rw-   0        0        0     4678 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/io/eeg.py
+-rw-rw-rw-   0        0        0     3317 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/empatica.py
+-rw-rw-rw-   0        0        0     3494 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/harp.py
+-rw-rw-rw-   0        0        0     1442 2024-05-03 12:22:48.000000 pluma_analysis-0.7.0/pluma/io/microphone.py
+-rw-rw-rw-   0        0        0     3777 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/path_helper.py
+-rw-rw-rw-   0        0        0     6800 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/io/ubx.py
+-rw-rw-rw-   0        0        0     1046 2024-05-02 08:42:57.000000 pluma_analysis-0.7.0/pluma/io/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.420112 pluma_analysis-0.7.0/pluma/preprocessing/
+-rw-rw-rw-   0        0        0     2107 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/preprocessing/ecg.py
+-rw-rw-rw-   0        0        0     2901 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/preprocessing/resampling.py
+-rw-rw-rw-   0        0        0      511 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/preprocessing/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.423110 pluma_analysis-0.7.0/pluma/schema/
+-rw-rw-rw-   0        0        0    11144 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/schema/__init__.py
+-rw-rw-rw-   0        0        0    11160 2024-05-02 08:42:57.000000 pluma_analysis-0.7.0/pluma/schema/outdoor.py
+-rw-rw-rw-   0        0        0    12228 2024-05-02 08:42:57.000000 pluma_analysis-0.7.0/pluma/schema/vr.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.436376 pluma_analysis-0.7.0/pluma/stream/
+-rw-rw-rw-   0        0        0     3221 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/__init__.py
+-rw-rw-rw-   0        0        0     1959 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/accelerometer.py
+-rw-rw-rw-   0        0        0     1611 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/csv.py
+-rw-rw-rw-   0        0        0     1808 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/eeg.py
+-rw-rw-rw-   0        0        0     1048 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/empatica.py
+-rw-rw-rw-   0        0        0     6626 2024-05-07 12:47:49.000000 pluma_analysis-0.7.0/pluma/stream/georeference.py
+-rw-rw-rw-   0        0        0     2367 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/harp.py
+-rw-rw-rw-   0        0        0     1097 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/microphone.py
+-rw-rw-rw-   0        0        0     1578 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/stream/siconversion.py
+-rw-rw-rw-   0        0        0     3023 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/stream/ubx.py
+-rw-rw-rw-   0        0        0     6730 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/stream/zeromq.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.439374 pluma_analysis-0.7.0/pluma/sync/
+-rw-rw-rw-   0        0        0     2049 2024-04-05 03:07:52.000000 pluma_analysis-0.7.0/pluma/sync/__init__.py
+-rw-rw-rw-   0        0        0     1337 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/sync/plotting.py
+-rw-rw-rw-   0        0        0     6918 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pluma/sync/ubx2harp.py
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.440375 pluma_analysis-0.7.0/pluma/templates/
+-rw-rw-rw-   0        0        0     2980 2024-01-04 11:17:02.000000 pluma_analysis-0.7.0/pluma/templates/metadata_template.j2
+drwxrwxrwx   0        0        0        0 2024-05-07 12:55:11.457889 pluma_analysis-0.7.0/pluma_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2605 2024-05-07 12:55:11.000000 pluma_analysis-0.7.0/pluma_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2024-05-07 12:55:11.000000 pluma_analysis-0.7.0/pluma_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 12:55:11.000000 pluma_analysis-0.7.0/pluma_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-07 12:55:11.000000 pluma_analysis-0.7.0/pluma_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 12:55:11.000000 pluma_analysis-0.7.0/pluma_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1580 2024-05-07 12:53:10.000000 pluma_analysis-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 12:55:11.460892 pluma_analysis-0.7.0/setup.cfg
```

### Comparing `pluma_analysis-0.6.0/LICENSE` & `pluma_analysis-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/PKG-INFO` & `pluma_analysis-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluma-analysis
-Version: 0.6.0
+Version: 0.7.0
 Summary: A low-level interface to data collected with the pluma urban data acquisition system
 Author-email: Goncalo Lopes <g.lopes@neurogears.org>, Bruno Cruz <b.cruz@neurogears.org>, Andrew Erskine <a.erskine@neurogears.org>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/emotional-cities/pluma-analysis/issues
 Project-URL: Source Code, https://github.com/emotional-cities/pluma-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -14,14 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
+Requires-Dist: mapclassify
+Requires-Dist: folium
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: s3fs
 Requires-Dist: pyubx2
 Requires-Dist: tilemapbase
```

### Comparing `pluma_analysis-0.6.0/README.md` & `pluma_analysis-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/export/ogcapi/features.py` & `pluma_analysis-0.7.0/pluma/export/ogcapi/features.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 from __future__ import annotations
 import os
 import datetime
 import pandas as pd
 import geopandas as gpd
-from dotmap import DotMap
+import pluma.preprocessing.resampling as resampling
 
+from dotmap import DotMap
 from pluma.stream import Stream
 
 
-exclude_devices = ["PupilLabs", "Microphone", "Empatica", "BioData", "UBX"]
+exclude_devices = ["PupilLabs", "Microphone", "Empatica", "BioData", "Enobio", "UBX"]
 
 
 def convert_dataset_to_geoframe(
         dataset,
         sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1)
         ):
 
+    georef = resampling.resample_georeference(dataset.georeference.spacetime, sampling_dt)
     streams_to_export = {}
     for stream in dataset.streams:
         _ = recursive_resample_stream(
-            streams_to_export, dataset.streams[stream], sampling_dt)
+            streams_to_export, dataset.streams[stream], georef)
 
     exclude = ['Latitude', 'Longitude', 'Elevation']
-
-    out = streams_to_export[list(streams_to_export.keys())[0]].copy()
-    out = out.iloc[:, 0:3]
-
     out_columns = []
     for stream in streams_to_export:
         cols = list(streams_to_export[stream].columns)
         for idx, entry in enumerate(cols):
             if entry in exclude:
                 continue
 
             cols[idx] = (stream if entry.lower() == "data" else
                          f"{stream}_{entry}").lower()
         streams_to_export[stream].columns = cols
-        out_columns.append(streams_to_export[stream].drop(exclude, axis=1))
-    out = out.join(out_columns)
-    out.index.name = 'time'
+        out_columns.append(streams_to_export[stream])
 
-    geometry = gpd.points_from_xy(
-        x=out['Longitude'],
-        y=out['Latitude'],
-        z=out['Elevation'])
-    out = gpd.GeoDataFrame(out.drop(exclude, axis=1), geometry=geometry)
-    out.crs = 'epsg:4326'
+    geometry = out_columns[0][out_columns[0].columns[-1]]
+    out = gpd.GeoDataFrame(pd.concat([d.drop(d.columns[-1], axis=1)
+                                      for d in out_columns], axis=1),
+                                      geometry=geometry)
+    out.index.name = 'time'
     return out
 
 def export_dataset_to_geojson(
         dataset,
         filename,
         sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1)
         ):
```

### Comparing `pluma_analysis-0.6.0/pluma/export/ogcapi/records.py` & `pluma_analysis-0.7.0/pluma/export/ogcapi/records.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/export/streams.py` & `pluma_analysis-0.7.0/pluma/export/streams.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ## Export streams to csv
 from __future__ import annotations
 import os
 import datetime
 import pandas as pd
+import geopandas as gpd
 
 from typing import Union, Optional, Callable, Dict
 
 from pluma.stream import Stream, StreamType
 
 import pluma.preprocessing.resampling as resampling
 
@@ -58,23 +59,22 @@
                                     georeference,
                                     **resampling_function_kws)
     resampled.to_csv(f"{outdir}\\{stream.streamlabel}.csv", date_format='%Y-%m-%dT%H:%M:%S.%fZ')
 
 
 def resample_stream_harp(stream: Stream,
                          sampling_dt: datetime.timedelta = datetime.timedelta(seconds=2),
-                         sampler: Callable = resampling.resample_temporospatial,
-                         **kwargs) -> pd.DataFrame:
+                         sampler: Callable = resampling.resample_temporospatial) -> gpd.GeoDataFrame:
     check_stream_data_integrity(stream)
-    return sampler(stream.data, _get_georef(stream), sampling_dt)
+    return sampler(stream.data, _get_resampled_georef(stream, sampling_dt), sampling_dt=None)
 
 
 def resample_stream_accelerometer(stream: Stream,
-                                  sampling_dt: datetime.timedelta = datetime.timedelta(seconds=2),
-                                  **kwargs) -> pd.DataFrame:
+                                  sampling_dt: Union[pd.DataFrame, datetime.timedelta]
+                                  ) -> gpd.GeoDataFrame:
     check_stream_data_integrity(stream)
     col_sampler = {
         'Orientation_X': resampling.resample_temporospatial_circ,
         'Orientation_Y': resampling.resample_temporospatial_circ,
         'Orientation_Z': resampling.resample_temporospatial_circ,
         'Gyroscope_X': resampling.resample_temporospatial,
         'Gyroscope_Y': resampling.resample_temporospatial,
@@ -87,55 +87,61 @@
         'Magnetometer_Z': resampling.resample_temporospatial,
         'Accl_X': resampling.resample_temporospatial,
         'Accl_Y': resampling.resample_temporospatial,
         'Accl_Z': resampling.resample_temporospatial,
         'Gravity_X': resampling.resample_temporospatial,
         'Gravity_Y': resampling.resample_temporospatial,
         'Gravity_Z': resampling.resample_temporospatial}
-    georef = _get_georef(stream)
-    resampled_data = {k: resampling_method(stream.data[k], georef, sampling_dt)
-                      for k, resampling_method in col_sampler.items()
-                      if k in stream.data.columns}
-    out = resampled_data[list(col_sampler.keys())[0]].copy()
-    out.drop(columns=['Data'], axis=1, inplace=True)
-
-    for key in resampled_data.keys():
-        out[key] = resampled_data[key]["Data"]
-    return out
+    return _resample_multistream(stream, col_sampler, sampling_dt)
 
 
 def resample_stream_empatica(stream: Stream,
-                            sampling_dt: datetime.timedelta = datetime.timedelta(seconds=2),
-                             **kwargs) -> pd.DataFrame:
-    check_stream_data_integrity(stream)
+                             sampling_dt: datetime.timedelta = datetime.timedelta(seconds=2)
+                             ) -> gpd.GeoDataFrame:
     col_sampler = {
         'E4_Gsr': resampling.resample_temporospatial,
         'E4_Hr': resampling.resample_temporospatial,
         'E4_Ibi': resampling.resample_temporospatial}
-    georef = _get_georef(stream)
-    resampled_data = {k: resampling_method(stream.data[k]["Value"], georef, sampling_dt)
-                      for k, resampling_method in col_sampler.items()
-                      if k in stream.data}
-    out = resampled_data[list(col_sampler.keys())[0]].copy()
-    out.drop(columns=['Data'], axis=1, inplace=True)
-
-    for key in resampled_data.keys():
-        out[key] = resampled_data[key]["Data"]
-    return out
+    return _resample_multistream(stream, col_sampler, sampling_dt)
+
+
+def _resample_multistream(
+        stream: Stream,
+        col_sampler: dict[str, Callable],
+        sampling_dt: Union[pd.DataFrame, datetime.timedelta]) -> gpd.GeoDataFrame:
+    check_stream_data_integrity(stream)
+    resampled = _get_resampled_georef(stream, sampling_dt)
+    resampled_data = [sampler(stream.data[key], resampled, sampling_dt=None)
+                      for key, sampler in col_sampler.items()
+                      if key in stream.data]
+    geometry = resampled_data[0].geometry
+    return gpd.GeoDataFrame(pd.concat([d.drop('geometry', axis=1)
+                                       for d in resampled_data], axis=1),
+                                       geometry=geometry)
 
 
 def check_stream_data_integrity(stream: Stream):
     if stream.data is None:
         raise ValueError("The stream does not have valid data.")
 
 
-def _get_georef(stream: Stream) -> pd.DataFrame:
+def _get_resampled_georef(stream: Stream, sampler: Union[pd.DataFrame, datetime.timedelta]) -> pd.DataFrame:
+    if isinstance(sampler, pd.DataFrame):
+        return sampler
+    
     if hasattr(stream, "parent_dataset") is False:
         raise AttributeError("The stream does not have a valid parent Dataset.")
     if stream.parent_dataset is None:
         raise ValueError("The stream does not have a valid parent Dataset.")
     if stream.parent_dataset.has_calibration is False:
         raise ValueError(
             "The stream's parent Dataset does not have a valid calibration.\
                 Calibrate the Dataset before exporting the stream by\
                     calling Dataset.add_georeference_and_calibrate()")
-    return stream.parent_dataset.georeference
+    georef = stream.parent_dataset.georeference.spacetime
+    return resampling.resample_georeference(georef, sampler)
+
+
+def shift_stream_index(data, offset):
+    """Offsets the specified stream data index."""
+    if len(data) > 0:
+        data.index += offset
```

### Comparing `pluma_analysis-0.6.0/pluma/io/_nepy/NedfReader.py` & `pluma_analysis-0.7.0/pluma/io/_nepy/NedfReader.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/accelerometer.py` & `pluma_analysis-0.7.0/pluma/io/accelerometer.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/eeg.py` & `pluma_analysis-0.7.0/pluma/io/eeg.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
     root = ensure_complexpath(root)
     filename = root
     filename.join("*.nedf")
 
     expected_files = filename.glob(filename.path)
     if len(expected_files) == 0:
-        raise FileNotFoundError(f"No *.nedf files found in {root}.")
+        warnings.warn(f"No *.nedf files found in {root}.")
+        ret = None
     elif len(expected_files) > 1:
         warnings.warn(f"Multiple *.nedf files found in {root}. "
                       f"Loading {expected_files[if_multiple_load_index]}.")
         ret = expected_files[if_multiple_load_index]
     else:
         ret = expected_files[0]
 
@@ -58,14 +59,16 @@
         object from the nepy package.
         - pd.DataFrame: returns a dataframe with the server lsl markers
     """
 
     root = ensure_complexpath(root)
     if filename is None:
         filename = get_eeg_file(root)
+        if filename is None:
+            return (None, None)
     else:
         root.join(filename)
         filename = root
 
     _out = NedfReader(filename, **kwargs)
     _server_lsl_markers = load_server_lsl_markers(root=root)
     _server_lsl_markers["EegSample"] = -1
```

### Comparing `pluma_analysis-0.6.0/pluma/io/empatica.py` & `pluma_analysis-0.7.0/pluma/io/empatica.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/harp.py` & `pluma_analysis-0.7.0/pluma/io/harp.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/microphone.py` & `pluma_analysis-0.7.0/pluma/io/microphone.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/path_helper.py` & `pluma_analysis-0.7.0/pluma/io/path_helper.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/ubx.py` & `pluma_analysis-0.7.0/pluma/io/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/io/zeromq.py` & `pluma_analysis-0.7.0/pluma/io/zeromq.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/preprocessing/ecg.py` & `pluma_analysis-0.7.0/pluma/preprocessing/ecg.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/schema/__init__.py` & `pluma_analysis-0.7.0/pluma/schema/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pickle
 import datetime
 
 from dotmap import DotMap
 from typing import Union, Optional, Callable
 
+from pluma.export.streams import shift_stream_index
 from pluma.schema.outdoor import build_schema
 
 from pluma.sync.ubx2harp import SyncLookup, get_clockcalibration_model, get_clockcalibration_lookup
 from pluma.sync import ClockRefId
 
 from pluma.stream import StreamType, Stream
 
@@ -224,47 +225,40 @@
             reference_from=ClockRefId.HARP)
         self.has_calibration = True
         return sync_lookup
 
     def showmap(self, **kwargs):
         """Overload to export.showmap that shows spatial information color-coded by time.
         """
-        temp_df = self.georeference.spacetime.assign(Data=1)
-        fig = maps.showmap(temp_df, **kwargs)
-        return fig
+        return maps.showmap(self.georeference.spacetime, **kwargs)
 
     def add_georeference_and_calibrate(self, plot_diagnosis=True):
         if self.has_calibration is False:
             self.calibrate_ubx_to_harp(plot_diagnosis=plot_diagnosis, dt_error=1)
             self.add_ubx_georeference(event=_UBX_MSGIDS.NAV_HPPOSLLH,
                                     calibrate_clock=True)
             self.has_calibration = True
         else:
             raise AssertionError('Dataset is already been automatically calibrated.')
         
-    @staticmethod
-    def _offset_data_index(data, offset):
-        if isinstance(data, DotMap):
-            for frame in data.values():
-                Dataset._offset_data_index(frame, offset)
-        else:
-            data.index += offset - data.index[0]
-        
     def reference_harp_to_ubx_time(self):
         if self.has_calibration is False:
             raise AssertionError('Dataset is not calibrated to UBX time.')
 
-        utc_offset = self.streams.UBX.positiondata['Time_UTC'][0]
-        Dataset._offset_data_index(self.georeference.spacetime, utc_offset)
-        Dataset._offset_data_index(self.georeference.time, utc_offset)
+        utc_offset = self.streams.UBX.positiondata['Time_UTC'][0] - self.georeference.time[0]
+        shift_stream_index(self.georeference.spacetime, utc_offset)
+        shift_stream_index(self.georeference.time, utc_offset)
+        shift_stream_index(self.georeference.latitude, utc_offset)
+        shift_stream_index(self.georeference.longitude, utc_offset)
+        shift_stream_index(self.georeference.elevation, utc_offset)
         for stream in self._iter_schema_streams(self.streams):
-            if len(stream.data) == 0:
+            if stream.data is None:
                 continue
             if stream.clockreference.referenceid == ClockRefId.HARP:
-                Dataset._offset_data_index(stream.data, utc_offset)
+                stream.add_clock_offset(utc_offset)
                 stream.clockreference.referenceid = ClockRefId.GNSS
         
     def to_geoframe(self,
                     sampling_dt: datetime.timedelta = datetime.timedelta(seconds=1)):
         return convert_dataset_to_geoframe(self, sampling_dt)
 
     def to_geojson(self,
```

### Comparing `pluma_analysis-0.6.0/pluma/schema/outdoor.py` & `pluma_analysis-0.7.0/pluma/schema/outdoor.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/schema/vr.py` & `pluma_analysis-0.7.0/pluma/schema/vr.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/stream/__init__.py` & `pluma_analysis-0.7.0/pluma/stream/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 		self._rootfolder = value
 
 	def load(self):
 		raise NotImplementedError("load() method is not implemented for the Stream base class.")
 
 	def resample(self):
 		raise NotImplementedError("resample() method is not implemented for the Stream base class.")
+	
+	def add_clock_offset(self, offset):
+		raise NotImplementedError("add_clock_offset() method is not implemented for the Stream base class.")
 
 	def reload(self):
 		self.load()
 
 	def plot(self, col=None, **kwargs):
 		if self.data.empty:
 			raise ValueError("Input dataframe is empty.")
```

### Comparing `pluma_analysis-0.6.0/pluma/stream/accelerometer.py` & `pluma_analysis-0.7.0/pluma/stream/accelerometer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import datetime
 
 from pluma.stream import Stream, StreamType
 from pluma.stream.siconversion import SiUnitConversion
 from pluma.io.accelerometer import load_accelerometer, _accelerometer_header
 from pluma.sync import ClockRefId
-from pluma.export.streams import resample_stream_accelerometer
+from pluma.export.streams import shift_stream_index, resample_stream_accelerometer
 
 class AccelerometerStream(Stream):
 	"""_summary_
 
 	Args:
 		Stream (_type_): _description_
 	"""
@@ -50,7 +50,10 @@
 		return f'Accelerometer stream from device {self.device},\
       stream {self.streamlabel}'
 
 	def resample(self,
 	      sampling_dt: datetime.timedelta,
 		  **kwargs) -> pd.DataFrame:
 		return resample_stream_accelerometer(self, sampling_dt, **kwargs)
+	
+	def add_clock_offset(self, offset):
+		shift_stream_index(self.data, offset)
```

### Comparing `pluma_analysis-0.6.0/pluma/stream/eeg.py` & `pluma_analysis-0.7.0/pluma/stream/eeg.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,29 +27,32 @@
 		super(EegStream, self).__init__(data=data, **kw)
 		self.streamtype = StreamType.EEG
 		self.clockreference.referenceid = clockreferenceid
 		self.autoalign = autoalign
 		self.server_lsl_marker = server_lsl_marker
 		if self.autoload:
 			self.load()
-			if (self.autoalign and (self.clockreference.referenceid == ClockRefId.HARP)):
-				self.align_to_harp()
 
 	def load(self):
 		self.data, _lsl_timestamp = load_eeg(
 			filename=None,
 			root=self.rootfolder)
 		if self.server_lsl_marker is None:
 			self.server_lsl_marker = _lsl_timestamp
-			if (self.autoalign and (self.clockreference.referenceid == ClockRefId.HARP)):
-				self.align_to_harp()
+		if self.data is not None and self.autoalign and (self.clockreference.referenceid == ClockRefId.HARP):
+			self.align_to_harp()
 
 	def align_to_harp(self):
 		print("Attempting to automatically correct eeg timestamps to harp timestamps...")
 		eeg_to_harp_model = (synchronize_eeg_to_harp(self.server_lsl_marker))
 		self.data.np_time = HarpStream.from_seconds(
 			eeg_to_harp_model.predict(self.data.np_time.reshape(-1, 1))
 			.flatten())
 		print("Done.")
 
+	def add_clock_offset(self, offset):
+		if self.server_lsl_marker is not None:
+			self.server_lsl_marker['Seconds'] += offset
+		self.data.np_time += offset
+
 	def __str__(self):
 		return f'EEG stream from device {self.device}, stream {self.streamlabel}'
```

### Comparing `pluma_analysis-0.6.0/pluma/stream/empatica.py` & `pluma_analysis-0.7.0/pluma/stream/empatica.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import datetime
 
 from pluma.stream import Stream, StreamType
 from pluma.io.empatica import load_empatica
 from pluma.sync import ClockRefId
-from pluma.export.streams import resample_stream_empatica
+from pluma.export.streams import shift_stream_index, resample_stream_empatica
 
 
 class EmpaticaStream(Stream):
 	"""_summary_
 
 	Args:
 		Stream (_type_): _description_
@@ -25,11 +25,13 @@
 
 	def load(self):
 		self.data = load_empatica(root=self.rootfolder)
 
 	def __str__(self):
 		return f'Empatica stream from device {self.device}, stream {self.streamlabel}'
 
-	def resample(self,
-	      sampling_dt: datetime.timedelta,
-	      **kwargs) -> pd.DataFrame:
-		return resample_stream_empatica(self, sampling_dt, **kwargs)
+	def resample(self, sampling_dt: datetime.timedelta) -> pd.DataFrame:
+		return resample_stream_empatica(self, sampling_dt)
+	
+	def add_clock_offset(self, offset):
+		for stream in self.data.values():
+			shift_stream_index(stream, offset)
```

### Comparing `pluma_analysis-0.6.0/pluma/stream/georeference.py` & `pluma_analysis-0.7.0/pluma/stream/georeference.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/stream/harp.py` & `pluma_analysis-0.7.0/pluma/stream/harp.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pluma.stream import Stream, StreamType
 from pluma.io.harp import load_harp_stream, _HARP_T0
 
 from pluma.stream.siconversion import SiUnitConversion
 
 from pluma.sync import ClockRefId
 
-from pluma.export.streams import export_stream_to_csv, resample_stream_harp
+from pluma.export.streams import export_stream_to_csv, resample_stream_harp, shift_stream_index
 
 
 class HarpStream(Stream):
 	"""_summary_
 
 	Args:
 		Stream (_type_): _description_
@@ -64,11 +64,12 @@
 	def from_seconds(index):
 		# Converts seconds (double) back to a harp referenced timedelta
 		return (_HARP_T0 + pd.to_timedelta(index, 's')).values
 
 	def export_to_csv(self, root_path, **kwargs):
 		export_stream_to_csv(self, root_path, **kwargs)
 
-	def resample(self,
-	      sampling_dt: datetime.timedelta,
-		  **kwargs) -> pd.DataFrame:
-		return resample_stream_harp(self, sampling_dt, **kwargs)
+	def resample(self, sampling_dt: datetime.timedelta) -> pd.DataFrame:
+		return resample_stream_harp(self, sampling_dt)
+	
+	def add_clock_offset(self, offset):
+		shift_stream_index(self.data, offset)
```

### Comparing `pluma_analysis-0.6.0/pluma/stream/microphone.py` & `pluma_analysis-0.7.0/pluma/stream/microphone.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/stream/siconversion.py` & `pluma_analysis-0.7.0/pluma/stream/siconversion.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/stream/ubx.py` & `pluma_analysis-0.7.0/pluma/stream/ubx.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/stream/zeromq.py` & `pluma_analysis-0.7.0/pluma/stream/zeromq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pandas as pd
 
 from pluma.stream import StreamType
 from pluma.stream import Stream
 from pluma.io.zeromq import load_zeromq
+from pluma.export.streams import shift_stream_index
 
 
 class PupilStream(Stream):
     def __init__(self, **kw):
         super(PupilStream, self).__init__(**kw)
 
         self.streamtype = StreamType.PUPIL
@@ -19,32 +20,38 @@
 
     def convert_to_si(self, data=None):
         pass
 
     def export_to_csv(self, export_path):
         self.data.to_csv(export_path)
 
+    def add_clock_offset(self, offset):
+        shift_stream_index(self.data, offset)
+
 
 class GliaStream(Stream):
     def __init__(self, **kw):
-        super(PupilStream, self).__init__(**kw)
+        super(GliaStream, self).__init__(**kw)
 
         self.streamtype = StreamType.GLIA
         if self.autoload:
             self.load()
 
     def resample(self):
         pass
 
     def convert_to_si(self, data=None):
         pass
 
     def export_to_csv(self, export_path):
         self.data.to_csv(export_path)
 
+    def add_clock_offset(self, offset):
+        shift_stream_index(self.data, offset)
+
 
 class UnityStream(Stream):
     def __init__(self, **kw):
         super(UnityStream, self).__init__(**kw)
 
         self.streamtype = StreamType.UNITY
         if self.autoload:
@@ -55,14 +62,17 @@
 
     def convert_to_si(self, data=None):
         pass
 
     def export_to_csv(self, export_path):
         self.data.to_csv(export_path)
 
+    def add_clock_offset(self, offset):
+        shift_stream_index(self.data, offset)
+
 
 class PupilGazeStream(PupilStream):
     def __init__(self, **kw):
         super(PupilGazeStream, self).__init__(**kw)
 
     def load(self):
         self.data = load_zeromq(
```

### Comparing `pluma_analysis-0.6.0/pluma/sync/__init__.py` & `pluma_analysis-0.7.0/pluma/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/sync/plotting.py` & `pluma_analysis-0.7.0/pluma/sync/plotting.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/sync/ubx2harp.py` & `pluma_analysis-0.7.0/pluma/sync/ubx2harp.py`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma/templates/metadata_template.j2` & `pluma_analysis-0.7.0/pluma/templates/metadata_template.j2`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pluma_analysis.egg-info/PKG-INFO` & `pluma_analysis-0.7.0/pluma_analysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluma-analysis
-Version: 0.6.0
+Version: 0.7.0
 Summary: A low-level interface to data collected with the pluma urban data acquisition system
 Author-email: Goncalo Lopes <g.lopes@neurogears.org>, Bruno Cruz <b.cruz@neurogears.org>, Andrew Erskine <a.erskine@neurogears.org>
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/emotional-cities/pluma-analysis/issues
 Project-URL: Source Code, https://github.com/emotional-cities/pluma-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -14,14 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: matplotlib
+Requires-Dist: mapclassify
+Requires-Dist: folium
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: s3fs
 Requires-Dist: pyubx2
 Requires-Dist: tilemapbase
```

### Comparing `pluma_analysis-0.6.0/pluma_analysis.egg-info/SOURCES.txt` & `pluma_analysis-0.7.0/pluma_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluma_analysis-0.6.0/pyproject.toml` & `pluma_analysis-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 requires-python = ">=3.9.0"
 dynamic = ["version"]
 license = {text = "MIT License"}
 
 dependencies = [
     "geopandas",
     "matplotlib",
+    "mapclassify",
+    "folium",
     "numpy",
     "scipy",
     "scikit-learn",
     "pandas",
     "s3fs",
     "pyubx2",
     "tilemapbase",
```

