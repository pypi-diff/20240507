# Comparing `tmp/rtc-tools-interface-0.7.4.tar.gz` & `tmp/rtc-tools-interface-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-interface-0.7.4.tar", last modified: Thu Apr 25 14:36:24 2024, max compression
+gzip compressed data, was "rtc-tools-interface-0.7.5.tar", last modified: Tue May  7 14:20:34 2024, max compression
```

## Comparing `rtc-tools-interface-0.7.4.tar` & `rtc-tools-interface-0.7.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      268 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12418 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.485177 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1882 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/rtctools_interface/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/rtctools_interface/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.487177 rtc-tools-interface-0.7.4/rtctools_interface/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10183 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_goal.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_generator_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5055 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_performance_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_table_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.487177 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3032 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/statistics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.488177 rtc-tools-interface-0.7.4/rtctools_interface/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11028 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    12382 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/subplot_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.488177 rtc-tools-interface-0.7.4/rtctools_interface/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.490177 rtc-tools-interface-0.7.4/rtctools_interface/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/plot_table_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/read_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/read_plot_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7748 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/results_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/type_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.490177 rtc-tools-interface-0.7.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.491177 rtc-tools-interface-0.7.4/tests/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1265 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_passing_goals_directly.py
--rw-rw-rw-   0 root         (0) root         (0)     2076 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/tests/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/test_base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/test_plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/utils/get_test.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.887678 rtc-tools-interface-0.7.5/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      268 2024-05-07 14:20:34.887678 rtc-tools-interface-0.7.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12413 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.881678 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-05-07 14:20:34.000000 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-05-07 14:20:34.000000 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 14:20:34.000000 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-07 14:20:34.000000 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-07 14:20:34.000000 rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.888678 rtc-tools-interface-0.7.5/rtctools_interface/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-07 14:20:34.888678 rtc-tools-interface-0.7.5/rtctools_interface/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.883678 rtc-tools-interface-0.7.5/rtctools_interface/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10183 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/base_goal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_generator_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_performance_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_table_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.883678 rtc-tools-interface-0.7.5/rtctools_interface/optimization/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/helpers/statistics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/plot_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/optimization/read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.884678 rtc-tools-interface-0.7.5/rtctools_interface/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11023 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/plotting/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    12382 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/plotting/subplot_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.884678 rtc-tools-interface-0.7.5/rtctools_interface/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/simulation/base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/simulation/plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.885678 rtc-tools-interface-0.7.5/rtctools_interface/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/plot_table_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/read_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/read_plot_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7748 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/results_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/rtctools_interface/utils/type_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-07 14:20:34.887678 rtc-tools-interface-0.7.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.885678 rtc-tools-interface-0.7.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.886678 rtc-tools-interface-0.7.5/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/optimization/test_base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/optimization/test_passing_goals_directly.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/optimization/test_plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/optimization/test_read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.887678 rtc-tools-interface-0.7.5/tests/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/simulation/test_base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/simulation/test_plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:20:34.887678 rtc-tools-interface-0.7.5/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/tests/utils/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2024-05-07 14:20:33.000000 rtc-tools-interface-0.7.5/versioneer.py
```

### Comparing `rtc-tools-interface-0.7.4/COPYING.LESSER` & `rtc-tools-interface-0.7.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/README.md` & `rtc-tools-interface-0.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -159,8 +159,8 @@
 |    id   |  y_axis_title   | variables_style_1 | variables_style_2 | variables_with_previous_result | custom_title | specified_in
 |---------|-----------------|------------------|------------------|------------------|------------------|------------------|
 | goal_1  | Volume (\$m^3\$)  |      "PowerPlant1.QOut.Q"            |                  | | | goal_generator
 | goal_2  | Volume (\$m^3\$)  |      "PowerPlant1.QOut.Q, PowerPlant2.QOut.Q"            |   | |               | goal_generator
 |  | Volume (\$m^3\$)  |                |                  | electricity_cost | "Goal for minimizing electricity cost, at priority 10" | python
 
 
-After running the model, in your output folder the folder `goal_figures` containing the figures is created.
+After running the model, in your output folder the folder `figures` containing the figures is created.
```

### Comparing `rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/SOURCES.txt` & `rtc-tools-interface-0.7.5/rtc_tools_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_goal.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/base_goal.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_optimization_problem.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_generator_mixin.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_generator_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_performance_metrics.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_table_schema.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/goal_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/statistics_mixin.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/helpers/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_mixin.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/optimization/read_goals.py` & `rtc-tools-interface-0.7.5/rtctools_interface/optimization/read_goals.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/plotting/plot_tools.py` & `rtc-tools-interface-0.7.5/rtctools_interface/plotting/plot_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     i_c, i_r = get_row_col_number(i_plot, n_rows, n_cols)
     subplot = axs[i_r, i_c]
     return subplot
 
 
 def get_file_write_path(output_folder: Union[str, Path], file_name="figure"):
     """Get path to to file."""
-    new_output_folder = Path(output_folder) / "goal_figures"
+    new_output_folder = Path(output_folder) / "figures"
     os.makedirs(new_output_folder, exist_ok=True)
     return os.path.join(new_output_folder, file_name)
 
 
 def get_file_name(priority: int, final_result: bool):
     """Get the file name for the figure to be written."""
     if final_result:
```

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/plotting/subplot_classes.py` & `rtc-tools-interface-0.7.5/rtctools_interface/plotting/subplot_classes.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/simulation/base_simulation_problem.py` & `rtc-tools-interface-0.7.5/rtctools_interface/simulation/base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/simulation/plot_mixin.py` & `rtc-tools-interface-0.7.5/rtctools_interface/simulation/plot_mixin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 """Mixin to store all required data for plotting. Can also call the plot function."""
 
 import logging
+from typing import Dict, List
+
+import numpy as np
 
 from rtctools_interface.plotting.plot_tools import create_plot_final_results
 from rtctools_interface.utils.results_collection import PlottingBaseMixin
 
 logger = logging.getLogger("rtctools")
 
 
 class PlotMixin(PlottingBaseMixin):
     """
     Class for plotting results based on the plot_table.
     """
 
     optimization_problem = False
+    _manual_extracted_states: Dict[str, list] = {}
+
+    def manual_extraction_from_state_vector(self):
+        for variable in self.custom_variables:
+            try:
+                self._manual_extracted_states[variable].append(self.get_var(variable))
+            except KeyError:
+                logger.debug("Variable {} not found in output of model.".format(variable))
+
+    def initialize(self):
+        super().initialize()
+        self._manual_extracted_states = {variable: [] for variable in self.custom_variables}
+        self.manual_extraction_from_state_vector()
+
+    def update(self, dt):
+        super().update(dt)
+        self.manual_extraction_from_state_vector()
 
     def post(self):
         """Tasks after optimizing."""
         super().post()
 
         timeseries_data = self.collect_timeseries_data(self.custom_variables)
         self._intermediate_results.append({"timeseries_data": timeseries_data, "priority": 0})
         current_run = self.create_plot_data_and_config([])
         self._store_current_results(self._cache_folder, current_run)
 
         if self.plot_final_results:
             create_plot_final_results(current_run, self._previous_run, plotting_library=self.plotting_library)
+
+    def collect_timeseries_data(self, all_variables_to_store: List[str]) -> Dict[str, np.ndarray]:
+        return {variable: np.array(self._manual_extracted_states[variable]) for variable in all_variables_to_store}
```

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/plot_table_schema.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/plot_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/read_goals_mixin.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/read_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/read_plot_table.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/read_plot_table.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/results_collection.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/results_collection.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/serialization.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/rtctools_interface/utils/type_definitions.py` & `rtc-tools-interface-0.7.5/rtctools_interface/utils/type_definitions.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/optimization/test_base_optimization_problem.py` & `rtc-tools-interface-0.7.5/tests/optimization/test_base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/optimization/test_passing_goals_directly.py` & `rtc-tools-interface-0.7.5/tests/optimization/test_passing_goals_directly.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/optimization/test_plot_goals_mixin.py` & `rtc-tools-interface-0.7.5/tests/optimization/test_plot_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/simulation/test_base_simulation_problem.py` & `rtc-tools-interface-0.7.5/tests/simulation/test_base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/simulation/test_plot_mixin.py` & `rtc-tools-interface-0.7.5/tests/simulation/test_plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/tests/utils/get_test.py` & `rtc-tools-interface-0.7.5/tests/utils/get_test.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.4/versioneer.py` & `rtc-tools-interface-0.7.5/versioneer.py`

 * *Files identical despite different names*

