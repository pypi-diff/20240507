# Comparing `tmp/edgegap_factory-1.1.0.tar.gz` & `tmp/edgegap_factory-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_factory-1.1.0.tar", max compression
+gzip compressed data, was "edgegap_factory-1.7.0.tar", max compression
```

## Comparing `edgegap_factory-1.1.0.tar` & `edgegap_factory-1.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/README.md
--rw-r--r--   0        0        0       17 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/edgegap_factory/BUILD
--rw-r--r--   0        0        0      144 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/edgegap_factory/__init__.py
--rw-r--r--   0        0        0      173 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/edgegap_factory/_base_factory.py
--rw-r--r--   0        0        0     1490 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/edgegap_factory/_generator.py
--rw-r--r--   0        0        0     3614 2024-05-03 20:16:05.423940 edgegap_factory-1.1.0/edgegap_factory/_sql_model_factory.py
--rw-r--r--   0        0        0      366 2024-05-03 20:17:05.516667 edgegap_factory-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 edgegap_factory-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-06 18:04:44.781040 edgegap_factory-1.7.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-06 18:04:44.781156 edgegap_factory-1.7.0/edgegap_factory/BUILD
+-rw-r--r--   0        0        0      144 2024-05-06 18:04:44.781340 edgegap_factory-1.7.0/edgegap_factory/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-06 18:04:44.781534 edgegap_factory-1.7.0/edgegap_factory/_base_factory.py
+-rw-r--r--   0        0        0     1490 2024-05-06 18:04:44.781738 edgegap_factory-1.7.0/edgegap_factory/_generator.py
+-rw-r--r--   0        0        0     3614 2024-05-06 20:32:49.188993 edgegap_factory-1.7.0/edgegap_factory/_sql_model_factory.py
+-rw-r--r--   0        0        0      366 2024-05-07 13:27:32.204185 edgegap_factory-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 edgegap_factory-1.7.0/PKG-INFO
```

### Comparing `edgegap_factory-1.1.0/edgegap_factory/_generator.py` & `edgegap_factory-1.7.0/edgegap_factory/_generator.py`

 * *Files identical despite different names*

### Comparing `edgegap_factory-1.1.0/edgegap_factory/_sql_model_factory.py` & `edgegap_factory-1.7.0/edgegap_factory/_sql_model_factory.py`

 * *Files identical despite different names*

