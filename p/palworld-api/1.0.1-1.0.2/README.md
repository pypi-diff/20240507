# Comparing `tmp/palworld-api-1.0.1.tar.gz` & `tmp/palworld-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palworld-api-1.0.1.tar", last modified: Wed Apr 10 13:09:10 2024, max compression
+gzip compressed data, was "palworld-api-1.0.2.tar", last modified: Tue May  7 16:42:29 2024, max compression
```

## Comparing `palworld-api-1.0.1.tar` & `palworld-api-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.282538 palworld-api-1.0.1/
--rw-rw-rw-   0        0        0     1378 2024-04-10 13:09:10.282538 palworld-api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2024-04-10 13:08:35.000000 palworld-api-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.258539 palworld-api-1.0.1/palworld_api/
--rw-rw-rw-   0        0        0       27 2024-04-04 23:38:01.000000 palworld-api-1.0.1/palworld_api/__init__.py
--rw-rw-rw-   0        0        0     7168 2024-04-10 13:05:01.000000 palworld-api-1.0.1/palworld_api/palworld_api.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.281537 palworld-api-1.0.1/palworld_api.egg-info/
--rw-rw-rw-   0        0        0     1378 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 13:09:10.282538 palworld-api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-04-10 13:08:29.000000 palworld-api-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:42:29.881642 palworld-api-1.0.2/
+-rw-rw-rw-   0        0        0     1378 2024-05-07 16:42:29.880640 palworld-api-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2024-04-10 13:08:35.000000 palworld-api-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 16:42:29.845641 palworld-api-1.0.2/palworld_api/
+-rw-rw-rw-   0        0        0       27 2024-04-04 23:38:01.000000 palworld-api-1.0.2/palworld_api/__init__.py
+-rw-rw-rw-   0        0        0     7168 2024-04-10 13:05:01.000000 palworld-api-1.0.2/palworld_api/palworld_api.py
+drwxrwxrwx   0        0        0        0 2024-05-07 16:42:29.879639 palworld-api-1.0.2/palworld_api.egg-info/
+-rw-rw-rw-   0        0        0     1378 2024-05-07 16:42:29.000000 palworld-api-1.0.2/palworld_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-07 16:42:29.000000 palworld-api-1.0.2/palworld_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 16:42:29.000000 palworld-api-1.0.2/palworld_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 16:42:29.000000 palworld-api-1.0.2/palworld_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 16:42:29.000000 palworld-api-1.0.2/palworld_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 16:42:29.881642 palworld-api-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-05-07 16:41:10.000000 palworld-api-1.0.2/setup.py
```

### Comparing `palworld-api-1.0.1/PKG-INFO` & `palworld-api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palworld-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python API wrapper for the Palworld Rest API.
 Home-page: https://github.com/dkoz/palworld-api
 Author: dkoz
 Author-email: koz@beskor.net
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `palworld-api-1.0.1/README.md` & `palworld-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `palworld-api-1.0.1/palworld_api/palworld_api.py` & `palworld-api-1.0.2/palworld_api/palworld_api.py`

 * *Files identical despite different names*

### Comparing `palworld-api-1.0.1/palworld_api.egg-info/PKG-INFO` & `palworld-api-1.0.2/palworld_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palworld-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python API wrapper for the Palworld Rest API.
 Home-page: https://github.com/dkoz/palworld-api
 Author: dkoz
 Author-email: koz@beskor.net
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

