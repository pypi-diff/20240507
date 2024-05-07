# Comparing `tmp/papers_dl-0.0.4.tar.gz` & `tmp/papers_dl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.4.tar", last modified: Sat May  4 19:22:27 2024, max compression
+gzip compressed data, was "papers_dl-0.0.5.tar", last modified: Tue May  7 19:27:27 2024, max compression
```

## Comparing `papers_dl-0.0.4.tar` & `papers_dl-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.048978 papers_dl-0.0.4/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.4/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     2450 2024-05-04 19:22:27.048654 papers_dl-0.0.4/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1131 2024-04-16 22:48:35.000000 papers_dl-0.0.4/README.md
--rw-r--r--   0 ben        (501) staff       (20)     1158 2024-05-04 19:21:22.000000 papers_dl-0.0.4/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-04 19:22:27.049041 papers_dl-0.0.4/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.046033 papers_dl-0.0.4/src/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.048227 papers_dl-0.0.4/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2450 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      318 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       23 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     3562 2024-05-04 19:19:41.000000 papers_dl-0.0.4/src/papers_dl.py
--rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.4/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.4/src/scihub.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.047929 papers_dl-0.0.4/tests/
--rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_cli.py
--rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_fetch.py
--rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_parse.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.596951 papers_dl-0.0.5/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.5/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-07 19:27:27.596624 papers_dl-0.0.5/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1296 2024-05-04 19:26:22.000000 papers_dl-0.0.5/README.md
+-rw-r--r--   0 ben        (501) staff       (20)     1206 2024-05-07 19:25:50.000000 papers_dl-0.0.5/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-07 19:27:27.597014 papers_dl-0.0.5/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.593840 papers_dl-0.0.5/src/
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.5/src/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.596167 papers_dl-0.0.5/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      374 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       32 2024-05-07 19:27:27.000000 papers_dl-0.0.5/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3562 2024-05-04 19:19:41.000000 papers_dl-0.0.5/src/papers_dl.py
+-rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.5/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.5/src/scihub.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-07 19:27:27.595889 papers_dl-0.0.5/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_cli.py
+-rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_fetch.py
+-rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.5/tests/test_parse.py
```

### Comparing `papers_dl-0.0.4/LICENSE` & `papers_dl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/PKG-INFO` & `papers_dl-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,44 +38,48 @@
 Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```
-usage: papers-dl.py [-h] {fetch,parse} ...
+usage: papers_dl.py [-h] {fetch,parse} ...
 
 Download scientific papers from the command line
 
 positional arguments:
   {fetch,parse}
-    fetch        try to download a paper from the given
-                 query
+    fetch        try to download a paper with the given identifier
     parse        parse identifiers from a file
 
 options:
-  -h, --help     show this help message and exit
-  
+  -h, --help     show this help message and exit  
+
 # fetch
-usage: papers-dl.py fetch [-h] [-o path] (DOI|PMID|URL)
+usage: papers_dl.py fetch [-h] [-o path] [-A USER_AGENT]
+                          (DOI|PMID|URL)
 
 positional arguments:
   (DOI|PMID|URL)        the identifier to try to download
 
 options:
   -h, --help            show this help message and exit
   -o path, --output path
-                        optional output directory for
-                        downloaded papers
+                        optional output directory for downloaded
+                        papers
+  -A USER_AGENT, --user-agent USER_AGENT
 
 # parse
-usage: papers-dl.py parse [-h] [-m type] path
+usage: papers_dl.py parse [-h] [-m type] [-f [fmt]] path
 
 positional arguments:
   path                  the path of the file to parse
 
 options:
   -h, --help            show this help message and exit
   -m type, --match type
                         the type of identifier to match
+  -f [fmt], --format [fmt]
+                        the output format for printing
 ```
-This project includes a modified version of [scihub.py](https://github.com/zaytoun/scihub.py).
+
+This project started as a impromptu fork of [scihub.py](https://github.com/zaytoun/scihub.py).
```

### Comparing `papers_dl-0.0.4/README.md` & `papers_dl-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```
-usage: papers-dl.py [-h] {fetch,parse} ...
+usage: papers_dl.py [-h] {fetch,parse} ...
 
 Download scientific papers from the command line
 
 positional arguments:
   {fetch,parse}
-    fetch        try to download a paper from the given
-                 query
+    fetch        try to download a paper with the given identifier
     parse        parse identifiers from a file
 
 options:
-  -h, --help     show this help message and exit
-  
+  -h, --help     show this help message and exit  
+
 # fetch
-usage: papers-dl.py fetch [-h] [-o path] (DOI|PMID|URL)
+usage: papers_dl.py fetch [-h] [-o path] [-A USER_AGENT]
+                          (DOI|PMID|URL)
 
 positional arguments:
   (DOI|PMID|URL)        the identifier to try to download
 
 options:
   -h, --help            show this help message and exit
   -o path, --output path
-                        optional output directory for
-                        downloaded papers
+                        optional output directory for downloaded
+                        papers
+  -A USER_AGENT, --user-agent USER_AGENT
 
 # parse
-usage: papers-dl.py parse [-h] [-m type] path
+usage: papers_dl.py parse [-h] [-m type] [-f [fmt]] path
 
 positional arguments:
   path                  the path of the file to parse
 
 options:
   -h, --help            show this help message and exit
   -m type, --match type
                         the type of identifier to match
+  -f [fmt], --format [fmt]
+                        the output format for printing
 ```
-This project includes a modified version of [scihub.py](https://github.com/zaytoun/scihub.py).
+
+This project started as a impromptu fork of [scihub.py](https://github.com/zaytoun/scihub.py).
```

### Comparing `papers_dl-0.0.4/pyproject.toml` & `papers_dl-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "papers-dl"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ben Muthalaly", email="benmuthalaly@gmail.com" },
 ]
 description = "A command line application for downloading scientific papers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -40,10 +40,13 @@
   "sgmllib3k==1.0.0",
   "six==1.16.0",
   "soupsieve==2.5",
   "urllib3==2.2.1",
   "w3lib==2.1.2",
 ]
 
+[project.scripts]
+papers-dl = "papers_dl:main"
+
 [project.urls]
 Homepage = "https://github.com/benmuth/papers-dl"
 Issues = "https://github.com/benmuth/papers-dl/issues"
```

### Comparing `papers_dl-0.0.4/src/papers_dl.egg-info/PKG-INFO` & `papers_dl-0.0.5/src/papers_dl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,44 +38,48 @@
 Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```
-usage: papers-dl.py [-h] {fetch,parse} ...
+usage: papers_dl.py [-h] {fetch,parse} ...
 
 Download scientific papers from the command line
 
 positional arguments:
   {fetch,parse}
-    fetch        try to download a paper from the given
-                 query
+    fetch        try to download a paper with the given identifier
     parse        parse identifiers from a file
 
 options:
-  -h, --help     show this help message and exit
-  
+  -h, --help     show this help message and exit  
+
 # fetch
-usage: papers-dl.py fetch [-h] [-o path] (DOI|PMID|URL)
+usage: papers_dl.py fetch [-h] [-o path] [-A USER_AGENT]
+                          (DOI|PMID|URL)
 
 positional arguments:
   (DOI|PMID|URL)        the identifier to try to download
 
 options:
   -h, --help            show this help message and exit
   -o path, --output path
-                        optional output directory for
-                        downloaded papers
+                        optional output directory for downloaded
+                        papers
+  -A USER_AGENT, --user-agent USER_AGENT
 
 # parse
-usage: papers-dl.py parse [-h] [-m type] path
+usage: papers_dl.py parse [-h] [-m type] [-f [fmt]] path
 
 positional arguments:
   path                  the path of the file to parse
 
 options:
   -h, --help            show this help message and exit
   -m type, --match type
                         the type of identifier to match
+  -f [fmt], --format [fmt]
+                        the output format for printing
 ```
-This project includes a modified version of [scihub.py](https://github.com/zaytoun/scihub.py).
+
+This project started as a impromptu fork of [scihub.py](https://github.com/zaytoun/scihub.py).
```

### Comparing `papers_dl-0.0.4/src/papers_dl.py` & `papers_dl-0.0.5/src/papers_dl.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/src/parse.py` & `papers_dl-0.0.5/src/parse.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/src/scihub.py` & `papers_dl-0.0.5/src/scihub.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/tests/test_cli.py` & `papers_dl-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/tests/test_fetch.py` & `papers_dl-0.0.5/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.4/tests/test_parse.py` & `papers_dl-0.0.5/tests/test_parse.py`

 * *Files identical despite different names*

