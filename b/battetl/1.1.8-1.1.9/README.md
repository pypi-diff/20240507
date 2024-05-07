# Comparing `tmp/battetl-1.1.8.tar.gz` & `tmp/battetl-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.1.8.tar", last modified: Wed Jan  3 07:47:12 2024, max compression
+gzip compressed data, was "battetl-1.1.9.tar", last modified: Wed Jan 10 21:26:47 2024, max compression
```

## Comparing `battetl-1.1.8.tar` & `battetl-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.470994 battetl-1.1.8/
--rw-rw-rw-   0        0        0     6350 2023-10-27 05:50:14.000000 battetl-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       32 2023-11-16 17:32:48.000000 battetl-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    19827 2024-01-03 07:47:12.469998 battetl-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    18839 2024-01-03 07:45:16.000000 battetl-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.411532 battetl-1.1.8/battetl/
--rw-rw-rw-   0        0        0     7528 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/BattETL.py
--rw-rw-rw-   0        0        0      155 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/__init__.py
--rw-rw-rw-   0        0        0     7449 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/battetl_quick.py
--rw-rw-rw-   0        0        0     9953 2024-01-03 07:45:16.000000 battetl-1.1.8/battetl/constants.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.459473 battetl-1.1.8/battetl/extract/
--rw-rw-rw-   0        0        0    29650 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/extract/Extractor.py
--rw-rw-rw-   0        0        0       33 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/extract/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.465473 battetl-1.1.8/battetl/load/
--rw-rw-rw-   0        0        0    42780 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/load/Loader.py
--rw-rw-rw-   0        0        0      115 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/load/__init__.py
--rw-rw-rw-   0        0        0     8711 2024-01-03 07:45:16.000000 battetl-1.1.8/battetl/load/batt_db_test_helper.py
--rw-rw-rw-   0        0        0     3334 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/load/quick_loader.py
--rw-rw-rw-   0        0        0     1795 2024-01-03 07:45:16.000000 battetl-1.1.8/battetl/logger.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.468998 battetl-1.1.8/battetl/transform/
--rw-rw-rw-   0        0        0    30601 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/transform/Transformer.py
--rw-rw-rw-   0        0        0       37 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/transform/__init__.py
--rw-rw-rw-   0        0        0    14716 2023-10-27 05:50:14.000000 battetl-1.1.8/battetl/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-03 07:47:12.455946 battetl-1.1.8/battetl.egg-info/
--rw-rw-rw-   0        0        0    19827 2024-01-03 07:47:12.000000 battetl-1.1.8/battetl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-01-03 07:47:12.000000 battetl-1.1.8/battetl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-03 07:47:12.000000 battetl-1.1.8/battetl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2024-01-03 07:47:12.000000 battetl-1.1.8/battetl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-03 07:47:12.000000 battetl-1.1.8/battetl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      189 2023-10-27 05:50:14.000000 battetl-1.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-03 07:47:12.470994 battetl-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      886 2024-01-03 07:45:16.000000 battetl-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.602234 battetl-1.1.9/
+-rw-rw-rw-   0        0        0     6350 2023-10-27 05:50:14.000000 battetl-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-11-16 17:32:48.000000 battetl-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    19827 2024-01-10 21:26:47.602234 battetl-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    18839 2023-12-27 23:08:03.000000 battetl-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.547549 battetl-1.1.9/battetl/
+-rw-rw-rw-   0        0        0     7528 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/BattETL.py
+-rw-rw-rw-   0        0        0      155 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/__init__.py
+-rw-rw-rw-   0        0        0     7449 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/battetl_quick.py
+-rw-rw-rw-   0        0        0     9953 2024-01-10 21:24:21.000000 battetl-1.1.9/battetl/constants.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.588757 battetl-1.1.9/battetl/extract/
+-rw-rw-rw-   0        0        0    29650 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/extract/Extractor.py
+-rw-rw-rw-   0        0        0       33 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/extract/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.593758 battetl-1.1.9/battetl/load/
+-rw-rw-rw-   0        0        0    42787 2024-01-10 21:24:21.000000 battetl-1.1.9/battetl/load/Loader.py
+-rw-rw-rw-   0        0        0      115 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/load/__init__.py
+-rw-rw-rw-   0        0        0     8711 2023-12-27 23:08:03.000000 battetl-1.1.9/battetl/load/batt_db_test_helper.py
+-rw-rw-rw-   0        0        0     3334 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/load/quick_loader.py
+-rw-rw-rw-   0        0        0     1795 2023-12-29 23:37:43.000000 battetl-1.1.9/battetl/logger.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.595757 battetl-1.1.9/battetl/transform/
+-rw-rw-rw-   0        0        0    30601 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/transform/Transformer.py
+-rw-rw-rw-   0        0        0       37 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/transform/__init__.py
+-rw-rw-rw-   0        0        0    14716 2023-10-27 05:50:14.000000 battetl-1.1.9/battetl/utils.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.585891 battetl-1.1.9/battetl.egg-info/
+-rw-rw-rw-   0        0        0    19827 2024-01-10 21:26:47.000000 battetl-1.1.9/battetl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2024-01-10 21:26:47.000000 battetl-1.1.9/battetl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-10 21:26:47.000000 battetl-1.1.9/battetl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2024-01-10 21:26:47.000000 battetl-1.1.9/battetl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-01-10 21:26:47.000000 battetl-1.1.9/battetl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      189 2023-10-27 05:50:14.000000 battetl-1.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-01-10 21:26:47.602234 battetl-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      886 2024-01-10 21:24:21.000000 battetl-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-10 21:26:47.600226 battetl-1.1.9/tests/
+-rw-rw-rw-   0        0        0     4383 2023-10-27 05:50:15.000000 battetl-1.1.9/tests/test_BattETL.py
+-rw-rw-rw-   0        0        0    17088 2023-10-27 05:50:15.000000 battetl-1.1.9/tests/test_Extractor.py
+-rw-rw-rw-   0        0        0    27156 2023-10-27 05:50:15.000000 battetl-1.1.9/tests/test_Loader.py
+-rw-rw-rw-   0        0        0    17781 2023-10-27 05:50:15.000000 battetl-1.1.9/tests/test_Transformer.py
+-rw-rw-rw-   0        0        0     2991 2023-10-27 05:50:15.000000 battetl-1.1.9/tests/test_utils.py
```

### Comparing `battetl-1.1.8/LICENSE` & `battetl-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/PKG-INFO` & `battetl-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battetl-1.1.8/README.md` & `battetl-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/BattETL.py` & `battetl-1.1.9/battetl/BattETL.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/battetl_quick.py` & `battetl-1.1.9/battetl/battetl_quick.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/constants.py` & `battetl-1.1.9/battetl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class Constants:
     DEFAULT_TIME_ZONE = 'America/Los_Angeles'
 
-    BATTDB_SCHEMA_VERSION = 9.2
+    BATTDB_SCHEMA_VERSION = 9.3
     BATTDB_QUICK_SCHEMA_VERSION = 1.1
 
     DATABASE_MAX_RETRIES = 10
     DATABASE_RETRY_DELAY = 10
     DATABASE_MAX_RETRY_DELAY = 60
 
     MAKE_ARBIN = 'arbin'
```

### Comparing `battetl-1.1.8/battetl/extract/Extractor.py` & `battetl-1.1.9/battetl/extract/Extractor.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/load/Loader.py` & `battetl-1.1.9/battetl/load/Loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         with self._conn.cursor() as cursor:
             stmt = psycopg2.sql.SQL("""
                 SELECT
                     version
                 FROM
                     flyway_schema_history
                 ORDER BY
-                    version
+                    version::float
                 DESC
                 LIMIT 1
             """)
             cursor.execute(stmt)
             result = cursor.fetchone()
 
         if result:
```

### Comparing `battetl-1.1.8/battetl/load/batt_db_test_helper.py` & `battetl-1.1.9/battetl/load/batt_db_test_helper.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/load/quick_loader.py` & `battetl-1.1.9/battetl/load/quick_loader.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/logger.py` & `battetl-1.1.9/battetl/logger.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/transform/Transformer.py` & `battetl-1.1.9/battetl/transform/Transformer.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl/utils.py` & `battetl-1.1.9/battetl/utils.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.8/battetl.egg-info/PKG-INFO` & `battetl-1.1.9/battetl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `battetl-1.1.8/battetl.egg-info/SOURCES.txt` & `battetl-1.1.9/battetl.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,8 +17,13 @@
 battetl/extract/Extractor.py
 battetl/extract/__init__.py
 battetl/load/Loader.py
 battetl/load/__init__.py
 battetl/load/batt_db_test_helper.py
 battetl/load/quick_loader.py
 battetl/transform/Transformer.py
-battetl/transform/__init__.py
+battetl/transform/__init__.py
+tests/test_BattETL.py
+tests/test_Extractor.py
+tests/test_Loader.py
+tests/test_Transformer.py
+tests/test_utils.py
```

### Comparing `battetl-1.1.8/setup.py` & `battetl-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="battetl",
-    version="1.1.8",
+    version="1.1.9",
     author="Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak",
     author_email="info@battgenie.life",
     description="A Python module for extracting, transforming, and loading battery data to a database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BattGenie/battetl",
     packages=setuptools.find_packages(),
```

