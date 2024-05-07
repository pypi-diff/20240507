# Comparing `tmp/agrc-sweeper-1.4.3.tar.gz` & `tmp/agrc-sweeper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agrc-sweeper-1.4.3.tar", last modified: Thu Jul  6 21:04:23 2023, max compression
+gzip compressed data, was "agrc-sweeper-2.0.0.tar", last modified: Tue May  7 17:18:51 2024, max compression
```

## Comparing `agrc-sweeper-1.4.3.tar` & `agrc-sweeper-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.235008 agrc-sweeper-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 21:04:23.000000 agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/credentials_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/street_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/sweepers/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/UseLimitations.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/empties.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/invalids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/sweepers/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:23.239008 agrc-sweeper-1.4.3/src/sweeper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-06 21:04:20.000000 agrc-sweeper-1.4.3/src/sweeper/workspace_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:51.125330 agrc-sweeper-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-07 17:18:51.125330 agrc-sweeper-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:18:51.125330 agrc-sweeper-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:51.121330 agrc-sweeper-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:51.121330 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 17:18:51.000000 agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:51.121330 agrc-sweeper-2.0.0/src/sweeper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/street_types.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:51.121330 agrc-sweeper-2.0.0/src/sweeper/sweepers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/UseLimitations.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/empties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/sweepers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-07 17:18:47.000000 agrc-sweeper-2.0.0/src/sweeper/workspace_info.py
```

### Comparing `agrc-sweeper-1.4.3/PKG-INFO` & `agrc-sweeper-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agrc-sweeper
-Version: 1.4.3
+Version: 2.0.0
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: UGRC
 Author-email: ugrc-developers@utah.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: develop
+License-File: LICENSE
 
 # agrc-sweeper [![PyPI version](https://badge.fury.io/py/agrc-sweeper.svg)](https://badge.fury.io/py/agrc-sweeper)[![Push Events](https://github.com/agrc/sweeper/actions/workflows/push.yml/badge.svg)](https://github.com/agrc/sweeper/actions/workflows/push.yml)
 
 The data cleaning service.
 
 ![sweeper_sm](https://user-images.githubusercontent.com/325813/90411835-91c4c080-e069-11ea-9d03-f3e60421b835.png)
 
@@ -121,34 +121,40 @@
 A normalized string representing the entire address that was passed into the constructor. PO Boxes are normalized in this format `PO BOX <number>`.
 
 ## Installation (requires Pro 2.7+)
 
 <!-- Current conda install arcpy -c esri seems to be wonky; just clone to be safe -->
 
 1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
+   - `conda create --name sweeper --clone arcgispro-py3`
 1. activate environment
-    - `activate sweeper`
+   - `activate sweeper`
 1. install sweeper
-    - `pip install agrc-sweeper`
+   - `pip install agrc-sweeper`
+1. Optionally duplicate `config.sample.json` as `config.json` in the folder where you will run sweeper.
 
-## Development
+> [!CAUTION]
+> This is required for the following functions:
+>
+> - `--scheduled` argument (required for sending emails)
+> - `--change-detect` argument
+> - using user-specific connection files via the `CONNECTIONS_FOLDER` config value
 
-1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
-1. activate environment
-    - `activate sweeper`
-1. `test_metadata.py` uses a SQL database that needs to be restored via `src/sweeper/tests/data/Sweeper.bak` to your local SQL Server.
+## Exclusions
 
-### Installing dependencies
+Tables can be skipped by adding values to the `EXCLUSIONS.<sweeper_key>` config array. These values are matched against table names using [fnmatch](https://docs.python.org/3/library/fnmatch.html#fnmatch.fnmatch). Note that these do not apply when using the `--table-name` argument.
+
+## Development
 
 1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
-1. install only required dependencies to run sweeper
-    - `pip install -e .`
+   - `conda create --name sweeper --clone arcgispro-py3`
+1. activate environment
+   - `activate sweeper`
 1. install required dependencies to work on sweeper
-    - `pip install -e ".[develop]"`
-1. install required dependencies to run sweeper tests
-    - `pip install -e ".[tests]"`
-1. run tests: `pytest`
+   - `pip install -e ".[tests]"`
+1. `test_metadata.py` uses a SQL database that needs to be restored via `src/sweeper/tests/data/Sweeper.bak` to your local SQL Server.
+1. run sweeper: `sweeper`
+1. test: `pytest`
+1. lint: `ruff check .`
+1. format: `ruff format .`
```

### Comparing `agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/PKG-INFO` & `agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agrc-sweeper
-Version: 1.4.3
+Version: 2.0.0
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: UGRC
 Author-email: ugrc-developers@utah.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: develop
+License-File: LICENSE
 
 # agrc-sweeper [![PyPI version](https://badge.fury.io/py/agrc-sweeper.svg)](https://badge.fury.io/py/agrc-sweeper)[![Push Events](https://github.com/agrc/sweeper/actions/workflows/push.yml/badge.svg)](https://github.com/agrc/sweeper/actions/workflows/push.yml)
 
 The data cleaning service.
 
 ![sweeper_sm](https://user-images.githubusercontent.com/325813/90411835-91c4c080-e069-11ea-9d03-f3e60421b835.png)
 
@@ -121,34 +121,40 @@
 A normalized string representing the entire address that was passed into the constructor. PO Boxes are normalized in this format `PO BOX <number>`.
 
 ## Installation (requires Pro 2.7+)
 
 <!-- Current conda install arcpy -c esri seems to be wonky; just clone to be safe -->
 
 1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
+   - `conda create --name sweeper --clone arcgispro-py3`
 1. activate environment
-    - `activate sweeper`
+   - `activate sweeper`
 1. install sweeper
-    - `pip install agrc-sweeper`
+   - `pip install agrc-sweeper`
+1. Optionally duplicate `config.sample.json` as `config.json` in the folder where you will run sweeper.
 
-## Development
+> [!CAUTION]
+> This is required for the following functions:
+>
+> - `--scheduled` argument (required for sending emails)
+> - `--change-detect` argument
+> - using user-specific connection files via the `CONNECTIONS_FOLDER` config value
 
-1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
-1. activate environment
-    - `activate sweeper`
-1. `test_metadata.py` uses a SQL database that needs to be restored via `src/sweeper/tests/data/Sweeper.bak` to your local SQL Server.
+## Exclusions
 
-### Installing dependencies
+Tables can be skipped by adding values to the `EXCLUSIONS.<sweeper_key>` config array. These values are matched against table names using [fnmatch](https://docs.python.org/3/library/fnmatch.html#fnmatch.fnmatch). Note that these do not apply when using the `--table-name` argument.
+
+## Development
 
 1. clone arcgis conda environment
-    - `conda create -name sweeper --clone arcgispro-py3`
-1. install only required dependencies to run sweeper
-    - `pip install -e .`
+   - `conda create --name sweeper --clone arcgispro-py3`
+1. activate environment
+   - `activate sweeper`
 1. install required dependencies to work on sweeper
-    - `pip install -e ".[develop]"`
-1. install required dependencies to run sweeper tests
-    - `pip install -e ".[tests]"`
-1. run tests: `pytest`
+   - `pip install -e ".[tests]"`
+1. `test_metadata.py` uses a SQL database that needs to be restored via `src/sweeper/tests/data/Sweeper.bak` to your local SQL Server.
+1. run sweeper: `sweeper`
+1. test: `pytest`
+1. lint: `ruff check .`
+1. format: `ruff format .`
```

### Comparing `agrc-sweeper-1.4.3/src/agrc_sweeper.egg-info/SOURCES.txt` & `agrc-sweeper-2.0.0/src/agrc_sweeper.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+LICENSE
 MANIFEST.in
-setup.cfg
+pyproject.toml
 setup.py
 src/agrc_sweeper.egg-info/PKG-INFO
 src/agrc_sweeper.egg-info/SOURCES.txt
 src/agrc_sweeper.egg-info/dependency_links.txt
 src/agrc_sweeper.egg-info/entry_points.txt
 src/agrc_sweeper.egg-info/not-zip-safe
 src/agrc_sweeper.egg-info/requires.txt
 src/agrc_sweeper.egg-info/top_level.txt
 src/sweeper/__init__.py
 src/sweeper/__main__.py
 src/sweeper/address_parser.py
 src/sweeper/backup.py
-src/sweeper/credentials_template.py
+src/sweeper/config.py
 src/sweeper/report.py
 src/sweeper/street_types.json
+src/sweeper/utilities.py
 src/sweeper/workspace_info.py
 src/sweeper/sweepers/UseLimitations.html
 src/sweeper/sweepers/__init__.py
 src/sweeper/sweepers/addresses.py
+src/sweeper/sweepers/base.py
 src/sweeper/sweepers/duplicates.py
 src/sweeper/sweepers/empties.py
 src/sweeper/sweepers/invalids.py
-src/sweeper/sweepers/metadata.py
-src/sweeper/tests/__init__.py
-src/sweeper/tests/test_address_parser.py
-src/sweeper/tests/test_addresses.py
-src/sweeper/tests/test_metadata.py
+src/sweeper/sweepers/metadata.py
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/__main__.py` & `agrc-sweeper-2.0.0/src/sweeper/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 sweeper
 
 Usage:
   sweeper sweep duplicates  --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
   sweeper sweep empties     --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
   sweeper sweep invalids    --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
   sweeper sweep addresses   --workspace=<workspace> --table-name=<table-name> --field-name=<field_name> [--verbose --try-fix --save-report=<report_path> --backup-to=<backup_path>]
@@ -17,171 +17,191 @@
   report_path   - folder to save report to eg: `c:\\temp`
   backup_path   - place to create a temp gdb and import original table
   field_name    - name of the field to check
 
 Examples:
   sweeper sweep           --workspace=c:\\data\\thing --try-fix --save-report=c:\\temp --backup-to=c:\\temp\\backup.gdb
   sweeper sweep addresses --workspace=c:\\data\\thing --try-fix --save-report=c:\\temp --backup-to=c:\\temp\\backup.gdb --field-name=ADDRESS
-'''
-import sys
+"""
+
 import datetime
 import logging
 import logging.handlers
-import pkg_resources
+import sys
 from pathlib import Path
 
+import pkg_resources
 from docopt import docopt
-
+from supervisor.message_handlers import SendGridHandler
 from supervisor.models import MessageDetails, Supervisor
-from supervisor.message_handlers import EmailHandler
 
-from . import backup, report, workspace_info, credentials
+from . import backup, config, report, utilities, workspace_info
+from .sweepers.addresses import AddressTest
 from .sweepers.duplicates import DuplicateTest
 from .sweepers.empties import EmptyTest
-from .sweepers.addresses import AddressTest
 from .sweepers.metadata import MetadataTest
 
 
 def main():
-    '''Main entry point for program. Parse arguments and pass to sweeper modules.
-    '''
-    args = docopt(__doc__, version=pkg_resources.require('agrc-sweeper')[0].version)
+    """Main entry point for program. Parse arguments and pass to sweeper modules."""
+    args = docopt(__doc__, version=pkg_resources.require("agrc-sweeper")[0].version)
 
-    log = setup_logging(args['--save-report'], args['--scheduled'])
+    log = setup_logging(args["--save-report"], args["--scheduled"])
 
-    if args['--scheduled']:
+    if args["--scheduled"]:
         #: set up supervisor, add email handler
         sweeper_supervisor = Supervisor()
-        sweeper_supervisor.add_message_handler(EmailHandler(credentials.EMAIL_SETTINGS, client_name='agrc-sweeper'))
+        sweeper_supervisor.add_message_handler(
+            SendGridHandler(
+                {
+                    "from_address": "noreply@utah.gov",
+                    "to_addresses": config.get_config("TO_ADDRESSES"),
+                    "api_key": config.get_config("SENDGRID_API_KEY"),
+                },
+                client_name="agrc-sweeper",
+                client_version=pkg_resources.require("agrc-sweeper")[0].version,
+            )
+        )
 
     #: backup input file before quality checks
-    if args['--backup-to']:
-        backup.backup_data(args['--workspace'], args['--table-name'], args['--backup-to'])
+    if args["--backup-to"]:
+        backup.backup_data(args["--workspace"], args["--table-name"], args["--backup-to"])
 
     #: create a list to hold the instantiated objects.
     closet = []
 
     #: check what quality check to run.
-    if args['duplicates']:
-        closet.append(DuplicateTest(args['--workspace'], args['--table-name']))
-    elif args['invalids']:
+    if args["duplicates"]:
+        closet.append(DuplicateTest(args["--workspace"], args["--table-name"]))
+    elif args["invalids"]:
         raise NotImplementedError('"Invalids" sweep/check not implemented yet.')
-    elif args['empties']:
-        closet.append(EmptyTest(args['--workspace'], args['--table-name']))
-    elif args['addresses']:
-        closet.append(AddressTest(args['--workspace'], args['--table-name'], args['--field-name']))
-    elif args['metadata']:
-        closet.append(MetadataTest(args['--workspace'], args['--table-name']))
+    elif args["empties"]:
+        closet.append(EmptyTest(args["--workspace"], args["--table-name"]))
+    elif args["addresses"]:
+        closet.append(AddressTest(args["--workspace"], args["--table-name"], args["--field-name"]))
+    elif args["metadata"]:
+        closet.append(MetadataTest(args["--workspace"], args["--table-name"]))
     else:
-        closet.append(DuplicateTest(args['--workspace'], args['--table-name']))
-        closet.append(EmptyTest(args['--workspace'], args['--table-name']))
-        closet.append(MetadataTest(args['--workspace'], args['--table-name']))
+        closet.append(DuplicateTest(args["--workspace"], args["--table-name"]))
+        closet.append(EmptyTest(args["--workspace"], args["--table-name"]))
+        closet.append(MetadataTest(args["--workspace"], args["--table-name"]))
 
-    reports = execute_sweepers(closet, args['--try-fix'], args['--change-detect'], log)
+    reports = execute_sweepers(closet, args["--try-fix"], args["--change-detect"], log)
 
     report.print_report(reports)
 
-    if args['--save-report']:
-        report.save_report(reports, args['--save-report'])
+    if args["--save-report"]:
+        report.save_report(reports, args["--save-report"])
 
-    if args['--scheduled']:
+    if args["--scheduled"]:
         report.add_to_log(reports)
 
         final_message = report.format_message(reports)
         log.info(final_message.getvalue())
 
         #: Build and send summary message
         summary_message = MessageDetails()
         summary_message.message = final_message.getvalue()
-        summary_message.project_name = 'agrc-sweeper'
-        summary_message.attachments = [credentials.LOG_FILE_PATH]
-        summary_message.subject = f'Sweeper Report {datetime.datetime.today()}'
+        summary_message.attachments = [config.LOG_FILE_PATH]
+        summary_message.subject = f"Sweeper Report {datetime.datetime.today()}"
 
         sweeper_supervisor.notify(summary_message)
 
 
 def execute_sweepers(closet, try_fix, using_change_detection, log):
-    '''
+    """
     orchestrate the sweeper calls.
 
     closet: array of sweepers.
     try_fix: bool whether to fix or not.
-    '''
+    """
 
     feature_class_names = []
     reports = []
 
     def run_tool(tool):
         reports.append(tool.sweep())
 
         if try_fix:
             reports.append(tool.try_fix())
 
             #: run sweeper again to ensure all errors were fixed.
             reports.append(tool.sweep())
 
-    log.info(f'running {len(closet)} sweepers. try fix: {try_fix}')
+    log.info(f"running {len(closet)} sweepers. try fix: {try_fix}")
     for tool in closet:
+        log.info(f"running sweeper: {tool.key}")
         if tool.table_name:
             run_tool(tool)
 
             continue
 
         #: get feature class names once
         if len(feature_class_names) == 0:
             if using_change_detection:
-                log.info('Getting table names from change detection table')
+                log.info("Getting table names from change detection table")
                 feature_class_names = workspace_info.get_change_detection()
             else:
-                log.info('Missing table name, executing over workspace')
+                log.info("Missing table name, executing over workspace")
                 feature_class_names = workspace_info.get_featureclasses(tool.workspace)
-                if any('SGID.' in fc for fc in feature_class_names):
-                    feature_class_names = [fc.split('SGID.', 1)[1] for fc in feature_class_names if 'SGID.' in fc]
+                if any("SGID." in fc for fc in feature_class_names):
+                    feature_class_names = [fc.split("SGID.", 1)[1] for fc in feature_class_names if "SGID." in fc]
+
+            #: apply exclusions
+            if config.has_config():
+                try:
+                    exclusions_config = config.get_config("EXCLUSIONS")
+                except KeyError:
+                    exclusions_config = {}
+
+                exclusions = exclusions_config.get(tool.key, [])
+            feature_class_names = utilities.apply_exclusions(feature_class_names, exclusions)
 
-        log.info(f'feature_class_names is: {feature_class_names}')
+        log.info(f"feature_class_names is: {feature_class_names}")
 
         if using_change_detection and feature_class_names is None:
             #: reset variable to empty list
-            log.info('Change detection found no updated tables')
+            log.info("Change detection found no updated tables")
             feature_class_names = []
 
             continue
 
         #: explode sweeper class for each feature class
         for table_name in feature_class_names:
-            new_tool = tool.clone(table_name)
+            new_tool = tool.clone(table_name, tool.workspace)
 
             run_tool(new_tool)
 
     if using_change_detection:
         workspace_info.update_last_check_date()
 
     return reports
 
 
 def setup_logging(save_report, scheduled):
-    logger = logging.getLogger('sweeper')
+    logger = logging.getLogger("sweeper")
     logger.setLevel(logging.INFO)
 
-    formatter = logging.Formatter(fmt='%(levelname)-7s %(asctime)s %(module)10s:%(lineno)5s %(message)s', datefmt='%m-%d %H:%M:%S')
+    formatter = logging.Formatter(
+        fmt="%(levelname)-7s %(asctime)s %(module)10s:%(lineno)5s %(message)s", datefmt="%m-%d %H:%M:%S"
+    )
 
     #: always set up console_handler
     console_handler = logging.StreamHandler(stream=sys.stdout)
     console_handler.setFormatter(formatter)
 
     #: use log file when report location not provided and when running from scheduled task
     if scheduled and not save_report:
-        #: get LOG_FILE_PATH from credentials.py
-        log_file = Path(credentials.LOG_FILE_PATH)
+        log_file = Path(config.LOG_FILE_PATH)
         file_handler = logging.handlers.RotatingFileHandler(log_file, backupCount=10)
         file_handler.doRollover()
         file_handler.setFormatter(formatter)
 
         logger.addHandler(file_handler)
 
     logger.addHandler(console_handler)
 
     return logger
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/address_parser.py` & `agrc-sweeper-2.0.0/src/sweeper/address_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,246 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 address_parser.py
 A module that parses street addresses into their various parts.
-'''
+"""
+
 import json
 import pprint
 import re
 from os.path import dirname, join, realpath
 
 import usaddress
 
 TAG_MAPPING = {
-    'AddressNumber': 'address_number',
-    'AddressNumberPrefix': 'address_number',
-    'AddressNumberSuffix': 'address_number_suffix',
-    'StreetNamePreDirectional': 'prefix_direction',
-    'StreetName': 'street_name',
+    "AddressNumber": "address_number",
+    "AddressNumberPrefix": "address_number",
+    "AddressNumberSuffix": "address_number_suffix",
+    "StreetNamePreDirectional": "prefix_direction",
+    "StreetName": "street_name",
     # 'StreetNamePreModifier': 'street_name', #: handled in class below
     # 'StreetNamePreType': 'street_name', #: handled in class below
-    'StreetNamePostDirectional': 'street_direction',
-    'StreetNamePostModifier': 'street_type',
-    'StreetNamePostType': 'street_type',
+    "StreetNamePostDirectional": "street_direction",
+    "StreetNamePostModifier": "street_type",
+    "StreetNamePostType": "street_type",
     # 'CornerOf': 'address1',
     # 'IntersectionSeparator': 'address1',
     # 'LandmarkName': 'address1',
     # 'USPSBoxGroupID': 'address1',
     # 'USPSBoxGroupType': 'address1',
     # 'USPSBoxID': 'address1',
     # 'USPSBoxType': 'address1',
-    'BuildingName': 'unit_id',
-    'OccupancyType': 'unit_type',
-    'OccupancyIdentifier': 'unit_id',
-    'SubaddressIdentifier': 'unit_id',
-    'SubaddressType': 'unit_type',
-    'PlaceName': 'city',
-    'StateName': 'state',
-    'ZipCode': 'zip_code',
-    'USPSBoxID': 'po_box'
+    "BuildingName": "unit_id",
+    "OccupancyType": "unit_type",
+    "OccupancyIdentifier": "unit_id",
+    "SubaddressIdentifier": "unit_id",
+    "SubaddressType": "unit_type",
+    "PlaceName": "city",
+    "StateName": "state",
+    "ZipCode": "zip_code",
+    "USPSBoxID": "po_box",
 }
-TWO_CHAR_DIRECTIONS = ['NO', 'SO', 'EA', 'WE']
-with open(join(dirname(realpath(__file__)), 'street_types.json'), 'r') as file:
+TWO_CHAR_DIRECTIONS = ["NO", "SO", "EA", "WE"]
+with open(join(dirname(realpath(__file__)), "street_types.json"), "r") as file:
     STREET_TYPES = json.loads(file.read())
-HWY_REGEX = re.compile('(SR|STATE ROUTE|HIGHWAY)')
-UNIT_VALUES_NOT_APPROPRIATE_FOR_HASH_SIGN = ['rear']
+HWY_REGEX = re.compile("(SR|STATE ROUTE|HIGHWAY)")
+UNIT_VALUES_NOT_APPROPRIATE_FOR_HASH_SIGN = ["rear"]
+CARDINALS = ["N", "S", "E", "W", "NO", "SO", "EA", "WE", "NORTH", "SOUTH", "EAST", "WEST"]
+SHORTENED_CARDINALS = re.compile("rd|nd|th$", re.IGNORECASE)
 
 
-class Address():
-    '''
+class Address:
+    """
     Class for parsing address strings
-    '''
+    """
+
     address_number = None
     address_number_suffix = None
     prefix_direction = None
     street_name = None
     street_direction = None
     street_type = None
     unit_type = None
     unit_id = None
     city = None
     zip_code = None
     po_box = None
     state = None
+    StreetNamePreType = None
+    StreetNamePreModifier = None
 
     def __init__(self, address_text):
-        parts, parsed_as = usaddress.tag(address_text.replace('.', ''), TAG_MAPPING)
-        if parsed_as not in ['Street Address', 'PO Box']:
+        address_text = address_text.replace(".", "")
+        extra_unit_parts = None
+        try:
+            parts, parsed_as = usaddress.tag(address_text, TAG_MAPPING)
+        except usaddress.RepeatedLabelError:
+            parts, parsed_as = usaddress.tag(" ".join(address_text.split(" ")[:-2]), TAG_MAPPING)
+            extra_unit_parts, _ = usaddress.tag(" ".join(address_text.split(" ")[-2:]), TAG_MAPPING)
+        if parsed_as not in ["Street Address", "PO Box"]:
             raise Exception(f'"{address_text}" is not recognized as a valid street address, or P.O. Box')
 
         for part in parts:
             try:
                 value = parts[part].upper()
-                if part.endswith('direction'):
+                if part.endswith("direction"):
                     value = normalize_direction(value)
 
                 setattr(self, part, value)
             except AttributeError:
                 pass
 
+        #: check for incorrectly included prefix directions in street name
+        if self.street_name is not None:
+            street_name_parts = self.street_name.split(" ")
+            first_word = street_name_parts[0].upper()
+            if len(street_name_parts) > 1 and is_cardinal(first_word) and self.prefix_direction is None:
+                self.prefix_direction = normalize_direction(first_word)
+                self.street_name = " ".join(street_name_parts[1:])
+
+        #: check for cardinals incorrectly parsed as address_number_suffix
+        if is_cardinal(self.address_number_suffix):
+            self.street_name = f"{parts['prefix_direction'].upper()} {self.street_name}"
+            self.prefix_direction = self.address_number_suffix
+            self.address_number_suffix = None
+
         if self.po_box is not None:
             return
 
-        try:
+        if self.StreetNamePreType is not None:
             #: e.g. US HWY
-            self.street_name = f'{normalize_street_name_pre_type(self.StreetNamePreType)} {self.street_name}'
+            self.street_name = f"{normalize_street_name_pre_type(self.StreetNamePreType)} {self.street_name}"
             del self.StreetNamePreType
-        except AttributeError:
-            pass
 
-        try:
-            self.street_name = f'{self.StreetNamePreModifier} {self.street_name}'
+        if self.StreetNamePreModifier is not None:
+            self.street_name = f"{self.StreetNamePreModifier} {self.street_name}"
             del self.StreetNamePreModifier
-        except AttributeError:
-            pass
 
         #: look for two-character prefix directions which usaddress does not handle
-        if self.street_name:
-            street_name_parts = self.street_name.split(' ')
+        if self.street_name is not None:
+            street_name_parts = self.street_name.split(" ")
             if len(street_name_parts) > 1:
                 if street_name_parts[0].upper() in TWO_CHAR_DIRECTIONS and self.prefix_direction is None:
                     self.prefix_direction = normalize_direction(street_name_parts[0])
-                    self.street_name = ' '.join(street_name_parts[1:])
+                    self.street_name = " ".join(street_name_parts[1:])
                 elif street_name_parts[-1].upper() in TWO_CHAR_DIRECTIONS and self.street_direction is None:
                     self.street_direction = normalize_direction(street_name_parts[-1])
-                    self.street_name = ' '.join(street_name_parts[:-1])
+                    self.street_name = " ".join(street_name_parts[:-1])
 
         if self.street_type is not None:
             #: handle multiple street_types (assume only the last one is valid and move all others to the street name)
-            if len(self.street_type.split(' ')) > 1:
-                parsed_street_types = self.street_type.split(' ')
-                self.street_name += ' ' + ' '.join(parsed_street_types[:-1])
+            if len(self.street_type.split(" ")) > 1:
+                parsed_street_types = self.street_type.split(" ")
+                new_street_name = " ".join(parsed_street_types[:-1])
+                if self.street_name is None:
+                    self.street_name = new_street_name
+                else:
+                    self.street_name += f" {new_street_name}"
                 self.street_type = parsed_street_types[-1]
 
             try:
                 self.street_type = normalize_street_type(self.street_type)
             except InvalidStreetTypeError:
                 #: must be part of the street name
-                self.street_name += f' {self.street_type}'
+                if self.street_name is None:
+                    self.street_name = self.street_type
+                else:
+                    self.street_name += f" {self.street_type}"
                 self.street_type = None
 
+        if self.street_direction is not None and self.street_name is not None:
+            #: check for shortened cardinals
+            self.street_name = SHORTENED_CARDINALS.sub("00", self.street_name)
+
         if self.unit_id is not None:
             #: add `#` if there is not unit type and the unit is numeric
-            if not self.unit_id.startswith('#') and self.unit_type is None and self.unit_id.lower() not in UNIT_VALUES_NOT_APPROPRIATE_FOR_HASH_SIGN:
-                self.unit_id = f'# {self.unit_id}'
+            if (
+                not self.unit_id.startswith("#")
+                and self.unit_type is None
+                and self.unit_id.lower() not in UNIT_VALUES_NOT_APPROPRIATE_FOR_HASH_SIGN
+            ):
+                self.unit_id = f"# {self.unit_id}"
 
             #: strip `#` if there is a unit type
-            elif self.unit_id.startswith('#') and self.unit_type is not None:
+            elif self.unit_id.startswith("#") and self.unit_type is not None:
                 self.unit_id = self.unit_id[1:].strip()
 
+            if extra_unit_parts:
+                self.unit_id = f"{self.unit_id}-{extra_unit_parts['unit_id']}"
+
     def __repr__(self):
         properties = vars(self)
-        properties.update({'normalized': self.normalized})
+        properties.update({"normalized": self.normalized})
 
-        return f'Parsed Address:\n{pprint.pformat(properties)}'
+        return f"Parsed Address:\n{pprint.pformat(properties)}"
 
     @property
     def normalized(self):
-        '''
+        """
         getter for normalized address string
-        '''
+        """
         if self.po_box is not None:
-            return f'PO BOX {self.po_box}'
+            return f"PO BOX {self.po_box}"
 
         parts = [
-            self.address_number, self.address_number_suffix, self.prefix_direction, self.street_name, self.street_type, self.street_direction, self.unit_type,
-            self.unit_id
+            self.address_number,
+            self.address_number_suffix,
+            self.prefix_direction,
+            self.street_name,
+            self.street_type,
+            self.street_direction,
+            self.unit_type,
+            self.unit_id,
         ]
 
-        return ' '.join([part for part in parts if part is not None])
+        return " ".join([part for part in parts if part is not None])
 
 
 def normalize_direction(direction_text):
-    '''
+    """
     returns the single letter corresponding to the input direction
-    '''
+    """
 
     return direction_text[0].upper()
 
 
 def normalize_street_type(type_text):
-    '''
+    """
     returns the standard abbreviation for the input street type
-    '''
+    """
 
     type_text = type_text.upper()
     for abbreviation, values in STREET_TYPES.items():
         if type_text in values:
             return abbreviation
 
     raise InvalidStreetTypeError(type_text)
 
 
 def normalize_street_name_pre_type(text):
-    '''normalizes highways by doing things like replaces SR with HWY and removes US
+    """normalizes highways by doing things like replaces SR with HWY and removes US
 
     No need to worried about casing or "."s because usaddress has already taken care of them by this point.
-    '''
-    return HWY_REGEX.sub('HWY', text).replace('US ', '')
+    """
+    return HWY_REGEX.sub("HWY", text).replace("US ", "")
 
 
 class InvalidStreetTypeError(Exception):
-    '''
+    """
     exception for when the street type does not have a corresponding value in street_types.json
-    '''
+    """
 
     def __init__(self, type_text):
         super().__init__()
-        self.message = f'No matching abbreviation found for {type_text}'
+        self.message = f"No matching abbreviation found for {type_text}"
+
+
+def is_cardinal(text):
+    """
+    returns True if the input text is a cardinal direction
+    """
+
+    if text is None:
+        return False
+
+    return text.upper() in CARDINALS
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/backup.py` & `agrc-sweeper-2.0.0/src/sweeper/backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 backup.py
 A module that creates a gdb if it doesn't exist and inserts a feature class
-'''
+"""
+
+import logging
 import os
 from datetime import datetime
 
 import arcpy
+
 from . import workspace_info
-import logging
 
-log = logging.getLogger('sweeper')
+log = logging.getLogger("sweeper")
+
 
 def backup_data(workspace_path, table_name, out_path):
-    '''
+    """
     workspace_path: the full path to the workspace or geodatabase containing the tables to be backed up.
     table_name: the table name to be backed up - if it was provided to the CLI.
     out_path: a geodatabase path where the feature class will be stored.
-    '''
-    now = datetime.now().strftime('%Y%m%d_%H%M')
+    """
+    now = datetime.now().strftime("%Y%m%d_%H%M")
 
     #: check if the db exists
     if not arcpy.Exists(out_path):
         #: if db does not exist, then create it
-        out_dir = out_path.rsplit('\\', 1)[0]
-        gdb_name = out_path.rsplit('\\', 1)[1]
+        out_dir = out_path.rsplit("\\", 1)[0]
+        gdb_name = out_path.rsplit("\\", 1)[1]
 
         arcpy.management.CreateFileGDB(out_dir, gdb_name)
 
     tables_to_backup = []
 
     #: populate the list with feature class name(s) to backup
-    if table_name: #: table name was provided.
+    if table_name:  #: table name was provided.
         tables_to_backup.append(table_name)
-    else: #: table name was not provided, use all tables in workspace.
+    else:  #: table name was not provided, use all tables in workspace.
         #: get a list of feature class names that are contained in the provided workspace
         feature_class_names = workspace_info.get_featureclasses(workspace_path)
         for feature_class in feature_class_names:
             tables_to_backup.append(feature_class)
 
     #: loop through the list and backup each feature class
     for table in tables_to_backup:
         full_table_path = os.path.join(workspace_path, table)
-        fc_name = full_table_path.rsplit('\\', 1)[1] + '_' + now
+        fc_name = full_table_path.rsplit("\\", 1)[1] + "_" + now
 
         #: backup the source feature class
         arcpy.management.Copy(full_table_path, os.path.join(out_path, fc_name))
 
-    log.info(f'The following feature classes were backed up here', out_path, ':', str(tables_to_backup))
+    log.info("The following feature classes were backed up here", out_path, ":", str(tables_to_backup))
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/report.py` & `agrc-sweeper-2.0.0/src/sweeper/report.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,181 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 report.py
 A module that contains the templates for the reports and functions to format data into the report
-'''
+"""
 
 import os
 import io
 from datetime import datetime
 import logging
 
-log = logging.getLogger('sweeper')
+log = logging.getLogger("sweeper")
+
 
 def _print_items(report, key, writer):
-    '''print out issues or fixes
+    """print out issues or fixes
     report: report dictionary
     key: 'issues' | 'fixes'
     writer: function
-    '''
+    """
     try:
         items = report[key]
     except KeyError:
         return
 
     items_found = len(items)
     if items_found == 0:
-        writer(f'No {key} found!')
-        writer('---')
+        writer(f"No {key} found!")
+        writer("---")
 
         return
 
-    writer(f'{items_found} {key} found:')
+    writer(f"{items_found} {key} found:")
 
     has_oids = True
     if isinstance(items, list):
         for item in items:
             if isinstance(item, int):
-                writer(f'    ObjectID {item}')
+                writer(f"    ObjectID {item}")
             else:
                 #: issues not associated with a specific row (e.g. metadata)
                 has_oids = False
-                writer(f'    {item}')
+                writer(f"    {item}")
     else:
         #: must be dict
         for oid in items:
-            writer(f'    ObjectID {oid}: {items[oid]}')
+            writer(f"    ObjectID {oid}: {items[oid]}")
 
     if has_oids:
-        writer(f'\nSelect statement to view {key} in ArcGIS:')
+        writer(f"\nSelect statement to view {key} in ArcGIS:")
         statement = f'OBJECTID IN ({", ".join([str(oid) for oid in items])})'
 
         writer(statement)
 
-    writer('---')
+    writer("---")
+
 
 def _generate_report(writer, reports):
     if len(reports) == 0:
-        writer('No issues found!')
+        writer("No issues found!")
 
         return None
 
     #: loop through each report dict in the list of dicts
     for report in reports:
         writer(f'{report["title"]} Report for {report["feature_class"]}')
 
-        _print_items(report, 'fixes', writer)
-        _print_items(report, 'issues', writer)
+        _print_items(report, "fixes", writer)
+        _print_items(report, "issues", writer)
+
 
 def save_report(reports, save_directory):
-    '''
+    """
     save_directory
       - folder sweeper_run_YYYYMMDD_HHmm
         - featureclassname_sweepername_numberofissues.txt `Counties_Empties_5.txt`   `Counties_Empties_0.txt`
-    '''
+    """
     report_directory = _create_report_directory(save_directory)
 
     for report in reports:
         file_name = _get_file_name(report)
         file_path = os.path.join(report_directory, file_name)
 
-        with open(file_path, 'w') as textfile:
+        with open(file_path, "w") as textfile:
+
             def write_lines(text):
-                textfile.writelines(f'{text}\n')
+                textfile.writelines(f"{text}\n")
 
             _generate_report(write_lines, [report])
 
+
 def print_report(reports):
     _generate_report(print, reports)
 
+
 def _get_file_name(report):
-    title = report['title'].replace(' ', '')
+    title = report["title"].replace(" ", "")
 
     return f'{report["feature_class"]}_{title}_{len(report["issues"])}.txt'
 
+
 def _create_report_directory(parent_directory):
-    now = datetime.now().strftime('%Y%m%d_%H%M')
+    now = datetime.now().strftime("%Y%m%d_%H%M")
 
-    report_directory = os.path.join(parent_directory, f'sweeper_run_{now}')
+    report_directory = os.path.join(parent_directory, f"sweeper_run_{now}")
     os.makedirs(report_directory)
 
     return report_directory
 
+
 def format_message(reports):
     message = io.StringIO()
-    now = datetime.now().strftime('%Y%m%d_%H%M')
-    message.write(f'<pre>Email summary for {now} Sweeper run \n\n</pre>')
+    now = datetime.now().strftime("%Y%m%d_%H%M")
+    message.write(f"<pre>Email summary for {now} Sweeper run \n\n</pre>")
 
     if not reports:
-        message.write('<pre>No changes identified or Sweeper tests run\n</pre>')
+        message.write("<pre>No changes identified or Sweeper tests run\n</pre>")
     else:
         for report in reports:
-            message.write(f'<pre>{len(report["issues"]):4} Issues \t {report["title"]:<16} \t {report["feature_class"]:<50} \n</pre>')
+            message.write(
+                f'<pre>{len(report["issues"]):4} Issues \t {report["title"]:<16} \t {report["feature_class"]:<50} \n</pre>'
+            )
 
     return message
 
 
 def _log_items(report, key):
-    '''print out issues or fixes to log
+    """print out issues or fixes to log
     report: report dictionary
     key: 'issues' | 'fixes'
-    '''
+    """
     try:
         items = report[key]
     except KeyError:
         return
 
     items_found = len(items)
     if items_found == 0:
-        log.info(f'No {key} found!')
-        log.info('---')
+        log.info(f"No {key} found!")
+        log.info("---")
 
         return
 
-    log.info(f'{items_found} {key} found:')
+    log.info(f"{items_found} {key} found:")
 
     has_oids = True
     if isinstance(items, list):
         for item in items:
             if isinstance(item, int):
-                log.info(f'    ObjectID {item}')
+                log.info(f"    ObjectID {item}")
             else:
                 #: issues not associated with a specific row (e.g. metadata)
                 has_oids = False
-                log.info(f'    {item}')
+                log.info(f"    {item}")
     else:
         #: must be dict
         for oid in items:
-            log.info(f'    ObjectID {oid}: {items[oid]}')
+            log.info(f"    ObjectID {oid}: {items[oid]}")
 
     if has_oids:
-        log.info(f'\nSelect statement to view {key} in ArcGIS:')
+        log.info(f"\nSelect statement to view {key} in ArcGIS:")
         statement = f'OBJECTID IN ({", ".join([str(oid) for oid in items])})'
 
         log.info(statement)
 
-    log.info('---')
+    log.info("---")
 
 
 def add_to_log(reports):
     if len(reports) == 0:
-        log.info('No issues found!')
+        log.info("No issues found!")
 
         return None
 
     #: loop through each report dict in the list of dicts
     for report in reports:
         log.info(f'{report["title"]} Report for {report["feature_class"]}')
 
-        _log_items(report, 'fixes')
-        _log_items(report, 'issues')
+        _log_items(report, "fixes")
+        _log_items(report, "issues")
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/street_types.json` & `agrc-sweeper-2.0.0/src/sweeper/street_types.json`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.3/src/sweeper/sweepers/UseLimitations.html` & `agrc-sweeper-2.0.0/src/sweeper/sweepers/UseLimitations.html`

 * *Files identical despite different names*

### Comparing `agrc-sweeper-1.4.3/src/sweeper/sweepers/addresses.py` & `agrc-sweeper-2.0.0/src/sweeper/sweepers/addresses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 addresses.py
 
 A sweeper that works on address fields
-'''
+"""
 
 import arcpy
+
+
 from ..address_parser import Address
 
 
-class AddressTest():
-    '''A class that validates address data
-    '''
+class AddressTest:
+    """A class that validates address data"""
+
+    key = "addresses"
+
     def __init__(self, workspace, table_name, field_name):
         self.workspace = workspace
         self.table_name = table_name
         self.field_name = field_name
         self.oids_with_issues = []
 
     def sweep(self):
-        '''Loop through all values and check addresses for problems returning a report
-        '''
-        report = {'title': 'Address Test', 'feature_class': self.table_name, 'issues': {}}
-        required_street_address_parts = set(['address_number', 'street_name'])
+        """Loop through all values and check addresses for problems returning a report"""
+        report = {"title": "Address Test", "feature_class": self.table_name, "issues": {}}
+        required_street_address_parts = set(["address_number", "street_name"])
 
         with arcpy.EnvManager(workspace=self.workspace):
-            with arcpy.da.SearchCursor(self.table_name, ['OID@', self.field_name]) as search_cursor:
+            with arcpy.da.SearchCursor(self.table_name, ["OID@", self.field_name]) as search_cursor:
                 for oid, address in search_cursor:
                     issue_message = None
                     try:
                         parsed_address = Address(address)
                     except Exception as exception:
                         issue_message = str(exception)
 
                     if issue_message is None:
                         parts_found = set(parsed_address.__dict__)
                         missing_parts = required_street_address_parts - parts_found
-                        if len(missing_parts) > 0 and 'po_box' not in parts_found:
+                        if len(missing_parts) > 0 and "po_box" not in parts_found:
                             issue_message = f'missing address parts: {", ".join(missing_parts)}'
                         elif parsed_address.normalized != address:
-                            issue_message = f'address not fully normalized: "{address}" -> "{parsed_address.normalized}"'
+                            issue_message = (
+                                f'address not fully normalized: "{address}" -> "{parsed_address.normalized}"'
+                            )
 
                     if issue_message is not None:
-                        report['issues'][oid] = issue_message
+                        report["issues"][oid] = issue_message
                         self.oids_with_issues.append(oid)
 
         return report
 
     def try_fix(self):
-        report = {'title': 'Address Try Fix', 'feature_class': self.table_name, 'issues': {}, 'fixes': {}}
+        report = {"title": "Address Try Fix", "feature_class": self.table_name, "issues": {}, "fixes": {}}
 
         with arcpy.EnvManager(workspace=self.workspace):
             describe = arcpy.da.Describe(self.table_name)
             where = f'{describe["OIDFieldName"]} IN ({", ".join([str(oid) for oid in self.oids_with_issues])})'
-            with arcpy.da.UpdateCursor(self.table_name, ['OID@', self.field_name], where_clause=where) as update_cursor:
+            with arcpy.da.UpdateCursor(self.table_name, ["OID@", self.field_name], where_clause=where) as update_cursor:
                 for oid, address in update_cursor:
                     try:
                         parsed_address = Address(address)
                         update_cursor.updateRow((oid, parsed_address.normalized))
-                        report['fixes'][oid] = f'{address} -> {parsed_address.normalized}'
+                        report["fixes"][oid] = f"{address} -> {parsed_address.normalized}"
                     except Exception as exception:
-                        report['issues'][oid] = str(exception)
+                        report["issues"][oid] = str(exception)
 
         return report
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/sweepers/duplicates.py` & `agrc-sweeper-2.0.0/src/sweeper/sweepers/duplicates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,128 @@
 #!/usr/bin/env python
 # * coding: utf8 *
+import logging
 import re
 
+import arcpy
 from xxhash import xxh64
-from .. import credentials
 
-import arcpy
-import logging
+from .base import SweeperBase
+
+log = logging.getLogger("sweeper")
+
 
-log = logging.getLogger('sweeper')
+class DuplicateTest(SweeperBase):
+    """A class that finds and removes duplicate geometries or attributes or both"""
+
+    key = "duplicates"
 
-class DuplicateTest():
-    '''A class that finds and removes duplicate geometries or attributes or both
-    '''
     def __init__(self, workspace, table_name):
         self.workspace = workspace
         self.table_name = table_name
         self.oids_with_issues = []
         self.is_table = False
 
-
     def sweep(self):
-        '''A method that finds duplicate records and returns a report dictionary
-        '''
-        report = {'title': 'Duplicate Test', 'feature_class': self.table_name, 'issues': []}
+        """A method that finds duplicate records and returns a report dictionary"""
+        report = {"title": "Duplicate Test", "feature_class": self.table_name, "issues": []}
         digests = set([])
 
-        truncate_shape_precision = re.compile(r'(\d+\.\d{2})(\d+)')
+        truncate_shape_precision = re.compile(r"(\d+\.\d{2})(\d+)")
 
         with arcpy.EnvManager(workspace=self.workspace):
             description = arcpy.da.Describe(self.table_name)
-            log.info(f'Working on Duplicates for: {self.table_name}')
-            if description['dataType'].casefold() == 'table':
+            log.info(f"Working on Duplicates for: {self.table_name}")
+            if description["dataType"].casefold() == "table":
                 self.is_table = True
-                skip_fields = ['guid']
+                skip_fields = ["guid"]
             else:
-                skip_fields = ['guid', description['shapeFieldName']]
-
+                skip_fields = ["guid", description["shapeFieldName"]]
 
-            if description['hasGlobalID']:
-                skip_fields.append(description['globalIDFieldName'])
+            if description["hasGlobalID"]:
+                skip_fields.append(description["globalIDFieldName"])
 
-            if description['hasOID']:
-                skip_fields.append(description['OIDFieldName'])
+            if description["hasOID"]:
+                skip_fields.append(description["OIDFieldName"])
 
-            fields = [field.name for field in description['fields'] if field.name not in skip_fields]
-            fields.append('OID@')
+            fields = [field.name for field in description["fields"] if field.name not in skip_fields]
+            fields.append("OID@")
 
             #: include or exclude shape field depending on if working on table or feature class
             if self.is_table:
-                oid_index = fields.index('OID@')
+                oid_index = fields.index("OID@")
 
                 with arcpy.da.SearchCursor(self.table_name, fields) as search_cursor:
                     for row in search_cursor:
                         object_id = row[oid_index]
 
-                        hasher = xxh64(f'{row[:-1]}')
+                        hasher = xxh64(f"{row[:-1]}")
                         digest = hasher.hexdigest()
 
                         if digest in digests:
-                            report['issues'].append(str(object_id))
+                            report["issues"].append(str(object_id))
                             self.oids_with_issues.append(object_id)
 
                         digests.add(digest)
             else:
-                oid_index = fields.index('OID@')
-                fields.append('SHAPE@WKT')
+                oid_index = fields.index("OID@")
+                fields.append("SHAPE@WKT")
 
-                shapefield_index = fields.index('SHAPE@WKT')
-                oid_index = fields.index('OID@')
+                shapefield_index = fields.index("SHAPE@WKT")
+                oid_index = fields.index("OID@")
 
                 with arcpy.da.SearchCursor(self.table_name, fields) as search_cursor:
                     for row in search_cursor:
                         shape_wkt = row[shapefield_index]
                         object_id = row[oid_index]
 
                         if shape_wkt is None:
                             continue
 
                         #: trim some digits to help with hash matching
-                        generalized_wkt = truncate_shape_precision.sub(r'\1', shape_wkt)
+                        generalized_wkt = truncate_shape_precision.sub(r"\1", shape_wkt)
 
-                        hasher = xxh64(f'{row[:-2]} {generalized_wkt}')
+                        hasher = xxh64(f"{row[:-2]} {generalized_wkt}")
                         digest = hasher.hexdigest()
 
                         if digest in digests:
-                            report['issues'].append(str(object_id))
+                            report["issues"].append(str(object_id))
                             self.oids_with_issues.append(object_id)
 
                         digests.add(digest)
 
         return report
 
-
     def try_fix(self):
-        '''a method that tries to remove the duplicate records
-        '''
-        report = {'title': 'Duplicate Try Fix', 'feature_class': self.table_name, 'issues': [], 'fixes': []}
+        """a method that tries to remove the duplicate records"""
+        report = {"title": "Duplicate Try Fix", "feature_class": self.table_name, "issues": [], "fixes": []}
 
         if len(self.oids_with_issues) == 0:
             return report
 
         sql = f'"OBJECTID" IN ({",".join([str(oid) for oid in self.oids_with_issues])})'
-        temp_feature_layer = 'temp_layer'
+        temp_feature_layer = "temp_layer"
 
-        log.info(f'Workspace is:   {self.workspace}')
+        log.info(f"Workspace is:   {self.workspace}")
         #: Delete duplicate rows using different arcpy tools for tables and feature classes
         with arcpy.EnvManager(workspace=self.workspace):
             if self.is_table:
                 duplicate_features = arcpy.management.MakeTableView(self.table_name, temp_feature_layer, sql)
             else:
                 duplicate_features = arcpy.management.MakeFeatureLayer(self.table_name, temp_feature_layer, sql)
 
             try:
-                log.info(f'attempting to delete {len(self.oids_with_issues)} duplicate records')
+                log.info(f"attempting to delete {len(self.oids_with_issues)} duplicate records")
                 if self.is_table:
                     arcpy.management.DeleteRows(duplicate_features)
                 else:
                     arcpy.management.DeleteFeatures(duplicate_features)
             except Exception as error:
-                error_message = f'unable to delete features {error}'
-                report['issues'].append(error_message)
+                error_message = f"unable to delete features {error}"
+                report["issues"].append(error_message)
             finally:
                 if arcpy.Exists(temp_feature_layer):
                     arcpy.management.Delete(temp_feature_layer)
 
-            report['fixes'].append(f'{len(self.oids_with_issues)} records deleted successfully')
+            report["fixes"].append(f"{len(self.oids_with_issues)} records deleted successfully")
 
         return report
-
-    def clone(self, table_name):
-        log.info(f'cloning to {table_name}')
-        user = table_name.split('.')[0].upper()
-        user_workspace = credentials.CONNECTIONS[user]
-        return DuplicateTest(user_workspace, table_name)
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/sweepers/empties.py` & `agrc-sweeper-2.0.0/src/sweeper/sweepers/empties.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 #!/usr/bin/env python
 # * coding: utf8 *
 
 
-import arcpy
-from .. import credentials
 import logging
 
-log = logging.getLogger('sweeper')
+import arcpy
+
+from .base import SweeperBase
+
+log = logging.getLogger("sweeper")
+
+
+class EmptyTest(SweeperBase):
+    """A class to find empty geometries"""
+
+    key = "empties"
 
-class EmptyTest():
-    '''A class to find empty geometries
-    '''
     def __init__(self, workspace, table_name):
         self.workspace = workspace
         self.table_name = table_name
         self.oids_with_issues = []
 
-
     def sweep(self):
-        '''A method to find empty geometries and return a report dictionary
-        '''
-        report = {'title': 'Empty Test', 'feature_class': self.table_name, 'issues': []}
-        fields = ['OID@', 'SHAPE@']
+        """A method to find empty geometries and return a report dictionary"""
+        report = {"title": "Empty Test", "feature_class": self.table_name, "issues": []}
+        fields = ["OID@", "SHAPE@"]
 
         with arcpy.EnvManager(workspace=self.workspace):
             description = arcpy.da.Describe(self.table_name)
 
-            if description['dataType'].casefold() == 'table':
-                log.info(f'{self.table_name} is a table, skipping EmptyTest ...')
+            if description["dataType"].casefold() == "table":
+                log.info(f"{self.table_name} is a table, skipping EmptyTest ...")
             else:
                 with arcpy.da.SearchCursor(self.table_name, fields) as search_cursor:
                     for oid, geometry in search_cursor:
                         if geometry is not None:
                             continue
 
-                        report['issues'].append(str(oid))
+                        report["issues"].append(str(oid))
                         self.oids_with_issues.append(oid)
 
         return report
 
-
     def try_fix(self):
-        '''A method to that attempts to remove records with empty geometries
-        '''
-        report = {'title': 'Empty Try Fix', 'feature_class': self.table_name, 'issues': [], 'fixes': []}
+        """A method to that attempts to remove records with empty geometries"""
+        report = {"title": "Empty Try Fix", "feature_class": self.table_name, "issues": [], "fixes": []}
         if len(self.oids_with_issues) == 0:
             return report
 
         #: for point, polylines, or polygons
-        fields = ['OID@']
+        fields = ["OID@"]
         query = f'OBJECTID IN ({",".join([str(oid) for oid in self.oids_with_issues])})'
 
-        log.info(f'Workspace is:   {self.workspace}')
+        log.info(f"Workspace is:   {self.workspace}")
         with arcpy.EnvManager(workspace=self.workspace):
             with arcpy.da.UpdateCursor(self.table_name, fields, query) as update_cursor:
-                for oid, in update_cursor:
+                for (oid,) in update_cursor:
                     if oid not in self.oids_with_issues:
                         continue
 
                     update_cursor.deleteRow()
 
-        report['fixes'].append(f'{len(self.oids_with_issues)} records deleted successfully')
+        report["fixes"].append(f"{len(self.oids_with_issues)} records deleted successfully")
 
         return report
-
-    def clone(self, table_name):
-        log.info(f'cloning to {table_name}')
-        user = table_name.split('.')[0].upper()
-        user_workspace = credentials.CONNECTIONS[user]
-        return EmptyTest(user_workspace, table_name)
```

### Comparing `agrc-sweeper-1.4.3/src/sweeper/workspace_info.py` & `agrc-sweeper-2.0.0/src/sweeper/workspace_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,123 @@
 #!/usr/bin/env python
 # * coding: utf8 *
-'''
+"""
 workspace_info.py
 A module that gets information about the workspace, including a list of feature classes.
-'''
-import arcpy
+"""
+
 import datetime
-from pathlib import Path
-from . import credentials
 import logging
+from pathlib import Path
+
+import arcpy
+
+from . import config
+
+log = logging.getLogger("sweeper")
 
-log = logging.getLogger('sweeper')
 
 #: A function to determine when change detection was last run
 def read_last_check_date():
-    last_checked = Path('./.last_checked')
+    last_checked = Path("./.last_checked")
 
-    last_date_string = ''
+    last_date_string = ""
 
     if last_checked.exists():
-        with open(last_checked, 'r') as log_file:
+        with open(last_checked, "r") as log_file:
             last_date_string = log_file.readline().strip()
 
     if last_date_string is None or len(last_date_string) < 1:
         return None
 
     return last_date_string
 
 
 #: A function to update the last_checked file
 def update_last_check_date():
-    last_checked = Path('./.last_checked')
+    last_checked = Path("./.last_checked")
 
     if not last_checked.exists():
         last_checked.touch()
 
-    with open(last_checked, 'w') as log_file:
-        log_file.write(datetime.datetime.today().strftime('%Y-%m-%d'))
+    with open(last_checked, "w") as log_file:
+        log_file.write(datetime.datetime.today().strftime("%Y-%m-%d"))
 
 
 #: A function to generate and return a list of workspace feature classes.
 def get_featureclasses(workspace_path):
-    '''
+    """
     workspace_path: full path to the feature workspace.
-    '''
+    """
+
+    try:
+        arcpy.da.Describe(workspace_path)
+    except ValueError:
+        raise ValueError(f"{workspace_path} is not a valid workspace.")
 
     with arcpy.EnvManager(workspace=workspace_path):
         fc_list = []
 
-        datasets = arcpy.ListDatasets(feature_type='feature')
-        datasets = [''] + datasets if datasets is not None else []
+        datasets = arcpy.ListDatasets(feature_type="feature")
+        #: add an empty string to make sure we get feature layers in the root
+        datasets = [""] + datasets if datasets is not None else []
 
         #: generate a list of feature classes showing their full path (Example: Directory/Workspace/Dataset/TableName)
         for ds in datasets:
             for fc in arcpy.ListFeatureClasses(feature_dataset=ds):
                 fc_list.append(fc)
 
         return fc_list
 
 
 #: A function to return a list of feature classes based on the change detection table.
 def get_change_detection():
-
     checked_date = read_last_check_date()
 
     if checked_date:
-        checked_string = datetime.datetime.strptime(checked_date, '%Y-%m-%d')
+        checked_string = datetime.datetime.strptime(checked_date, "%Y-%m-%d")
     else:
         checked_string = datetime.date.today()
 
-    last_checked = checked_string.strftime('%m/%d/%Y')
-    log.info(f'Last date change detection was checked: {last_checked}')
+    last_checked = checked_string.strftime("%m/%d/%Y")
+    log.info(f"Last date change detection was checked: {last_checked}")
 
-    egdb = Path(credentials.DB)
-    cd_table = credentials.CHANGE_DETECTION
+    egdb = Path(config.get_config("CHANGE_DETECTION_CONNECTION"))
+    cd_table = config.get_config("CHANGE_DETECTION_TABLE")
 
     egdb_conn = arcpy.ArcSDESQLExecute(str(egdb))
     sql = f"SELECT table_name FROM {cd_table} WHERE last_modified >= '{last_checked}'"
 
     #: result will typically be a nested list
     result = egdb_conn.execute(sql)
-    log.info(f'SQL execution result: {result}')
+    log.info(f"SQL execution result: {result}")
 
     #: handle cases where result is a string (single feature class) or not a list (None type)
     if isinstance(result, str):
         #: reset list to None if single table doesn't exist in Internal database
         if not arcpy.Exists(str(egdb / result)):
-            fc_list = None
+            fc_list = []
             return fc_list
-        
+
         fc_list = []
         fc_list.append(result)
-        fc_list = [item.split('.', 1)[1] for item in fc_list]
-        log.info(f'fc_list is: {fc_list}')
+        fc_list = [item.split(".", 1)[1] for item in fc_list]
+        log.info(f"fc_list is: {fc_list}")
         return fc_list
-    
+
     elif not isinstance(result, list):
-        fc_list = None
+        fc_list = []
         return fc_list
 
     #: Flatten resulting list
     fc_list = [item for sublist in result for item in sublist]
 
     #: Remove tables that aren't in the Internal database (but were in the change detection table)
     for fc in fc_list:
         if not arcpy.Exists(str(egdb / fc)):
             fc_list.remove(fc)
 
     #: Strip off the leading 'sgid.' of each table name
-    fc_list = [item.split('.', 1)[1] for item in fc_list]
-    log.info(f'fc_list is: {fc_list}')
+    fc_list = [item.split(".", 1)[1] for item in fc_list]
+    log.info(f"fc_list is: {fc_list}")
 
     return fc_list
```

