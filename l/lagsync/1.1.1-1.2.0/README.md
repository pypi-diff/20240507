# Comparing `tmp/lagsync-1.1.1.tar.gz` & `tmp/lagsync-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lagsync-1.1.1.tar", last modified: Mon May  6 21:56:54 2024, max compression
+gzip compressed data, was "lagsync-1.2.0.tar", last modified: Tue May  7 19:21:45 2024, max compression
```

## Comparing `lagsync-1.1.1.tar` & `lagsync-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.030833 lagsync-1.1.1/
--rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:56:54.029834 lagsync-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.1.1/README.md
--rw-rw-rw-   0        0        0      933 2024-05-06 21:56:46.000000 lagsync-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 21:56:54.030833 lagsync-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.013834 lagsync-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.016833 lagsync-1.1.1/src/lagsync/
--rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.1.1/src/lagsync/__init__.py
--rw-rw-rw-   0        0        0     6537 2024-05-06 21:56:46.000000 lagsync-1.1.1/src/lagsync/lagsync.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:56:54.029834 lagsync-1.1.1/src/lagsync.egg-info/
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:56:53.000000 lagsync-1.1.1/src/lagsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 21:56:54.000000 lagsync-1.1.1/src/lagsync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 19:21:45.507732 lagsync-1.2.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2086 2024-05-07 19:21:45.507732 lagsync-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.2.0/README.md
+-rw-rw-rw-   0        0        0      933 2024-05-07 19:21:35.000000 lagsync-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:21:45.507732 lagsync-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 19:21:45.490731 lagsync-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 19:21:45.494732 lagsync-1.2.0/src/lagsync/
+-rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.2.0/src/lagsync/__init__.py
+-rw-rw-rw-   0        0        0     6766 2024-05-07 19:21:35.000000 lagsync-1.2.0/src/lagsync/lagsync.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:21:45.506765 lagsync-1.2.0/src/lagsync.egg-info/
+-rw-rw-rw-   0        0        0     2086 2024-05-07 19:21:45.000000 lagsync-1.2.0/src/lagsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-07 19:21:45.000000 lagsync-1.2.0/src/lagsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:21:45.000000 lagsync-1.2.0/src/lagsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-07 19:21:45.000000 lagsync-1.2.0/src/lagsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 19:21:45.000000 lagsync-1.2.0/src/lagsync.egg-info/top_level.txt
```

### Comparing `lagsync-1.1.1/LICENSE` & `lagsync-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lagsync-1.1.1/PKG-INFO` & `lagsync-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.1.1
+Version: 1.2.0
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lagsync-1.1.1/pyproject.toml` & `lagsync-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lagsync"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
     { name="bluePlatinum", email="jukic.rok@gmail.com" },
 ]
 description="A rsync based backup utility for laggy connections"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `lagsync-1.1.1/src/lagsync/lagsync.py` & `lagsync-1.2.0/src/lagsync/lagsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     try:
         dry_run = kwargs['dry_run']
     except KeyError:
         dry_run = False
 
     sync_objects = dirlist + filelist
 
+    failed = list()
+
     if len(destination.split(":")) == 2:
         remote, remote_dir = destination.split(":")
         remote += ":"       # add the : delimiter to the remote variable
     else:
         remote = ""
         remote_dir = destination
 
@@ -111,20 +113,26 @@
                 time.sleep(fail_delay)
                 retry += 1
                 proc = subprocess.run(
                     ["rsync", f"-{options}", src, f"{remote}{dst}"])
                 if retry >= max_retries:
                     logging.critical(f"Reached maximum amount of retries "
                                      f"(max_retries={max_retries}). Sync job "
-                                     f"{sync_object} failed. Aborting.")
-                    return 1
+                                     f"{sync_object} failed. Skipping chunk.")
+                    failed.append(sync_object)
 
         else:
             print(f"rsync -{options} {src} {remote}{dst}")
 
+    if len(failed) != 0:
+        logging.critical("Failed to sync the following directories:")
+        for fail in failed:
+            logging.critical(fail)
+        return 1
+
     return 0
 
 
 def main():
     """
     The main function to be run for the script in cli mode.
     :return: Exitcode
```

### Comparing `lagsync-1.1.1/src/lagsync.egg-info/PKG-INFO` & `lagsync-1.2.0/src/lagsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.1.1
+Version: 1.2.0
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

