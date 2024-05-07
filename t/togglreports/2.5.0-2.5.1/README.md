# Comparing `tmp/togglreports-2.5.0.tar.gz` & `tmp/togglreports-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "togglreports-2.5.0.tar", last modified: Wed Mar 15 16:09:45 2023, max compression
+gzip compressed data, was "togglreports-2.5.1.tar", last modified: Tue May  7 11:53:13 2024, max compression
```

## Comparing `togglreports-2.5.0.tar` & `togglreports-2.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.528849 togglreports-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-15 16:09:20.000000 togglreports-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-15 16:09:20.000000 togglreports-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-15 16:09:45.532849 togglreports-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-15 16:09:20.000000 togglreports-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-15 16:09:45.532849 togglreports-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-15 16:09:20.000000 togglreports-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.524849 togglreports-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.524849 togglreports-2.5.0/src/togglreports/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 16:09:42.000000 togglreports-2.5.0/src/togglreports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.528849 togglreports-2.5.0/src/togglreports/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/core/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/core/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/core/report_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.528849 togglreports-2.5.0/src/togglreports/data/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/data/reports.json
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/data/reports_example.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.528849 togglreports-2.5.0/src/togglreports/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/plugins/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/plugins/sgu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/togglapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-15 16:09:20.000000 togglreports-2.5.0/src/togglreports/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:09:45.528849 togglreports-2.5.0/src/togglreports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-15 16:09:45.000000 togglreports-2.5.0/src/togglreports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 11:52:51.000000 togglreports-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 11:52:51.000000 togglreports-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-07 11:53:13.399569 togglreports-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-07 11:52:51.000000 togglreports-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-07 11:53:13.403569 togglreports-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 11:52:51.000000 togglreports-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.395568 togglreports-2.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/src/togglreports/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 11:53:11.000000 togglreports-2.5.1/src/togglreports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/src/togglreports/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/core/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/core/report_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/src/togglreports/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/data/reports.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/data/reports_example.json
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/src/togglreports/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/plugins/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/plugins/sgu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/togglapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-07 11:52:51.000000 togglreports-2.5.1/src/togglreports/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:53:13.399569 togglreports-2.5.1/src/togglreports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 11:53:13.000000 togglreports-2.5.1/src/togglreports.egg-info/top_level.txt
```

### Comparing `togglreports-2.5.0/LICENSE` & `togglreports-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/PKG-INFO` & `togglreports-2.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: togglreports
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple project to automate the creation of reports using the Toggl API.
 Home-page: https://github.com/ro-56/togglReports
 Author: Rodrigo Mendonça
 Author-email: rodrigogr.mendonca@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,18 @@
 
 The `--period` tag can be used to build reports with common start and end times. Possible values are: 
  - `today`: entries for today
  - `thisweek`: entries from the last sunday to the next saturday
  - `lastweek`: entries from past week, from sunday to saturday
  - `thismonth`: entries from the first day to the last day of this month
 
-The `--start` and `--end` tags can be used to define a specific time frame. The generated report will contain entries from the specified `--start` date, to the specified `--end` date. 
+The `--start` and `--end` tags can be used to define a specific time frame. Expects `YYYY-MM-DD` format, e.g. 2023-10-30. 
+
+The generated report will contain entries from the specified `--start` date, to the specified `--end` date.
+
 
 The `--end` tag is optional. If not specified, today's date will be used.
 
 **Default:** If no argument is specified, the report will contain only this week's time entries (Same behaviour as using `-p thisweek`).
 
 ## Report: SGU - Expected Toggl Data Structure
```

### Comparing `togglreports-2.5.0/README.md` & `togglreports-2.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
 The `--period` tag can be used to build reports with common start and end times. Possible values are: 
  - `today`: entries for today
  - `thisweek`: entries from the last sunday to the next saturday
  - `lastweek`: entries from past week, from sunday to saturday
  - `thismonth`: entries from the first day to the last day of this month
 
-The `--start` and `--end` tags can be used to define a specific time frame. The generated report will contain entries from the specified `--start` date, to the specified `--end` date. 
+The `--start` and `--end` tags can be used to define a specific time frame. Expects `YYYY-MM-DD` format, e.g. 2023-10-30. 
+
+The generated report will contain entries from the specified `--start` date, to the specified `--end` date.
+
 
 The `--end` tag is optional. If not specified, today's date will be used.
 
 **Default:** If no argument is specified, the report will contain only this week's time entries (Same behaviour as using `-p thisweek`).
 
 ## Report: SGU - Expected Toggl Data Structure
```

### Comparing `togglreports-2.5.0/setup.cfg` & `togglreports-2.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/build.py` & `togglreports-2.5.1/src/togglreports/build.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/cli_parser.py` & `togglreports-2.5.1/src/togglreports/cli_parser.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/config.py` & `togglreports-2.5.1/src/togglreports/config.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/core/app.py` & `togglreports-2.5.1/src/togglreports/core/app.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/core/plugin_loader.py` & `togglreports-2.5.1/src/togglreports/core/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/core/report_factory.py` & `togglreports-2.5.1/src/togglreports/core/report_factory.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/plugins/example.py` & `togglreports-2.5.1/src/togglreports/plugins/example.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/plugins/sgu.py` & `togglreports-2.5.1/src/togglreports/plugins/sgu.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     _base_data: list[dict]
     _base_config: dict
     _config: dict
 
     _default_filename: str = 'SGU_report'
     _file_format: str = 'csv'
-    _file_encoding: str = 'ansi'
+    _file_encoding: str = 'cp1252'
     _separator: str = ';'
 
     _default_ignore_tag: str = '<IGNORE>'
     _max_num_chars: int = 50
 
     def __init__(self, data: list[dict], base_config: dict, config: dict):
         self._base_data = data
```

### Comparing `togglreports-2.5.0/src/togglreports/togglapi.py` & `togglreports-2.5.1/src/togglreports/togglapi.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports/utils.py` & `togglreports-2.5.1/src/togglreports/utils.py`

 * *Files identical despite different names*

### Comparing `togglreports-2.5.0/src/togglreports.egg-info/PKG-INFO` & `togglreports-2.5.1/src/togglreports.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: togglreports
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple project to automate the creation of reports using the Toggl API.
 Home-page: https://github.com/ro-56/togglReports
 Author: Rodrigo Mendonça
 Author-email: rodrigogr.mendonca@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,18 @@
 
 The `--period` tag can be used to build reports with common start and end times. Possible values are: 
  - `today`: entries for today
  - `thisweek`: entries from the last sunday to the next saturday
  - `lastweek`: entries from past week, from sunday to saturday
  - `thismonth`: entries from the first day to the last day of this month
 
-The `--start` and `--end` tags can be used to define a specific time frame. The generated report will contain entries from the specified `--start` date, to the specified `--end` date. 
+The `--start` and `--end` tags can be used to define a specific time frame. Expects `YYYY-MM-DD` format, e.g. 2023-10-30. 
+
+The generated report will contain entries from the specified `--start` date, to the specified `--end` date.
+
 
 The `--end` tag is optional. If not specified, today's date will be used.
 
 **Default:** If no argument is specified, the report will contain only this week's time entries (Same behaviour as using `-p thisweek`).
 
 ## Report: SGU - Expected Toggl Data Structure
```

### Comparing `togglreports-2.5.0/src/togglreports.egg-info/SOURCES.txt` & `togglreports-2.5.1/src/togglreports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

