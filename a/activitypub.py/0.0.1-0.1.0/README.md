# Comparing `tmp/activitypub_py-0.0.1.tar.gz` & `tmp/activitypub_py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitypub_py-0.0.1.tar", max compression
+gzip compressed data, was "activitypub_py-0.1.0.tar", max compression
```

## Comparing `activitypub_py-0.0.1.tar` & `activitypub_py-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-18 07:46:47.567254 activitypub_py-0.0.1/LICENSE
--rw-r--r--   0        0        0       79 2024-04-18 07:53:53.603888 activitypub_py-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-18 07:53:52.464556 activitypub_py-0.0.1/activitypub/__init__.py
--rw-r--r--   0        0        0      477 2024-04-18 07:54:17.649256 activitypub_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 activitypub_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-18 07:46:47.567254 activitypub_py-0.1.0/LICENSE
+-rw-r--r--   0        0        0       79 2024-04-18 07:53:53.603888 activitypub_py-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 07:53:52.464556 activitypub_py-0.1.0/activitypub/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-18 07:50:34.170974 activitypub_py-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 activitypub_py-0.1.0/PKG-INFO
```

### Comparing `activitypub_py-0.0.1/LICENSE` & `activitypub_py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `activitypub_py-0.0.1/PKG-INFO` & `activitypub_py-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activitypub-py
-Version: 0.0.1
+Version: 0.1.0
 Summary: Yet another ActivityPUB framework written in Python.
 License: MIT
 Author: Mattholy
 Author-email: smile.used@hotmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

