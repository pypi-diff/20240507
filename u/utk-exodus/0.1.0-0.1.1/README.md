# Comparing `tmp/utk_exodus-0.1.0.tar.gz` & `tmp/utk_exodus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.0.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.1.tar", max compression
```

## Comparing `utk_exodus-0.1.0.tar` & `utk_exodus-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1379 2024-05-01 13:05:37.349327 utk_exodus-0.1.0/README.md
--rw-r--r--   0        0        0      485 2024-05-06 16:39:05.980578 utk_exodus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      182 2024-05-05 21:08:12.642357 utk_exodus-0.1.0/utk_exodus/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-06 17:17:45.477547 utk_exodus-0.1.0/utk_exodus/exodus.py
--rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.0/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.0/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      355 2024-05-05 21:08:12.642568 utk_exodus-0.1.0/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.0/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.0/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    39221 2024-05-06 17:40:03.297262 utk_exodus-0.1.0/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.0/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0     7674 2024-05-01 12:51:59.027899 utk_exodus-0.1.0/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 utk_exodus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1918 2024-05-07 19:02:36.432909 utk_exodus-0.1.1/README.md
+-rw-r--r--   0        0        0      485 2024-05-07 18:57:02.531468 utk_exodus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      291 2024-05-07 18:16:58.420598 utk_exodus-0.1.1/utk_exodus/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.1/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3413 2024-05-07 18:16:58.418021 utk_exodus-0.1.1/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     4179 2024-05-07 18:51:15.729586 utk_exodus-0.1.1/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.1/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.1/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.1/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.1/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.1/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    39221 2024-05-06 19:12:21.699513 utk_exodus-0.1.1/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.1/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0     7674 2024-05-01 12:51:59.027899 utk_exodus-0.1.1/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.1/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6232 2024-05-07 15:31:28.330943 utk_exodus-0.1.1/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     2558 1970-01-01 00:00:00.000000 utk_exodus-0.1.1/PKG-INFO
```

### Comparing `utk_exodus-0.1.0/utk_exodus/finder/finder.py` & `utk_exodus-0.1.1/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.0/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.1/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.0/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.1/utk_exodus/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.0/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.1/utk_exodus/risearch/risearch.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.0/PKG-INFO` & `utk_exodus-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utk-exodus
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.4.2,<25.0.0)
@@ -22,14 +22,45 @@
 
 ## About
 
 This application is a complete rewrite of the code used to migrate UTK content from Islandora 7 to Hyku.
 
 Unlike the previous code, this aims to be more flexible, easier to understand, and easier to use as a whole.
 
+## Installing
+
+To install, simply:
+
+```shell
+pip install utk_exodus
+```
+
+## Using
+
+There are several interfaces for the application.
+
+If you want to get works and files, use:
+
+```shell
+exodus works_and_files --path /path/to/metadata -o /path/to/directory/to/store/files
+```
+
+If you just want works, use:
+
+```shell
+exodus works --path /path/to/metadata
+```
+
+If for some reason you need to create a files sheet for  works after the fact, use:
+
+```shell
+exodus add_files --sheet path/to/sheet.csv --files_sheet path/to/files_sheet.csv 
+```
+
+
 ## Understanding Configs
 
 Exodus uses `yml` files for migration.  By default, exodus treats everything agnostically and relies on the `xpaths` 
 section of the base mapping to determine how a concept is mapped. If a property (or properties) have complex rules, a 
 class can be written to handle the special case.  When this happens, the `yml` should have a `special` property, and 
 it should be defined in `MetadataMapping().__lookup_special_property()`.
```

