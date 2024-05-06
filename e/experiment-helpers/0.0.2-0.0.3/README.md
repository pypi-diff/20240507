# Comparing `tmp/experiment_helpers-0.0.2.tar.gz` & `tmp/experiment_helpers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_helpers-0.0.2.tar", last modified: Mon May  6 22:18:10 2024, max compression
+gzip compressed data, was "experiment_helpers-0.0.3.tar", last modified: Mon May  6 22:49:48 2024, max compression
```

## Comparing `experiment_helpers-0.0.2.tar` & `experiment_helpers-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:18:10.662617 experiment_helpers-0.0.2/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.2/LICENSE
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:18:10.661352 experiment_helpers-0.0.2/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.2/README.md
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-06 22:18:02.000000 experiment_helpers-0.0.2/pyproject.toml
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-06 22:18:10.662778 experiment_helpers-0.0.2/setup.cfg
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:18:10.653746 experiment_helpers-0.0.2/src/
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:18:10.656862 experiment_helpers-0.0.2/src/experiment_helpers/
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.2/src/experiment_helpers/__init__.py
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.2/src/experiment_helpers/better_vit_model.py
-drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:18:10.660401 experiment_helpers-0.0.2/src/experiment_helpers.egg-info/
--rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:18:10.658602 experiment_helpers-0.0.2/src/experiment_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      294 2024-05-06 22:18:10.659292 experiment_helpers-0.0.2/src/experiment_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-06 22:18:10.659927 experiment_helpers-0.0.2/src/experiment_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-06 22:18:10.660542 experiment_helpers-0.0.2/src/experiment_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.041377 experiment_helpers-0.0.3/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1071 2024-05-06 22:03:19.000000 experiment_helpers-0.0.3/LICENSE
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:49:48.040413 experiment_helpers-0.0.3/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:01:10.000000 experiment_helpers-0.0.3/README.md
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      361 2024-05-06 22:49:37.000000 experiment_helpers-0.0.3/pyproject.toml
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       38 2024-05-06 22:49:48.041573 experiment_helpers-0.0.3/setup.cfg
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.028836 experiment_helpers-0.0.3/src/
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.035521 experiment_helpers-0.0.3/src/experiment_helpers/
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:05:13.000000 experiment_helpers-0.0.3/src/experiment_helpers/__init__.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)    18911 2024-05-06 22:05:55.000000 experiment_helpers-0.0.3/src/experiment_helpers/better_vit_model.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     5290 2024-05-06 22:49:01.000000 experiment_helpers-0.0.3/src/experiment_helpers/measuring.py
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)     1084 2024-05-06 22:40:35.000000 experiment_helpers-0.0.3/src/experiment_helpers/static_globals.py
+drwxrwxr-x   0 jlb638   (157170) jlb638   (157170)        0 2024-05-06 22:49:48.039197 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/
+-rw-r--r--   0 jlb638   (157170) jlb638   (157170)      375 2024-05-06 22:49:48.036627 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)      371 2024-05-06 22:49:48.037636 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)        1 2024-05-06 22:49:48.038479 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlb638   (157170) jlb638   (157170)       19 2024-05-06 22:49:48.039384 experiment_helpers-0.0.3/src/experiment_helpers.egg-info/top_level.txt
```

### Comparing `experiment_helpers-0.0.2/LICENSE` & `experiment_helpers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `experiment_helpers-0.0.2/src/experiment_helpers/better_vit_model.py` & `experiment_helpers-0.0.3/src/experiment_helpers/better_vit_model.py`

 * *Files identical despite different names*

