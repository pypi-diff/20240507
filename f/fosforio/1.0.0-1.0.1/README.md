# Comparing `tmp/fosforio-1.0.0.tar.gz` & `tmp/fosforio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosforio-1.0.0.tar", last modified: Tue May  7 08:58:39 2024, max compression
+gzip compressed data, was "fosforio-1.0.1.tar", last modified: Tue May  7 09:28:46 2024, max compression
```

## Comparing `fosforio-1.0.0.tar` & `fosforio-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:58:39.059999 fosforio-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11529 2024-05-07 08:58:39.059999 fosforio-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10850 2024-05-07 08:56:47.000000 fosforio-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:58:39.055999 fosforio-1.0.0/fosforio/
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3742 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/amazons3.py
--rw-r--r--   0 root         (0) root         (0)     3611 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/azure.py
--rw-r--r--   0 root         (0) root         (0)     1656 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/feature_store.py
--rw-r--r--   0 root         (0) root         (0)     8063 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/hive.py
--rw-r--r--   0 root         (0) root         (0)     4297 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/manager.py
--rw-r--r--   0 root         (0) root         (0)     4487 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/postgres.py
--rw-r--r--   0 root         (0) root         (0)    16439 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/refractio.py
--rw-r--r--   0 root         (0) root         (0)     4289 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/sftp.py
--rw-r--r--   0 root         (0) root         (0)     5937 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6331 2024-05-07 08:56:47.000000 fosforio-1.0.0/fosforio/sqlserver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 08:58:39.059999 fosforio-1.0.0/fosforio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11529 2024-05-07 08:58:39.000000 fosforio-1.0.0/fosforio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-07 08:58:39.000000 fosforio-1.0.0/fosforio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 08:58:39.000000 fosforio-1.0.0/fosforio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-07 08:58:39.000000 fosforio-1.0.0/fosforio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 08:58:39.000000 fosforio-1.0.0/fosforio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 08:58:39.059999 fosforio-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2028 2024-05-07 08:56:47.000000 fosforio-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:28:46.707297 fosforio-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11529 2024-05-07 09:28:46.707297 fosforio-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10850 2024-05-07 09:28:05.000000 fosforio-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:28:46.707297 fosforio-1.0.1/fosforio/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/amazons3.py
+-rw-r--r--   0 root         (0) root         (0)     3611 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/feature_store.py
+-rw-r--r--   0 root         (0) root         (0)    16439 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/fosforio.py
+-rw-r--r--   0 root         (0) root         (0)     8063 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/hive.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/manager.py
+-rw-r--r--   0 root         (0) root         (0)     4487 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     4289 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     5937 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2024-05-07 09:28:05.000000 fosforio-1.0.1/fosforio/sqlserver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 09:28:46.707297 fosforio-1.0.1/fosforio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11529 2024-05-07 09:28:46.000000 fosforio-1.0.1/fosforio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-07 09:28:46.000000 fosforio-1.0.1/fosforio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 09:28:46.000000 fosforio-1.0.1/fosforio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-07 09:28:46.000000 fosforio-1.0.1/fosforio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 09:28:46.000000 fosforio-1.0.1/fosforio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 09:28:46.707297 fosforio-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2028 2024-05-07 09:28:05.000000 fosforio-1.0.1/setup.py
```

### Comparing `fosforio-1.0.0/PKG-INFO` & `fosforio-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosforio
-Version: 1.0.0
+Version: 1.0.1
 Summary: FOSFOR-IO: To read and write dataframe from different connectors.
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 Project-URL: Product, https://www.fosfor.com/
 Project-URL: Source, https://gitlab.fosfor.com/fosfor-decision-cloud/intelligence/refract-sdk
 Keywords: fosforio
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `fosforio-1.0.0/README.md` & `fosforio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/__init__.py` & `fosforio-1.0.1/fosforio/__init__.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/amazons3.py` & `fosforio-1.0.1/fosforio/amazons3.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/azure.py` & `fosforio-1.0.1/fosforio/azure.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/feature_store.py` & `fosforio-1.0.1/fosforio/feature_store.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/hive.py` & `fosforio-1.0.1/fosforio/hive.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/manager.py` & `fosforio-1.0.1/fosforio/manager.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/mysql.py` & `fosforio-1.0.1/fosforio/mysql.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/postgres.py` & `fosforio-1.0.1/fosforio/postgres.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/refractio.py` & `fosforio-1.0.1/fosforio/fosforio.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/sftp.py` & `fosforio-1.0.1/fosforio/sftp.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/snowflake.py` & `fosforio-1.0.1/fosforio/snowflake.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio/sqlserver.py` & `fosforio-1.0.1/fosforio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/fosforio.egg-info/PKG-INFO` & `fosforio-1.0.1/fosforio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosforio
-Version: 1.0.0
+Version: 1.0.1
 Summary: FOSFOR-IO: To read and write dataframe from different connectors.
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 Project-URL: Product, https://www.fosfor.com/
 Project-URL: Source, https://gitlab.fosfor.com/fosfor-decision-cloud/intelligence/refract-sdk
 Keywords: fosforio
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `fosforio-1.0.0/fosforio.egg-info/requires.txt` & `fosforio-1.0.1/fosforio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fosforio-1.0.0/setup.py` & `fosforio-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'FOSFOR-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.6.0",
         "boto3==1.26.116",
         "azure==4.0.0",
```

