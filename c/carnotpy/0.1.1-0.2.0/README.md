# Comparing `tmp/carnotpy-0.1.1.tar.gz` & `tmp/carnotpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carnotpy-0.1.1.tar", last modified: Wed Aug  9 10:42:56 2023, max compression
+gzip compressed data, was "carnotpy-0.2.0.tar", last modified: Tue May  7 10:32:48 2024, max compression
```

## Comparing `carnotpy-0.1.1.tar` & `carnotpy-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 choy       (501) staff       (20)        0 2023-08-09 10:42:56.621539 carnotpy-0.1.1/
--rw-r--r--   0 choy       (501) staff       (20)      190 2023-08-09 10:42:56.621361 carnotpy-0.1.1/PKG-INFO
--rw-r--r--   0 choy       (501) staff       (20)       49 2023-05-10 10:38:39.000000 carnotpy-0.1.1/README.md
-drwxr-xr-x   0 choy       (501) staff       (20)        0 2023-08-09 10:42:56.621180 carnotpy-0.1.1/carnotpy.egg-info/
--rw-r--r--   0 choy       (501) staff       (20)      190 2023-08-09 10:42:56.000000 carnotpy-0.1.1/carnotpy.egg-info/PKG-INFO
--rw-r--r--   0 choy       (501) staff       (20)      189 2023-08-09 10:42:56.000000 carnotpy-0.1.1/carnotpy.egg-info/SOURCES.txt
--rw-r--r--   0 choy       (501) staff       (20)        1 2023-08-09 10:42:56.000000 carnotpy-0.1.1/carnotpy.egg-info/dependency_links.txt
--rw-r--r--   0 choy       (501) staff       (20)       32 2023-08-09 10:42:56.000000 carnotpy-0.1.1/carnotpy.egg-info/requires.txt
--rw-r--r--   0 choy       (501) staff       (20)        9 2023-08-09 10:42:56.000000 carnotpy-0.1.1/carnotpy.egg-info/top_level.txt
--rw-r--r--   0 choy       (501) staff       (20)    12624 2023-08-09 10:40:16.000000 carnotpy-0.1.1/carnotpy.py
--rw-r--r--   0 choy       (501) staff       (20)       38 2023-08-09 10:42:56.621586 carnotpy-0.1.1/setup.cfg
--rw-r--r--   0 choy       (501) staff       (20)      295 2023-08-09 10:41:59.000000 carnotpy-0.1.1/setup.py
+drwxr-xr-x   0 choy       (501) staff       (20)        0 2024-05-07 10:32:48.809164 carnotpy-0.2.0/
+-rw-r--r--   0 choy       (501) staff       (20)      190 2024-05-07 10:32:48.808969 carnotpy-0.2.0/PKG-INFO
+-rw-r--r--   0 choy       (501) staff       (20)       49 2023-05-10 10:38:39.000000 carnotpy-0.2.0/README.md
+drwxr-xr-x   0 choy       (501) staff       (20)        0 2024-05-07 10:32:48.808754 carnotpy-0.2.0/carnotpy.egg-info/
+-rw-r--r--   0 choy       (501) staff       (20)      190 2024-05-07 10:32:48.000000 carnotpy-0.2.0/carnotpy.egg-info/PKG-INFO
+-rw-r--r--   0 choy       (501) staff       (20)      189 2024-05-07 10:32:48.000000 carnotpy-0.2.0/carnotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 choy       (501) staff       (20)        1 2024-05-07 10:32:48.000000 carnotpy-0.2.0/carnotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 choy       (501) staff       (20)       32 2024-05-07 10:32:48.000000 carnotpy-0.2.0/carnotpy.egg-info/requires.txt
+-rw-r--r--   0 choy       (501) staff       (20)        9 2024-05-07 10:32:48.000000 carnotpy-0.2.0/carnotpy.egg-info/top_level.txt
+-rw-r--r--   0 choy       (501) staff       (20)    12624 2023-08-09 10:40:16.000000 carnotpy-0.2.0/carnotpy.py
+-rw-r--r--   0 choy       (501) staff       (20)       38 2024-05-07 10:32:48.809219 carnotpy-0.2.0/setup.cfg
+-rw-r--r--   0 choy       (501) staff       (20)      295 2024-05-07 10:32:45.000000 carnotpy-0.2.0/setup.py
```

### Comparing `carnotpy-0.1.1/carnotpy.py` & `carnotpy-0.2.0/carnotpy.py`

 * *Files identical despite different names*

