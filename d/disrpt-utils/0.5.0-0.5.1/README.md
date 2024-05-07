# Comparing `tmp/disrpt_utils-0.5.0.tar.gz` & `tmp/disrpt_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disrpt_utils-0.5.0.tar", last modified: Tue May  7 15:39:06 2024, max compression
+gzip compressed data, was "disrpt_utils-0.5.1.tar", last modified: Tue May  7 15:48:44 2024, max compression
```

## Comparing `disrpt_utils-0.5.0.tar` & `disrpt_utils-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.546239 disrpt_utils-0.5.0/
--rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:39:06.530239 disrpt_utils-0.5.0/PKG-INFO
--rw-r--r--   0 dsileo   (668667) magnet   (208235)       36 2024-02-12 13:51:20.000000 disrpt_utils-0.5.0/README.md
-drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.178229 disrpt_utils-0.5.0/disrpt_utils/
--rw-r--r--   0 dsileo   (668667) magnet   (208235)     3260 2024-05-07 15:22:17.000000 disrpt_utils-0.5.0/disrpt_utils/__init__.py
--rw-r--r--   0 dsileo   (668667) magnet   (208235)    25769 2024-05-07 15:21:10.000000 disrpt_utils-0.5.0/disrpt_utils/process_underscore.py
-drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.446236 disrpt_utils-0.5.0/disrpt_utils.egg-info/
--rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/PKG-INFO
--rw-r--r--   0 dsileo   (668667) magnet   (208235)      222 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/SOURCES.txt
--rw-r--r--   0 dsileo   (668667) magnet   (208235)        1 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/dependency_links.txt
--rw-r--r--   0 dsileo   (668667) magnet   (208235)       13 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/top_level.txt
--rw-r--r--   0 dsileo   (668667) magnet   (208235)       38 2024-05-07 15:39:06.562240 disrpt_utils-0.5.0/setup.cfg
--rw-r--r--   0 dsileo   (668667) magnet   (208235)      264 2024-05-07 15:30:23.000000 disrpt_utils-0.5.0/setup.py
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:48:44.086612 disrpt_utils-0.5.1/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:48:44.058611 disrpt_utils-0.5.1/PKG-INFO
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       36 2024-02-12 13:51:20.000000 disrpt_utils-0.5.1/README.md
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:48:43.658599 disrpt_utils-0.5.1/disrpt_utils/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)     3260 2024-05-07 15:22:17.000000 disrpt_utils-0.5.1/disrpt_utils/__init__.py
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)    25769 2024-05-07 15:21:10.000000 disrpt_utils-0.5.1/disrpt_utils/process_underscore.py
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:48:43.966608 disrpt_utils-0.5.1/disrpt_utils.egg-info/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:48:43.000000 disrpt_utils-0.5.1/disrpt_utils.egg-info/PKG-INFO
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      222 2024-05-07 15:48:43.000000 disrpt_utils-0.5.1/disrpt_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)        1 2024-05-07 15:48:43.000000 disrpt_utils-0.5.1/disrpt_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       13 2024-05-07 15:48:43.000000 disrpt_utils-0.5.1/disrpt_utils.egg-info/top_level.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       38 2024-05-07 15:48:44.102612 disrpt_utils-0.5.1/setup.cfg
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      264 2024-05-07 15:47:50.000000 disrpt_utils-0.5.1/setup.py
```

### Comparing `disrpt_utils-0.5.0/disrpt_utils/__init__.py` & `disrpt_utils-0.5.1/disrpt_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `disrpt_utils-0.5.0/disrpt_utils/process_underscore.py` & `disrpt_utils-0.5.1/disrpt_utils/process_underscore.py`

 * *Files identical despite different names*

