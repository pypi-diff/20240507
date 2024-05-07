# Comparing `tmp/conway-polynomials-0.8.tar.gz` & `tmp/conway-polynomials-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conway-polynomials-0.8.tar", last modified: Sun Nov 26 23:04:46 2023, max compression
+gzip compressed data, was "conway-polynomials-0.9.tar", last modified: Sat Jan 13 03:17:07 2024, max compression
```

## Comparing `conway-polynomials-0.8.tar` & `conway-polynomials-0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 23:04:46.467705 conway-polynomials-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-11-26 23:04:40.000000 conway-polynomials-0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-26 23:04:40.000000 conway-polynomials-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-26 23:04:40.000000 conway-polynomials-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-11-26 23:04:40.000000 conway-polynomials-0.8/NEWS
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2023-11-26 23:04:46.467705 conway-polynomials-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-26 23:04:40.000000 conway-polynomials-0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-26 23:04:40.000000 conway-polynomials-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 23:04:46.467705 conway-polynomials-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 23:04:46.463705 conway-polynomials-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 23:04:46.467705 conway-polynomials-0.8/src/conway_polynomials/
--rw-r--r--   0 runner    (1001) docker     (127)  1053150 2023-11-26 23:04:40.000000 conway-polynomials-0.8/src/conway_polynomials/CPimport.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-26 23:04:40.000000 conway-polynomials-0.8/src/conway_polynomials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 23:04:46.467705 conway-polynomials-0.8/src/conway_polynomials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2023-11-26 23:04:46.000000 conway-polynomials-0.8/src/conway_polynomials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-26 23:04:46.000000 conway-polynomials-0.8/src/conway_polynomials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 23:04:46.000000 conway-polynomials-0.8/src/conway_polynomials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-26 23:04:46.000000 conway-polynomials-0.8/src/conway_polynomials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:17:07.349596 conway-polynomials-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-13 03:17:01.000000 conway-polynomials-0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-13 03:17:01.000000 conway-polynomials-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-13 03:17:01.000000 conway-polynomials-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-13 03:17:01.000000 conway-polynomials-0.9/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-01-13 03:17:07.349596 conway-polynomials-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-13 03:17:01.000000 conway-polynomials-0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-13 03:17:01.000000 conway-polynomials-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 03:17:07.349596 conway-polynomials-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-13 03:17:01.000000 conway-polynomials-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:17:07.345596 conway-polynomials-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:17:07.345596 conway-polynomials-0.9/src/conway_polynomials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1053150 2024-01-13 03:17:01.000000 conway-polynomials-0.9/src/conway_polynomials/CPimport.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-01-13 03:17:01.000000 conway-polynomials-0.9/src/conway_polynomials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 03:17:07.349596 conway-polynomials-0.9/src/conway_polynomials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-01-13 03:17:07.000000 conway-polynomials-0.9/src/conway_polynomials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-13 03:17:07.000000 conway-polynomials-0.9/src/conway_polynomials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 03:17:07.000000 conway-polynomials-0.9/src/conway_polynomials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-13 03:17:07.000000 conway-polynomials-0.9/src/conway_polynomials.egg-info/top_level.txt
```

### Comparing `conway-polynomials-0.8/COPYING` & `conway-polynomials-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `conway-polynomials-0.8/LICENSE` & `conway-polynomials-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `conway-polynomials-0.8/NEWS` & `conway-polynomials-0.9/NEWS`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+conway-polynomials-0.9 (2024-01-12)
+
+  * Support for pytest (just run "pytest").
+
+  * The database is now xz compressed during the "build."
+
+
 conway-polynomials-0.8 (2023-11-26)
 
   * Include LICENSE and COPYING in the distribution.
 
   * Fix an example in README.rst, and include README.rst in the
     example doctest command.
```

### Comparing `conway-polynomials-0.8/PKG-INFO` & `conway-polynomials-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conway-polynomials
-Version: 0.8
+Version: 0.9
 Summary: Python interface to Frank Lübeck's Conway polynomial database
 License: conway-polynomials - a python interface to Frank Lübeck's Conway polynomial database
         Copyright (C) 2023 The Sage Developers
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -98,7 +98,11 @@
 A few doctests within the module (and this README) ensure that
 everything is working. You can run them from the repository or from a
 release tarball using::
 
   PYTHONPATH=src python -m doctest \
     README.rst \
     src/conway_polynomials/__init__.py
+
+Or, if you have pytest installed, with simply::
+
+  pytest
```

### Comparing `conway-polynomials-0.8/README.rst` & `conway-polynomials-0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -62,7 +62,11 @@
 A few doctests within the module (and this README) ensure that
 everything is working. You can run them from the repository or from a
 release tarball using::
 
   PYTHONPATH=src python -m doctest \
     README.rst \
     src/conway_polynomials/__init__.py
+
+Or, if you have pytest installed, with simply::
+
+  pytest
```

### Comparing `conway-polynomials-0.8/pyproject.toml` & `conway-polynomials-0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conway-polynomials"
-version = "0.8"
+version = "0.9"
 description = "Python interface to Frank Lübeck's Conway polynomial database"
 readme = "README.rst"
 requires-python = ">=3.9"
 keywords = ["mathematics", "algebra", "Conway polynomials"]
 license = { file = "COPYING" }
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -23,7 +23,10 @@
 
 [project.urls]
 Homepage = "https://github.com/sagemath/conway-polynomials"
 Documentation = "https://github.com/sagemath/conway-polynomials/blob/master/README.rst"
 Repository = "https://github.com/sagemath/conway-polynomials.git"
 Issues = "https://github.com/sagemath/conway-polynomials/issues"
 Changelog = "https://github.com/sagemath/conway-polynomials/raw/master/NEWS"
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules --doctest-glob='*.rst'"
```

### Comparing `conway-polynomials-0.8/src/conway_polynomials/CPimport.txt` & `conway-polynomials-0.9/src/conway_polynomials/CPimport.txt`

 * *Files identical despite different names*

### Comparing `conway-polynomials-0.8/src/conway_polynomials/__init__.py` & `conway-polynomials-0.9/src/conway_polynomials/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 >>> len(cpdb[p][n]) == n + 1
 True
 >>> cpdb[p][n][n] == 1
 True
 
 """
 
+from typing import Optional, TextIO
+
 
 def _parse_line(l: str) -> tuple[int, int, tuple[int,...]]:
     r"""
     Parse a single line (not the first or the last) from Frank
     Lübeck's data file.
 
     According to Frank's webpage, each line has the form,
@@ -85,16 +87,46 @@
     # Convert everything to integers before returning.
     p = int(fields[0])
     n = int(fields[1])
     coeffs = tuple( int(c) for c in fields[2:] )
 
     return (p, n, coeffs)
 
+def _open_database() -> TextIO:
+    r"""
+    Open the database, possibly xz compressed.
+
+    Typically, the build/install process for the package will compress
+    the database and remove the uncompressed copy. During development,
+    however, it would be annoying to have to build/install the package
+    to a temporary location before the test suite could be run. For
+    that reason we retain the uncompressed filename as a fallback.
+
+    Returns
+    -------
+
+    file : TextIO
+      A file-like object, opened for reading in text mode, representing the
+      database.
+
+    """
+    import lzma
+    from importlib.resources import as_file, files
+    from io import TextIOWrapper
+
+    dbpath = files('conway_polynomials').joinpath('CPimport.txt')
+    with as_file(dbpath) as p:
+        try:
+            # Open as binary and wrap in TextIO to guarantee
+            # that the return type is correct.
+            return TextIOWrapper(lzma.open(p.with_suffix(".txt.xz")))
+        except FileNotFoundError:
+            return open(p, "r")
+
 
-from typing import Optional
 _conway_dict: Optional[ dict[int,dict[int,tuple[int,...]]] ]
 _conway_dict = None    # cached result of database()
 def database() -> dict[int,dict[int,tuple[int,...]]]:
     r"""
     Load (if necessary) and return a dict of pre-computed Conway
     polynomial coefficients.
 
@@ -113,17 +145,15 @@
     """
     global _conway_dict
 
     if _conway_dict is not None:
         return _conway_dict
 
     _conway_dict = {}
-    from importlib.resources import files
-    dbpath = files('conway_polynomials').joinpath('CPimport.txt')
-    with dbpath.open("r") as f:
+    with _open_database() as f:
         # The first line of the file is "allConwayPolynomials := ["
         f.readline()
 
         for line in f:
             if line[0] == "0":
                 # This is the last line in the file; otherwise it would
                 # start with a square bracket.
```

### Comparing `conway-polynomials-0.8/src/conway_polynomials.egg-info/PKG-INFO` & `conway-polynomials-0.9/src/conway_polynomials.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conway-polynomials
-Version: 0.8
+Version: 0.9
 Summary: Python interface to Frank Lübeck's Conway polynomial database
 License: conway-polynomials - a python interface to Frank Lübeck's Conway polynomial database
         Copyright (C) 2023 The Sage Developers
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -98,7 +98,11 @@
 A few doctests within the module (and this README) ensure that
 everything is working. You can run them from the repository or from a
 release tarball using::
 
   PYTHONPATH=src python -m doctest \
     README.rst \
     src/conway_polynomials/__init__.py
+
+Or, if you have pytest installed, with simply::
+
+  pytest
```

