# Comparing `tmp/verify_import-0.1.0.tar.gz` & `tmp/verify_import-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify_import-0.1.0.tar", last modified: Tue May  7 13:13:13 2024, max compression
+gzip compressed data, was "verify_import-0.1.1.tar", last modified: Tue May  7 13:14:24 2024, max compression
```

## Comparing `verify_import-0.1.0.tar` & `verify_import-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:13:13.242426 verify_import-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-07 13:13:13.242426 verify_import-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-07 13:12:10.000000 verify_import-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-07 13:13:04.000000 verify_import-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:13:13.252426 verify_import-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:13:13.242426 verify_import-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:13:13.242426 verify_import-0.1.0/src/import_checker/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      182 2024-05-07 13:05:41.000000 verify_import-0.1.0/src/import_checker/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-05-07 13:10:54.000000 verify_import-0.1.0/src/import_checker/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-05-07 13:11:33.000000 verify_import-0.1.0/src/import_checker/cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      551 2024-05-07 13:10:26.000000 verify_import-0.1.0/src/import_checker/errors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:13:13.242426 verify_import-0.1.0/src/verify_import.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      390 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-07 13:13:13.000000 verify_import-0.1.0/src/verify_import.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:14:24.962426 verify_import-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-07 13:14:24.962426 verify_import-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      204 2024-05-07 13:12:10.000000 verify_import-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      534 2024-05-07 13:14:22.000000 verify_import-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-07 13:14:24.962426 verify_import-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:14:24.962426 verify_import-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:14:24.962426 verify_import-0.1.1/src/verify_import/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      182 2024-05-07 13:13:56.000000 verify_import-0.1.1/src/verify_import/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       58 2024-05-07 13:14:08.000000 verify_import-0.1.1/src/verify_import/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-05-07 13:13:44.000000 verify_import-0.1.1/src/verify_import/cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      551 2024-05-07 13:10:26.000000 verify_import-0.1.1/src/verify_import/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-07 13:14:24.962426 verify_import-0.1.1/src/verify_import.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      384 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-07 13:14:24.000000 verify_import-0.1.1/src/verify_import.egg-info/top_level.txt
```

### Comparing `verify_import-0.1.0/PKG-INFO` & `verify_import-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify-import
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple tool to verify all submodules import without error
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/codegen.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
```

### Comparing `verify_import-0.1.0/pyproject.toml` & `verify_import-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verify-import"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tool to verify all submodules import without error"
 dependencies = [
   "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/marciclabas/codegen.git"
 
 [project.scripts]
-import-checker = "import_checker.cli:main"
+verify-import = "verify_import.cli:main"
```

### Comparing `verify_import-0.1.0/src/import_checker/cli.py` & `verify_import-0.1.1/src/verify_import/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def main():
   parser = argparse.ArgumentParser(description='Import Checker')
   parser.add_argument('PKG', help='Module/package to verify')
   parser.add_argument('-v', '--verbose', action='store_true', help='Verbose output')
 
   args = parser.parse_args()
-  from import_checker import walk_modules
+  from verify_import import walk_modules
   errored = False
   for pkg, e in walk_modules(args.PKG):
     if e is not None:
       print(f"ERROR importing '{pkg}':", e)
       errored = True
     elif args.verbose:
       print(f"Imported '{pkg}'")
```

### Comparing `verify_import-0.1.0/src/import_checker/errors.py` & `verify_import-0.1.1/src/verify_import/main.py`

 * *Files identical despite different names*

### Comparing `verify_import-0.1.0/src/verify_import.egg-info/PKG-INFO` & `verify_import-0.1.1/src/verify_import.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify-import
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple tool to verify all submodules import without error
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/codegen.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
```

