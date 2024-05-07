# Comparing `tmp/sprocketship-1.0.3.tar.gz` & `tmp/sprocketship-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-1.0.3.tar", last modified: Tue May  7 16:01:18 2024, max compression
+gzip compressed data, was "sprocketship-1.0.4.tar", last modified: Tue May  7 16:44:08 2024, max compression
```

## Comparing `sprocketship-1.0.3.tar` & `sprocketship-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 16:01:14.000000 sprocketship-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 16:01:14.000000 sprocketship-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:01:18.380092 sprocketship-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 16:01:14.000000 sprocketship-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 16:01:14.000000 sprocketship-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:01:18.380092 sprocketship-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.376092 sprocketship-1.0.3/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-07 16:01:14.000000 sprocketship-1.0.3/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:01:18.380092 sprocketship-1.0.3/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 16:01:18.000000 sprocketship-1.0.3/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:44:08.700096 sprocketship-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 16:43:55.000000 sprocketship-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 16:43:55.000000 sprocketship-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:44:08.700096 sprocketship-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 16:43:55.000000 sprocketship-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 16:43:55.000000 sprocketship-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:44:08.700096 sprocketship-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:44:08.696096 sprocketship-1.0.4/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-07 16:43:55.000000 sprocketship-1.0.4/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:44:08.700096 sprocketship-1.0.4/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 16:43:55.000000 sprocketship-1.0.4/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-07 16:43:55.000000 sprocketship-1.0.4/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:44:08.700096 sprocketship-1.0.4/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 16:44:08.000000 sprocketship-1.0.4/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-1.0.3/LICENSE` & `sprocketship-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.3/PKG-INFO` & `sprocketship-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 1.0.3
+Version: 1.0.4
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.3 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.4 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

### Comparing `sprocketship-1.0.3/README.md` & `sprocketship-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.3/pyproject.toml` & `sprocketship-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-1.0.3/sprocketship/cli.py` & `sprocketship-1.0.4/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.3/sprocketship/utils.py` & `sprocketship-1.0.4/sprocketship/utils.py`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.3/sprocketship.egg-info/PKG-INFO` & `sprocketship-1.0.4/sprocketship.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 1.0.3
+Version: 1.0.4
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.3 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.4 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
```

