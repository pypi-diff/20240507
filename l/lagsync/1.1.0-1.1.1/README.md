# Comparing `tmp/lagsync-1.1.0.tar.gz` & `tmp/lagsync-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lagsync-1.1.0.tar", last modified: Mon May  6 21:49:27 2024, max compression
+gzip compressed data, was "lagsync-1.1.1.tar", last modified: Mon May  6 21:56:54 2024, max compression
```

## Comparing `lagsync-1.1.0.tar` & `lagsync-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.672261 lagsync-1.1.0/
--rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:49:27.672261 lagsync-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.1.0/README.md
--rw-rw-rw-   0        0        0      933 2024-05-06 21:49:14.000000 lagsync-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 21:49:27.672261 lagsync-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.654721 lagsync-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.658263 lagsync-1.1.0/src/lagsync/
--rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.1.0/src/lagsync/__init__.py
--rw-rw-rw-   0        0        0     6527 2024-05-06 21:49:14.000000 lagsync-1.1.0/src/lagsync/lagsync.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.671262 lagsync-1.1.0/src/lagsync.egg-info/
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.030833 lagsync-1.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:56:54.029834 lagsync-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.1.1/README.md
+-rw-rw-rw-   0        0        0      933 2024-05-06 21:56:46.000000 lagsync-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 21:56:54.030833 lagsync-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.013834 lagsync-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.016833 lagsync-1.1.1/src/lagsync/
+-rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.1.1/src/lagsync/__init__.py
+-rw-rw-rw-   0        0        0     6537 2024-05-06 21:56:46.000000 lagsync-1.1.1/src/lagsync/lagsync.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.029834 lagsync-1.1.1/src/lagsync.egg-info/
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:56:53.000000 lagsync-1.1.1/src/lagsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/top_level.txt
```

### Comparing `lagsync-1.1.0/LICENSE` & `lagsync-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lagsync-1.1.0/PKG-INFO` & `lagsync-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.1.0
+Version: 1.1.1
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lagsync-1.1.0/pyproject.toml` & `lagsync-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lagsync"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name="bluePlatinum", email="jukic.rok@gmail.com" },
 ]
 description="A rsync based backup utility for laggy connections"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `lagsync-1.1.0/src/lagsync/lagsync.py` & `lagsync-1.1.1/src/lagsync/lagsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         help="The maximum amount of retries for the rsync job"
                              "per chunk")
     parser.add_argument("--dry-run", action="store_true",
                         help="Perform a dry run, which will only print out"
                              "the resync jobs instead of running them.")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="verbose mode")
-    parser.add_argument("--delay", default=3,
+    parser.add_argument("--delay", default=3, type=int,
                         help="Time to delay (in seconds) after failed chunk."
                              "Default is 3.")
 
     args = parser.parse_args()
 
     # enable verbose logging
     if args.verbose:
```

### Comparing `lagsync-1.1.0/src/lagsync.egg-info/PKG-INFO` & `lagsync-1.1.1/src/lagsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.1.0
+Version: 1.1.1
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

