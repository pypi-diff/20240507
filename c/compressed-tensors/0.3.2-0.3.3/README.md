# Comparing `tmp/compressed-tensors-0.3.2.tar.gz` & `tmp/compressed-tensors-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressed-tensors-0.3.2.tar", last modified: Mon Apr 29 14:01:33 2024, max compression
+gzip compressed data, was "compressed-tensors-0.3.3.tar", last modified: Tue May  7 15:25:54 2024, max compression
```

## Comparing `compressed-tensors-0.3.2.tar` & `compressed-tensors-0.3.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/
--rw-rw-r--   0 damian    (1006) damian    (1007)    11357 2024-04-25 16:30:47.000000 compressed-tensors-0.3.2/LICENSE
--rw-rw-r--   0 damian    (1006) damian    (1007)     3682 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/PKG-INFO
--rw-rw-r--   0 damian    (1006) damian    (1007)     3288 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/README.md
--rw-rw-r--   0 damian    (1006) damian    (1007)       56 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/pyproject.toml
--rw-rw-r--   0 damian    (1006) damian    (1007)      388 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/setup.cfg
--rw-rw-r--   0 damian    (1006) damian    (1007)     1838 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/setup.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/
--rw-rw-r--   0 damian    (1006) damian    (1007)      789 2024-04-29 09:32:10.000000 compressed-tensors-0.3.2/src/compressed_tensors/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)      717 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/base.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/compressors/
--rw-rw-r--   0 damian    (1006) damian    (1007)      841 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3902 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1271 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/dense.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     5458 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/helpers.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     8647 2024-04-29 14:01:27.000000 compressed-tensors-0.3.2/src/compressed_tensors/compressors/sparse_bitmask.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/config/
--rw-rw-r--   0 damian    (1006) damian    (1007)      704 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1373 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1311 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/dense.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1284 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/config/sparse_bitmask.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/
--rw-rw-r--   0 damian    (1006) damian    (1007)      760 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/__init__.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/
--rw-rw-r--   0 damian    (1006) damian    (1007)      772 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     6651 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/apply.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1776 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/calibration.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     4941 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/forward.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1606 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/frozen.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3697 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/initialize.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/
--rw-rw-r--   0 damian    (1006) damian    (1007)      745 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2786 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/base.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2109 2024-04-25 14:00:11.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/helpers.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1859 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/memoryless.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     2439 2024-04-25 14:00:11.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/min_max.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3371 2024-04-29 09:33:38.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_args.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     6650 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_config.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1480 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_scheme.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/
--rw-rw-r--   0 damian    (1006) damian    (1007)      656 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     3694 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/helpers.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/registry/
--rw-rw-r--   0 damian    (1006) damian    (1007)      658 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/registry/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)    11890 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/src/compressed_tensors/registry/registry.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/src/compressed_tensors/utils/
--rw-rw-r--   0 damian    (1006) damian    (1007)      665 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/utils/__init__.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     8502 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/src/compressed_tensors/utils/safetensors_load.py
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.369350 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/
--rw-r--r--   0 damian    (1006) damian    (1007)     3682 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/PKG-INFO
--rw-rw-r--   0 damian    (1006) damian    (1007)     1911 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/SOURCES.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)        1 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/dependency_links.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)      139 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/requires.txt
--rw-rw-r--   0 damian    (1006) damian    (1007)       19 2024-04-29 14:01:33.000000 compressed-tensors-0.3.2/src/compressed_tensors.egg-info/top_level.txt
-drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-04-29 14:01:33.373350 compressed-tensors-0.3.2/tests/
--rw-rw-r--   0 damian    (1006) damian    (1007)     4322 2024-04-19 09:24:17.000000 compressed-tensors-0.3.2/tests/test_bitmask.py
--rw-rw-r--   0 damian    (1006) damian    (1007)     1662 2024-04-25 13:53:48.000000 compressed-tensors-0.3.2/tests/test_registry.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/
+-rw-rw-r--   0 damian    (1006) damian    (1007)    11357 2024-04-25 16:30:47.000000 compressed-tensors-0.3.3/LICENSE
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3681 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/PKG-INFO
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3287 2024-05-02 14:03:54.000000 compressed-tensors-0.3.3/README.md
+-rw-rw-r--   0 damian    (1006) damian    (1007)       56 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/pyproject.toml
+-rw-rw-r--   0 damian    (1006) damian    (1007)      388 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/setup.cfg
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1838 2024-05-07 15:25:43.000000 compressed-tensors-0.3.3/setup.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      789 2024-04-29 09:32:10.000000 compressed-tensors-0.3.3/src/compressed_tensors/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)      717 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/base.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/compressors/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      841 2024-04-29 14:01:27.000000 compressed-tensors-0.3.3/src/compressed_tensors/compressors/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3902 2024-04-29 14:01:27.000000 compressed-tensors-0.3.3/src/compressed_tensors/compressors/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1271 2024-04-29 14:01:27.000000 compressed-tensors-0.3.3/src/compressed_tensors/compressors/dense.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     5458 2024-04-29 14:01:27.000000 compressed-tensors-0.3.3/src/compressed_tensors/compressors/helpers.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     8652 2024-05-07 10:11:43.000000 compressed-tensors-0.3.3/src/compressed_tensors/compressors/sparse_bitmask.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/config/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      704 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/config/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1373 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/config/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1311 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/config/dense.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1284 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/config/sparse_bitmask.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/quantization/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      760 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/__init__.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      772 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     6973 2024-05-02 14:03:54.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/apply.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1776 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/calibration.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     7600 2024-05-07 14:42:15.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/forward.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1606 2024-05-07 14:42:15.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/frozen.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3697 2024-04-29 09:33:38.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/initialize.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      745 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     5097 2024-05-07 14:42:15.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/base.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     2109 2024-05-07 14:42:15.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/helpers.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1859 2024-04-29 09:33:38.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/memoryless.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     2439 2024-04-25 14:00:11.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/min_max.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     4360 2024-05-07 10:11:43.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/quant_args.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     6650 2024-05-07 14:42:15.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/quant_config.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1480 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/quant_scheme.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/src/compressed_tensors/quantization/utils/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      656 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/utils/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     3695 2024-05-07 10:11:43.000000 compressed-tensors-0.3.3/src/compressed_tensors/quantization/utils/helpers.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/src/compressed_tensors/registry/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      658 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/registry/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)    11890 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/src/compressed_tensors/registry/registry.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/src/compressed_tensors/utils/
+-rw-rw-r--   0 damian    (1006) damian    (1007)      665 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/utils/__init__.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1735 2024-05-02 14:03:54.000000 compressed-tensors-0.3.3/src/compressed_tensors/utils/helpers.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     8502 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/src/compressed_tensors/utils/safetensors_load.py
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.911155 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/
+-rw-r--r--   0 damian    (1006) damian    (1007)     3681 2024-05-07 15:25:54.000000 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/PKG-INFO
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1951 2024-05-07 15:25:54.000000 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/SOURCES.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)        1 2024-05-07 15:25:54.000000 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/dependency_links.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)      139 2024-05-07 15:25:54.000000 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/requires.txt
+-rw-rw-r--   0 damian    (1006) damian    (1007)       19 2024-05-07 15:25:54.000000 compressed-tensors-0.3.3/src/compressed_tensors.egg-info/top_level.txt
+drwxrwxr-x   0 damian    (1006) damian    (1007)        0 2024-05-07 15:25:54.915155 compressed-tensors-0.3.3/tests/
+-rw-rw-r--   0 damian    (1006) damian    (1007)     4322 2024-04-19 09:24:17.000000 compressed-tensors-0.3.3/tests/test_bitmask.py
+-rw-rw-r--   0 damian    (1006) damian    (1007)     1662 2024-04-25 13:53:48.000000 compressed-tensors-0.3.3/tests/test_registry.py
```

### Comparing `compressed-tensors-0.3.2/LICENSE` & `compressed-tensors-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/PKG-INFO` & `compressed-tensors-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: compressed-tensors
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for utilization of compressed safetensors of neural network models
 Home-page: https://github.com/neuralmagic/compressed-tensors
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# compressed-tensors
+# compressed_tensors
 
 This repository extends a [safetensors](https://github.com/huggingface/safetensors) format to efficiently store sparse and/or quantized tensors on disk. `compressed-tensors` format supports multiple compression types to minimize the disk space and facilitate the tensor manipulation.
 
 ## Motivation
 
 ### Reduce disk space by saving sparse tensors in a compressed format
 
@@ -93,8 +93,7 @@
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
 
 For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
 
 
-
```

### Comparing `compressed-tensors-0.3.2/README.md` & `compressed-tensors-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# compressed-tensors
+# compressed_tensors
 
 This repository extends a [safetensors](https://github.com/huggingface/safetensors) format to efficiently store sparse and/or quantized tensors on disk. `compressed-tensors` format supports multiple compression types to minimize the disk space and facilitate the tensor manipulation.
 
 ## Motivation
 
 ### Reduce disk space by saving sparse tensors in a compressed format
 
@@ -78,8 +78,7 @@
 save_compressed_model(model, "compressed_model.safetensors", compression_format=compression_config.format)
 
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
 
 For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
-
```

### Comparing `compressed-tensors-0.3.2/setup.py` & `compressed-tensors-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return ["torch>=1.7.0", "transformers<4.41", "pydantic<2.7"]
 
 def _setup_extras() -> Dict:
     return {"dev": ["black==22.12.0", "isort==5.8.0", "wheel>=0.36.2", "flake8>=3.8.3", "pytest>=6.0.0", "nbconvert>=7.16.3"]}
 
 setup(
     name="compressed-tensors",
-    version="0.3.2",
+    version="0.3.3",
     author="Neuralmagic, Inc.",
     author_email="support@neuralmagic.com",
     license="Apache 2.0",
     description="Library for utilization of compressed safetensors of neural network models",
     long_description=_setup_long_description()[0],
     long_description_content_type=_setup_long_description()[1],
     url="https://github.com/neuralmagic/compressed-tensors",
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/base.py` & `compressed-tensors-0.3.3/src/compressed_tensors/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/compressors/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/compressors/base.py` & `compressed-tensors-0.3.3/src/compressed_tensors/compressors/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/compressors/dense.py` & `compressed-tensors-0.3.3/src/compressed_tensors/compressors/dense.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/compressors/helpers.py` & `compressed-tensors-0.3.3/src/compressed_tensors/compressors/helpers.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/compressors/sparse_bitmask.py` & `compressed-tensors-0.3.3/src/compressed_tensors/compressors/sparse_bitmask.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             for key in bitmask_dict.keys():
                 if key in compressed_dict:
                     _LOGGER.warn(
                         f"Expected all compressed state_dict keys to be unique, but "
                         f"found an existing entry for {key}. The existing entry will "
                         "be replaced."
                     )
-            compressed_dict |= bitmask_dict
+            compressed_dict.update(bitmask_dict)
 
         return compressed_dict
 
     def decompress(
         self, path_to_model_or_tensors: str, device: str = "cpu"
     ) -> Generator[Tuple[str, Tensor], None, None]:
         """
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/config/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/config/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/config/base.py` & `compressed-tensors-0.3.3/src/compressed_tensors/config/base.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/config/dense.py` & `compressed-tensors-0.3.3/src/compressed_tensors/config/dense.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/config/sparse_bitmask.py` & `compressed-tensors-0.3.3/src/compressed_tensors/config/sparse_bitmask.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/apply.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/apply.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from torch.nn import Module
 
 
 __all__ = [
     "load_pretrained_quantization",
     "apply_quantization_config",
     "apply_quantization_status",
+    "find_first_name_or_class_match",
 ]
 
 from compressed_tensors.quantization.utils.helpers import is_module_quantized
 from compressed_tensors.utils.safetensors_load import get_quantization_state_dict
 
 
 def load_pretrained_quantization(model: Module, model_name_or_path: str):
@@ -95,17 +96,17 @@
     target_to_scheme = OrderedDict()
     for scheme in config.config_groups.values():
         for target in scheme.targets:
             target_to_scheme[target] = scheme
 
     # mark appropriate layers for quantization by setting their quantization schemes
     for name, submodule in iter_named_leaf_modules(model):
-        if _find_first_name_or_class_match(name, submodule, config.ignore):
+        if find_first_name_or_class_match(name, submodule, config.ignore):
             continue  # layer matches ignore list, continue
-        target = _find_first_name_or_class_match(name, submodule, target_to_scheme)
+        target = find_first_name_or_class_match(name, submodule, target_to_scheme)
         if target is not None:
             # target matched - add layer and scheme to target list
             submodule.quantization_scheme = target_to_scheme[target]
 
     # apply current quantization status across all targeted layers
     apply_quantization_status(model, config.quantization_status)
 
@@ -121,35 +122,39 @@
         model.apply(initialize_module_for_quantization)
     if status >= QuantizationStatus.CALIBRATION:
         model.apply(set_module_for_calibration)
     if status >= QuantizationStatus.FROZEN:
         model.apply(freeze_module_quantization)
 
 
-def _find_first_name_or_class_match(
-    name: str,
-    module: Module,
-    targets: Iterable[str],
+def find_first_name_or_class_match(
+    name: str, module: Module, targets: Iterable[str], check_contains: bool = False
 ) -> Optional[str]:
     # first element of targets that matches the given name
     # if no name matches returns first target that matches the class name
     # returns None otherwise
     return _find_first_match(name, targets) or _find_first_match(
-        module.__class__.__name__, targets
+        module.__class__.__name__, targets, check_contains
     )
 
 
-def _find_first_match(value: str, targets: Iterable[str]) -> Optional[str]:
+def _find_first_match(
+    value: str, targets: Iterable[str], check_contains: bool = False
+) -> Optional[str]:
     # returns first element of target that matches value either
-    # exactly or as a regex after 're:'
+    # exactly or as a regex after 're:'. if check_contains is set to True,
+    # additionally checks if the target string is contained with value.
     for target in targets:
         if target.startswith("re:"):
             pattern = target[3:]
             if re.match(pattern, value):
                 return target
+        elif check_contains:
+            if target.lower() in value.lower():
+                return target
         elif target == value:
             return target
     return None
 
 
 def _load_quant_args_from_state_dict(
     base_name: str, module_name: str, module: Module, state_dict: Dict
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/calibration.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/calibration.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/frozen.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/frozen.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/lifecycle/initialize.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/lifecycle/initialize.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/base.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/min_max.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,62 +8,58 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Tuple
+from typing import Tuple
 
+import torch
+from compressed_tensors.quantization.observers.base import Observer
+from compressed_tensors.quantization.observers.helpers import calculate_qparams
 from compressed_tensors.quantization.quant_args import QuantizationArgs
-from compressed_tensors.registry.registry import RegistryMixin
 from torch import FloatTensor, IntTensor, Tensor
-from torch.nn import Module
 
 
-__all__ = ["Observer"]
+__all__ = ["MovingAverageMinMaxObserver"]
 
 
-class Observer(Module, RegistryMixin):
+@Observer.register("minmax")
+class MovingAverageMinMaxObserver(Observer):
     """
-    Base Observer class to be subclassed for specific implementation.
-    Subclasses should override `calculate_qparams` to return a scale, zero_point
-    pair
+    Implements a dynamic quantization observer that sets the scale and
+    zero point based on a moving average of the overall min and max observed values
     """
 
-    def __init__(self, quantization_args: QuantizationArgs):
-        self.quantization_args: QuantizationArgs = quantization_args
-        super().__init__()
-        self._scale = None
-        self._zero_point = None
-
-    def forward(self, observed: Tensor) -> Tuple[FloatTensor, IntTensor]:
-        """
-        maps directly to get_qparams
-        :param observed: optional observed tensor to calculate quantization parameters
-            from
-        :return: tuple of scale and zero point based on last observed value
-        """
-        return self.get_qparams(observed=observed)
+    def __init__(
+        self, quantization_args: QuantizationArgs, averaging_constant: float = 0.01
+    ):
+        super().__init__(quantization_args=quantization_args)
+
+        self.min_val = float("inf")
+        self.max_val = -float("inf")
+        self.averaging_constant = averaging_constant
 
     def calculate_qparams(self, observed: Tensor) -> Tuple[FloatTensor, IntTensor]:
         """
+        Updates the observed min and max using a moving average smoothed by the
+        averaging_constant
+
         :param observed: observed tensor to calculate quantization parameters for
         :return: tuple of scale and zero point derived from the observed tensor
         """
-        raise NotImplementedError(f"{self.__class__} must implement calculate_qparams")
 
-    def get_qparams(
-        self, observed: Optional[Tensor] = None
-    ) -> Tuple[FloatTensor, IntTensor]:
-        """
-        Convenience function to wrap overwritten calculate_qparams
-        adds support to make observed tensor optional and support for tracking latest
-        calculated scale and zero point
-        :param observed: optional observed tensor to calculate quantization parameters
-            from
-        :return: tuple of scale and zero point based on last observed value
-        """
-        if observed is not None:
-            # re-calcualte scale and zero point, update the stored value
-            self._scale, self._zero_point = self.calculate_qparams(observed)
-        return self._scale, self._zero_point
+        min_val, max_val = torch.aminmax(observed)
+
+        if self.min_val == float("inf") and self.max_val == float("-inf"):
+            self.min_val = min_val
+            self.max_val = max_val
+        else:
+            self.min_val = self.min_val + self.averaging_constant * (
+                min_val - self.min_val
+            )
+            self.max_val = self.max_val + self.averaging_constant * (
+                max_val - self.max_val
+            )
+
+        return calculate_qparams(self.min_val, self.max_val, self.quantization_args)
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/helpers.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/helpers.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/observers/memoryless.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/observers/memoryless.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_config.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/quant_config.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/quant_scheme.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/quant_scheme.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/quantization/utils/helpers.py` & `compressed-tensors-0.3.3/src/compressed_tensors/quantization/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,12 +104,13 @@
             try:
                 uncompressed_bits = torch.finfo(parameter.dtype).bits
             except TypeError:
                 uncompressed_bits = torch.iinfo(parameter.dtype).bits
             compressed_bits = uncompressed_bits
             if is_module_quantized(submodule):
                 compressed_bits = submodule.quantization_scheme.weights.num_bits
+
             num_weights = parameter.numel()
             total_compressed += compressed_bits * num_weights
             total_uncompressed += uncompressed_bits * num_weights
 
     return total_uncompressed / total_compressed
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/registry/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/registry/registry.py` & `compressed-tensors-0.3.3/src/compressed_tensors/registry/registry.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/utils/__init__.py` & `compressed-tensors-0.3.3/src/compressed_tensors/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors/utils/safetensors_load.py` & `compressed-tensors-0.3.3/src/compressed_tensors/utils/safetensors_load.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors.egg-info/PKG-INFO` & `compressed-tensors-0.3.3/src/compressed_tensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: compressed-tensors
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library for utilization of compressed safetensors of neural network models
 Home-page: https://github.com/neuralmagic/compressed-tensors
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# compressed-tensors
+# compressed_tensors
 
 This repository extends a [safetensors](https://github.com/huggingface/safetensors) format to efficiently store sparse and/or quantized tensors on disk. `compressed-tensors` format supports multiple compression types to minimize the disk space and facilitate the tensor manipulation.
 
 ## Motivation
 
 ### Reduce disk space by saving sparse tensors in a compressed format
 
@@ -93,8 +93,7 @@
 # load compressed model weights (`dict` turns generator into a dictionary)
 state_dict = dict(load_compressed("compressed_model.safetensors", compression_config))
 ```
 
 For more in-depth tutorial on bitmask compression, refer to the [notebook](https://github.com/neuralmagic/compressed-tensors/blob/d707c5b84bc3fef164aebdcd97cb6eaa571982f8/examples/bitmask_compression.ipynb).
 
 
-
```

### Comparing `compressed-tensors-0.3.2/src/compressed_tensors.egg-info/SOURCES.txt` & `compressed-tensors-0.3.3/src/compressed_tensors.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,10 +35,11 @@
 src/compressed_tensors/quantization/observers/memoryless.py
 src/compressed_tensors/quantization/observers/min_max.py
 src/compressed_tensors/quantization/utils/__init__.py
 src/compressed_tensors/quantization/utils/helpers.py
 src/compressed_tensors/registry/__init__.py
 src/compressed_tensors/registry/registry.py
 src/compressed_tensors/utils/__init__.py
+src/compressed_tensors/utils/helpers.py
 src/compressed_tensors/utils/safetensors_load.py
 tests/test_bitmask.py
 tests/test_registry.py
```

### Comparing `compressed-tensors-0.3.2/tests/test_bitmask.py` & `compressed-tensors-0.3.3/tests/test_bitmask.py`

 * *Files identical despite different names*

### Comparing `compressed-tensors-0.3.2/tests/test_registry.py` & `compressed-tensors-0.3.3/tests/test_registry.py`

 * *Files identical despite different names*

