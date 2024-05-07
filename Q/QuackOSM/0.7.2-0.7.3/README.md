# Comparing `tmp/quackosm-0.7.2.tar.gz` & `tmp/quackosm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.7.2.tar", last modified: Sun Apr 28 17:24:01 2024, max compression
+gzip compressed data, was "quackosm-0.7.3.tar", last modified: Tue May  7 15:07:10 2024, max compression
```

## Comparing `quackosm-0.7.2.tar` & `quackosm-0.7.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11339 2024-04-28 17:23:35.371569 quackosm-0.7.2/LICENSE
--rw-r--r--   0        0        0    27879 2024-04-28 17:23:35.371569 quackosm-0.7.2/README.md
--rw-r--r--   0        0        0     4378 2024-04-28 17:24:01.651726 quackosm-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      560 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_constants.py
--rw-r--r--   0        0        0      181 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_exceptions.py
--rw-r--r--   0        0        0     6497 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0    12674 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/_typing.py
--rw-r--r--   0        0        0    24446 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/cli.py
--rw-r--r--   0        0        0     2031 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/conftest.py
--rw-r--r--   0        0        0    52502 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/functions.py
--rw-r--r--   0        0        0    19193 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     2941 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1709 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4376 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-04-28 17:23:35.379569 quackosm-0.7.2/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   108664 2024-04-28 17:23:35.383570 quackosm-0.7.2/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/__init__.py
--rw-r--r--   0        0        0      746 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/conftest.py
--rw-r--r--   0        0        0    24831 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    29285 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_osm_tags_filtering.py
--rw-r--r--   0        0        0    36504 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      945 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0      238 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/conftest.py
--rw-r--r--   0        0        0     1472 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-04-28 17:23:35.383570 quackosm-0.7.2/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0    29715 1970-01-01 00:00:00.000000 quackosm-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-07 15:06:41.640138 quackosm-0.7.3/LICENSE
+-rw-r--r--   0        0        0    27879 2024-05-07 15:06:41.640138 quackosm-0.7.3/README.md
+-rw-r--r--   0        0        0     4378 2024-05-07 15:07:10.152255 quackosm-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_constants.py
+-rw-r--r--   0        0        0      181 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     6497 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0    12674 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/_typing.py
+-rw-r--r--   0        0        0    24446 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/cli.py
+-rw-r--r--   0        0        0     2031 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/conftest.py
+-rw-r--r--   0        0        0    53246 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/functions.py
+-rw-r--r--   0        0        0    19193 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     2941 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1709 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4376 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   110453 2024-05-07 15:06:41.652138 quackosm-0.7.3/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/conftest.py
+-rw-r--r--   0        0        0    24831 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    29285 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_osm_tags_filtering.py
+-rw-r--r--   0        0        0    36528 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0      238 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/conftest.py
+-rw-r--r--   0        0        0     1472 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-05-07 15:06:41.652138 quackosm-0.7.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-05-07 15:06:41.656138 quackosm-0.7.3/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0    29715 1970-01-01 00:00:00.000000 quackosm-0.7.3/PKG-INFO
```

### Comparing `quackosm-0.7.2/LICENSE` & `quackosm-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/README.md` & `quackosm-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/pyproject.toml` & `quackosm-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.7.2"
+version = "0.7.3"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas",
     "shapely>=2",
@@ -185,15 +185,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.2"
+current_version = "0.7.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.7.2/quackosm/__init__.py` & `quackosm-0.7.3/quackosm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.7.2/quackosm/_osm_tags_filters.py` & `quackosm-0.7.3/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/_osm_way_polygon_features.py` & `quackosm-0.7.3/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/_rich_progress.py` & `quackosm-0.7.3/quackosm/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/_typing.py` & `quackosm-0.7.3/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/cli.py` & `quackosm-0.7.3/quackosm/cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/conftest.py` & `quackosm-0.7.3/quackosm/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/functions.py` & `quackosm-0.7.3/quackosm/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     save_as_wkt: bool = False,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
+    debug: bool = False,
 ) -> Path:
     """
     Convert PBF file to GeoParquet file.
 
     Args:
         pbf_path (Union[str, Path]): Pbf file to be parsed to GeoParquet.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
@@ -73,14 +74,16 @@
         save_as_wkt (bool): Whether to save the file with geometry in the WKT form instead of WKB.
             If `True`, it will be saved as a `.parquet` file, because it won't be in the GeoParquet
             standard. Defaults to `False`.
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
+        debug (bool, optional): If turned on, will keep all temporary files after operation
+            for debugging. Defaults to `False`.
 
     Returns:
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from a PBF file.
 
@@ -225,14 +228,15 @@
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
+        debug=debug,
     ).convert_pbf_to_gpq(
         pbf_path=pbf_path,
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
@@ -250,14 +254,15 @@
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     save_as_wkt: bool = False,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
     allow_uncovered_geometry: bool = False,
+    debug: bool = False,
 ) -> Path:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
@@ -304,14 +309,16 @@
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
         allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
             by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
             automatically. Defaults to `False`.
+        debug (bool, optional): If turned on, will keep all temporary files after operation
+            for debugging. Defaults to `False`.
 
     Returns:
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from the center of Monaco.
 
@@ -410,14 +417,15 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
+        debug=debug,
     ).convert_geometry_filter_to_gpq(
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
         save_as_wkt=save_as_wkt,
@@ -431,14 +439,15 @@
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
+    debug: bool = False,
 ) -> gpd.GeoDataFrame:
     """
     Get features GeoDataFrame from a PBF file or list of PBF files.
 
     Function can parse multiple PBF files and returns a single GeoDataFrame with loaded
     OSM objects.
 
@@ -476,14 +485,16 @@
             Config used to determine which closed way features are polygons.
             Modifications to this config left are left for experienced OSM users.
             Defaults to predefined "osm_way_polygon_features.json".
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
+        debug (bool, optional): If turned on, will keep all temporary files after operation
+            for debugging. Defaults to `False`.
 
     Returns:
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from a PBF file.
 
@@ -595,14 +606,15 @@
     """
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
+        debug=debug,
     ).get_features_gdf(
         file_paths=file_paths,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
@@ -616,14 +628,15 @@
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
     allow_uncovered_geometry: bool = False,
+    debug: bool = False,
 ) -> gpd.GeoDataFrame:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
@@ -664,14 +677,16 @@
         verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
             verbosity mode. Can be one of: silent, transient and verbose. Silent disables
             output completely. Transient tracks progress, but removes output after finished.
             Verbose leaves all progress outputs in the stdout. Defaults to "transient".
         allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
             by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
             automatically. Defaults to `False`.
+        debug (bool, optional): If turned on, will keep all temporary files after operation
+            for debugging. Defaults to `False`.
 
     Returns:
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from the center of Monaco.
 
@@ -724,13 +739,14 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
+        debug=debug,
     ).get_features_gdf_from_geometry(
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
```

### Comparing `quackosm-0.7.2/quackosm/osm_extracts/__init__.py` & `quackosm-0.7.3/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.7.3/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/osm_extracts/bbbike.py` & `quackosm-0.7.3/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.7.3/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.7.3/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/osm_way_polygon_features.json` & `quackosm-0.7.3/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/quackosm/pbf_file_reader.py` & `quackosm-0.7.3/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         osm_way_polygon_features_config: Optional[
             Union[OsmWayPolygonConfig, dict[str, Any]]
         ] = None,
         parquet_compression: str = "snappy",
         osm_extract_source: Union[OsmExtractSource, str] = OsmExtractSource.geofabrik,
         verbosity_mode: Literal["silent", "transient", "verbose"] = "transient",
         allow_uncovered_geometry: bool = False,
+        debug: bool = False,
     ) -> None:
         """
         Initialize PbfFileReader.
 
         Args:
             tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
                 specifying which tags to download.
@@ -129,26 +130,28 @@
                 intersecting OSM objects. Defaults to `None`.
             working_directory (Union[str, Path], optional): Directory where to save
                 the parsed `*.parquet` files. Defaults to "files".
             osm_way_polygon_features_config (Union[OsmWayPolygonConfig, dict[str, Any]], optional):
                 Config used to determine which closed way features are polygons.
                 Modifications to this config left are left for experienced OSM users.
                 Defaults to predefined "osm_way_polygon_features.json".
-            parquet_compression (str): Compression of intermediate parquet files.
+            parquet_compression (str, optional): Compression of intermediate parquet files.
                 Check https://duckdb.org/docs/sql/statements/copy#parquet-options for more info.
                 Defaults to "snappy".
             osm_extract_source (Union[OsmExtractSource, str], optional): A source for automatic
                 downloading of OSM extracts. Can be Geofabrik, BBBike, OSMfr or any.
                 Defaults to `geofabrik`.
             verbosity_mode (Literal["silent", "transient", "verbose"], optional): Set progress
                 verbosity mode. Can be one of: silent, transient and verbose. Silent disables
                 output completely. Transient tracks progress, but removes output after finished.
                 Verbose leaves all progress outputs in the stdout. Defaults to "transient".
-            allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't
-                covered by any OSM extract. Defaults to `False`.
+            allow_uncovered_geometry (bool, optional): Suppress an error if some geometry parts
+                aren't covered by any OSM extract. Defaults to `False`.
+            debug (bool, optional): If turned on, will keep all temporary files after operation
+                for debugging. Defaults to `False`.
 
         Raises:
             InvalidGeometryFilter: When provided geometry filter has parts without area.
         """
         self.geometry_filter = geometry_filter
         self._check_if_valid_geometry_filter()
 
@@ -164,14 +167,15 @@
         self.allow_uncovered_geometry = allow_uncovered_geometry
         self.osm_extract_source = osm_extract_source
         self.working_directory = Path(working_directory)
         self.working_directory.mkdir(parents=True, exist_ok=True)
         self.connection: duckdb.DuckDBPyConnection = None
         self.encountered_query_exception = False
         self.verbosity_mode = verbosity_mode
+        self.debug = debug
         self.task_progress_tracker: TaskProgressTracker = None
 
         self.rows_per_group = PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[0]
         actual_memory = psutil.virtual_memory()
         # If more than 8 / 16 / 24 GB total memory, increase the number of rows per group
         for memory_gb, rows_per_group in PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG.items():
             if actual_memory.total >= (memory_gb * MEMORY_1GB):
@@ -244,14 +248,18 @@
         if explode_tags is None:
             explode_tags = (
                 self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
             )
 
         with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as self.tmp_dir_name:
             self.tmp_dir_path = Path(self.tmp_dir_name)
+
+            if self.debug:
+                self.tmp_dir_path = self._prepare_debug_directory()
+
             try:
                 self.encountered_query_exception = False
                 self.connection = _set_up_duckdb_connection(tmp_dir_path=self.tmp_dir_path)
                 result_file_path = result_file_path or self._generate_result_file_path(
                     pbf_path,
                     filter_osm_ids=filter_osm_ids,
                     keep_all_tags=keep_all_tags,
@@ -378,14 +386,17 @@
                     )
                     parsed_geoparquet_files.append(parsed_geoparquet_file)
 
                 if parsed_geoparquet_files:
                     with tempfile.TemporaryDirectory(
                         dir=self.working_directory.resolve()
                     ) as tmp_dir_name:
+                        if self.debug:
+                            tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
+
                         try:
                             joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
                                 parsed_geoparquet_files
                             )
                         except pa.ArrowInvalid:
                             tmp_dir_path = Path(tmp_dir_name)
                             try:
@@ -488,14 +499,17 @@
                 ignore_cache=ignore_cache,
                 filter_osm_ids=filter_osm_ids,
             )
             parsed_geoparquet_files.append(parsed_geoparquet_file)
 
         if parsed_geoparquet_files:
             with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as tmp_dir_name:
+                if self.debug:
+                    tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
+
                 try:
                     joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
                         parsed_geoparquet_files
                     )
                 except pa.ArrowInvalid:
                     tmp_dir_path = Path(tmp_dir_name)
                     try:
@@ -616,14 +630,16 @@
                 ) TO '{output_file_name}' (
                     FORMAT 'parquet',
                     PER_THREAD_OUTPUT true,
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
             """
+            if self.debug:
+                log_message(f"Saved to directory: {output_file_name}")
             self._run_query(query, run_in_separate_process=True, tmp_dir_path=tmp_dir_path)
             return pq.read_table(output_file_name)
 
     def _drop_duplicated_features_in_joined_table_one_by_one(
         self, parsed_geoparquet_files: list[Path], tmp_dir_path: Path
     ) -> pa.Table:
         if len(parsed_geoparquet_files) == 1:
@@ -651,14 +667,16 @@
                     ) TO '{filtered_result_parquet_file}' (
                         FORMAT 'parquet',
                         PER_THREAD_OUTPUT true,
                         ROW_GROUP_SIZE 25000,
                         COMPRESSION '{self.parquet_compression}'
                     )
                 """
+                if self.debug:
+                    log_message(f"Saved to directory: {filtered_result_parquet_file}")
                 connection.sql(query)
                 result_parquet_files.extend(filtered_result_parquet_file.glob("*.parquet"))
         return pq.read_table(result_parquet_files)
 
     def _parse_pbf_file(
         self,
         pbf_path: Union[str, Path],
@@ -1278,15 +1296,20 @@
             ways_required_ids=ways_required_ids,
             ways_filtered_ids=ways_filtered_ids,
             relations_all_with_tags=relations_all_with_tags,
             relations_with_unnested_way_refs=relations_with_unnested_way_refs,
             relations_filtered_ids=relations_filtered_ids,
         )
 
-    def _delete_directories(self, directories: Union[str, Path, list[Union[str, Path]]]) -> None:
+    def _delete_directories(
+        self, directories: Union[str, Path, list[Union[str, Path]]], override_debug: bool = False
+    ) -> None:
+        if self.debug and not override_debug:
+            return
+
         _directories = []
         if isinstance(directories, (str, Path)):
             _directories = [directories]
         else:
             _directories = directories
         for directory in _directories:
             if isinstance(directory, Path):
@@ -1300,14 +1323,22 @@
                 except Exception as ex:
                     if tries == 0:
                         raise ex
                     sleep(0.5)
                 finally:
                     tries -= 1
 
+    def _prepare_debug_directory(self) -> Path:
+        if self.debug:
+            dir_path = Path(self.working_directory) / "debug" / secrets.token_hex(16)
+            self._delete_directories(dir_path, override_debug=True)
+            dir_path.mkdir(exist_ok=True, parents=True)
+            return dir_path
+        raise RuntimeError("Cannot prepare debug directory when debug mode is not activated.")
+
     def _generate_osm_tags_sql_filter(self) -> str:
         """Prepare features filter clauses based on tags filter."""
         positive_filter_clauses: list[str] = []
         negative_filter_clauses: list[str] = []
 
         if self.merged_tags_filter:
             positive_filter_clauses.clear()
@@ -1418,14 +1449,16 @@
                 FORMAT 'parquet',
                 PER_THREAD_OUTPUT true,
                 ROW_GROUP_SIZE 25000,
                 COMPRESSION '{self.parquet_compression}'
             )
         """
         self._run_query(query, run_in_separate_process)
+        if self.debug:
+            log_message(f"Saved to directory: {file_path}")
         return self.connection.sql(f"SELECT * FROM read_parquet('{file_path}/**')")
 
     def _run_query(
         self,
         sql_queries: Union[str, list[str]],
         run_in_separate_process: bool = False,
         query_timeout_seconds: Optional[int] = None,
@@ -1479,14 +1512,16 @@
                 FORMAT 'parquet',
                 PER_THREAD_OUTPUT true,
                 ROW_GROUP_SIZE 25000,
                 COMPRESSION '{self.parquet_compression}'
             )
             """
         )
+        if self.debug:
+            log_message(f"Saved to directory: {result_path}")
 
         return self.connection.sql(f"SELECT * FROM read_parquet('{result_path}/**')")
 
     def _get_filtered_nodes_with_geometry(
         self,
         osm_parquet_files: ConvertedOSMParquetFiles,
     ) -> Path:
@@ -1771,14 +1806,16 @@
                     FORMAT 'parquet',
                     PARTITION_BY ("group"),
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
                 """
             )
+            if self.debug:
+                log_message(f"Saved to directory: {grouped_ways_path}")
 
         return groups
 
     def _construct_ways_linestrings(
         self,
         bar: TaskProgressBar,
         groups: int,
@@ -1811,14 +1848,16 @@
 
             self._run_query(
                 queries,
                 run_in_separate_process=(
                     self.rows_per_group > PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[0]
                 ),
             )
+            if self.debug:
+                log_message(f"Saved to directory: {current_destination_path}")
 
             self._delete_directories(current_ways_group_path)
 
     def _get_filtered_ways_with_proper_geometry(
         self,
         osm_parquet_files: ConvertedOSMParquetFiles,
         required_ways_with_linestrings: "duckdb.DuckDBPyRelation",
@@ -1880,16 +1919,16 @@
             ),
             proper_geometries AS (
                 SELECT
                     id,
                     tags,
                     (CASE
                         WHEN is_polygon
-                        THEN linestring_to_polygon_wkt(linestring)
-                        ELSE linestring_to_linestring_wkt(linestring)
+                        THEN linestring_to_polygon_geometry(linestring)
+                        ELSE linestring_to_linestring_geometry(linestring)
                     END)::GEOMETRY AS geometry
                 FROM
                     required_ways_with_linestrings w
             )
             SELECT 'way/' || id as feature_id, tags, geometry FROM proper_geometries
             """
         )
@@ -1909,15 +1948,15 @@
         valid_relation_parts = self.connection.sql(
             f"""
             WITH unnested_relations AS (
                 SELECT
                     r.id,
                     COALESCE(r.ref_role, 'outer') as ref_role,
                     r.ref,
-                    linestring_to_linestring_wkt(w.linestring)::GEOMETRY as geometry
+                    linestring_to_linestring_geometry(w.linestring)::GEOMETRY as geometry
                 FROM ({osm_parquet_files.relations_with_unnested_way_refs.sql_query()}) r
                 SEMI JOIN ({osm_parquet_files.relations_filtered_ids.sql_query()}) fr
                 ON r.id = fr.id
                 JOIN ({required_ways_with_linestrings.sql_query()}) w
                 ON w.id = r.ref
             ),
             any_outer_refs AS (
@@ -2072,14 +2111,16 @@
                     FORMAT 'parquet',
                     PER_THREAD_OUTPUT true,
                     ROW_GROUP_SIZE 25000,
                     COMPRESSION '{self.parquet_compression}'
                 )
                 """
             )
+            if self.debug:
+                log_message(f"Saved to directory: {file_path}")
 
         return self.connection.sql(
             f"""
             SELECT * EXCLUDE (geometry_wkb), ST_GeomFromWKB(geometry_wkb) geometry
             FROM read_parquet('{file_path}/**')
             """
         )
@@ -2434,26 +2475,22 @@
     )
     connection.sql("SET enable_progress_bar = false;")
     connection.sql("SET enable_progress_bar_print = false;")
     for extension_name in ("parquet", "spatial"):
         connection.install_extension(extension_name)
         connection.load_extension(extension_name)
 
-    connection.sql(
-        """
-        CREATE OR REPLACE MACRO linestring_to_linestring_wkt(ls) AS
-        'LINESTRING (' || array_to_string([pt.x || ' ' || pt.y for pt in ls], ', ') || ')';
-        """
-    )
-    connection.sql(
-        """
-        CREATE OR REPLACE MACRO linestring_to_polygon_wkt(ls) AS
-        'POLYGON ((' || array_to_string([pt.x || ' ' || pt.y for pt in ls], ', ') || '))';
-        """
-    )
+    connection.sql("""
+        CREATE OR REPLACE MACRO linestring_to_linestring_geometry(ls) AS
+        ls::struct(x DECIMAL(10, 7), y DECIMAL(10, 7))[]::LINESTRING_2D::GEOMETRY;
+    """)
+    connection.sql("""
+        CREATE OR REPLACE MACRO linestring_to_polygon_geometry(ls) AS
+        [ls::struct(x DECIMAL(10, 7), y DECIMAL(10, 7))[]]::POLYGON_2D::GEOMETRY;
+    """)
 
     return connection
 
 
 def _run_query(sql_queries: Union[str, list[str]], tmp_dir_path: Path) -> None:
     if isinstance(sql_queries, str):
         sql_queries = [sql_queries]
```

### Comparing `quackosm-0.7.2/tests/base/conftest.py` & `quackosm-0.7.3/tests/base/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/base/test_cli.py` & `quackosm-0.7.3/tests/base/test_cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/base/test_osm_extracts.py` & `quackosm-0.7.3/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/base/test_osm_tags_filtering.py` & `quackosm-0.7.3/tests/base/test_osm_tags_filtering.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/base/test_pbf_file_reader.py` & `quackosm-0.7.3/tests/base/test_pbf_file_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 
 @pytest.mark.parametrize("operation_mode", ["gdf", "gpq"])  # type: ignore
 @pytest.mark.parametrize("patch_methods", [0, 1, 2])  # type: ignore
 def test_combining_files_different_techniques(
     mocker: MockerFixture, operation_mode: str, patch_methods: int
 ) -> None:
-    """Test if all files merging techniques work as expected."""
+    """Test if all files merging techniques work as expected in debug mode."""
     if patch_methods > 0:
         # Leave _drop_duplicated_features_in_joined_table as backup
         mocker.patch(
             "quackosm.pbf_file_reader.PbfFileReader._drop_duplicated_features_in_pyarrow_table",
             side_effect=pa.ArrowInvalid(),
         )
 
@@ -181,15 +181,15 @@
         result_gdf = get_features_gdf(
             file_paths=[
                 monaco_file_path,
                 monaco_file_path,
             ],
             ignore_cache=True,
         )
-        single_result_gdf = PbfFileReader().get_features_gdf(
+        single_result_gdf = PbfFileReader(debug=True).get_features_gdf(
             file_paths=[monaco_file_path], ignore_cache=True
         )
 
         assert result_gdf.index.is_unique
         assert len(result_gdf.index) == len(single_result_gdf.index)
     elif operation_mode == "gpq":
         result = convert_geometry_to_gpq(
```

### Comparing `quackosm-0.7.2/tests/benchmark/test_big_file.py` & `quackosm-0.7.3/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.7.3/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.7.3/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.7.3/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.7.3/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/test_files/monaco.osm.pbf` & `quackosm-0.7.3/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/tests/test_files/monaco_boundary.geojson` & `quackosm-0.7.3/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.7.2/PKG-INFO` & `quackosm-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.7.2
+Version: 0.7.3
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QuackOSM Version: 0.7.2 Summary: An open-source
+Metadata-Version: 2.1 Name: QuackOSM Version: 0.7.3 Summary: An open-source
 tool for reading OpenStreetMap PBF files using DuckDB Author-Email: Kamil
 Raczycki
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
```

