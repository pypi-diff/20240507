# Comparing `tmp/pyaro-0.0.8.tar.gz` & `tmp/pyaro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaro-0.0.8.tar", last modified: Tue Apr 16 15:44:15 2024, max compression
+gzip compressed data, was "pyaro-0.0.9.tar", last modified: Tue May  7 15:51:59 2024, max compression
```

## Comparing `pyaro-0.0.8.tar` & `pyaro-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-04-16 15:44:11.000000 pyaro-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:44:15.393234 pyaro-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-16 15:44:11.000000 pyaro-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-16 15:44:15.397235 pyaro-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 15:44:11.000000 pyaro-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.389234 pyaro-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/csvreader/
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/csvreader/CSVTimeseriesReader.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/csvreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/pandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/AutoFilterReaderEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    26414 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Station.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-16 15:44:11.000000 pyaro-0.0.8/tests/test_CSVTimeSeriesReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.654183 pyaro-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-05-07 15:51:55.000000 pyaro-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-07 15:51:59.654183 pyaro-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-07 15:51:55.000000 pyaro-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-07 15:51:59.654183 pyaro-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 15:51:55.000000 pyaro-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.650183 pyaro-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.650183 pyaro-0.0.9/src/pyaro/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.654183 pyaro-0.0.9/src/pyaro/csvreader/
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/csvreader/CSVTimeseriesReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/csvreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/pandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.654183 pyaro-0.0.9/src/pyaro/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/AutoFilterReaderEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26414 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/Wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 15:51:55.000000 pyaro-0.0.9/src/pyaro/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.654183 pyaro-0.0.9/src/pyaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 15:51:59.000000 pyaro-0.0.9/src/pyaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:51:59.654183 pyaro-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-07 15:51:55.000000 pyaro-0.0.9/tests/test_CSVTimeSeriesReader.py
```

### Comparing `pyaro-0.0.8/LICENSE` & `pyaro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/PKG-INFO` & `pyaro-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaro
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyaro py-aerocom reader objects
 Home-page: https://pyaro.readthedocs.io
 Author: Heiko Klein, Daniel Heinesen
 Author-email: Heiko.Klein@met.no
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyaro-0.0.8/README.md` & `pyaro-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/setup.cfg` & `pyaro-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyaro
-version = 0.0.8
+version = 0.0.9
 author = Heiko Klein, Daniel Heinesen
 author_email = Heiko.Klein@met.no
 description = pyaro py-aerocom reader objects
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `pyaro-0.0.8/src/pyaro/csvreader/CSVTimeseriesReader.py` & `pyaro-0.0.9/src/pyaro/csvreader/CSVTimeseriesReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             i.e. altitude or standard_deviation.
         :variable_units: dict translating variable-names to units, e.g. overwrite units given in columns
         :country_lookup: use pyaro_readers.geocoder_reverse_natural_earth to lookup country-codes from lat/lon
         :csvreader_kwargs: kwargs send directly to csv.reader module
         :filters: default auto-filter filters
         """
         self._filename = filename
+        self._metadata = {"path": str(filename)}
         self._stations = {}
         self._data = {}  # var -> {data-array}
         self._set_filters(filters)
         self._extra_metadata = tuple(set(columns.keys()) - set(self.col_keys()))
         if country_lookup:
             lookupISO2 = _lookup_function()
         with open(self._filename, newline="") as csvfile:
@@ -122,15 +123,14 @@
                             "end_time",
                             "flag",
                             "standard_deviation",
                         )
                     ]
                 )
                 if not r["station"] in self._stations:
-
                     station_fields = {
                         "station": r["station"],
                         "longitude": r["longitude"],
                         "latitude": r["latitude"],
                         "altitude": r["altitude"],
                         "country": r["country"],
                         "url": "",
@@ -148,14 +148,17 @@
     def col_keys(cls):
         """Column keys possible to initialize with this reader.
 
         :return: list of columns possible to initialize with columns argument of this reader
         """
         return cls._col_keys
 
+    def metadata(self) -> dict():
+        return self._metadata
+
     def _unfiltered_data(self, varname) -> Data:
         return self._data[varname]
 
     def _unfiltered_stations(self) -> dict[str, Station]:
         return self._stations
 
     def _unfiltered_variables(self) -> list[str]:
```

### Comparing `pyaro-0.0.8/src/pyaro/plugins.py` & `pyaro-0.0.9/src/pyaro/plugins.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/AutoFilterReaderEngine.py` & `pyaro-0.0.9/src/pyaro/timeseries/AutoFilterReaderEngine.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Data.py` & `pyaro-0.0.9/src/pyaro/timeseries/Data.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Engine.py` & `pyaro-0.0.9/src/pyaro/timeseries/Engine.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Filter.py` & `pyaro-0.0.9/src/pyaro/timeseries/Filter.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Reader.py` & `pyaro-0.0.9/src/pyaro/timeseries/Reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,24 @@
         All parameters should also be listed in the Engine's args function.
 
         :param filename_or_obj_or_url: location of database instance
         :param filters: list of filters, or dict of (name, kwargs) for FilterFactory
         """
         pass
 
+    def metadata(self) -> dict[str, str]:
+        """Metadata set by the datasource.
+
+        The reader-implementation might add metadata depending on the data-source
+        to this method.
+
+        :return dictionary with different metadata
+        """
+        return dict()
+
     @abc.abstractmethod
     def data(self, varname) -> Data:
         """Return all data for a variable
 
         :param varname: variable name as returned from variables
         :return: a data object
         """
```

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Station.py` & `pyaro-0.0.9/src/pyaro/timeseries/Station.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro/timeseries/Wrappers.py` & `pyaro-0.0.9/src/pyaro/timeseries/Wrappers.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/src/pyaro.egg-info/PKG-INFO` & `pyaro-0.0.9/src/pyaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaro
-Version: 0.0.8
+Version: 0.0.9
 Summary: pyaro py-aerocom reader objects
 Home-page: https://pyaro.readthedocs.io
 Author: Heiko Klein, Daniel Heinesen
 Author-email: Heiko.Klein@met.no
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyaro-0.0.8/src/pyaro.egg-info/SOURCES.txt` & `pyaro-0.0.9/src/pyaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.8/tests/test_CSVTimeSeriesReader.py` & `pyaro-0.0.9/tests/test_CSVTimeSeriesReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,21 @@
             "csv_timeseries", *[self.file], **{"filters": [], "columns": columns}
         ) as ts:
             areas = ["Rural", "Urban"]
             stations = ts.stations()
             self.assertEqual(stations["station1"]["area_classification"], areas[0])
             self.assertEqual(stations["station2"]["area_classification"], areas[1])
 
+    def test_metadata(self):
+        with pyaro.open_timeseries(
+            "csv_timeseries", *[self.file], **{"filters": []}
+        ) as ts:
+            self.assertIsInstance(ts.metadata(), dict)
+            self.assertIn("path", ts.metadata())
+
     def test_data(self):
         engines = pyaro.list_timeseries_engines()
         with engines["csv_timeseries"].open(
             filename=self.file,
             filters=[pyaro.timeseries.filters.get("countries", include=["NO"])],
         ) as ts:
             for var in ts.variables():
@@ -119,15 +126,17 @@
                     end_time=data.end_times,
                     latitude=data.latitudes,
                     longitude=data.longitudes,
                     altitude=data.altitudes,
                     flag=data.flags,
                     standard_deviation=data.standard_deviations,
                 )
-            self.assertEqual((2**rounds) * old_size, len(data), "data append by array")
+            self.assertEqual(
+                (2**rounds) * old_size, len(data), "data append by array"
+            )
 
     def test_stationfilter(self):
         engine = pyaro.list_timeseries_engines()["csv_timeseries"]
         sfilter = pyaro.timeseries.filters.get("stations", exclude=["station1"])
         with engine.open(self.file, filters=[sfilter]) as ts:
             count = 0
             for var in ts.variables():
```

