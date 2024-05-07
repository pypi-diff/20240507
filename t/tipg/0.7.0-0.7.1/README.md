# Comparing `tmp/tipg-0.7.0.tar.gz` & `tmp/tipg-0.7.1.tar.gz`

## Comparing `tipg-0.7.0.tar` & `tipg-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/__init__.py
--rw-r--r--   0        0        0    32930 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/collections.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/database.py
--rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/errors.py
--rw-r--r--   0        0        0    73931 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/logger.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/main.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/middleware.py
--rw-r--r--   0        0        0    27240 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/enums.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/resources/response.py
--rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/collection.html
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/collections.html
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/header.html
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/item.html
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/items.html
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/landing.html
--rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/map.html
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tileset.html
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 tipg-0.7.0/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tipg-0.7.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.7.0/LICENSE
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tipg-0.7.0/README.md
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 tipg-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 tipg-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/__init__.py
+-rw-r--r--   0        0        0    32930 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/collections.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/database.py
+-rw-r--r--   0        0        0    15579 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/errors.py
+-rw-r--r--   0        0        0    73931 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/logger.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/main.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/middleware.py
+-rw-r--r--   0        0        0    27240 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/resources/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/resources/enums.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/resources/response.py
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/collections.html
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/header.html
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/item.html
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/items.html
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/landing.html
+-rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/map.html
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 tipg-0.7.1/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tipg-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tipg-0.7.1/README.md
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 tipg-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 tipg-0.7.1/PKG-INFO
```

### Comparing `tipg-0.7.0/tipg/collections.py` & `tipg-0.7.1/tipg/collections.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/database.py` & `tipg-0.7.1/tipg/database.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/dependencies.py` & `tipg-0.7.1/tipg/dependencies.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/errors.py` & `tipg-0.7.1/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/factory.py` & `tipg-0.7.1/tipg/factory.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/main.py` & `tipg-0.7.1/tipg/main.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/middleware.py` & `tipg-0.7.1/tipg/middleware.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/model.py` & `tipg-0.7.1/tipg/model.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/settings.py` & `tipg-0.7.1/tipg/settings.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/filter/evaluate.py` & `tipg-0.7.1/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/filter/filters.py` & `tipg-0.7.1/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/resources/enums.py` & `tipg-0.7.1/tipg/resources/enums.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/resources/response.py` & `tipg-0.7.1/tipg/resources/response.py`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/sql/dbcatalog.sql` & `tipg-0.7.1/tipg/sql/dbcatalog.sql`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/collection.html` & `tipg-0.7.1/tipg/templates/collection.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/collections.html` & `tipg-0.7.1/tipg/templates/collections.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/conformance.html` & `tipg-0.7.1/tipg/templates/conformance.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/header.html` & `tipg-0.7.1/tipg/templates/header.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/item.html` & `tipg-0.7.1/tipg/templates/item.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/items.html` & `tipg-0.7.1/tipg/templates/items.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/landing.html` & `tipg-0.7.1/tipg/templates/landing.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/map.html` & `tipg-0.7.1/tipg/templates/map.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/queryables.html` & `tipg-0.7.1/tipg/templates/queryables.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/tilematrixset.html` & `tipg-0.7.1/tipg/templates/tilematrixset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/tilematrixsets.html` & `tipg-0.7.1/tipg/templates/tilematrixsets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/tileset.html` & `tipg-0.7.1/tipg/templates/tileset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/tipg/templates/tilesets.html` & `tipg-0.7.1/tipg/templates/tilesets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/.gitignore` & `tipg-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/LICENSE` & `tipg-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/README.md` & `tipg-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.7.0/pyproject.toml` & `tipg-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "orjson",
     "asyncpg>=0.23.0",
     "buildpg>=0.3",
-    "fastapi>=0.107.0",
+    "fastapi-slim",
     "jinja2>=2.11.2,<4.0.0",
     "morecantile>=5.0,<6.0",
     "pydantic>=2.4,<3.0",
     "pydantic-settings~=2.0",
     "geojson-pydantic>=1.0,<2.0",
     "pygeofilter>=0.2.0,<0.3.0",
     "ciso8601~=2.3",
```

### Comparing `tipg-0.7.0/PKG-INFO` & `tipg-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tipg
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
         
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: asyncpg>=0.23.0
 Requires-Dist: buildpg>=0.3
 Requires-Dist: ciso8601~=2.3
-Requires-Dist: fastapi>=0.107.0
+Requires-Dist: fastapi-slim
 Requires-Dist: geojson-pydantic<2.0,>=1.0
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
 Requires-Dist: jinja2<4.0.0,>=2.11.2
 Requires-Dist: morecantile<6.0,>=5.0
 Requires-Dist: orjson
 Requires-Dist: pydantic-settings~=2.0
 Requires-Dist: pydantic<3.0,>=2.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: tipg Version: 0.7.0 Summary: Simple and Fast
+Metadata-Version: 2.3 Name: tipg Version: 0.7.1 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -22,15 +22,15 @@
 Features,OGC Tiles,POSTGIS Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS Requires-
 Python: >=3.8 Requires-Dist: asyncpg>=0.23.0 Requires-Dist: buildpg>=0.3
-Requires-Dist: ciso8601~=2.3 Requires-Dist: fastapi>=0.107.0 Requires-Dist:
+Requires-Dist: ciso8601~=2.3 Requires-Dist: fastapi-slim Requires-Dist:
 geojson-pydantic<2.0,>=1.0 Requires-Dist: importlib-resources>=1.1.0;
 python_version < '3.9' Requires-Dist: jinja2<4.0.0,>=2.11.2 Requires-Dist:
 morecantile<6.0,>=5.0 Requires-Dist: orjson Requires-Dist: pydantic-
 settings~=2.0 Requires-Dist: pydantic<3.0,>=2.4 Requires-Dist:
 pygeofilter<0.3.0,>=0.2.0 Requires-Dist: starlette-cramjam<0.4,>=0.3 Requires-
 Dist: typing-extensions; python_version < '3.9' Provides-Extra: dev Requires-
 Dist: pre-commit; extra == 'dev' Provides-Extra: docs Requires-Dist: mkdocs;
```

