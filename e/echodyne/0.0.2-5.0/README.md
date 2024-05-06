# Comparing `tmp/echodyne-0.0.2.tar.gz` & `tmp/echodyne-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echodyne-0.0.2.tar", last modified: Mon May  6 22:21:05 2024, max compression
+gzip compressed data, was "echodyne-5.0.tar", last modified: Mon May  6 22:42:00 2024, max compression
```

## Comparing `echodyne-0.0.2.tar` & `echodyne-5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:21:05.399603 echodyne-0.0.2/
--rw-r--r--   0 user      (1000) user      (1000)      261 2024-05-06 22:21:05.399603 echodyne-0.0.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      242 2024-05-06 22:20:55.000000 echodyne-0.0.2/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-06 22:21:05.399603 echodyne-0.0.2/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:21:05.398604 echodyne-0.0.2/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:21:05.398604 echodyne-0.0.2/src/echodyne/
--rw-r--r--   0 user      (1000) user      (1000)       22 2024-05-06 22:16:15.000000 echodyne-0.0.2/src/echodyne/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:21:05.399603 echodyne-0.0.2/src/echodyne.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      261 2024-05-06 22:21:05.000000 echodyne-0.0.2/src/echodyne.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      183 2024-05-06 22:21:05.000000 echodyne-0.0.2/src/echodyne.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-06 22:21:05.000000 echodyne-0.0.2/src/echodyne.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        9 2024-05-06 22:21:05.000000 echodyne-0.0.2/src/echodyne.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:42:00.401579 echodyne-5.0/
+-rw-r--r--   0 user      (1000) user      (1000)      259 2024-05-06 22:42:00.400579 echodyne-5.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      240 2024-05-06 22:41:02.000000 echodyne-5.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-06 22:42:00.401579 echodyne-5.0/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:42:00.400579 echodyne-5.0/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:42:00.400579 echodyne-5.0/src/echodyne/
+-rw-r--r--   0 user      (1000) user      (1000)       35 2024-05-06 22:41:41.000000 echodyne-5.0/src/echodyne/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-06 22:42:00.400579 echodyne-5.0/src/echodyne.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      259 2024-05-06 22:42:00.000000 echodyne-5.0/src/echodyne.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      183 2024-05-06 22:42:00.000000 echodyne-5.0/src/echodyne.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-06 22:42:00.000000 echodyne-5.0/src/echodyne.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2024-05-06 22:42:00.000000 echodyne-5.0/src/echodyne.egg-info/top_level.txt
```

