# Comparing `tmp/pvradar-0.0.1.tar.gz` & `tmp/pvradar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvradar-0.0.1.tar", last modified: Thu Jan 11 21:53:28 2024, max compression
+gzip compressed data, was "pvradar-0.0.2.tar", last modified: Tue May  7 20:14:16 2024, max compression
```

## Comparing `pvradar-0.0.1.tar` & `pvradar-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxr-xr-x   0 or         (501) staff       (20)        0 2024-01-11 21:53:28.744390 pvradar-0.0.1/
--rw-r--r--   0 or         (501) staff       (20)     1133 2024-01-11 21:42:05.000000 pvradar-0.0.1/LICENSE
--rw-r--r--   0 or         (501) staff       (20)      553 2024-01-11 21:53:28.744219 pvradar-0.0.1/PKG-INFO
--rw-r--r--   0 or         (501) staff       (20)      155 2024-01-11 21:46:51.000000 pvradar-0.0.1/README.md
-drwxr-xr-x   0 or         (501) staff       (20)        0 2024-01-11 21:53:28.743452 pvradar-0.0.1/pvradar/
--rw-r--r--   0 or         (501) staff       (20)       25 2024-01-11 21:24:50.000000 pvradar-0.0.1/pvradar/__init__.py
--rw-r--r--   0 or         (501) staff       (20)       87 2024-01-11 21:23:58.000000 pvradar-0.0.1/pvradar/constants.py
-drwxr-xr-x   0 or         (501) staff       (20)        0 2024-01-11 21:53:28.744058 pvradar-0.0.1/pvradar.egg-info/
--rw-r--r--   0 or         (501) staff       (20)      553 2024-01-11 21:53:28.000000 pvradar-0.0.1/pvradar.egg-info/PKG-INFO
--rw-r--r--   0 or         (501) staff       (20)      197 2024-01-11 21:53:28.000000 pvradar-0.0.1/pvradar.egg-info/SOURCES.txt
--rw-r--r--   0 or         (501) staff       (20)        1 2024-01-11 21:53:28.000000 pvradar-0.0.1/pvradar.egg-info/dependency_links.txt
--rw-r--r--   0 or         (501) staff       (20)        8 2024-01-11 21:53:28.000000 pvradar-0.0.1/pvradar.egg-info/top_level.txt
--rw-r--r--   0 or         (501) staff       (20)      485 2024-01-11 21:53:22.000000 pvradar-0.0.1/pyproject.toml
--rw-r--r--   0 or         (501) staff       (20)       38 2024-01-11 21:53:28.744422 pvradar-0.0.1/setup.cfg
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.711914 pvradar-0.0.2/
+-rw-r--r--   0 or         (501) staff       (20)     1133 2024-01-11 21:42:05.000000 pvradar-0.0.2/LICENSE
+-rw-r--r--   0 or         (501) staff       (20)      765 2024-05-07 20:14:16.711708 pvradar-0.0.2/PKG-INFO
+-rw-r--r--   0 or         (501) staff       (20)      324 2024-05-06 17:07:35.000000 pvradar-0.0.2/README.md
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.708764 pvradar-0.0.2/mixin/
+-rw-r--r--   0 or         (501) staff       (20)       78 2024-05-07 19:14:46.000000 pvradar-0.0.2/mixin/__init__.py
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.709080 pvradar-0.0.2/pvradar/
+-rw-r--r--   0 or         (501) staff       (20)       78 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/__init__.py
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.710301 pvradar-0.0.2/pvradar/sdk/
+-rw-r--r--   0 or         (501) staff       (20)      229 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/__init__.py
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.710716 pvradar-0.0.2/pvradar/sdk/client/
+-rw-r--r--   0 or         (501) staff       (20)     4006 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/client/Query.py
+-rw-r--r--   0 or         (501) staff       (20)     3214 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/client/SyncClient.py
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.711288 pvradar-0.0.2/pvradar/sdk/common/
+-rw-r--r--   0 or         (501) staff       (20)       22 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/common/constants.py
+-rw-r--r--   0 or         (501) staff       (20)      511 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/common/csv_utils.py
+-rw-r--r--   0 or         (501) staff       (20)      736 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/common/dd_types.py
+-rw-r--r--   0 or         (501) staff       (20)      567 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/common/exceptions.py
+-rw-r--r--   0 or         (501) staff       (20)     1198 2024-05-07 19:34:39.000000 pvradar-0.0.2/pvradar/sdk/sdk_facade.py
+drwxr-xr-x   0 or         (501) staff       (20)        0 2024-05-07 20:14:16.711485 pvradar-0.0.2/pvradar.egg-info/
+-rw-r--r--   0 or         (501) staff       (20)      765 2024-05-07 20:14:16.000000 pvradar-0.0.2/pvradar.egg-info/PKG-INFO
+-rw-r--r--   0 or         (501) staff       (20)      463 2024-05-07 20:14:16.000000 pvradar-0.0.2/pvradar.egg-info/SOURCES.txt
+-rw-r--r--   0 or         (501) staff       (20)        1 2024-05-07 20:14:16.000000 pvradar-0.0.2/pvradar.egg-info/dependency_links.txt
+-rw-r--r--   0 or         (501) staff       (20)       13 2024-05-07 20:14:16.000000 pvradar-0.0.2/pvradar.egg-info/requires.txt
+-rw-r--r--   0 or         (501) staff       (20)       25 2024-05-07 20:14:16.000000 pvradar-0.0.2/pvradar.egg-info/top_level.txt
+-rw-r--r--   0 or         (501) staff       (20)      632 2024-05-07 19:37:48.000000 pvradar-0.0.2/pyproject.toml
+-rw-r--r--   0 or         (501) staff       (20)       38 2024-05-07 20:14:16.711952 pvradar-0.0.2/setup.cfg
```

### Comparing `pvradar-0.0.1/LICENSE` & `pvradar-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pvradar-0.0.1/PKG-INFO` & `pvradar-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: pvradar
-Version: 0.0.1
+Version: 0.0.2
 Summary: constants and shared function for PVRADAR SDK and API client
 Author-email: Kostiantyn Pogorelov <kp@pvradar.com>
 Project-URL: homepage, https://pvradar.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: httpx
+
+This package contains constants and shared function for PVRADAR SDK and API client
 
 # Installation
 
 ```sh
 pip install pvradar
 ```
 
 # Usage
 
 ```python
-from pvradar import SECONDS_PER_HOUR
-print ('seconds in an hour:', SECONDS_PER_HOUR)
+import pvradar
+modeled_soiling = pvradar.sdk.get_soiling_ratio({
+    'location': { 'lat': 37.63, 'lon': -2.95 },
+    'period': { 'year': 2022 }})
+
+modeled_soiling.plot()
 ```
```

### Comparing `pvradar-0.0.1/pvradar.egg-info/PKG-INFO` & `pvradar-0.0.2/pvradar.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: pvradar
-Version: 0.0.1
+Version: 0.0.2
 Summary: constants and shared function for PVRADAR SDK and API client
 Author-email: Kostiantyn Pogorelov <kp@pvradar.com>
 Project-URL: homepage, https://pvradar.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: httpx
+
+This package contains constants and shared function for PVRADAR SDK and API client
 
 # Installation
 
 ```sh
 pip install pvradar
 ```
 
 # Usage
 
 ```python
-from pvradar import SECONDS_PER_HOUR
-print ('seconds in an hour:', SECONDS_PER_HOUR)
+import pvradar
+modeled_soiling = pvradar.sdk.get_soiling_ratio({
+    'location': { 'lat': 37.63, 'lon': -2.95 },
+    'period': { 'year': 2022 }})
+
+modeled_soiling.plot()
 ```
```

