# Comparing `tmp/verify_import-0.1.2.tar.gz` & `tmp/verify_import-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify_import-0.1.2.tar", last modified: Tue May  7 13:26:43 2024, max compression
+gzip compressed data, was "verify_import-0.1.3.tar", last modified: Tue May  7 13:29:45 2024, max compression
```

## Comparing `verify_import-0.1.2.tar` & `verify_import-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:26:43.872405 verify_import-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      557 2024-05-07 13:26:43.872405 verify_import-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-07 13:12:10.000000 verify_import-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-05-07 13:26:41.000000 verify_import-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:26:43.872405 verify_import-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:26:43.862405 verify_import-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:26:43.872405 verify_import-0.1.2/src/verify_import/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      182 2024-05-07 13:13:56.000000 verify_import-0.1.2/src/verify_import/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-07 13:14:08.000000 verify_import-0.1.2/src/verify_import/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      742 2024-05-07 13:26:12.000000 verify_import-0.1.2/src/verify_import/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      551 2024-05-07 13:10:26.000000 verify_import-0.1.2/src/verify_import/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:26:43.872405 verify_import-0.1.2/src/verify_import.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      557 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      384 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-07 13:26:43.000000 verify_import-0.1.2/src/verify_import.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:29:45.382414 verify_import-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-05-07 13:29:45.382414 verify_import-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-07 13:12:10.000000 verify_import-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-05-07 13:29:42.000000 verify_import-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:29:45.382414 verify_import-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:29:45.372414 verify_import-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:29:45.382414 verify_import-0.1.3/src/verify_import/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      182 2024-05-07 13:13:56.000000 verify_import-0.1.3/src/verify_import/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-07 13:14:08.000000 verify_import-0.1.3/src/verify_import/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      742 2024-05-07 13:26:12.000000 verify_import-0.1.3/src/verify_import/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      551 2024-05-07 13:10:26.000000 verify_import-0.1.3/src/verify_import/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:29:45.382414 verify_import-0.1.3/src/verify_import.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      384 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-07 13:29:45.000000 verify_import-0.1.3/src/verify_import.egg-info/top_level.txt
```

### Comparing `verify_import-0.1.2/PKG-INFO` & `verify_import-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: verify-import
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple tool to verify all submodules import without error
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/codegen.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
-Requires-Dist: dslog
+Requires-Dist: dslog[rich]
 
 # Import Checker
 
 > Simple tool to verify all submodules import without error
 
 ## Usage
```

### Comparing `verify_import-0.1.2/pyproject.toml` & `verify_import-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verify-import"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tool to verify all submodules import without error"
 dependencies = [
-  "lazy-loader", "dslog"
+  "lazy-loader", "dslog[rich]"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/codegen.git"
```

### Comparing `verify_import-0.1.2/src/verify_import/cli.py` & `verify_import-0.1.3/src/verify_import/cli.py`

 * *Files identical despite different names*

### Comparing `verify_import-0.1.2/src/verify_import/main.py` & `verify_import-0.1.3/src/verify_import/main.py`

 * *Files identical despite different names*

### Comparing `verify_import-0.1.2/src/verify_import.egg-info/PKG-INFO` & `verify_import-0.1.3/src/verify_import.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: verify-import
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple tool to verify all submodules import without error
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/codegen.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
-Requires-Dist: dslog
+Requires-Dist: dslog[rich]
 
 # Import Checker
 
 > Simple tool to verify all submodules import without error
 
 ## Usage
```

