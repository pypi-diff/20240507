# Comparing `tmp/disrpt_utils-0.1.3.tar.gz` & `tmp/disrpt_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disrpt_utils-0.1.3.tar", max compression
+gzip compressed data, was "disrpt_utils-0.5.0.tar", last modified: Tue May  7 15:39:06 2024, max compression
```

## Comparing `disrpt_utils-0.1.3.tar` & `disrpt_utils-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,13 @@
--rw-r--r--   0        0        0       36 2024-02-12 12:56:29.672429 disrpt_utils-0.1.3/README.md
--rw-r--r--   0        0        0       47 2024-02-12 12:56:29.672429 disrpt_utils-0.1.3/disrpt_utils/__init__.py
--rw-r--r--   0        0        0      242 2024-02-12 12:56:29.672429 disrpt_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 disrpt_utils-0.1.3/PKG-INFO
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.546239 disrpt_utils-0.5.0/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:39:06.530239 disrpt_utils-0.5.0/PKG-INFO
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       36 2024-02-12 13:51:20.000000 disrpt_utils-0.5.0/README.md
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.178229 disrpt_utils-0.5.0/disrpt_utils/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)     3260 2024-05-07 15:22:17.000000 disrpt_utils-0.5.0/disrpt_utils/__init__.py
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)    25769 2024-05-07 15:21:10.000000 disrpt_utils-0.5.0/disrpt_utils/process_underscore.py
+drwxr-xr-x   0 dsileo   (668667) magnet   (208235)        0 2024-05-07 15:39:06.446236 disrpt_utils-0.5.0/disrpt_utils.egg-info/
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      150 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/PKG-INFO
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      222 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)        1 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       13 2024-05-07 15:39:05.000000 disrpt_utils-0.5.0/disrpt_utils.egg-info/top_level.txt
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)       38 2024-05-07 15:39:06.562240 disrpt_utils-0.5.0/setup.cfg
+-rw-r--r--   0 dsileo   (668667) magnet   (208235)      264 2024-05-07 15:30:23.000000 disrpt_utils-0.5.0/setup.py
```

