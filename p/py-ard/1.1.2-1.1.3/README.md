# Comparing `tmp/py-ard-1.1.2.tar.gz` & `tmp/py-ard-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.1.2.tar", last modified: Fri Mar 22 21:14:28 2024, max compression
+gzip compressed data, was "py-ard-1.1.3.tar", last modified: Tue May  7 20:57:12 2024, max compression
```

## Comparing `py-ard-1.1.2.tar` & `py-ard-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:14:28.476371 py-ard-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-22 21:14:15.000000 py-ard-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-22 21:14:15.000000 py-ard-1.1.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-22 21:14:15.000000 py-ard-1.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-22 21:14:15.000000 py-ard-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-22 21:14:15.000000 py-ard-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-03-22 21:14:28.476371 py-ard-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-03-22 21:14:15.000000 py-ard-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:14:28.472371 py-ard-1.1.2/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 21:14:28.000000 py-ard-1.1.2/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:14:28.476371 py-ard-1.1.2/pyard/
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37971 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/serology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-22 21:14:15.000000 py-ard-1.1.2/pyard/smart_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 21:14:15.000000 py-ard-1.1.2/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 21:14:15.000000 py-ard-1.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:14:28.476371 py-ard-1.1.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-03-22 21:14:15.000000 py-ard-1.1.2/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-03-22 21:14:15.000000 py-ard-1.1.2/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-03-22 21:14:15.000000 py-ard-1.1.2/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-03-22 21:14:15.000000 py-ard-1.1.2/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-22 21:14:28.480371 py-ard-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-22 21:14:15.000000 py-ard-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-07 20:57:03.000000 py-ard-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-07 20:57:03.000000 py-ard-1.1.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 20:57:03.000000 py-ard-1.1.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 20:57:03.000000 py-ard-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 20:57:03.000000 py-ard-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-05-07 20:57:12.710717 py-ard-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-05-07 20:57:03.000000 py-ard-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.706717 py-ard-1.1.3/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/pyard/
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38295 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/serology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 20:57:03.000000 py-ard-1.1.3/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:57:03.000000 py-ard-1.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:57:12.710717 py-ard-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-07 20:57:03.000000 py-ard-1.1.3/setup.py
```

### Comparing `py-ard-1.1.2/CONTRIBUTING.rst` & `py-ard-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/COPYING` & `py-ard-1.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/LICENSE` & `py-ard-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/PKG-INFO` & `py-ard-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.1.2
+Version: 1.1.3
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.1.2/README.md` & `py-ard-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/py_ard.egg-info/PKG-INFO` & `py-ard-1.1.3/py_ard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.1.2
+Version: 1.1.3
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
```

### Comparing `py-ard-1.1.2/py_ard.egg-info/SOURCES.txt` & `py-ard-1.1.3/py_ard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/CWD2.csv` & `py-ard-1.1.3/pyard/CWD2.csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/__init__.py` & `py-ard-1.1.3/pyard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #    > http://www.opensource.org/licenses/lgpl-license.php
 #
 from .blender import blender as dr_blender
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.1.2/pyard/ard.py` & `py-ard-1.1.3/pyard/ard.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,16 +254,23 @@
                 if last_char in expression_chars:
                     exon_short_null_allele = exon_group_allele + last_char
                     if self.is_shortnull(exon_short_null_allele):
                         return exon_short_null_allele
 
                 return exon_group_allele
             else:
-                # for 'exon' return allele with only first 3 fields
-                return ":".join(allele.split(":")[0:3])
+                # Expand to W level and then reduce to exon
+                w_redux = self.redux(allele, "W")
+                # If the W redux produces 2 field allele or the same allele,
+                # don't recurse
+                if w_redux == allele or len(w_redux.split(":")) == 2:
+                    return allele
+                else:
+                    # recurse with the W fields
+                    return self.redux(w_redux, "exon")
         elif redux_type == "U2":
             allele_fields = allele.split(":")
             # If resolved out to second field leave alone
             if len(allele_fields) == 2:
                 return allele
             # If the 2 field reduction is unambiguous, reduce to 2 field level
             allele_2_fields = get_n_field_allele(allele, 2, preserve_expression=True)
```

### Comparing `py-ard-1.1.2/pyard/blender.py` & `py-ard-1.1.3/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/constants.py` & `py-ard-1.1.3/pyard/constants.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/data_repository.py` & `py-ard-1.1.3/pyard/data_repository.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/db.py` & `py-ard-1.1.3/pyard/db.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/drbx.py` & `py-ard-1.1.3/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/exceptions.py` & `py-ard-1.1.3/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/load.py` & `py-ard-1.1.3/pyard/load.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/mappings.py` & `py-ard-1.1.3/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/misc.py` & `py-ard-1.1.3/pyard/misc.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/serology.py` & `py-ard-1.1.3/pyard/serology.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/pyard/smart_sort.py` & `py-ard-1.1.3/pyard/smart_sort.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/scripts/pyard` & `py-ard-1.1.3/scripts/pyard`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/scripts/pyard-import` & `py-ard-1.1.3/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/scripts/pyard-reduce-csv` & `py-ard-1.1.3/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/scripts/pyard-status` & `py-ard-1.1.3/scripts/pyard-status`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.2/setup.cfg` & `py-ard-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.2
+current_version = 1.1.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.1.2/setup.py` & `py-ard-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.1.2",
+    version="1.1.3",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

