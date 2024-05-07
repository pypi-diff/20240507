# Comparing `tmp/carrot-cdm-0.6.9.tar.gz` & `tmp/carrot-cdm-0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-0.6.9.tar", last modified: Thu Sep 14 13:01:24 2023, max compression
+gzip compressed data, was "carrot-cdm-0.72.tar", last modified: Tue May  7 14:28:12 2024, max compression
```

## Comparing `carrot-cdm-0.6.9.tar` & `carrot-cdm-0.72.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/analyses/example_serology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cdm/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cdm/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33784 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cdm/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cdm/objects/versions/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/death.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/specimen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cdm/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.176981 carrot-cdm-0.6.9/carrot/cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    41561 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23111 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/pseudonymise.py
--rw-r--r--   0 runner    (1001) docker     (127)    45804 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/cli/subcommands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/carrot/io/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/carrot/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/plugins/bclink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/io/plugins/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/carrot/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/bash_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/bclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/carrot/tools/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/extract/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/mappingrules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/omopcdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/carrot/tools/rules_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/carrot_cdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-14 13:01:24.000000 carrot-cdm-0.6.9/carrot_cdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 13:01:24.180981 carrot-cdm-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-09-14 13:01:23.000000 carrot-cdm-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.587171 carrot-cdm-0.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 14:28:11.000000 carrot-cdm-0.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 14:28:12.587171 carrot-cdm-0.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-07 14:28:11.000000 carrot-cdm-0.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.575171 carrot-cdm-0.72/carrot/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/analyses/example_serology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cdm/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cdm/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33952 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cdm/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cdm/objects/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/death.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/specimen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cdm/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.579171 carrot-cdm-0.72/carrot/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.583171 carrot-cdm-0.72/carrot/cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41561 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7841 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/pseudonymise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47910 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/cli/subcommands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.583171 carrot-cdm-0.72/carrot/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.583171 carrot-cdm-0.72/carrot/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/plugins/bclink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/io/plugins/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.583171 carrot-cdm-0.72/carrot/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/bash_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/bclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.583171 carrot-cdm-0.72/carrot/tools/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/extract/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/mappingrules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/omopcdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-07 14:28:11.000000 carrot-cdm-0.72/carrot/tools/rules_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:28:12.587171 carrot-cdm-0.72/carrot_cdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:28:12.000000 carrot-cdm-0.72/carrot_cdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:28:12.587171 carrot-cdm-0.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-07 14:28:11.000000 carrot-cdm-0.72/setup.py
```

### Comparing `carrot-cdm-0.6.9/LICENSE` & `carrot-cdm-0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/PKG-INFO` & `carrot-cdm-0.72/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.9
+Version: 0.72
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: pdappleby@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.9/carrot/analyses/example_serology.py` & `carrot-cdm-0.72/carrot/analyses/example_serology.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/__init__.py` & `carrot-cdm-0.72/carrot/cdm/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/decorators.py` & `carrot-cdm-0.72/carrot/cdm/decorators.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/model.py` & `carrot-cdm-0.72/carrot/cdm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                                  called 'output_data'.
             inputs (dict or DataCollection): inputs can be a dictionary mapping file names to pandas dataframes,
                                         or can be a DataCollection object
             use_profiler (bool): Turn on/off profiling of the CPU/Memory of running the current process.
                                  The default is set to false.
         """
         self.profiler = None
-        self.metrics = Metrics()
+        self.metrics = Metrics("Unknown")
         name = self.__class__.__name__ if name is None else self.__class__.__name__ + "::" + name
 
         self.logger.info(f"CommonDataModel ({omop_version}) created with co-connect-tools version {carrot_version}")
 
         self.omop_version = omop_version
 
         self.drop_duplicates = drop_duplicates
@@ -181,21 +181,28 @@
             if isinstance(getattr(self,name),analysis)
         }
 
         #bookkeep some logs
         self.logs = {
             'meta':{
                 'version': carrot_version,
-                'created_by': getpass.getuser(),
+                'created_by': self._get_user(),
                 'created_at': strftime("%Y-%m-%dT%H%M%S", gmtime()),
                 'dataset':name,
                 'total_data_processed':{}
             }
         }
 
+    def _get_user(self):
+        try:
+            user = getpass.getuser()
+            return user
+        except (OSError, KeyError):
+            return None
+
     def _load_inputs(self,inputs):
         for fname in inputs.keys():
             destination_table,_ = os.path.splitext(fname)
             try:
                 obj = get_cdm_class(destination_table).from_df(inputs[fname],destination_table)
             except KeyError:
                 self.logger.warning(f"Not loading {fname}, this is not a valid CDM Table")
```

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/__init__.py` & `carrot-cdm-0.72/carrot/cdm/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/common.py` & `carrot-cdm-0.72/carrot/cdm/objects/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/death.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/death.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/measurement.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/measurement.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/observation.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/observation.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/person.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/person.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/specimen.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/specimen.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py` & `carrot-cdm-0.72/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cdm/operations.py` & `carrot-cdm-0.72/carrot/cdm/operations.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/cli.py` & `carrot-cdm-0.72/carrot/cli/cli.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/airflow.py` & `carrot-cdm-0.72/carrot/cli/subcommands/airflow.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/display.py` & `carrot-cdm-0.72/carrot/cli/subcommands/display.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/etl.py` & `carrot-cdm-0.72/carrot/cli/subcommands/etl.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/generate.py` & `carrot-cdm-0.72/carrot/cli/subcommands/generate.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/get.py` & `carrot-cdm-0.72/carrot/cli/subcommands/get.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/info.py` & `carrot-cdm-0.72/carrot/cli/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/pseudonymise.py` & `carrot-cdm-0.72/carrot/cli/subcommands/pseudonymise.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/run.py` & `carrot-cdm-0.72/carrot/cli/subcommands/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -589,79 +589,100 @@
     cdm.close()
 
     if merge_output:
         ctx.invoke(merge,
                    inputs=glob.glob(f"{output_folder}{os.path.sep}*"),
                    output_folder=output_folder)
 @click.command()
-@click.option("--rules",
+@click.option("--rules-file",
               required=True,
               help="json file containing mapping rules")
-@click.option("--output-folder",
+@click.option("--output-dir",
               default=None,
-              help="define the output folder for tsv files")
+              help="define the output directory for tsv files")
 @click.option("--write-mode",
               default='w',
               type=click.Choice(['w','a']),
               help="force write-mode on output files")
 @click.option("--person-file",
               required=True,
               help="File containing person_ids in the first column")
-@click.option("--omop-config",
+@click.option("--omop-ddl-file",
+              required=True,
+              help="File containing OHDSI ddl statements for OMOP tables")
+@click.option("--omop-config-file",
               required=True,
-              help="File containing json config for omop outputs")
-@click.option("--saved-person-id-filename",
-              default='person_ids.tsv',
+              help="File containing additional / override json config for omop outputs")
+@click.option("--saved-person-id-file",
+              default=None,
               required=False,
-              help="Person id file used to save state between runs")
+              help="Full path to person id file used to save person_id state and share person_ids between data sets")
 @click.option("--use-input-person-ids",
-              required=True,
-              default='No',
+              required=False,
+              default='N',
               help="Use person ids as input without generating new integers")
+@click.option("--log-file-threshold",
+              required=False,
+              default=0,
+              help="Lower outcount limit for logfile output")
 @click.argument("input-dir",
                 required=False,
                 nargs=-1)
-def mapstream(rules, output_folder, write_mode, person_file, omop_config, saved_person_id_filename, use_input_person_ids, input_dir):
+def mapstream(rules_file, output_dir, write_mode, person_file, omop_ddl_file, omop_config_file, saved_person_id_file, use_input_person_ids, log_file_threshold, input_dir):
     """
     Map to output using input streams
     """
-    #profiler = cProfile.Profile()
-    #profiler.enable()
+    print(input_dir)
     if os.path.isdir(input_dir[0]) == False:
-        print("Not a directory {0}".format(input_dir[0]))
+        print("Not a directory, input dir {0}".format(input_dir[0]))
         sys.exit(1)
 
+    if os.path.isdir(output_dir) == False:
+        print("Not a directory, output dir {0}".format(output_dir))
+        sys.exit(1)
+
+    if saved_person_id_file == None:
+        saved_person_id_file = output_dir + "/" + "person_ids.tsv"
+        if os.path.exists(saved_person_id_file):
+            os.remove(saved_person_id_file)
+    
     starttime = time.time()
-    metrics = tools.metrics.Metrics()
-    omopcdm = tools.omopcdm.OmopCDM(omop_config)
-    mappingrules = tools.mappingrules.MappingRules(rules, omop_config)
+    omopcdm = tools.omopcdm.OmopCDM(omop_ddl_file, omop_config_file)
+    #print(omopcdm.dump_ddl())
+    mappingrules = tools.mappingrules.MappingRules(rules_file, omopcdm)
+    metrics = tools.metrics.Metrics(mappingrules.get_dataset_name(), log_file_threshold)
     nowtime = time.time()
 
     print("--------------------------------------------------------------------------------")
-    print("Loaded mapping rules from: {0} after {1:.5f} secs".format(rules, (nowtime - starttime)))
+    print("Loaded mapping rules from: {0} after {1:.5f} secs".format(rules_file, (nowtime - starttime)))
     output_files = mappingrules.get_all_outfile_names()
     record_numbers = {}
     for output_file in output_files:
-        record_numbers[output_file] = 0
+        record_numbers[output_file] = 1
 
     fhd = {}
     tgtcolmaps = {}
 
     try:
-        # TODO: add in person_ids.tsv existence testing and reload
-        fhp = open(person_file, mode="r")
-        person_lookup, rejected_person_count = load_person_ids(fhp, mappingrules, use_input_person_ids)
-        fhp.close()
-        fhpout = open(output_folder + "/person_ids.tsv", mode="w")
+        # Add in a saved-person-file existence test and reload from it is necessary returning the last used integer
+        if os.path.isfile(saved_person_id_file):
+            person_lookup, last_used_integer = load_saved_person_ids(saved_person_id_file)
+        else:
+            person_lookup = {}
+            last_used_integer = 1
+        #fhp = open(person_file, mode="r", encoding="utf-8-sig")
+        #csvrp = csv.reader(fhp)
+        person_lookup, rejected_person_count = load_person_ids(person_file, person_lookup, mappingrules, use_input_person_ids, last_used_integer)
+        fhpout = open(saved_person_id_file, mode="w")
         fhpout.write("SOURCE_SUBJECT\tTARGET_SUBJECT\n")
         for person_id, person_assigned_id in person_lookup.items():
             fhpout.write("{0}\t{1}\n".format(str(person_id), str(person_assigned_id)))
         fhpout.close()
         for tgtfile in output_files:
-            fhd[tgtfile] = open(output_folder + "/" + tgtfile + ".tsv", mode=write_mode)
+            fhd[tgtfile] = open(output_dir + "/" + tgtfile + ".tsv", mode=write_mode)
             if write_mode == 'w':
                 outhdr = omopcdm.get_omop_column_list(tgtfile)
                 fhd[tgtfile].write("\t".join(outhdr) + "\n")
             tgtcolmaps[tgtfile] = omopcdm.get_omop_column_map(tgtfile)
 
     except IOError as e:
         print("I/O - error({0}): {1} -> {2}".format(e.errno, e.strerror, str(e)))
@@ -680,28 +701,28 @@
     for infile in rules_input_files:
         if infile not in existing_input_files:
             msg = "ERROR: no data for mapped input file - {0}".format(infile)
             print(msg)
             metrics.add_log_data(msg)
     rejidcounts = {}
     rejdatecounts = {}
-    src_tgt_counts = {}
+    #src_tgt_counts = {}
     print(rules_input_files)
 
     for srcfilename in rules_input_files:
         rejidcounts[srcfilename] = 0
         rejdatecounts[srcfilename] = 0
 
     for srcfilename in rules_input_files:
         outcounts = {}
         rejcounts = {}
         rcount = 0
 
         try:
-            fh = open(input_dir[0] + "/" + srcfilename, mode='r')
+            fh = open(input_dir[0] + "/" + srcfilename, mode="r", encoding="utf-8-sig")
             csvr = csv.reader(fh)
         except IOError as e:
             print("Unable to open: {0}".format(input_dir[0] + "/" + srcfilename))
             print("I/O error({0}): {1}".format(e.errno, e.strerror))
             continue
 
         tgtfiles, src_to_tgt = mappingrules.parse_rules_src_to_tgt(srcfilename)
@@ -719,124 +740,131 @@
         datetime_col = inputcolmap[infile_datetime_source]
         print("--------------------------------------------------------------------------------")
         print("Processing input: {0}".format(srcfilename))
 #        print("Processing input: {0}, All input cols = {1}, Data cols = {2}".format(srcfilename, str(datacolsall), str(dflist)))
 
         for indata in csvr:
             #indata = inputline.strip().split(",")
-            key = srcfilename + "~all~all"
+            key = srcfilename + "~all~all~all~"
             metrics.increment_key_count(key, "input_count")
             rcount += 1
             strdate = indata[datetime_col].split(" ")[0]
             fulldate = parse_date(strdate)
             if fulldate != None:
                 #fulldate = "{0}-{1:02}-{2:02}".format(dt.year, dt.month, dt.day)
                 indata[datetime_col] = fulldate
             else:
                 metrics.increment_key_count(key, "invalid_date_fields")
                 continue
 
             for tgtfile in tgtfiles:
                 tgtcolmap = tgtcolmaps[tgtfile]
-                count_key = srcfilename + "~" + tgtfile
-                date_col_data = omopcdm.get_omop_date_fields(tgtfile)
-                date_component_data = omopcdm.get_omop_date_field_components(tgtfile)
                 auto_num_col = omopcdm.get_omop_auto_number_field(tgtfile)
                 pers_id_col = omopcdm.get_omop_person_id_field(tgtfile)
 
                 datacols = datacolsall
                 if tgtfile in dflist:
                     datacols = dflist[tgtfile]
 
                 for datacol in datacols:
-                    built_records, outrecords, metrics = get_target_records(tgtfile, tgtcolmap, src_to_tgt, datacol, indata, inputcolmap, srcfilename, date_col_data, date_component_data, metrics)
+                    built_records, outrecords, metrics = get_target_records(tgtfile, tgtcolmap, src_to_tgt, datacol, indata, inputcolmap, srcfilename, omopcdm, metrics)
                     if built_records == True:
                         for outrecord in outrecords:
                             if auto_num_col != None:
                                 outrecord[tgtcolmap[auto_num_col]] = str(record_numbers[tgtfile])
                                 record_numbers[tgtfile] += 1
                             if (outrecord[tgtcolmap[pers_id_col]]) in person_lookup:
                                 outrecord[tgtcolmap[pers_id_col]] = person_lookup[outrecord[tgtcolmap[pers_id_col]]]
                                 outcounts[tgtfile] += 1
-                                key = srcfilename + "~all~all"
-                                metrics.increment_key_count(key, "output_count")
-                                key = "all~" + tgtfile + "~all"
+                                key = srcfilename + "~all~all~all~"
                                 metrics.increment_key_count(key, "output_count")
-                                key = srcfilename + "~" + tgtfile + "~all"
+                                key = "all~all~" + tgtfile + "~all~"
                                 metrics.increment_key_count(key, "output_count")
-                                key = srcfilename + "~" + tgtfile + "~" + datacol
+                                key = srcfilename + "~all~" + tgtfile + "~all~"
                                 metrics.increment_key_count(key, "output_count")
+                                if tgtfile == "person":
+                                    key = srcfilename + "~all~" + tgtfile + "~" + outrecord[1] +"~"
+                                    metrics.increment_key_count(key, "output_count")
+                                    key = srcfilename + "~" + datacol +"~" + tgtfile + "~" + outrecord[1] + "~" + outrecord[2]
+                                    metrics.increment_key_count(key, "output_count")
+                                else:
+                                    key = srcfilename + "~" + datacol +"~" + tgtfile + "~" + outrecord[2] + "~"
+                                    metrics.increment_key_count(key, "output_count")
                                 fhd[tgtfile].write("\t".join(outrecord) + "\n")
                             else:
-                                key = srcfilename + "~" + tgtfile + "~all"
+                                key = srcfilename + "~all~" + tgtfile + "~all~"
                                 metrics.increment_key_count(key, "invalid_person_ids")
                                 rejidcounts[srcfilename] += 1
 
         fh.close()
 
         nowtime= time.time()
         print("INPUT file data : {0}: input count {1}, time since start {2:.5} secs".format(srcfilename, str(rcount), (nowtime - starttime)))
         for outtablename, count in outcounts.items():
             print("TARGET: {0}: output count {1}".format(outtablename, str(count)))
 
     print("--------------------------------------------------------------------------------")
     data_summary = metrics.get_mapstream_summary()
     log_report = metrics.get_log_data()
     try:
-        dsfh = open(output_folder + "/summary_mapstream.tsv", mode="w")
+        dsfh = open(output_dir + "/summary_mapstream.tsv", mode="w")
         dsfh.write(data_summary)
         dsfh.close()
-        logfh = open(output_folder + "/error_report.txt", mode="w")
+        logfh = open(output_dir + "/error_report.txt", mode="w")
         logfh.write(log_report)
         logfh.close()
     except IOError as e:
         print("I/O error({0}): {1}".format(e.errno, e.strerror))
         print("Unable to write file")
 
     nowtime = time.time()
     print("Elapsed time = {0:.5f} secs".format(nowtime - starttime))
     #profiler.disable()
     #stats = pstats.Stats(profiler).sort_stats('ncalls')
     #stats.print_stats()
 
-def get_target_records(tgtfilename, tgtcolmap, rulesmap, srcfield, srcdata, srccolmap, srcfilename, date_col_data, date_component_data, metrics):
+def get_target_records(tgtfilename, tgtcolmap, rulesmap, srcfield, srcdata, srccolmap, srcfilename, omopcdm, metrics):
     build_records = False
     tgtrecords = []
+    date_col_data = omopcdm.get_omop_datetime_linked_fields(tgtfilename)
+    date_component_data = omopcdm.get_omop_date_field_components(tgtfilename)
+    notnull_numeric_fields = omopcdm.get_omop_notnull_numeric_fields(tgtfilename)
 
     srckey = srcfilename + "~" + srcfield + "~" + tgtfilename
-    summarykey = srcfilename + "~" + tgtfilename + "~" + srcfield
+    summarykey = srcfilename + "~" + srcfield + "~" + tgtfilename + "~all~"
     if valid_value(str(srcdata[srccolmap[srcfield]])):
         srcfullkey = srcfilename + "~" + srcfield + "~" + str(srcdata[srccolmap[srcfield]]) + "~" + tgtfilename
         dictkeys = []
         if srcfullkey in rulesmap:
             build_records = True
             dictkeys.append(srcfullkey)
         if srckey in rulesmap:
             build_records = True
             dictkeys.append(srckey)
         if build_records == True:
             for dictkey in dictkeys:
                 for out_data_elem in rulesmap[dictkey]:
                     valid_data_elem = True
-                    tgtarray = [" "]*len(tgtcolmap)
+                    tgtarray = ['']*len(tgtcolmap)
+                    for req_integer in notnull_numeric_fields:
+                        tgtarray[tgtcolmap[req_integer]] = "0"
                     for infield, outfield_list in out_data_elem.items():
                         for output_col_data in outfield_list:
                             if "~" in output_col_data:
                                 outcol, term = output_col_data.split("~")
                                 tgtarray[tgtcolmap[outcol]] = term
                             else:
                                 tgtarray[tgtcolmap[output_col_data]] = srcdata[srccolmap[infield]]
                             if output_col_data in date_component_data:
                                 strdate = srcdata[srccolmap[infield]].split(" ")[0]
                                 dt = get_datetime_value(strdate)
                                 if dt != None:
                                     year_field = date_component_data[output_col_data]["year"]
                                     month_field = date_component_data[output_col_data]["month"]
                                     day_field = date_component_data[output_col_data]["day"]
-                                    #print("DATE Fieldnames {0} {1} {2}".format(year_field, month_field, day_field))
                                     tgtarray[tgtcolmap[year_field]] = str(dt.year)
                                     tgtarray[tgtcolmap[month_field]] = str(dt.month)
                                     tgtarray[tgtcolmap[day_field]] = str(dt.day)
                                     fulldate = "{0}-{1:02}-{2:02}".format(dt.year, dt.month, dt.day)
                                     tgtarray[tgtcolmap[output_col_data]] = fulldate
                                 else:
                                     metrics.increment_key_count(summarykey, "invalid_date_fields")
@@ -950,47 +978,61 @@
     try:
         datetime.datetime.strptime(item, "%d/%m/%Y")
     except ValueError:
         return(False)
 
     return(True)
 
-def load_person_ids(fh, mappingrules, use_input_person_ids, person_number=1, delim=","):
+def load_saved_person_ids(person_file):
+    fh = open(person_file, mode="r", encoding="utf-8-sig")
+    csvr = csv.reader(fh, delimiter="\t")
+    last_int = 1
     person_ids = {}
+
+    next(csvr)
+    for persondata in csvr:
+        person_ids[persondata[0]] = persondata[1]
+        last_int += 1
+
+    fh.close()
+    return person_ids, last_int
+
+def load_person_ids(person_file, person_ids, mappingrules, use_input_person_ids, person_number=1, delim=","):
+    fh = open(person_file, mode="r", encoding="utf-8-sig")
+    csvr = csv.reader(fh, delimiter=delim)
     person_columns = {}
     person_col_in_hdr_number = 0
     reject_count = 0
 
-    phdr = fh.readline()
-    personhdr = phdr.strip().split(delim)
+    personhdr = next(csvr)
     print(personhdr)
 
     # Make a dictionary of column names vs their positions
     for col in personhdr:
         person_columns[col] = person_col_in_hdr_number
         person_col_in_hdr_number += 1
 
     birth_datetime_source, person_id_source = mappingrules.get_person_source_field_info("person")
     print("Load Person Data {0}, {1}".format(birth_datetime_source, person_id_source))
-    person_col = 0
+    person_col = person_columns[person_id_source]
 
-    for line in fh:
-        persondata = line.strip().split(delim)
+    for persondata in csvr:
         if not valid_value(persondata[person_columns[person_id_source]]):
             reject_count += 1
             continue
         if not valid_date_value(persondata[person_columns[birth_datetime_source]]):
             reject_count += 1
             continue
         if persondata[person_col] not in person_ids:
             if use_input_person_ids == "N":
                 person_ids[persondata[person_col]] = str(person_number)
                 person_number += 1
             else:
                 person_ids[persondata[person_col]] = str(persondata[person_col])
+    fh.close()
 
     return person_ids, reject_count
 
 @click.command(help="Perform OMOP Mapping given a python configuration file.")
 @click.option("--rules",
               help="input json file containing all the mapping rules to be applied")
 @click.option("--pyconf","--conf",
```

### Comparing `carrot-cdm-0.6.9/carrot/cli/subcommands/search.py` & `carrot-cdm-0.72/carrot/cli/subcommands/search.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/io/common.py` & `carrot-cdm-0.72/carrot/io/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/io/plugins/bclink.py` & `carrot-cdm-0.72/carrot/io/plugins/bclink.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/io/plugins/local.py` & `carrot-cdm-0.72/carrot/io/plugins/local.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/io/plugins/sql.py` & `carrot-cdm-0.72/carrot/io/plugins/sql.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/__init__.py` & `carrot-cdm-0.72/carrot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/bash_helpers.py` & `carrot-cdm-0.72/carrot/tools/bash_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/bclink_helpers.py` & `carrot-cdm-0.72/carrot/tools/bclink_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/dag.py` & `carrot-cdm-0.72/carrot/tools/dag.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/extract/__init__.py` & `carrot-cdm-0.72/carrot/tools/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/extract/templates.py` & `carrot-cdm-0.72/carrot/tools/extract/templates.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/file_helpers.py` & `carrot-cdm-0.72/carrot/tools/file_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/logger.py` & `carrot-cdm-0.72/carrot/tools/logger.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/mappingrules.py` & `carrot-cdm-0.72/carrot/tools/mappingrules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 import os
 import json
 from .omopcdm import OmopCDM
 
 class MappingRules:
 
-    def __init__(self, rulesfilepath, omopcfgfilepath):
+    def __init__(self, rulesfilepath, omopcdm):
         self.rules_data = self.load_json(rulesfilepath)
-        self.omopcdm = OmopCDM(omopcfgfilepath)
+        self.omopcdm = omopcdm
+        
         self.parsed_rules = {}
         self.outfile_names = {}
 
+        self.dataset_name = self.get_dsname_from_rules()
+
     def load_json(self, f_in):
         """
         """
         if os.path.exists(f_in):
             data = json.load(open(f_in))
         else:
             try:
                 data = json.loads(f_in)
             except Exception as err:
                 raise FileNotFoundError(f"{f_in} not found. Or cannot parse as json")
 
         return data
+    
+    def dump_parsed_rules(self):
+        return(json.dumps(self.parsed_rules, indent=2))
+
+    def get_dsname_from_rules(self):
+        dsname = "Unknown"
+
+        if "metadata" in self.rules_data:
+            if "dataset" in self.rules_data["metadata"]:
+                dsname = self.rules_data["metadata"]["dataset"]
+
+        return dsname
+
+    def get_dataset_name(self):
+        return self.dataset_name
 
     def get_all_outfile_names(self):
         file_list = []
         
         for outfilename in self.rules_data["cdm"]:
             file_list.append(outfilename)
```

### Comparing `carrot-cdm-0.6.9/carrot/tools/metrics.py` & `carrot-cdm-0.72/carrot/tools/metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 class Metrics():
-    def __init__(self):
+    def __init__(self, dataset_name, log_threshold=0):
         self.datasummary={}
         self.allcounts={}
         self.log_data=""
+        self.dataset_name=dataset_name
+        self.log_threshold = log_threshold
 
     def get_new_mapstream_counts(self):
         counts = {}
         counts["input_count"] = 0
         counts["invalid_persids"] = 0
         counts["invalid_dates"] = 0
         counts["invalid_source_fields"] = 0
@@ -76,37 +78,48 @@
 
         return summary_str
 
     def get_data_summary(self):
         return self.datasummary
 
     def get_mapstream_summary(self):
-        summary_str = "source\ttarget\tsource field\tincount\tinvalid persid\tinvalid date\tinvalid source\toutcount\n"
+        summary_str = "dsname\tsource\tsource_field\ttarget\tconcept_id\tadditional\tincount\tinvalid_persid\tinvalid_date\tinvalid_source\toutcount\n"
 
         for dkey in sorted(self.datasummary):
-            source, fieldname, tablename = dkey.split('~')
+            try:
+                source, fieldname, tablename, concept_id, additional = dkey.split('~')
+            except ValueError:
+                print("get_mapstream_summary - ValueError: {0}".format(dkey))
+                break
+              
             source = self.get_prefix(source)
-            input_count = ""
             dvalue = self.datasummary[dkey]
+
+            input_count = "0"
             if "input_count" in dvalue:
                 input_count = str(dvalue["input_count"])
-            invalid_person_ids = ""
+
+            invalid_person_ids = "0"
             if "invalid_person_ids" in dvalue:
                 invalid_person_ids = str(dvalue["invalid_person_ids"])
-            invalid_source_fields = ""
+
+            invalid_source_fields = "0"
             if "invalid_source_fields" in dvalue:
                 invalid_source_fields = str(dvalue["invalid_source_fields"])
-            invalid_date_fields = ""
+
+            invalid_date_fields = "0"
             if "invalid_date_fields" in dvalue:
                 invalid_date_fields = str(dvalue["invalid_date_fields"])
-            output_count = ""
+
+            output_count = "0"
             if "output_count" in dvalue:
                 output_count = str(dvalue["output_count"])
 
-            summary_str += source + "\t" + fieldname + "\t" + tablename + "\t" + input_count + "\t" + invalid_person_ids + "\t" + invalid_date_fields + "\t" + invalid_source_fields + "\t" + output_count + "\n"
+            if (int(output_count) >= self.log_threshold) or (tablename != "person"):
+              summary_str += self.dataset_name + "\t" + source + "\t" + fieldname + "\t" + tablename + "\t" + concept_id + "\t" + additional +"\t" + input_count + "\t" + invalid_person_ids + "\t" + invalid_date_fields + "\t" + invalid_source_fields + "\t" + output_count + "\n"
 
         return summary_str
 
     def add_log_data(self, msg):
         self.log_data += msg + "\n"
 
     def get_log_data(self):
```

### Comparing `carrot-cdm-0.6.9/carrot/tools/profiling.py` & `carrot-cdm-0.72/carrot/tools/profiling.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot/tools/rules_helpers.py` & `carrot-cdm-0.72/carrot/tools/rules_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/carrot_cdm.egg-info/PKG-INFO` & `carrot-cdm-0.72/carrot_cdm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.9
+Version: 0.72
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: pdappleby@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.9/carrot_cdm.egg-info/SOURCES.txt` & `carrot-cdm-0.72/carrot_cdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.9/setup.py` & `carrot-cdm-0.72/setup.py`

 * *Files identical despite different names*

