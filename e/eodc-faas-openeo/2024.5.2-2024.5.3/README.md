# Comparing `tmp/eodc_faas_openeo-2024.5.2.tar.gz` & `tmp/eodc_faas_openeo-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_openeo-2024.5.2.tar", max compression
+gzip compressed data, was "eodc_faas_openeo-2024.5.3.tar", max compression
```

## Comparing `eodc_faas_openeo-2024.5.2.tar` & `eodc_faas_openeo-2024.5.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       11 2024-05-06 14:58:39.808000 eodc_faas_openeo-2024.5.2/README.md
--rw-r--r--   0        0        0       76 2024-05-06 14:58:39.808000 eodc_faas_openeo-2024.5.2/openeo_executor_bindings/__init__.py
--rw-r--r--   0        0        0      901 2024-05-06 14:58:39.808000 eodc_faas_openeo-2024.5.2/openeo_executor_bindings/model.py
--rw-r--r--   0        0        0      659 2024-05-06 14:58:39.808000 eodc_faas_openeo-2024.5.2/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2024.5.2/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-06 15:27:44.220000 eodc_faas_openeo-2024.5.3/README.md
+-rw-r--r--   0        0        0       76 2024-05-06 15:27:44.220000 eodc_faas_openeo-2024.5.3/openeo_executor_bindings/__init__.py
+-rw-r--r--   0        0        0      901 2024-05-06 15:27:44.220000 eodc_faas_openeo-2024.5.3/openeo_executor_bindings/model.py
+-rw-r--r--   0        0        0      659 2024-05-06 15:27:44.220000 eodc_faas_openeo-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2024.5.3/PKG-INFO
```

### Comparing `eodc_faas_openeo-2024.5.2/openeo_executor_bindings/model.py` & `eodc_faas_openeo-2024.5.3/openeo_executor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_openeo-2024.5.2/pyproject.toml` & `eodc_faas_openeo-2024.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-openeo"
-version = "2024.5.2"
+version = "2024.5.3"
 description = "Bindings for the OpenEO processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "openeo_executor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

