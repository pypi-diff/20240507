# Comparing `tmp/way2dssat-0.0.6.tar.gz` & `tmp/way2dssat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way2dssat-0.0.6.tar", last modified: Tue May  7 03:27:56 2024, max compression
+gzip compressed data, was "way2dssat-0.0.7.tar", last modified: Tue May  7 04:09:01 2024, max compression
```

## Comparing `way2dssat-0.0.6.tar` & `way2dssat-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.375572 way2dssat-0.0.6/
--rw-rw-rw-   0        0        0      667 2024-05-07 03:27:56.375572 way2dssat-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.242369 way2dssat-0.0.6/Way2DSSAT/
--rw-rw-rw-   0        0        0     4264 2024-05-07 03:15:55.000000 way2dssat-0.0.6/Way2DSSAT/WTH.py
--rw-rw-rw-   0        0        0       93 2024-05-07 03:13:16.000000 way2dssat-0.0.6/Way2DSSAT/__init__.py
--rw-rw-rw-   0        0        0     8080 2024-05-07 03:16:28.000000 way2dssat-0.0.6/Way2DSSAT/gssurgo2soil.py
--rw-rw-rw-   0        0        0     6920 2024-05-07 03:05:29.000000 way2dssat-0.0.6/Way2DSSAT/xfiles.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:27:56.375572 way2dssat-0.0.6/Way2DSSAT.egg-info/
--rw-rw-rw-   0        0        0      667 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 03:27:56.000000 way2dssat-0.0.6/Way2DSSAT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2024-05-07 03:15:53.000000 way2dssat-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 03:27:56.375572 way2dssat-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      481 2024-05-07 03:15:22.000000 way2dssat-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:01.207424 way2dssat-0.0.7/
+-rw-rw-rw-   0        0        0      688 2024-05-07 04:09:01.202281 way2dssat-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:01.161710 way2dssat-0.0.7/Way2DSSAT/
+-rw-rw-rw-   0        0        0     4264 2024-05-07 03:15:55.000000 way2dssat-0.0.7/Way2DSSAT/WTH.py
+-rw-rw-rw-   0        0        0       93 2024-05-07 03:13:16.000000 way2dssat-0.0.7/Way2DSSAT/__init__.py
+-rw-rw-rw-   0        0        0     8064 2024-05-07 03:48:38.000000 way2dssat-0.0.7/Way2DSSAT/gssurgo2soil.py
+-rw-rw-rw-   0        0        0     6920 2024-05-07 03:05:29.000000 way2dssat-0.0.7/Way2DSSAT/xfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-07 04:09:01.201146 way2dssat-0.0.7/Way2DSSAT.egg-info/
+-rw-rw-rw-   0        0        0      688 2024-05-07 04:09:01.000000 way2dssat-0.0.7/Way2DSSAT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-07 04:09:01.000000 way2dssat-0.0.7/Way2DSSAT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 04:09:01.000000 way2dssat-0.0.7/Way2DSSAT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 04:09:01.000000 way2dssat-0.0.7/Way2DSSAT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 04:09:01.000000 way2dssat-0.0.7/Way2DSSAT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2024-05-07 04:08:01.000000 way2dssat-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 04:09:01.207424 way2dssat-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      481 2024-05-07 03:15:22.000000 way2dssat-0.0.7/setup.py
```

### Comparing `way2dssat-0.0.6/PKG-INFO` & `way2dssat-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package to handle input DSSAT files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
+Requires-Dist: math
 
 ## README
 This is a package to handle DSSAT input and output files
```

### Comparing `way2dssat-0.0.6/Way2DSSAT/WTH.py` & `way2dssat-0.0.7/Way2DSSAT/WTH.py`

 * *Files identical despite different names*

### Comparing `way2dssat-0.0.6/Way2DSSAT/gssurgo2soil.py` & `way2dssat-0.0.7/Way2DSSAT/gssurgo2soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-    """
+"""
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
     ------
         path: string
             path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
             WC15Bar_DCP_0to5
@@ -30,21 +30,21 @@
     Example
     -------
             path = 'Username/pathtothecsv'
             A,B = ssurgo2soil(path)
         
    
           
-    """
+"""
 
 def SOL(path):
     
     import pandas
     import math
-    """
+"""
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
     ------
         path: string
             path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
             WC15Bar_DCP_0to5
@@ -74,15 +74,15 @@
     Example
     -------
             path = 'Username/pathtothecsv'
             A,B = ssurgo2soil(path)
         
    
           
-    """
+"""
     #Reading csv  
     
     df_soil = pandas.read_csv(path)
     #Returns list of columns not required with specific keyword
     # data from ssurgo contains columns suchas pct_Silt** which aren't required
     # Removing those columns form the dataframe
     # These have column name are duplicate of the required soil properties with additional pct in
```

### Comparing `way2dssat-0.0.6/Way2DSSAT/xfiles.py` & `way2dssat-0.0.7/Way2DSSAT/xfiles.py`

 * *Files identical despite different names*

### Comparing `way2dssat-0.0.6/Way2DSSAT.egg-info/PKG-INFO` & `way2dssat-0.0.7/Way2DSSAT.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.6
+Version: 0.0.7
 Summary: Package to handle input DSSAT files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
+Requires-Dist: math
 
 ## README
 This is a package to handle DSSAT input and output files
```

### Comparing `way2dssat-0.0.6/pyproject.toml` & `way2dssat-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
-dependencies = [ "pandas"]
+dependencies = [ "pandas","math"]
 name = "Way2DSSAT"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Manavjot", email="manavjotsingh97@gmail.com" },
 ]
 description = "Package to handle input DSSAT files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

