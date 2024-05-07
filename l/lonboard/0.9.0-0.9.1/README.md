# Comparing `tmp/lonboard-0.9.0.tar.gz` & `tmp/lonboard-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lonboard-0.9.0.tar", max compression
+gzip compressed data, was "lonboard-0.9.1.tar", max compression
```

## Comparing `lonboard-0.9.0.tar` & `lonboard-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1073 2024-05-06 17:24:05.319344 lonboard-0.9.0/LICENSE
--rw-r--r--   0        0        0       36 2024-05-06 17:24:05.319344 lonboard-0.9.0/MANIFEST.in
--rw-r--r--   0        0        0     3074 2024-05-06 17:24:05.319344 lonboard-0.9.0/README.md
--rw-r--r--   0        0        0      445 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/__init__.py
--rw-r--r--   0        0        0       39 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/__main__.py
--rw-r--r--   0        0        0     1418 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_base.py
--rw-r--r--   0        0        0     4645 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_cli.py
--rw-r--r--   0        0        0      862 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_constants.py
--rw-r--r--   0        0        0     1421 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_environment.py
--rw-r--r--   0        0        0       95 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/__init__.py
--rw-r--r--   0        0        0     8042 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/_duckdb.py
--rw-r--r--   0        0        0      509 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/crs.py
--rw-r--r--   0        0        0    13399 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/extension_types.py
--rw-r--r--   0        0        0      716 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/geopandas_interop.py
--rw-r--r--   0        0        0      174 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/ops/__init__.py
--rw-r--r--   0        0        0     2619 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/ops/bbox.py
--rw-r--r--   0        0        0     4584 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/ops/centroid.py
--rw-r--r--   0        0        0     3170 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/ops/coord_layout.py
--rw-r--r--   0        0        0     8208 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/ops/reproject.py
--rw-r--r--   0        0        0     4725 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/parse_wkb.py
--rw-r--r--   0        0        0     1801 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_geoarrow/sanitize.py
--rw-r--r--   0        0        0    60118 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_layer.py
--rw-r--r--   0        0        0    13878 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_map.py
--rw-r--r--   0        0        0     3578 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_serialization.py
--rw-r--r--   0        0        0      285 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_testing.py
--rw-r--r--   0        0        0     5293 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_utils.py
--rw-r--r--   0        0        0      166 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_version.py
--rw-r--r--   0        0        0     2380 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_viewport.py
--rw-r--r--   0        0        0    20582 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/_viz.py
--rw-r--r--   0        0        0     1367 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/basemap.py
--rw-r--r--   0        0        0     6914 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/colormap.py
--rw-r--r--   0        0        0     2758 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/controls.py
--rw-r--r--   0        0        0      207 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/experimental/__init__.py
--rw-r--r--   0        0        0     9728 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/experimental/_layer.py
--rw-r--r--   0        0        0    14555 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/layer_extension.py
--rw-r--r--   0        0        0      357 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/models.py
--rw-r--r--   0        0        0        0 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/py.typed
--rw-r--r--   0        0        0      385 2024-05-06 17:24:14.711408 lonboard-0.9.0/lonboard/static/index.css
--rw-r--r--   0        0        0  2155294 2024-05-06 17:24:14.711408 lonboard-0.9.0/lonboard/static/index.js
--rw-r--r--   0        0        0    37110 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/traits.py
--rw-r--r--   0        0        0        0 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/types/__init__.py
--rw-r--r--   0        0        0     4535 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/types/layer.py
--rw-r--r--   0        0        0      466 2024-05-06 17:24:05.523345 lonboard-0.9.0/lonboard/types/map.py
--rw-r--r--   0        0        0     2211 2024-05-06 17:24:05.527345 lonboard-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 lonboard-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 19:06:06.930557 lonboard-0.9.1/LICENSE
+-rw-r--r--   0        0        0       36 2024-05-07 19:06:06.930557 lonboard-0.9.1/MANIFEST.in
+-rw-r--r--   0        0        0     3074 2024-05-07 19:06:06.930557 lonboard-0.9.1/README.md
+-rw-r--r--   0        0        0      445 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/__main__.py
+-rw-r--r--   0        0        0     1418 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_base.py
+-rw-r--r--   0        0        0     4645 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_cli.py
+-rw-r--r--   0        0        0      862 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_constants.py
+-rw-r--r--   0        0        0     1421 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_environment.py
+-rw-r--r--   0        0        0       95 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/__init__.py
+-rw-r--r--   0        0        0     8042 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/_duckdb.py
+-rw-r--r--   0        0        0      509 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/crs.py
+-rw-r--r--   0        0        0    13399 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/extension_types.py
+-rw-r--r--   0        0        0      716 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/geopandas_interop.py
+-rw-r--r--   0        0        0      174 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/__init__.py
+-rw-r--r--   0        0        0     2619 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/bbox.py
+-rw-r--r--   0        0        0     4584 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/centroid.py
+-rw-r--r--   0        0        0     3170 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/coord_layout.py
+-rw-r--r--   0        0        0     8208 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/ops/reproject.py
+-rw-r--r--   0        0        0     4725 2024-05-07 19:06:07.134559 lonboard-0.9.1/lonboard/_geoarrow/parse_wkb.py
+-rw-r--r--   0        0        0     1801 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_geoarrow/sanitize.py
+-rw-r--r--   0        0        0    60118 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_layer.py
+-rw-r--r--   0        0        0    13878 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_map.py
+-rw-r--r--   0        0        0     3578 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_serialization.py
+-rw-r--r--   0        0        0      285 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_testing.py
+-rw-r--r--   0        0        0     5293 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_utils.py
+-rw-r--r--   0        0        0      166 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_version.py
+-rw-r--r--   0        0        0     2380 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_viewport.py
+-rw-r--r--   0        0        0    20582 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/_viz.py
+-rw-r--r--   0        0        0     1367 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/basemap.py
+-rw-r--r--   0        0        0     6914 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/colormap.py
+-rw-r--r--   0        0        0     2758 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/controls.py
+-rw-r--r--   0        0        0      207 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/experimental/__init__.py
+-rw-r--r--   0        0        0     9728 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/experimental/_layer.py
+-rw-r--r--   0        0        0    14555 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/layer_extension.py
+-rw-r--r--   0        0        0      357 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/models.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/py.typed
+-rw-r--r--   0        0        0      385 2024-05-07 19:06:16.526643 lonboard-0.9.1/lonboard/static/index.css
+-rw-r--r--   0        0        0  2155294 2024-05-07 19:06:16.526643 lonboard-0.9.1/lonboard/static/index.js
+-rw-r--r--   0        0        0    37110 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/traits.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/__init__.py
+-rw-r--r--   0        0        0     4535 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/layer.py
+-rw-r--r--   0        0        0      466 2024-05-07 19:06:07.138558 lonboard-0.9.1/lonboard/types/map.py
+-rw-r--r--   0        0        0     2211 2024-05-07 19:06:07.138558 lonboard-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 lonboard-0.9.1/PKG-INFO
```

### Comparing `lonboard-0.9.0/LICENSE` & `lonboard-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/README.md` & `lonboard-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_base.py` & `lonboard-0.9.1/lonboard/_base.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_cli.py` & `lonboard-0.9.1/lonboard/_cli.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_constants.py` & `lonboard-0.9.1/lonboard/_constants.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_environment.py` & `lonboard-0.9.1/lonboard/_environment.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/_duckdb.py` & `lonboard-0.9.1/lonboard/_geoarrow/_duckdb.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/extension_types.py` & `lonboard-0.9.1/lonboard/_geoarrow/extension_types.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/geopandas_interop.py` & `lonboard-0.9.1/lonboard/_geoarrow/geopandas_interop.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/ops/bbox.py` & `lonboard-0.9.1/lonboard/_geoarrow/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/ops/centroid.py` & `lonboard-0.9.1/lonboard/_geoarrow/ops/centroid.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/ops/coord_layout.py` & `lonboard-0.9.1/lonboard/_geoarrow/ops/coord_layout.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/ops/reproject.py` & `lonboard-0.9.1/lonboard/_geoarrow/ops/reproject.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/parse_wkb.py` & `lonboard-0.9.1/lonboard/_geoarrow/parse_wkb.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_geoarrow/sanitize.py` & `lonboard-0.9.1/lonboard/_geoarrow/sanitize.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_layer.py` & `lonboard-0.9.1/lonboard/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_map.py` & `lonboard-0.9.1/lonboard/_map.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_serialization.py` & `lonboard-0.9.1/lonboard/_serialization.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_utils.py` & `lonboard-0.9.1/lonboard/_utils.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_viewport.py` & `lonboard-0.9.1/lonboard/_viewport.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/_viz.py` & `lonboard-0.9.1/lonboard/_viz.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/basemap.py` & `lonboard-0.9.1/lonboard/basemap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/colormap.py` & `lonboard-0.9.1/lonboard/colormap.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/controls.py` & `lonboard-0.9.1/lonboard/controls.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/experimental/_layer.py` & `lonboard-0.9.1/lonboard/experimental/_layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/layer_extension.py` & `lonboard-0.9.1/lonboard/layer_extension.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/static/index.js` & `lonboard-0.9.1/lonboard/static/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -69879,15 +69879,15 @@
 Xn.throughDOM = CH;
 uu.throughDOM = E3;
 Og.throughDOM = E3;
 Sp.throughDOM = E3;
 Bg.throughDOM = P3;
 C2.throughDOM = P3;
 I2.throughDOM = P3;
-var Tdt = "0.6.0",
+var Tdt = "0.6.1",
     Mdt = `https://cdn.jsdelivr.net/npm/parquet-wasm@${Tdt}/esm/parquet_wasm_bg.wasm`,
     JO = !1;
 async function LH() {
     JO || (await B9(Mdt), JO = !0)
 }
 
 function Edt(e) {
```

### Comparing `lonboard-0.9.0/lonboard/traits.py` & `lonboard-0.9.1/lonboard/traits.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/lonboard/types/layer.py` & `lonboard-0.9.1/lonboard/types/layer.py`

 * *Files identical despite different names*

### Comparing `lonboard-0.9.0/pyproject.toml` & `lonboard-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lonboard"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python library for fast, interactive geospatial vector data visualization in Jupyter."
 authors = ["Kyle Barron <kyle@developmentseed.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lonboard" }]
 include = ["lonboard/static/*.js", "lonboard/static/*.css", "MANIFEST.in"]
```

### Comparing `lonboard-0.9.0/PKG-INFO` & `lonboard-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lonboard
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python library for fast, interactive geospatial vector data visualization in Jupyter.
 License: MIT
 Author: Kyle Barron
 Author-email: kyle@developmentseed.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lonboard Version: 0.9.0 Summary: Python library for
+Metadata-Version: 2.1 Name: lonboard Version: 0.9.1 Summary: Python library for
 fast, interactive geospatial vector data visualization in Jupyter. License: MIT
 Author: Kyle Barron Author-email: kyle@developmentseed.org Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
```

