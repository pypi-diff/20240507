# Comparing `tmp/henry-temp-fix-0.3.3.tar.gz` & `tmp/henry-temp-fix-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henry-temp-fix-0.3.3.tar", last modified: Thu Apr 11 15:39:33 2024, max compression
+gzip compressed data, was "henry-temp-fix-0.3.4.tar", last modified: Tue May  7 14:48:38 2024, max compression
```

## Comparing `henry-temp-fix-0.3.3.tar` & `henry-temp-fix-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,29 @@
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.485415 henry-temp-fix-0.3.3/
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     1106 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/LICENSE.txt
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-11 15:39:33.481415 henry-temp-fix-0.3.3/PKG-INFO
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)    13971 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/README.md
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.477415 henry-temp-fix-0.3.3/henry/
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.477415 henry-temp-fix-0.3.3/henry/.support_files/
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     2239 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/.support_files/help.rtf
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/__init__.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       22 2024-04-11 15:39:29.000000 henry-temp-fix-0.3.3/henry/__version__.py
--rwxr-x---   0 rbobrowski (924420) primarygroup (89939)     7242 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/cli.py
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.477415 henry-temp-fix-0.3.3/henry/commands/
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/commands/__init__.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4330 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/commands/analyze.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     6830 2024-04-10 16:56:17.000000 henry-temp-fix-0.3.3/henry/commands/pulse.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     2163 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/commands/vacuum.py
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.481415 henry-temp-fix-0.3.3/henry/modules/
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/modules/__init__.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/modules/exceptions.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)    16532 2024-04-11 15:38:01.000000 henry-temp-fix-0.3.3/henry/modules/fetcher.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)      758 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/henry/modules/spinner.py
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.481415 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/
--rw-r--r--   0 rbobrowski (924420) primarygroup (89939)    14387 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/PKG-INFO
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)      631 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/SOURCES.txt
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)        1 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/dependency_links.txt
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       41 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/entry_points.txt
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       24 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/requires.txt
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       35 2024-04-11 15:39:33.000000 henry-temp-fix-0.3.3/henry_temp_fix.egg-info/top_level.txt
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)       38 2024-04-11 15:39:33.485415 henry-temp-fix-0.3.3/setup.cfg
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)      887 2024-04-10 18:29:44.000000 henry-temp-fix-0.3.3/setup.py
-drwxr-x---   0 rbobrowski (924420) primarygroup (89939)        0 2024-04-11 15:39:33.481415 henry-temp-fix-0.3.3/tests/
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4252 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/tests/test_analyze.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)      739 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/tests/test_cli.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)    10927 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/tests/test_fetcher.py
--rw-r-----   0 rbobrowski (924420) primarygroup (89939)     4877 2024-04-10 16:36:47.000000 henry-temp-fix-0.3.3/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.760506 henry-temp-fix-0.3.4/henry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.760506 henry-temp-fix-0.3.4/henry/.support_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/.support_files/help.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7242 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/henry/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/commands/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/commands/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/commands/vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/henry/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/modules/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16532 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/modules/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/henry/modules/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 14:48:38.000000 henry-temp-fix-0.3.4/henry_temp_fix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:48:38.764505 henry-temp-fix-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 14:48:36.000000 henry-temp-fix-0.3.4/setup.py
```

### Comparing `henry-temp-fix-0.3.3/LICENSE.txt` & `henry-temp-fix-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/PKG-INFO` & `henry-temp-fix-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: henry-temp-fix
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Looker Cleanup Tool (Temp Fix Version)
 Home-page: https://pypi.python.org/pypi/henry
 Author: Ryan Bobrowski
 Author-email: rbobrowski@google.com
 License: MIT
 Keywords: Looker Cleanup,Looker Henry,Henry
+Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: looker-sdk>=21
-Requires-Dist: tabulate
 
 ![image](https://github.com/looker-open-source/henry/blob/master/doc/logo/logo.png?raw=true)
 
 ---
 
 # Henry: A Looker Cleanup Tool
 
@@ -270,7 +269,9 @@
 Everyone interacting in the Henry project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/looker-open-source/henry/blob/master/CODE_OF_CONDUCT.md).
 
 <a name="copyright"></a>
 
 ## Copyright
 
 Copyright (c) 2018 Joseph Axisa for Looker Data Sciences. See [MIT License](LICENSE.txt) for further details.
+
+
```

### Comparing `henry-temp-fix-0.3.3/README.md` & `henry-temp-fix-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/.support_files/help.rtf` & `henry-temp-fix-0.3.4/henry/.support_files/help.rtf`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/cli.py` & `henry-temp-fix-0.3.4/henry/cli.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/commands/analyze.py` & `henry-temp-fix-0.3.4/henry/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/commands/pulse.py` & `henry-temp-fix-0.3.4/henry/commands/pulse.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         pulse.check_legacy_features()
 
     @spinner.Spinner()
     def check_db_connections(self):
         """Gets all db connections and runs all supported tests against them."""
         print("\bTest 1/6: Checking connections")
 
-        reserved_names = ["looker__internal__analytics", "looker", "looker__ilooker"]
+        reserved_names = ["looker__internal__analytics__replica", "looker__internal__analytics", "looker", "looker__ilooker"]
         db_connections: Sequence[models.DBConnection] = list(
             filter(lambda c: c.name not in reserved_names, self.sdk.all_connections())
         )
 
         if not db_connections:
             raise exceptions.NotFoundError("No connections found.")
```

### Comparing `henry-temp-fix-0.3.3/henry/commands/vacuum.py` & `henry-temp-fix-0.3.4/henry/commands/vacuum.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/modules/fetcher.py` & `henry-temp-fix-0.3.4/henry/modules/fetcher.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry/modules/spinner.py` & `henry-temp-fix-0.3.4/henry/modules/spinner.py`

 * *Files identical despite different names*

### Comparing `henry-temp-fix-0.3.3/henry_temp_fix.egg-info/PKG-INFO` & `henry-temp-fix-0.3.4/henry_temp_fix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: henry-temp-fix
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Looker Cleanup Tool (Temp Fix Version)
 Home-page: https://pypi.python.org/pypi/henry
 Author: Ryan Bobrowski
 Author-email: rbobrowski@google.com
 License: MIT
 Keywords: Looker Cleanup,Looker Henry,Henry
+Platform: UNKNOWN
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: looker-sdk>=21
-Requires-Dist: tabulate
 
 ![image](https://github.com/looker-open-source/henry/blob/master/doc/logo/logo.png?raw=true)
 
 ---
 
 # Henry: A Looker Cleanup Tool
 
@@ -270,7 +269,9 @@
 Everyone interacting in the Henry project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](https://github.com/looker-open-source/henry/blob/master/CODE_OF_CONDUCT.md).
 
 <a name="copyright"></a>
 
 ## Copyright
 
 Copyright (c) 2018 Joseph Axisa for Looker Data Sciences. See [MIT License](LICENSE.txt) for further details.
+
+
```

### Comparing `henry-temp-fix-0.3.3/henry_temp_fix.egg-info/SOURCES.txt` & `henry-temp-fix-0.3.4/henry_temp_fix.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,12 +14,8 @@
 henry/modules/fetcher.py
 henry/modules/spinner.py
 henry_temp_fix.egg-info/PKG-INFO
 henry_temp_fix.egg-info/SOURCES.txt
 henry_temp_fix.egg-info/dependency_links.txt
 henry_temp_fix.egg-info/entry_points.txt
 henry_temp_fix.egg-info/requires.txt
-henry_temp_fix.egg-info/top_level.txt
-tests/test_analyze.py
-tests/test_cli.py
-tests/test_fetcher.py
-tests/test_vacuum.py
+henry_temp_fix.egg-info/top_level.txt
```

### Comparing `henry-temp-fix-0.3.3/setup.py` & `henry-temp-fix-0.3.4/setup.py`

 * *Files identical despite different names*

