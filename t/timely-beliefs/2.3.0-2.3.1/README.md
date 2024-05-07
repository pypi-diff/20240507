# Comparing `tmp/timely-beliefs-2.3.0.tar.gz` & `tmp/timely-beliefs-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timely-beliefs-2.3.0.tar", last modified: Mon Mar 25 09:52:39 2024, max compression
+gzip compressed data, was "timely-beliefs-2.3.1.tar", last modified: Tue May  7 13:11:58 2024, max compression
```

## Comparing `timely-beliefs-2.3.0.tar` & `timely-beliefs-2.3.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.803604 timely-beliefs-2.3.0/
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.483604 timely-beliefs-2.3.0/.github/
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.503604 timely-beliefs-2.3.0/.github/workflows/
--rw-r--r--   0 felix     (1000) felix     (1000)     1497 2023-06-06 09:17:32.000000 timely-beliefs-2.3.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0 felix     (1000) felix     (1000)     1203 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/.gitignore
--rw-r--r--   0 felix     (1000) felix     (1000)      732 2024-02-29 21:27:59.000000 timely-beliefs-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 felix     (1000) felix     (1000)     1065 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/MANIFEST.in
--rw-r--r--   0 felix     (1000) felix     (1000)      761 2023-10-30 14:57:17.000000 timely-beliefs-2.3.0/Makefile
--rw-r--r--   0 felix     (1000) felix     (1000)     2155 2024-03-25 09:52:39.803604 timely-beliefs-2.3.0/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)    10472 2022-11-23 12:02:09.000000 timely-beliefs-2.3.0/README.md
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.535604 timely-beliefs-2.3.0/dev/
--rw-r--r--   0 felix     (1000) felix     (1000)      670 2022-04-11 14:42:42.000000 timely-beliefs-2.3.0/dev/dev.md
--rw-r--r--   0 felix     (1000) felix     (1000)     1333 2024-02-06 13:12:09.000000 timely-beliefs-2.3.0/dev/requirements.txt
--rw-r--r--   0 felix     (1000) felix     (1000)     3151 2024-02-06 14:31:45.000000 timely-beliefs-2.3.0/pyproject.toml
--rw-r--r--   0 felix     (1000) felix     (1000)      356 2024-03-25 09:52:39.807604 timely-beliefs-2.3.0/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)       69 2022-09-12 09:28:47.000000 timely-beliefs-2.3.0/setup.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.555604 timely-beliefs-2.3.0/timely_beliefs/
--rw-r--r--   0 felix     (1000) felix     (1000)     1251 2022-09-12 09:25:37.000000 timely-beliefs-2.3.0/timely_beliefs/__init__.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.603604 timely-beliefs-2.3.0/timely_beliefs/beliefs/
--rw-r--r--   0 felix     (1000) felix     (1000)     6393 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/beliefs/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    98605 2024-03-23 20:54:22.000000 timely-beliefs-2.3.0/timely_beliefs/beliefs/classes.py
--rw-r--r--   0 felix     (1000) felix     (1000)    24534 2024-03-23 20:54:22.000000 timely-beliefs-2.3.0/timely_beliefs/beliefs/probabilistic_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2710 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/beliefs/queries.py
--rw-r--r--   0 felix     (1000) felix     (1000)    49889 2024-03-23 20:54:22.000000 timely-beliefs-2.3.0/timely_beliefs/beliefs/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)       71 2024-02-06 12:59:36.000000 timely-beliefs-2.3.0/timely_beliefs/db_base.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.659604 timely-beliefs-2.3.0/timely_beliefs/docs/
--rw-r--r--   0 felix     (1000) felix     (1000)     2646 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/accuracy.md
--rw-r--r--   0 felix     (1000) felix     (1000)   189137 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/belief_history_ridgeline.png
--rw-r--r--   0 felix     (1000) felix     (1000)   172491 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png
--rw-r--r--   0 felix     (1000) felix     (1000)     1948 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/confidence.md
--rw-r--r--   0 felix     (1000) felix     (1000)     6880 2022-09-05 08:25:46.000000 timely-beliefs-2.3.0/timely_beliefs/docs/db.md
--rw-r--r--   0 felix     (1000) felix     (1000)   187292 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/fixed_viewpoint_ridgeline.png
--rw-r--r--   0 felix     (1000) felix     (1000)     5702 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/docs/init.md
--rw-r--r--   0 felix     (1000) felix     (1000)      287 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/lineage.md
--rw-r--r--   0 felix     (1000) felix     (1000)     4804 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/docs/resampling.md
--rw-r--r--   0 felix     (1000) felix     (1000)     4654 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/docs/slicing.md
--rw-r--r--   0 felix     (1000) felix     (1000)     5004 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/docs/timing.md
--rw-r--r--   0 felix     (1000) felix     (1000)     3735 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/docs/viz.md
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.687604 timely-beliefs-2.3.0/timely_beliefs/examples/
--rw-r--r--   0 felix     (1000) felix     (1000)      589 2022-10-14 13:27:34.000000 timely-beliefs-2.3.0/timely_beliefs/examples/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1970 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/examples/beliefs_data_frames.py
--rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/examples/chart.html
--rw-r--r--   0 felix     (1000) felix     (1000)      311 2023-10-30 14:35:30.000000 timely-beliefs-2.3.0/timely_beliefs/examples/locale_datetime_sample.csv
--rw-r--r--   0 felix     (1000) felix     (1000)  1362729 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/examples/temperature.csv
--rw-r--r--   0 felix     (1000) felix     (1000)      272 2022-10-14 13:27:34.000000 timely-beliefs-2.3.0/timely_beliefs/examples/timezone_naive_sample.csv
--rw-r--r--   0 felix     (1000) felix     (1000)      451 2022-04-11 14:42:42.000000 timely-beliefs-2.3.0/timely_beliefs/examples/visualize_example.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.699604 timely-beliefs-2.3.0/timely_beliefs/sensors/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5444 2024-02-06 13:08:12.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/classes.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.703604 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      433 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/event_values.py
--rw-r--r--   0 felix     (1000) felix     (1000)     6413 2024-03-23 14:24:22.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/knowledge_horizons.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10178 2024-03-23 14:36:32.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/test_knowledge_horizons.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2757 2024-03-23 14:35:36.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3538 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/sensors/utils.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.715604 timely-beliefs-2.3.0/timely_beliefs/sources/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/sources/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1598 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/sources/classes.py
--rw-r--r--   0 felix     (1000) felix     (1000)      638 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/sources/utils.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.767604 timely-beliefs-2.3.0/timely_beliefs/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/tests/README.md
--rw-r--r--   0 felix     (1000) felix     (1000)      204 2023-08-29 14:27:22.000000 timely-beliefs-2.3.0/timely_beliefs/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5733 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5535 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_accuracy.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3561 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_init.py
--rw-r--r--   0 felix     (1000) felix     (1000)    24147 2024-02-06 14:31:05.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_io.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2193 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_persistence.py
--rw-r--r--   0 felix     (1000) felix     (1000)    17413 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_query.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10113 2023-06-13 07:34:19.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5016 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_db_subclassing.py
--rw-r--r--   0 felix     (1000) felix     (1000)    18766 2024-03-23 20:54:39.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_df_resampling.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2542 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_forecast__belief_formation.py
--rw-r--r--   0 felix     (1000) felix     (1000)      429 2023-06-06 09:17:32.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_ignore_36__belief_init.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9996 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_probabilistic_downsampling.py
--rw-r--r--   0 felix     (1000) felix     (1000)      750 2023-06-29 09:29:41.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_sensor_init.py
--rw-r--r--   0 felix     (1000) felix     (1000)      192 2024-02-06 12:59:36.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_sensor_query.py
--rw-r--r--   0 felix     (1000) felix     (1000)      323 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)      606 2022-11-23 11:57:25.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_viz__plotting.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1352 2023-04-19 10:09:16.000000 timely-beliefs-2.3.0/timely_beliefs/tests/test_viz__ridgeline.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1963 2023-05-08 09:32:25.000000 timely-beliefs-2.3.0/timely_beliefs/tests/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8162 2024-02-06 13:07:59.000000 timely-beliefs-2.3.0/timely_beliefs/utils.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.775604 timely-beliefs-2.3.0/timely_beliefs/visualization/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.0/timely_beliefs/visualization/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12537 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/visualization/graphs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8741 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/visualization/selectors.py
--rw-r--r--   0 felix     (1000) felix     (1000)    17856 2024-02-06 13:06:35.000000 timely-beliefs-2.3.0/timely_beliefs/visualization/utils.py
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-03-25 09:52:39.791604 timely-beliefs-2.3.0/timely_beliefs.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     2155 2024-03-25 09:52:38.000000 timely-beliefs-2.3.0/timely_beliefs.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     2824 2024-03-25 09:52:39.000000 timely-beliefs-2.3.0/timely_beliefs.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2024-03-25 09:52:38.000000 timely-beliefs-2.3.0/timely_beliefs.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      435 2024-03-25 09:52:38.000000 timely-beliefs-2.3.0/timely_beliefs.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       15 2024-03-25 09:52:38.000000 timely-beliefs-2.3.0/timely_beliefs.egg-info/top_level.txt
--rwxr-xr-x   0 felix     (1000) felix     (1000)     1356 2024-01-09 11:28:36.000000 timely-beliefs-2.3.0/to_pypi.sh
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.384480 timely-beliefs-2.3.1/
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.332480 timely-beliefs-2.3.1/.github/
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.336480 timely-beliefs-2.3.1/.github/workflows/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1497 2023-06-06 09:17:32.000000 timely-beliefs-2.3.1/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 felix     (1000) felix     (1000)     1203 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/.gitignore
+-rw-r--r--   0 felix     (1000) felix     (1000)      732 2024-02-29 21:27:59.000000 timely-beliefs-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 felix     (1000) felix     (1000)     1065 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/MANIFEST.in
+-rw-r--r--   0 felix     (1000) felix     (1000)      761 2023-10-30 14:57:17.000000 timely-beliefs-2.3.1/Makefile
+-rw-r--r--   0 felix     (1000) felix     (1000)     2183 2024-05-07 13:11:58.384480 timely-beliefs-2.3.1/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)    10472 2022-11-23 12:02:09.000000 timely-beliefs-2.3.1/README.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.340480 timely-beliefs-2.3.1/dev/
+-rw-r--r--   0 felix     (1000) felix     (1000)      670 2022-04-11 14:42:42.000000 timely-beliefs-2.3.1/dev/dev.md
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1333 2024-05-07 12:49:58.000000 timely-beliefs-2.3.1/dev/requirements.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)     3232 2024-05-07 12:50:05.000000 timely-beliefs-2.3.1/pyproject.toml
+-rw-r--r--   0 felix     (1000) felix     (1000)      356 2024-05-07 13:11:58.384480 timely-beliefs-2.3.1/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)       69 2022-09-12 09:28:47.000000 timely-beliefs-2.3.1/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.340480 timely-beliefs-2.3.1/timely_beliefs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1251 2022-09-12 09:25:37.000000 timely-beliefs-2.3.1/timely_beliefs/__init__.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.344480 timely-beliefs-2.3.1/timely_beliefs/beliefs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     6393 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/beliefs/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)    98605 2024-05-07 12:39:50.000000 timely-beliefs-2.3.1/timely_beliefs/beliefs/classes.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    24534 2024-03-23 20:54:22.000000 timely-beliefs-2.3.1/timely_beliefs/beliefs/probabilistic_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2710 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/beliefs/queries.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    49889 2024-03-23 20:54:22.000000 timely-beliefs-2.3.1/timely_beliefs/beliefs/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       71 2024-02-06 12:59:36.000000 timely-beliefs-2.3.1/timely_beliefs/db_base.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.352480 timely-beliefs-2.3.1/timely_beliefs/docs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2646 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/accuracy.md
+-rw-r--r--   0 felix     (1000) felix     (1000)   189137 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/belief_history_ridgeline.png
+-rw-r--r--   0 felix     (1000) felix     (1000)   172491 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png
+-rw-r--r--   0 felix     (1000) felix     (1000)     1948 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/confidence.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     6880 2022-09-05 08:25:46.000000 timely-beliefs-2.3.1/timely_beliefs/docs/db.md
+-rw-r--r--   0 felix     (1000) felix     (1000)   187292 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/fixed_viewpoint_ridgeline.png
+-rw-r--r--   0 felix     (1000) felix     (1000)     5702 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/docs/init.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      287 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/lineage.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     4804 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/docs/resampling.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     4654 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/docs/slicing.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     5004 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/docs/timing.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     3735 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/docs/viz.md
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.364480 timely-beliefs-2.3.1/timely_beliefs/examples/
+-rw-r--r--   0 felix     (1000) felix     (1000)      589 2022-10-14 13:27:34.000000 timely-beliefs-2.3.1/timely_beliefs/examples/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1970 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/examples/beliefs_data_frames.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/examples/chart.html
+-rw-r--r--   0 felix     (1000) felix     (1000)      311 2023-10-30 14:35:30.000000 timely-beliefs-2.3.1/timely_beliefs/examples/locale_datetime_sample.csv
+-rw-r--r--   0 felix     (1000) felix     (1000)  1362729 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/examples/temperature.csv
+-rw-r--r--   0 felix     (1000) felix     (1000)      272 2022-10-14 13:27:34.000000 timely-beliefs-2.3.1/timely_beliefs/examples/timezone_naive_sample.csv
+-rw-r--r--   0 felix     (1000) felix     (1000)      451 2022-04-11 14:42:42.000000 timely-beliefs-2.3.1/timely_beliefs/examples/visualize_example.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.364480 timely-beliefs-2.3.1/timely_beliefs/sensors/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5444 2024-02-06 13:08:12.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/classes.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.364480 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      433 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/event_values.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     6413 2024-03-23 14:24:22.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/knowledge_horizons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10178 2024-03-23 14:36:32.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/test_knowledge_horizons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2757 2024-03-23 14:35:36.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3538 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/sensors/utils.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.364480 timely-beliefs-2.3.1/timely_beliefs/sources/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/sources/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1598 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/sources/classes.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      638 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/sources/utils.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.372480 timely-beliefs-2.3.1/timely_beliefs/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/tests/README.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      204 2023-08-29 14:27:22.000000 timely-beliefs-2.3.1/timely_beliefs/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5733 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5535 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_accuracy.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3561 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_init.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    24147 2024-02-06 14:31:05.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_io.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2193 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_persistence.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    17413 2024-04-09 09:49:48.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_query.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10113 2023-06-13 07:34:19.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5016 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_db_subclassing.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    18766 2024-03-23 20:54:39.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_df_resampling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2542 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_forecast__belief_formation.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      429 2023-06-06 09:17:32.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_ignore_36__belief_init.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9996 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_probabilistic_downsampling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      750 2023-06-29 09:29:41.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_sensor_init.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      192 2024-02-06 12:59:36.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_sensor_query.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      323 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      606 2022-11-23 11:57:25.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_viz__plotting.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1352 2023-04-19 10:09:16.000000 timely-beliefs-2.3.1/timely_beliefs/tests/test_viz__ridgeline.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1963 2023-05-08 09:32:25.000000 timely-beliefs-2.3.1/timely_beliefs/tests/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8162 2024-02-06 13:07:59.000000 timely-beliefs-2.3.1/timely_beliefs/utils.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.376480 timely-beliefs-2.3.1/timely_beliefs/visualization/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-2.3.1/timely_beliefs/visualization/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12537 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/visualization/graphs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8741 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/visualization/selectors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    17856 2024-02-06 13:06:35.000000 timely-beliefs-2.3.1/timely_beliefs/visualization/utils.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2024-05-07 13:11:58.380480 timely-beliefs-2.3.1/timely_beliefs.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2183 2024-05-07 13:11:57.000000 timely-beliefs-2.3.1/timely_beliefs.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     2824 2024-05-07 13:11:58.000000 timely-beliefs-2.3.1/timely_beliefs.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2024-05-07 13:11:57.000000 timely-beliefs-2.3.1/timely_beliefs.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      448 2024-05-07 13:11:57.000000 timely-beliefs-2.3.1/timely_beliefs.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       15 2024-05-07 13:11:57.000000 timely-beliefs-2.3.1/timely_beliefs.egg-info/top_level.txt
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     1356 2024-01-09 11:28:36.000000 timely-beliefs-2.3.1/to_pypi.sh
```

### Comparing `timely-beliefs-2.3.0/.github/workflows/lint-and-test.yml` & `timely-beliefs-2.3.1/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/.gitignore` & `timely-beliefs-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/.pre-commit-config.yaml` & `timely-beliefs-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/LICENSE` & `timely-beliefs-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/Makefile` & `timely-beliefs-2.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/PKG-INFO` & `timely-beliefs-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timely-beliefs
-Version: 2.3.0
+Version: 2.3.1
 Summary: Data modelled as beliefs (at a certain time) about events (at a certain time).
 Author-email: Seita BV <felix@seita.nl>
 Project-URL: homepage, https://github.com/seitabv/timely-beliefs
 Project-URL: documentation, https://github.com/SeitaBV/timely-beliefs#readme
 Keywords: time series,forecasting,analytics,visualization,uncertainty,lineage
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,15 @@
 Requires-Dist: SQLAlchemy>=2
 Requires-Dist: numpy==1.19.5; python_version <= "3.6"
 Requires-Dist: numpy==1.21.4; python_version <= "3.7"
 Requires-Dist: numpy; python_version > "3.7"
 Requires-Dist: pandas<1.2,>=1.1.5; python_version <= "3.6"
 Requires-Dist: pandas<1.3,>=1.1.5; python_version == "3.7"
 Requires-Dist: pandas!=2.1.0,!=2.1.1,>=1.4.0; python_version > "3.7"
+Requires-Dist: pandas<2.2.2
 Requires-Dist: scipy<1.6; python_version <= "3.6"
 Requires-Dist: scipy<1.8; python_version <= "3.7"
 Requires-Dist: scipy; python_version > "3.7"
 Provides-Extra: viz
 Requires-Dist: altair<5,>=4.0.0; extra == "viz"
 Provides-Extra: forecast
 Requires-Dist: sktime; extra == "forecast"
```

### Comparing `timely-beliefs-2.3.0/README.md` & `timely-beliefs-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/dev/dev.md` & `timely-beliefs-2.3.1/dev/dev.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/dev/requirements.txt` & `timely-beliefs-2.3.1/dev/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via timely-beliefs (setup.py)
 attrs==20.2.0
     # via jsonschema
 entrypoints==0.3
     # via altair
 isodate==0.6.0
     # via timely-beliefs (setup.py)
-jinja2==3.1.3
+jinja2==3.1.4
     # via altair
 jsonschema==3.2.0
     # via altair
 markupsafe==1.1.1
     # via jinja2
 numpy==1.22.0
     # via
```

### Comparing `timely-beliefs-2.3.0/pyproject.toml` & `timely-beliefs-2.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     "numpy==1.21.4; python_version <= '3.7'",
     "numpy; python_version > '3.7'",
     # https://pandas.pydata.org/pandas-docs/stable/whatsnew/v1.2.0.html#increased-minimum-version-for-python
     "pandas >= 1.1.5, < 1.2; python_version <= '3.6'",
     "pandas >= 1.1.5, < 1.3; python_version == '3.7'",
     # https://github.com/SeitaBV/timely-beliefs/issues/148
     "pandas >= 1.4.0, != 2.1.0, !=2.1.1; python_version > '3.7'",
+    # https://github.com/SeitaBV/timely-beliefs/issues/177
+    "pandas < 2.2.2",
     # scipy's setup requires minimal Python versions
     "scipy<1.6; python_version <= '3.6'",
     "scipy<1.8; python_version <= '3.7'",
     "scipy; python_version > '3.7'",
 ]
 dynamic = ["version"]
```

### Comparing `timely-beliefs-2.3.0/timely_beliefs/__init__.py` & `timely-beliefs-2.3.1/timely_beliefs/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/beliefs/__init__.py` & `timely-beliefs-2.3.1/timely_beliefs/beliefs/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/beliefs/classes.py` & `timely-beliefs-2.3.1/timely_beliefs/beliefs/classes.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/beliefs/probabilistic_utils.py` & `timely-beliefs-2.3.1/timely_beliefs/beliefs/probabilistic_utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/beliefs/queries.py` & `timely-beliefs-2.3.1/timely_beliefs/beliefs/queries.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/beliefs/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/beliefs/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/accuracy.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/accuracy.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/belief_history_ridgeline.png` & `timely-beliefs-2.3.1/timely_beliefs/docs/belief_history_ridgeline.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png` & `timely-beliefs-2.3.1/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/confidence.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/confidence.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/db.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/db.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/fixed_viewpoint_ridgeline.png` & `timely-beliefs-2.3.1/timely_beliefs/docs/fixed_viewpoint_ridgeline.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/init.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/init.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/resampling.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/resampling.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/slicing.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/slicing.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/timing.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/timing.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/docs/viz.md` & `timely-beliefs-2.3.1/timely_beliefs/docs/viz.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/examples/__init__.py` & `timely-beliefs-2.3.1/timely_beliefs/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/examples/beliefs_data_frames.py` & `timely-beliefs-2.3.1/timely_beliefs/examples/beliefs_data_frames.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/examples/chart.html` & `timely-beliefs-2.3.1/timely_beliefs/examples/chart.html`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/examples/temperature.csv` & `timely-beliefs-2.3.1/timely_beliefs/examples/temperature.csv`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sensors/classes.py` & `timely-beliefs-2.3.1/timely_beliefs/sensors/classes.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/knowledge_horizons.py` & `timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/knowledge_horizons.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/test_knowledge_horizons.py` & `timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/test_knowledge_horizons.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sensors/func_store/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/sensors/func_store/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sensors/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sources/classes.py` & `timely-beliefs-2.3.1/timely_beliefs/sources/classes.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/sources/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/sources/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/README.md` & `timely-beliefs-2.3.1/timely_beliefs/tests/README.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/conftest.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_accuracy.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_init.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_init.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_io.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_io.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_persistence.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_persistence.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_query.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_query.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_belief_utils.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_belief_utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_db_subclassing.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_db_subclassing.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_df_resampling.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_df_resampling.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_forecast__belief_formation.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_forecast__belief_formation.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_probabilistic_downsampling.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_probabilistic_downsampling.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_sensor_init.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_sensor_init.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_viz__plotting.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_viz__plotting.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/test_viz__ridgeline.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/test_viz__ridgeline.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/tests/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/visualization/graphs.py` & `timely-beliefs-2.3.1/timely_beliefs/visualization/graphs.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/visualization/selectors.py` & `timely-beliefs-2.3.1/timely_beliefs/visualization/selectors.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs/visualization/utils.py` & `timely-beliefs-2.3.1/timely_beliefs/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/timely_beliefs.egg-info/PKG-INFO` & `timely-beliefs-2.3.1/timely_beliefs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timely-beliefs
-Version: 2.3.0
+Version: 2.3.1
 Summary: Data modelled as beliefs (at a certain time) about events (at a certain time).
 Author-email: Seita BV <felix@seita.nl>
 Project-URL: homepage, https://github.com/seitabv/timely-beliefs
 Project-URL: documentation, https://github.com/SeitaBV/timely-beliefs#readme
 Keywords: time series,forecasting,analytics,visualization,uncertainty,lineage
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,15 @@
 Requires-Dist: SQLAlchemy>=2
 Requires-Dist: numpy==1.19.5; python_version <= "3.6"
 Requires-Dist: numpy==1.21.4; python_version <= "3.7"
 Requires-Dist: numpy; python_version > "3.7"
 Requires-Dist: pandas<1.2,>=1.1.5; python_version <= "3.6"
 Requires-Dist: pandas<1.3,>=1.1.5; python_version == "3.7"
 Requires-Dist: pandas!=2.1.0,!=2.1.1,>=1.4.0; python_version > "3.7"
+Requires-Dist: pandas<2.2.2
 Requires-Dist: scipy<1.6; python_version <= "3.6"
 Requires-Dist: scipy<1.8; python_version <= "3.7"
 Requires-Dist: scipy; python_version > "3.7"
 Provides-Extra: viz
 Requires-Dist: altair<5,>=4.0.0; extra == "viz"
 Provides-Extra: forecast
 Requires-Dist: sktime; extra == "forecast"
```

### Comparing `timely-beliefs-2.3.0/timely_beliefs.egg-info/SOURCES.txt` & `timely-beliefs-2.3.1/timely_beliefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timely-beliefs-2.3.0/to_pypi.sh` & `timely-beliefs-2.3.1/to_pypi.sh`

 * *Files identical despite different names*

