# Comparing `tmp/pydvl-0.9.1.tar.gz` & `tmp/pydvl-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvl-0.9.1.tar", last modified: Mon Apr 22 09:35:46 2024, max compression
+gzip compressed data, was "pydvl-0.9.2.tar", last modified: Tue May  7 13:38:22 2024, max compression
```

## Comparing `pydvl-0.9.1.tar` & `pydvl-0.9.2.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.826394 pydvl-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 09:34:20.000000 pydvl-0.9.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 09:34:20.000000 pydvl-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 09:34:20.000000 pydvl-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 09:35:46.826394 pydvl-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-22 09:34:20.000000 pydvl-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-22 09:34:21.000000 pydvl-0.9.1/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-22 09:34:21.000000 pydvl-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 09:34:21.000000 pydvl-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:35:46.826394 pydvl-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-22 09:34:21.000000 pydvl-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.806394 pydvl-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.826394 pydvl-0.9.1/src/pyDVL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/influence/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/base_influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28378 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/influence_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/influence/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38897 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    64263 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/pre_conditioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/joblib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/futures/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/futures/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/utils/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/games.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/least_core/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/loo/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/loo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/loo/loo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/oob/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/oob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/oob/oob.py
--rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33246 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/semivalues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/shapley/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/classwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/owen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/truncated.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28615 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-22 09:34:21.000000 pydvl-0.9.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-22 09:34:21.000000 pydvl-0.9.1/tests/test_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.773841 pydvl-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 13:37:01.000000 pydvl-0.9.2/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 13:37:01.000000 pydvl-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 13:37:01.000000 pydvl-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-07 13:38:22.773841 pydvl-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-05-07 13:37:01.000000 pydvl-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-07 13:37:01.000000 pydvl-0.9.2/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-07 13:37:01.000000 pydvl-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 13:37:01.000000 pydvl-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:38:22.773841 pydvl-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-07 13:37:01.000000 pydvl-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.757841 pydvl-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/src/pyDVL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 13:38:22.000000 pydvl-0.9.2/src/pyDVL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/influence/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/base_influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29176 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/influence_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/influence/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38897 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/torch/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67570 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/torch/influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/torch/pre_conditioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20664 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/influence/torch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/parallel/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/backends/joblib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/backends/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.761841 pydvl-0.9.2/src/pydvl/parallel/futures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/futures/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/parallel/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.765841 pydvl-0.9.2/src/pydvl/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/reporting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/reporting/scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.765841 pydvl-0.9.2/src/pydvl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.765841 pydvl-0.9.2/src/pydvl/utils/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/caching/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/utils/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.765841 pydvl-0.9.2/src/pydvl/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/games.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/src/pydvl/value/least_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/least_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/least_core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/least_core/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/least_core/naive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/src/pydvl/value/loo/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/loo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/loo/loo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/src/pydvl/value/oob/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/oob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/oob/oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33246 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/semivalues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/src/pydvl/value/shapley/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/owen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/shapley/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28615 2024-05-07 13:37:01.000000 pydvl-0.9.2/src/pydvl/value/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:38:22.769841 pydvl-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 13:37:01.000000 pydvl-0.9.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-05-07 13:37:01.000000 pydvl-0.9.2/tests/test_results.py
```

### Comparing `pydvl-0.9.1/COPYING.LESSER` & `pydvl-0.9.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/LICENSE` & `pydvl-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/PKG-INFO` & `pydvl-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDVL
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Python Data Valuation Library
 Author: appliedAI Institute gGmbH
 Project-URL: Source, https://github.com/aai-institute/pydvl
 Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.9.1 Summary: The Python Data
+Metadata-Version: 2.1 Name: pyDVL Version: 0.9.2 Summary: The Python Data
 Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
 //github.com/aai-institute/pydvl Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `pydvl-0.9.1/README.md` & `pydvl-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/logo.svg` & `pydvl-0.9.2/logo.svg`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/pyproject.toml` & `pydvl-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/setup.py` & `pydvl-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="pyDVL",
     package_dir={"": "src"},
     package_data={"pydvl": ["py.typed"]},
     packages=find_packages(where="src"),
     include_package_data=True,
-    version="0.9.1",
+    version="0.9.2",
     description="The Python Data Valuation Library",
     install_requires=[
         line
         for line in open("requirements.txt").readlines()
         if not line.startswith("--")
     ],
     setup_requires=["wheel"],
```

### Comparing `pydvl-0.9.1/src/pyDVL.egg-info/PKG-INFO` & `pydvl-0.9.2/src/pyDVL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDVL
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Python Data Valuation Library
 Author: appliedAI Institute gGmbH
 Project-URL: Source, https://github.com/aai-institute/pydvl
 Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.9.1 Summary: The Python Data
+Metadata-Version: 2.1 Name: pyDVL Version: 0.9.2 Summary: The Python Data
 Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
 //github.com/aai-institute/pydvl Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `pydvl-0.9.1/src/pyDVL.egg-info/SOURCES.txt` & `pydvl-0.9.2/src/pyDVL.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/pydvl/parallel/futures/ray.py
 src/pydvl/reporting/__init__.py
 src/pydvl/reporting/plots.py
 src/pydvl/reporting/scores.py
 src/pydvl/utils/__init__.py
 src/pydvl/utils/config.py
 src/pydvl/utils/dataset.py
+src/pydvl/utils/exceptions.py
 src/pydvl/utils/functional.py
 src/pydvl/utils/numeric.py
 src/pydvl/utils/progress.py
 src/pydvl/utils/score.py
 src/pydvl/utils/status.py
 src/pydvl/utils/types.py
 src/pydvl/utils/utility.py
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/__init__.py` & `pydvl-0.9.2/src/pydvl/influence/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/influence/array.py` & `pydvl-0.9.2/src/pydvl/influence/array.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,33 @@
 This module provides classes and utilities for handling large arrays that are chunked
 and lazily evaluated. It includes abstract base classes for converting between tensor
 types and NumPy arrays, aggregating blocks of data, and abstract representations of
 lazy arrays. Concrete implementations are provided for handling chunked lazy arrays
 (chunked in one resp. two dimensions), with support for efficient storage and retrieval
 using the Zarr library.
 """
+from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
-from typing import Callable, Generator, Generic, List, Optional, Tuple, Union
+from typing import (
+    Callable,
+    Generator,
+    Generic,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+)
 
 import zarr
 from numpy.typing import NDArray
+from tqdm import tqdm
 from zarr.storage import StoreLike
 
 from ..utils import log_duration
 from .base_influence_function_model import TensorType
 
 
 class NumpyConverter(Generic[TensorType], ABC):
@@ -31,99 +43,123 @@
     @abstractmethod
     def from_numpy(self, x: NDArray) -> TensorType:
         """Override this method for converting a numpy array into a TensorType object"""
 
 
 class SequenceAggregator(Generic[TensorType], ABC):
     @abstractmethod
-    def __call__(self, tensor_generator: Generator[TensorType, None, None]):
+    def __call__(
+        self,
+        tensor_sequence: LazyChunkSequence,
+    ):
         """
-        Aggregates tensors from a generator.
+        Aggregates tensors from a sequence.
 
         Implement this method to define how a sequence of tensors, provided by a
         generator, should be combined.
         """
 
 
 class ListAggregator(SequenceAggregator):
     def __call__(
-        self, tensor_generator: Generator[TensorType, None, None]
+        self,
+        tensor_sequence: LazyChunkSequence,
     ) -> List[TensorType]:
         """
         Aggregates tensors from a single-level generator into a list. This method simply
         collects each tensor emitted by the generator into a single list.
 
         Args:
-            tensor_generator: A generator that yields TensorType objects.
+            tensor_sequence: Object wrapping a generator that yields `TensorType`
+                objects.
 
         Returns:
             A list containing all the tensors provided by the tensor_generator.
         """
-        return [t for t in tensor_generator]
+
+        gen = cast(Iterator[TensorType], tensor_sequence.generator_factory())
+
+        if tensor_sequence.len_generator is not None:
+            gen = cast(
+                Iterator[TensorType],
+                tqdm(gen, total=tensor_sequence.len_generator, desc="Blocks"),
+            )
+
+        return [t for t in gen]
 
 
 class NestedSequenceAggregator(Generic[TensorType], ABC):
     @abstractmethod
-    def __call__(
-        self,
-        nested_generators_of_tensors: Generator[
-            Generator[TensorType, None, None], None, None
-        ],
-    ):
+    def __call__(self, nested_sequence_of_tensors: NestedLazyChunkSequence):
         """
-        Aggregates tensors from a generator of generators.
+        Aggregates tensors from a nested sequence of tensors.
 
         Implement this method to specify how tensors, nested in two layers of
         generators, should be combined. Useful for complex data structures where tensors
         are not directly accessible in a flat list.
         """
 
 
 class NestedListAggregator(NestedSequenceAggregator):
     def __call__(
         self,
-        nested_generators_of_tensors: Generator[
-            Generator[TensorType, None, None], None, None
-        ],
+        nested_sequence_of_tensors: NestedLazyChunkSequence,
     ) -> List[List[TensorType]]:
         """
          Aggregates tensors from a nested generator structure into a list of lists.
          Each inner generator is converted into a list of tensors, resulting in a nested
          list structure.
 
          Args:
-             nested_generators_of_tensors: A generator of generators, where each inner
-                generator yields TensorType objects.
+             nested_sequence_of_tensors: Object wrapping a generator of generators,
+                where each inner generator yields TensorType objects.
 
         Returns:
             A list of lists, where each inner list contains tensors returned from one
                 of the inner generators.
         """
-        return [list(tensor_gen) for tensor_gen in nested_generators_of_tensors]
+        outer_gen = cast(
+            Iterator[Iterator[TensorType]],
+            nested_sequence_of_tensors.generator_factory(),
+        )
+        len_outer_gen = nested_sequence_of_tensors.len_outer_generator
+        if len_outer_gen is not None:
+            outer_gen = cast(
+                Iterator[Iterator[TensorType]],
+                tqdm(outer_gen, total=len_outer_gen, desc="Row blocks"),
+            )
 
+        return [list(tensor_gen) for tensor_gen in outer_gen]
 
-class LazyChunkSequence:
+
+class LazyChunkSequence(Generic[TensorType]):
     """
     A class representing a chunked, and lazily evaluated array,
     where the chunking is restricted to the first dimension
 
     This class is designed to handle large arrays that don't fit in memory.
     It works by generating chunks of the array on demand and can
     also convert these chunks to a Zarr array
     for efficient storage and retrieval.
 
     Attributes:
         generator_factory: A factory function that returns
             a generator. This generator yields chunks of the large array when called.
+        len_generator: if the number of elements from the generator is
+            known from the context, this optional parameter can be used to improve
+            logging by adding a progressbar.
     """
 
     def __init__(
-        self, generator_factory: Callable[[], Generator[TensorType, None, None]]
+        self,
+        generator_factory: Callable[[], Generator[TensorType, None, None]],
+        len_generator: Optional[int] = None,
     ):
         self.generator_factory = generator_factory
+        self.len_generator = len_generator
 
     @log_duration(log_level=logging.INFO)
     def compute(self, aggregator: Optional[SequenceAggregator] = None):
         """
         Computes and optionally aggregates the chunks of the array using the provided
         aggregator. This method initiates the generation of chunks and then
         combines them according to the aggregator's logic.
@@ -136,15 +172,15 @@
         Returns:
             The aggregated result of all chunks of the array, the format of which
                 depends on the aggregator used.
 
         """
         if aggregator is None:
             aggregator = ListAggregator()
-        return aggregator(self.generator_factory())
+        return aggregator(self)
 
     @log_duration(log_level=logging.INFO)
     def to_zarr(
         self,
         path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
@@ -167,15 +203,23 @@
                 If False, an error is raised in case of existing data.
 
         Returns:
             The Zarr array if return_stored is True; otherwise, None.
         """
         row_idx = 0
         z = None
-        for block in self.generator_factory():
+
+        gen = cast(Iterator[TensorType], self.generator_factory())
+
+        if self.len_generator is not None:
+            gen = cast(
+                Iterator[TensorType], tqdm(gen, total=self.len_generator, desc="Blocks")
+            )
+
+        for block in gen:
             numpy_block = converter.to_numpy(block)
 
             if z is None:
                 z = self._initialize_zarr_array(numpy_block, path_or_url, overwrite)
 
             new_shape = self._new_shape_according_to_block(numpy_block, row_idx)
             z.resize(new_shape)
@@ -200,36 +244,41 @@
             mode="w" if overwrite else "w-",
             shape=initial_shape,
             chunks=block.shape,
             dtype=block.dtype,
         )
 
 
-class NestedLazyChunkSequence:
+class NestedLazyChunkSequence(Generic[TensorType]):
     """
     A class representing chunked, and lazily evaluated array, where the chunking is
     restricted to the first two dimensions.
 
     This class is designed for handling large arrays where individual chunks are
     loaded and processed lazily. It supports converting these chunks into a Zarr array
     for efficient storage and retrieval, with chunking applied along the first two
     dimensions.
 
     Attributes:
         generator_factory: A factory function that returns a generator of generators.
-            Each inner generator yields chunks.
+            Each inner generator yields chunks
+        len_outer_generator: if the number of elements from the outer generator is
+            known from the context, this optional parameter can be used to improve
+            logging by adding a progressbar.
     """
 
     def __init__(
         self,
         generator_factory: Callable[
             [], Generator[Generator[TensorType, None, None], None, None]
         ],
+        len_outer_generator: Optional[int] = None,
     ):
         self.generator_factory = generator_factory
+        self.len_outer_generator = len_outer_generator
 
     @log_duration(log_level=logging.INFO)
     def compute(self, aggregator: Optional[NestedSequenceAggregator] = None):
         """
         Computes and optionally aggregates the chunks of the array using the provided
         aggregator. This method initiates the generation of chunks and then
         combines them according to the aggregator's logic.
@@ -243,15 +292,15 @@
         Returns:
             The aggregated result of all chunks of the array, the format of which
             depends on the aggregator used.
 
         """
         if aggregator is None:
             aggregator = NestedListAggregator()
-        return aggregator(self.generator_factory())
+        return aggregator(self)
 
     @log_duration(log_level=logging.INFO)
     def to_zarr(
         self,
         path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
@@ -276,15 +325,25 @@
         Returns:
             The Zarr array if return_stored is True; otherwise, None.
         """
 
         row_idx = 0
         z = None
         numpy_block = None
-        for row_blocks in self.generator_factory():
+        block_generator = cast(Iterator[Iterator[TensorType]], self.generator_factory())
+
+        if self.len_outer_generator is not None:
+            block_generator = cast(
+                Iterator[Iterator[TensorType]],
+                tqdm(
+                    block_generator, total=self.len_outer_generator, desc="Row blocks"
+                ),
+            )
+
+        for row_blocks in block_generator:
             col_idx = 0
             for block in row_blocks:
                 numpy_block = converter.to_numpy(block)
                 if z is None:
                     z = self._initialize_zarr_array(numpy_block, path_or_url, overwrite)
                 new_shape = self._new_shape_according_to_block(
                     z, numpy_block, row_idx, col_idx
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/base_influence_function_model.py` & `pydvl-0.9.2/src/pydvl/influence/base_influence_function_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Collection, Generic, Iterable, Optional, Type, TypeVar
 
+__all__ = ["InfluenceMode"]
+
 
 class InfluenceMode(str, Enum):
     """
     Enum representation for the types of influence.
 
     Attributes:
         Up: [Approximating the influence of a point]
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/influence_calculator.py` & `pydvl-0.9.2/src/pydvl/influence/influence_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The computation is based on a chunk computation model in the form of an instance of
 [InfluenceFunctionModel][pydvl.influence.base_influence_function_model.InfluenceFunctionModel],
 which is mapped over collection of chunks.
 """
 
 import logging
 from functools import partial
-from typing import Generator, Iterable, Optional, Tuple, Type, Union
+from typing import Generator, Iterable, Optional, Sized, Tuple, Type, Union, cast
 
 import distributed
 from dask import array as da
 from dask import delayed
 from distributed import Client
 from numpy.typing import NDArray
 
@@ -615,16 +615,22 @@
             data_iterable: An iterable that returns tuples of tensors.
                 Each tuple consists of a pair of tensors (x, y), representing input data
                 and corresponding targets.
 
         Returns:
             A lazy data structure representing the chunks of the resulting tensor
         """
+        try:
+            len_iterable = len(cast(Sized, data_iterable))
+        except Exception as e:
+            logger.debug(f"Failed to retrieve len of data iterable: {e}")
+            len_iterable = None
+
         tensors_gen_factory = partial(self._influence_factors_gen, data_iterable)
-        return LazyChunkSequence(tensors_gen_factory)
+        return LazyChunkSequence(tensors_gen_factory, len_generator=len_iterable)
 
     def _influences_gen(
         self,
         test_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         train_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         mode: InfluenceMode,
     ) -> Generator[Generator[TensorType, None, None], None, None]:
@@ -673,15 +679,23 @@
         nested_tensor_gen_factory = partial(
             self._influences_gen,
             test_data_iterable,
             train_data_iterable,
             mode,
         )
 
-        return NestedLazyChunkSequence(nested_tensor_gen_factory)
+        try:
+            len_iterable = len(cast(Sized, test_data_iterable))
+        except Exception as e:
+            logger.debug(f"Failed to retrieve len of test data iterable: {e}")
+            len_iterable = None
+
+        return NestedLazyChunkSequence(
+            nested_tensor_gen_factory, len_outer_generator=len_iterable
+        )
 
     def _influences_from_factors_gen(
         self,
         z_test_factors: Iterable[TensorType],
         train_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         mode: InfluenceMode,
     ):
@@ -731,8 +745,17 @@
         """
         nested_tensor_gen = partial(
             self._influences_from_factors_gen,
             z_test_factors,
             train_data_iterable,
             mode,
         )
-        return NestedLazyChunkSequence(nested_tensor_gen)
+
+        try:
+            len_iterable = len(cast(Sized, z_test_factors))
+        except Exception as e:
+            logger.debug(f"Failed to retrieve len of factors iterable: {e}")
+            len_iterable = None
+
+        return NestedLazyChunkSequence(
+            nested_tensor_gen, len_outer_generator=len_iterable
+        )
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/torch/functional.py` & `pydvl-0.9.2/src/pydvl/influence/torch/functional.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/influence/torch/influence_function_model.py` & `pydvl-0.9.2/src/pydvl/influence/torch/influence_function_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,26 @@
     model_hessian_nystroem_approximation,
 )
 from .pre_conditioner import PreConditioner
 from .util import (
     EkfacRepresentation,
     empirical_cross_entropy_loss_fn,
     flatten_dimensions,
+    safe_torch_linalg_eigh,
 )
 
+__all__ = [
+    "DirectInfluence",
+    "CgInfluence",
+    "LissaInfluence",
+    "ArnoldiInfluence",
+    "EkfacInfluence",
+    "NystroemSketchInfluence",
+]
+
 logger = logging.getLogger(__name__)
 
 
 class TorchInfluenceFunctionModel(
     InfluenceFunctionModel[torch.Tensor, DataLoader], ABC
 ):
     """
@@ -299,21 +309,21 @@
 
         Returns:
             Tensor representing the element-wise scalar products for the provided batch
 
         """
         if mode == InfluenceMode.Up:
             return (
-                z_test_factors
+                z_test_factors.to(self.model_device)
                 @ self._loss_grad(x.to(self.model_device), y.to(self.model_device)).T
             )
         elif mode == InfluenceMode.Perturbation:
             return torch.einsum(
                 "ia,j...a->ij...",
-                z_test_factors,
+                z_test_factors.to(self.model_device),
                 self._flat_loss_mixed_grad(
                     x.to(self.model_device), y.to(self.model_device)
                 ),
             )
         else:
             raise UnsupportedInfluenceModeException(mode)
 
@@ -451,23 +461,27 @@
               the scalar loss.
         hessian_regularization: Optional regularization parameter added
             to the Hessian-vector product for numerical stability.
         x0: Initial guess for hvp. If None, defaults to b.
         rtol: Maximum relative tolerance of result.
         atol: Absolute tolerance of result.
         maxiter: Maximum number of iterations. If None, defaults to 10*len(b).
-        progress: If True, display progress bars.
+        progress: If True, display progress bars for computing in the non-block mode
+            (use_block_cg=False).
         precompute_grad: If True, the full data gradient is precomputed and kept
             in memory, which can speed up the hessian vector product computation.
             Set this to False, if you can't afford to keep the full computation graph
             in memory.
         pre_conditioner: Optional pre-conditioner to improve convergence of conjugate
             gradient method
         use_block_cg: If True, use block variant of conjugate gradient method, which
             solves several right hand sides simultaneously
+        warn_on_max_iteration: If True, logs a warning, if the desired tolerance is not
+            achieved within `maxiter` iterations. If False, the log level for this
+            information is `logging.DEBUG`
 
     """
 
     def __init__(
         self,
         model: nn.Module,
         loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
@@ -476,16 +490,18 @@
         rtol: float = 1e-7,
         atol: float = 1e-7,
         maxiter: Optional[int] = None,
         progress: bool = False,
         precompute_grad: bool = False,
         pre_conditioner: Optional[PreConditioner] = None,
         use_block_cg: bool = False,
+        warn_on_max_iteration: bool = True,
     ):
         super().__init__(model, loss)
+        self.warn_on_max_iteration = warn_on_max_iteration
         self.use_block_cg = use_block_cg
         self.pre_conditioner = pre_conditioner
         self.precompute_grad = precompute_grad
         self.progress = progress
         self.maxiter = maxiter
         self.atol = atol
         self.rtol = rtol
@@ -648,14 +664,15 @@
         if self.pre_conditioner is not None:
             p = z0 = self.pre_conditioner.solve(r0)
         else:
             p = z0 = r0
 
         for k in range(maxiter):
             if torch.norm(r0) < tol:
+                logger.debug(f"Terminated cg after {k} iterations with residuum={r0}")
                 break
             Ap = hvp(p)
             alpha = torch.dot(r0, z0) / torch.dot(p, Ap)
             x += alpha * p
             r = r0 - alpha * Ap
 
             if self.pre_conditioner is not None:
@@ -664,14 +681,24 @@
                 z = r
 
             beta = torch.dot(r, z) / torch.dot(r0, z0)
 
             r0 = r
             p = z + beta * p
             z0 = z
+        else:
+            log_level = logging.WARNING if self.warn_on_max_iteration else logging.DEBUG
+            logger.log(
+                log_level,
+                f"Reached max number of iterations {maxiter=} without "
+                f"achieving the desired tolerance {tol}. \n"
+                f"Achieved residuum is {torch.norm(r0)}.\n"
+                f"Consider increasing 'maxiter', the desired tolerance or the "
+                f"parameter 'hessian_regularization'.",
+            )
 
         return x
 
     def _solve_pbcg(
         self,
         rhs: torch.Tensor,
     ):
@@ -702,15 +729,17 @@
             )(x)
 
         X = torch.clone(rhs.T)
 
         R = (rhs - mat_mat(X)).T
         Z = R if self.pre_conditioner is None else self.pre_conditioner.solve(R)
         P, _, _ = torch.linalg.svd(Z, full_matrices=False)
-        active_indices = torch.as_tensor(list(range(X.shape[-1])), dtype=torch.long)
+        active_indices = torch.as_tensor(
+            list(range(X.shape[-1])), dtype=torch.long, device=self.model_device
+        )
 
         maxiter = self.maxiter if self.maxiter is not None else len(rhs) * 10
         y_norm = torch.linalg.norm(rhs, dim=1)
         tol = torch.clamp(self.rtol**2 * y_norm, min=self.atol**2)
 
         # In the case the parameter dimension is smaller than the number of right
         # hand sides, we do not shrink the indices due to resulting wrong
@@ -730,14 +759,18 @@
             num_remaining_indices = non_finished_indices.numel()
             non_finished_indices = non_finished_indices.squeeze()
 
             if num_remaining_indices == 1:
                 non_finished_indices = non_finished_indices.unsqueeze(-1)
 
             if num_remaining_indices == 0:
+                logger.debug(
+                    f"Terminated block cg after {k} iterations with max "
+                    f"residuum={B.max()}"
+                )
                 break
 
             # Reduce problem size by removing finished columns from the iteration
             if shrink_finished_indices:
                 active_indices = active_indices[non_finished_indices]
                 R = R[:, non_finished_indices]
                 P = P[:, non_finished_indices]
@@ -751,17 +784,33 @@
 
             if Z_tmp.ndim == 1:
                 Z_tmp = Z_tmp.unsqueeze(-1)
 
             # Orthogonalization search directions to stabilize the action of
             # (P^tAP)^{-1}
             P, _, _ = torch.linalg.svd(Z_tmp, full_matrices=False)
+        else:
+            log_level = logging.WARNING if self.warn_on_max_iteration else logging.DEBUG
+            logger.log(
+                log_level,
+                f"Reached max number of iterations {maxiter=} of block cg "
+                f"without achieving the desired tolerance {tol.min()}. \n"
+                f"Achieved max residuum is "
+                f"{torch.linalg.norm(R, dim=0).max()}.\n"
+                f"Consider increasing 'maxiter', the desired tolerance or "
+                f"the parameter 'hessian_regularization'.",
+            )
 
         return X.T
 
+    def to(self, device: torch.device):
+        if self.pre_conditioner is not None:
+            self.pre_conditioner = self.pre_conditioner.to(device)
+        return super().to(device)
+
 
 class LissaInfluence(TorchInfluenceFunctionModel):
     r"""
     Uses LISSA, Linear time Stochastic Second-Order Algorithm, to iteratively
     approximate the inverse Hessian. More precisely, it finds x s.t. \(Hx = b\),
     with \(H\) being the model's second derivative wrt. the parameters.
     This is done with the update
@@ -782,29 +831,34 @@
             to the Hessian-vector product for numerical stability.
         maxiter: Maximum number of iterations.
         dampen: Dampening factor, defaults to 0 for no dampening.
         scale: Scaling factor, defaults to 10.
         h0: Initial guess for hvp.
         rtol: tolerance to use for early stopping
         progress: If True, display progress bars.
+        warn_on_max_iteration: If True, logs a warning, if the desired tolerance is not
+            achieved within `maxiter` iterations. If False, the log level for this
+            information is `logging.DEBUG`
     """
 
     def __init__(
         self,
         model: nn.Module,
         loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
         hessian_regularization: float = 0.0,
         maxiter: int = 1000,
         dampen: float = 0.0,
         scale: float = 10.0,
         h0: Optional[torch.Tensor] = None,
         rtol: float = 1e-4,
         progress: bool = False,
+        warn_on_max_iteration: bool = True,
     ):
         super().__init__(model, loss)
+        self.warn_on_max_iteration = warn_on_max_iteration
         self.maxiter = maxiter
         self.hessian_regularization = hessian_regularization
         self.progress = progress
         self.rtol = rtol
         self.h0 = h0
         self.scale = scale
         self.dampen = dampen
@@ -851,35 +905,46 @@
         model_params = {
             k: p.detach() for k, p in self.model.named_parameters() if p.requires_grad
         }
         b_hvp = torch.vmap(
             create_batch_hvp_function(self.model, self.loss),
             in_dims=(None, None, None, 0),
         )
-        for _ in tqdm(range(self.maxiter), disable=not self.progress, desc="Lissa"):
+        for k in tqdm(
+            range(self.maxiter), disable=not self.progress, desc="Lissa iteration"
+        ):
             x, y = next(iter(shuffled_training_data))
             x = x.to(self.model_device)
             y = y.to(self.model_device)
             reg_hvp = (
                 lambda v: b_hvp(model_params, x, y, v) + self.hessian_regularization * v
             )
             residual = lissa_step(h_estimate, reg_hvp) - h_estimate
             h_estimate += residual
             if torch.isnan(h_estimate).any():
                 raise RuntimeError("NaNs in h_estimate. Increase scale or dampening.")
             max_residual = torch.max(torch.abs(residual / h_estimate))
             if max_residual < self.rtol:
+                mean_residual = torch.mean(torch.abs(residual / h_estimate))
+                logger.debug(
+                    f"Terminated Lissa after {k} iterations with "
+                    f"{max_residual*100:.2f} % max residual and"
+                    f" mean residual {mean_residual*100:.5f} %"
+                )
                 break
-
-        mean_residual = torch.mean(torch.abs(residual / h_estimate))
-
-        logger.info(
-            f"Terminated Lissa with {max_residual*100:.2f} % max residual."
-            f" Mean residual: {mean_residual*100:.5f} %"
-        )
+        else:
+            mean_residual = torch.mean(torch.abs(residual / h_estimate))
+            log_level = logging.WARNING if self.warn_on_max_iteration else logging.DEBUG
+            logger.log(
+                log_level,
+                f"Reached max number of iterations {self.maxiter} without "
+                f"achieving the desired tolerance {self.rtol}.\n "
+                f"Achieved max residual {max_residual*100:.2f} % and"
+                f" {mean_residual*100:.5f} % mean residual",
+            )
         return h_estimate / self.scale
 
 
 class ArnoldiInfluence(TorchInfluenceFunctionModel):
     r"""
     Solves the linear system Hx = b, where H is the Hessian of the model's loss function
     and b is the given right-hand side vector.
@@ -1191,15 +1256,15 @@
             hooks.append(module.register_forward_hook(layer_input_hook))
             hooks.append(module.register_full_backward_hook(layer_grad_hook))
 
         for x, *_ in tqdm(
             data, disable=not self.progress, desc="K-FAC blocks - batch progress"
         ):
             data_len += x.shape[0]
-            pred_y = self.model(x)
+            pred_y = self.model(x.to(self.model_device))
             loss = empirical_cross_entropy_loss_fn(pred_y)
             loss.backward()
 
         for key in forward_x.keys():
             forward_x[key] /= data_len
             grad_y[key] /= data_len
 
@@ -1216,16 +1281,16 @@
         each layer, their eigenvalue decomposition and diagonal values.
         """
         forward_x, grad_y = self._get_kfac_blocks(data)
         layers_evecs_a = {}
         layers_evect_g = {}
         layers_diags = {}
         for key in self.active_layers.keys():
-            evals_a, evecs_a = torch.linalg.eigh(forward_x[key])
-            evals_g, evecs_g = torch.linalg.eigh(grad_y[key])
+            evals_a, evecs_a = safe_torch_linalg_eigh(forward_x[key])
+            evals_g, evecs_g = safe_torch_linalg_eigh(grad_y[key])
             layers_evecs_a[key] = evecs_a
             layers_evect_g[key] = evecs_g
             layers_diags[key] = torch.kron(evals_g.view(-1, 1), evals_a.view(-1, 1))
 
         self.ekfac_representation = EkfacRepresentation(
             self.active_layers.keys(),
             self.active_layers.values(),
@@ -1315,15 +1380,15 @@
             hooks.append(module.register_forward_hook(input_hook))
             hooks.append(module.register_full_backward_hook(grad_hook))
 
         for x, *_ in tqdm(
             data, disable=not self.progress, desc="Update Diagonal - batch progress"
         ):
             data_len += x.shape[0]
-            pred_y = self.model(x)
+            pred_y = self.model(x.to(self.model_device))
             loss = empirical_cross_entropy_loss_fn(pred_y)
             loss.backward()
 
         for key in diags.keys():
             diags[key] /= data_len
 
         for hook in hooks:
@@ -1522,28 +1587,31 @@
             total_grad = self._loss_grad(
                 x.to(self.model_device), y.to(self.model_device)
             )
             start_idx = 0
             influences = {}
             for layer_id, layer_z_test in z_test_factors.items():
                 end_idx = start_idx + layer_z_test.shape[1]
-                influences[layer_id] = layer_z_test @ total_grad[:, start_idx:end_idx].T
+                influences[layer_id] = (
+                    layer_z_test.to(self.model_device)
+                    @ total_grad[:, start_idx:end_idx].T
+                )
                 start_idx = end_idx
             return influences
         elif mode == InfluenceMode.Perturbation:
             total_mixed_grad = self._flat_loss_mixed_grad(
                 x.to(self.model_device), y.to(self.model_device)
             )
             start_idx = 0
             influences = {}
             for layer_id, layer_z_test in z_test_factors.items():
                 end_idx = start_idx + layer_z_test.shape[1]
                 influences[layer_id] = torch.einsum(
                     "ia,j...a->ij...",
-                    layer_z_test,
+                    layer_z_test.to(self.model_device),
                     total_mixed_grad[:, start_idx:end_idx],
                 )
                 start_idx = end_idx
             return influences
         else:
             raise UnsupportedInfluenceModeException(mode)
 
@@ -1622,15 +1690,15 @@
             regularization_values: list of regularization values to use
 
         Returns:
             A dictionary containing with keys being the regularization values and values
             being dictionaries containing the influences for each layer of the model,
             with the layer name as key.
         """
-        grad = self._loss_grad(x, y)
+        grad = self._loss_grad(x.to(self.model_device), y.to(self.model_device))
         influences_by_reg_value = {}
         for reg_value in regularization_values:
             reg_factors = self._solve_hvp_by_layer(
                 grad, self.ekfac_representation, reg_value
             )
             values = {}
             start_idx = 0
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/torch/pre_conditioner.py` & `pydvl-0.9.2/src/pydvl/influence/torch/pre_conditioner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import Callable, Optional
 
 import torch
 
 from ..base_influence_function_model import NotFittedException
 from .functional import LowRankProductRepresentation, randomized_nystroem_approximation
@@ -66,14 +68,19 @@
 
         return self._solve(rhs)
 
     @abstractmethod
     def _solve(self, rhs: torch.Tensor):
         pass
 
+    @abstractmethod
+    def to(self, device: torch.device) -> PreConditioner:
+        """Implement this to move the (potentially fitted) preconditioner to a
+        specific device"""
+
 
 class JacobiPreConditioner(PreConditioner):
     r"""
     Pre-conditioner for improving the convergence of CG for systems of the form
 
     $$ ( A + \lambda \operatorname{I})x = \operatorname{rhs} $$
 
@@ -137,14 +144,19 @@
         inv_diag = 1.0 / (self._diag + self._reg)
 
         if rhs.ndim == 1:
             return rhs * inv_diag
 
         return rhs * inv_diag.unsqueeze(-1)
 
+    def to(self, device: torch.device) -> JacobiPreConditioner:
+        if self._diag is not None:
+            self._diag = self._diag.to(device)
+        return self
+
 
 class NystroemPreConditioner(PreConditioner):
     r"""
     Pre-conditioner for improving the convergence of CG for systems of the form
 
     $$ (A + \lambda \operatorname{I})x = \operatorname{rhs} $$
 
@@ -229,7 +241,12 @@
 
         result += rhs_view - self._low_rank_approx.projections @ proj_rhs
 
         if rhs_is_one_dim:
             result = result.squeeze()
 
         return result
+
+    def to(self, device: torch.device) -> NystroemPreConditioner:
+        if self._low_rank_approx is not None:
+            self._low_rank_approx = self._low_rank_approx.to(device)
+        return self
```

### Comparing `pydvl-0.9.1/src/pydvl/influence/torch/util.py` & `pydvl-0.9.2/src/pydvl/influence/torch/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 import logging
 import math
 from dataclasses import dataclass
 from functools import partial
 from typing import (
     Collection,
     Dict,
-    Generator,
     Iterable,
+    Iterator,
     List,
     Mapping,
     Optional,
     Tuple,
     Type,
     Union,
+    cast,
 )
 
 import dask
 import numpy as np
 import torch
 from dask import array as da
 from numpy.typing import NDArray
 from torch.utils.data import Dataset
+from tqdm import tqdm
 
-from ..array import NestedSequenceAggregator, NumpyConverter, SequenceAggregator
+from ...utils.exceptions import catch_and_raise_exception
+from ..array import (
+    LazyChunkSequence,
+    NestedLazyChunkSequence,
+    NestedSequenceAggregator,
+    NumpyConverter,
+    SequenceAggregator,
+)
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "to_model_device",
     "TorchTensorContainerType",
     "align_structure",
     "align_with_model",
     "flatten_dimensions",
     "TorchNumpyConverter",
     "TorchCatAggregator",
     "NestedTorchCatAggregator",
     "torch_dataset_to_dask_array",
+    "EkfacRepresentation",
+    "empirical_cross_entropy_loss_fn",
 ]
 
 
 def to_model_device(x: torch.Tensor, model: torch.nn.Module) -> torch.Tensor:
     """
     Returns the tensor `x` moved to the device of the `model`, if device of model is set
 
@@ -292,19 +303,19 @@
                 logger.warning(
                     err_msg
                     + f" Using the provided total number of samples {total_size}."
                 )
                 return total_size
             else:
                 logger.warning(
-                    err_msg + f" Infer the number of samples from the dataset, "
-                    f"via iterating the dataset once. "
-                    f"This might induce severe overhead, so consider"
-                    f"providing total_size, if you know the number of samples "
-                    f"beforehand."
+                    err_msg + " Infer the number of samples from the dataset, "
+                    "via iterating the dataset once. "
+                    "This might induce severe overhead, so consider"
+                    "providing total_size, if you know the number of samples "
+                    "beforehand."
                 )
                 idx = 0
                 while True:
                     try:
                         t = d_set[idx]
                         if all(_t.numel() == 0 for _t in t):
                             return idx
@@ -394,62 +405,82 @@
 
 class TorchCatAggregator(SequenceAggregator[torch.Tensor]):
     """
     An aggregator that concatenates tensors using PyTorch's [torch.cat][torch.cat]
     function. Concatenation is done along the first dimension of the chunks.
     """
 
-    def __call__(self, tensor_generator: Generator[torch.Tensor, None, None]):
+    def __call__(
+        self,
+        tensor_sequence: LazyChunkSequence[torch.Tensor],
+    ):
         """
         Aggregates tensors from a single-level generator into a single tensor by
         concatenating them. This method is a straightforward way to combine a sequence
         of tensors into one larger tensor.
 
         Args:
-            tensor_generator: A generator that yields `torch.Tensor` objects.
+            tensor_sequence: Object wrapping a generator that yields `torch.Tensor`
+                objects.
 
         Returns:
             A single tensor formed by concatenating all tensors from the generator.
                 The concatenation is performed along the default dimension (0).
         """
-        return torch.cat(list(tensor_generator))
+        t_gen = cast(Iterator[torch.Tensor], tensor_sequence.generator_factory())
+        len_generator = tensor_sequence.len_generator
+        if len_generator is not None:
+            t_gen = cast(
+                Iterator[torch.Tensor], tqdm(t_gen, total=len_generator, desc="Blocks")
+            )
+
+        return torch.cat(list(t_gen))
 
 
 class NestedTorchCatAggregator(NestedSequenceAggregator[torch.Tensor]):
     """
     An aggregator that concatenates tensors using PyTorch's [torch.cat][torch.cat]
     function. Concatenation is done along the first two dimensions of the chunks.
     """
 
     def __call__(
-        self,
-        nested_generators_of_tensors: Generator[
-            Generator[torch.Tensor, None, None], None, None
-        ],
+        self, nested_sequence_of_tensors: NestedLazyChunkSequence[torch.Tensor]
     ):
         """
         Aggregates tensors from a nested generator structure into a single tensor by
         concatenating. Each inner generator is first concatenated along dimension 1 into
         a tensor, and then these tensors are concatenated along dimension 0 together to
         form the final tensor.
 
         Args:
-            nested_generators_of_tensors: A generator of generators, where each inner
-                generator yields `torch.Tensor` objects.
+            nested_sequence_of_tensors: Object wrapping a generator of generators,
+                where each inner generator yields `torch.Tensor` objects.
 
         Returns:
             A single tensor formed by concatenating all tensors from the nested
             generators.
 
         """
+
+        outer_gen = cast(
+            Iterator[Iterator[torch.Tensor]],
+            nested_sequence_of_tensors.generator_factory(),
+        )
+        len_outer_generator = nested_sequence_of_tensors.len_outer_generator
+        if len_outer_generator is not None:
+            outer_gen = cast(
+                Iterator[Iterator[torch.Tensor]],
+                tqdm(outer_gen, total=len_outer_generator, desc="Row blocks"),
+            )
+
         return torch.cat(
             list(
                 map(
                     lambda tensor_gen: torch.cat(list(tensor_gen), dim=1),
-                    nested_generators_of_tensors,
+                    outer_gen,
                 )
             )
         )
 
 
 @dataclass(frozen=True)
 class EkfacRepresentation:
@@ -517,7 +548,53 @@
     """
     probs_ = torch.softmax(model_output, dim=1)
     log_probs_ = torch.log(probs_)
     log_probs_ = torch.where(
         torch.isfinite(log_probs_), log_probs_, torch.zeros_like(log_probs_)
     )
     return torch.sum(log_probs_ * probs_.detach() ** 0.5)
+
+
+@catch_and_raise_exception(RuntimeError, lambda e: TorchLinalgEighException(e))
+def safe_torch_linalg_eigh(*args, **kwargs):
+    """
+    A wrapper around `torch.linalg.eigh` that safely handles potential runtime errors
+    by raising a custom `TorchLinalgEighException` with more context,
+    especially related to the issues reported in
+    [https://github.com/pytorch/pytorch/issues/92141](
+    https://github.com/pytorch/pytorch/issues/92141).
+
+    Args:
+        *args: Positional arguments passed to `torch.linalg.eigh`.
+        **kwargs: Keyword arguments passed to `torch.linalg.eigh`.
+
+    Returns:
+        The result of calling `torch.linalg.eigh` with the provided arguments.
+
+    Raises:
+        TorchLinalgEighException: If a `RuntimeError` occurs during the execution of
+            `torch.linalg.eigh`.
+    """
+    return torch.linalg.eigh(*args, **kwargs)
+
+
+class TorchLinalgEighException(Exception):
+    """
+    Exception to wrap a RunTimeError raised by torch.linalg.eigh, when used
+    with large matrices,
+    see [https://github.com/pytorch/pytorch/issues/92141](
+    https://github.com/pytorch/pytorch/issues/92141)
+    """
+
+    def __init__(self, original_exception: RuntimeError):
+        func = torch.linalg.eigh
+        err_msg = (
+            f"A RunTimeError occurred in '{func.__module__}.{func.__qualname__}'. "
+            "This might be related to known issues with "
+            "[torch.linalg.eigh][torch.linalg.eigh] on certain matrix sizes.\n "
+            "For more details, refer to "
+            "https://github.com/pytorch/pytorch/issues/92141. \n"
+            "In this case, consider to use a different implementation, which does not "
+            "depend on the usage of [torch.linalg.eigh][torch.linalg.eigh].\n"
+            f" Inspect the original exception message: \n{str(original_exception)}"
+        )
+        super().__init__(err_msg)
```

### Comparing `pydvl-0.9.1/src/pydvl/parallel/__init__.py` & `pydvl-0.9.2/src/pydvl/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/backend.py` & `pydvl-0.9.2/src/pydvl/parallel/backend.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/backends/joblib.py` & `pydvl-0.9.2/src/pydvl/parallel/backends/joblib.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/backends/ray.py` & `pydvl-0.9.2/src/pydvl/parallel/backends/ray.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/config.py` & `pydvl-0.9.2/src/pydvl/parallel/config.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/futures/__init__.py` & `pydvl-0.9.2/src/pydvl/parallel/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/futures/ray.py` & `pydvl-0.9.2/src/pydvl/parallel/futures/ray.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/parallel/map_reduce.py` & `pydvl-0.9.2/src/pydvl/parallel/map_reduce.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/reporting/plots.py` & `pydvl-0.9.2/src/pydvl/reporting/plots.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/reporting/scores.py` & `pydvl-0.9.2/src/pydvl/reporting/scores.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/__init__.py` & `pydvl-0.9.2/src/pydvl/utils/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/base.py` & `pydvl-0.9.2/src/pydvl/utils/caching/base.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/config.py` & `pydvl-0.9.2/src/pydvl/utils/caching/config.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/disk.py` & `pydvl-0.9.2/src/pydvl/utils/caching/disk.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/memcached.py` & `pydvl-0.9.2/src/pydvl/utils/caching/memcached.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/caching/memory.py` & `pydvl-0.9.2/src/pydvl/utils/caching/memory.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/dataset.py` & `pydvl-0.9.2/src/pydvl/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/functional.py` & `pydvl-0.9.2/src/pydvl/utils/functional.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/numeric.py` & `pydvl-0.9.2/src/pydvl/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/progress.py` & `pydvl-0.9.2/src/pydvl/utils/progress.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,21 +45,19 @@
     It can be used with or without specifying a log level.
     """
 
     def decorator_log_duration(func):
         @wraps(func)
         def wrapper_log_duration(*args, **kwargs):
             func_name = func.__qualname__
-            duration_logger = logging.getLogger(func_name)
-            duration_logger.setLevel(log_level)
-            duration_logger.log(log_level, f"Function '{func_name}' is starting.")
+            logger.log(log_level, f"Function '{func_name}' is starting.")
             start_time = time()
             result = func(*args, **kwargs)
             duration = time() - start_time
-            duration_logger.log(
+            logger.log(
                 log_level,
                 f"Function '{func_name}' completed. " f"Duration: {duration:.2f} sec",
             )
             return result
 
         return wrapper_log_duration
```

### Comparing `pydvl-0.9.1/src/pydvl/utils/score.py` & `pydvl-0.9.2/src/pydvl/utils/score.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/status.py` & `pydvl-0.9.2/src/pydvl/utils/status.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/types.py` & `pydvl-0.9.2/src/pydvl/utils/types.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/utils/utility.py` & `pydvl-0.9.2/src/pydvl/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/games.py` & `pydvl-0.9.2/src/pydvl/value/games.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/least_core/__init__.py` & `pydvl-0.9.2/src/pydvl/value/least_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/least_core/common.py` & `pydvl-0.9.2/src/pydvl/value/least_core/common.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/least_core/montecarlo.py` & `pydvl-0.9.2/src/pydvl/value/least_core/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/least_core/naive.py` & `pydvl-0.9.2/src/pydvl/value/least_core/naive.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/loo/loo.py` & `pydvl-0.9.2/src/pydvl/value/loo/loo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/oob/oob.py` & `pydvl-0.9.2/src/pydvl/value/oob/oob.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/result.py` & `pydvl-0.9.2/src/pydvl/value/result.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/sampler.py` & `pydvl-0.9.2/src/pydvl/value/sampler.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/semivalues.py` & `pydvl-0.9.2/src/pydvl/value/semivalues.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/__init__.py` & `pydvl-0.9.2/src/pydvl/value/shapley/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/classwise.py` & `pydvl-0.9.2/src/pydvl/value/shapley/classwise.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/common.py` & `pydvl-0.9.2/src/pydvl/value/shapley/common.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/gt.py` & `pydvl-0.9.2/src/pydvl/value/shapley/gt.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/knn.py` & `pydvl-0.9.2/src/pydvl/value/shapley/knn.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/montecarlo.py` & `pydvl-0.9.2/src/pydvl/value/shapley/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/naive.py` & `pydvl-0.9.2/src/pydvl/value/shapley/naive.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/owen.py` & `pydvl-0.9.2/src/pydvl/value/shapley/owen.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/truncated.py` & `pydvl-0.9.2/src/pydvl/value/shapley/truncated.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/shapley/types.py` & `pydvl-0.9.2/src/pydvl/value/shapley/types.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/src/pydvl/value/stopping.py` & `pydvl-0.9.2/src/pydvl/value/stopping.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/tests/test_plugin.py` & `pydvl-0.9.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9.1/tests/test_results.py` & `pydvl-0.9.2/tests/test_results.py`

 * *Files identical despite different names*

