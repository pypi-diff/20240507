# Comparing `tmp/filchatter-1.5.tar.gz` & `tmp/filchatter-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filchatter-1.5.tar", last modified: Tue May  7 09:21:29 2024, max compression
+gzip compressed data, was "filchatter-1.6.tar", last modified: Tue May  7 09:35:43 2024, max compression
```

## Comparing `filchatter-1.5.tar` & `filchatter-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.318900 filchatter-1.5/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.289013 filchatter-1.5/Filchatter/
--rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.5/Filchatter/__init__.py
--rw-rw-rw-   0        0        0     1035 2024-05-07 09:19:17.000000 filchatter-1.5/Filchatter/filchatter.py
--rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.5/LICENSE.md
--rw-rw-rw-   0        0        0      106 2024-05-07 09:21:29.317902 filchatter-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:21:29.316907 filchatter-1.5/filchatter.egg-info/
--rw-rw-rw-   0        0        0      106 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 09:21:29.000000 filchatter-1.5/filchatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 09:21:29.319897 filchatter-1.5/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-07 09:20:04.000000 filchatter-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:35:43.328090 filchatter-1.6/
+drwxrwxrwx   0        0        0        0 2024-05-07 09:35:43.298171 filchatter-1.6/Filchatter/
+-rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.6/Filchatter/__init__.py
+-rw-rw-rw-   0        0        0     1034 2024-05-07 09:35:13.000000 filchatter-1.6/Filchatter/filchatter.py
+-rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.6/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2024-05-07 09:35:43.327093 filchatter-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 09:35:43.325097 filchatter-1.6/filchatter.egg-info/
+-rw-rw-rw-   0        0        0      106 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-07 09:35:43.000000 filchatter-1.6/filchatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:35:43.328090 filchatter-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-07 09:34:38.000000 filchatter-1.6/setup.py
```

### Comparing `filchatter-1.5/Filchatter/filchatter.py` & `filchatter-1.6/Filchatter/filchatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 class Filchatter:
-    url = "http://210.113.121.214:4440"
+    url = "http://211.211.70.210:4444"
 
     def __init__(self, api_key= None):
         self.session = requests.Session()
         self.set_api_key(api_key)
         
     def set_api_key(self, key):
         self.api_key = key
```

### Comparing `filchatter-1.5/LICENSE.md` & `filchatter-1.6/LICENSE.md`

 * *Files identical despite different names*

