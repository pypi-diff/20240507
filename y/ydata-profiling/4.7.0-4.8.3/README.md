# Comparing `tmp/ydata-profiling-4.7.0.tar.gz` & `tmp/ydata-profiling-4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-profiling-4.7.0.tar", last modified: Mon Mar 18 18:30:07 2024, max compression
+gzip compressed data, was "ydata-profiling-4.8.3.tar", last modified: Tue May  7 20:05:24 2024, max compression
```

## Comparing `ydata-profiling-4.7.0.tar` & `ydata-profiling-4.8.3.tar`

### file list

```diff
@@ -1,268 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    19877 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/requirements-spark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.200625 ydata-profiling-4.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.204625 ydata-profiling-4.7.0/src/pandas_profiling/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/pandas_profiling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.204625 ydata-profiling-4.7.0/src/ydata_profiling/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/compare_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/config_minimal.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.208625 ydata-profiling-4.7.0/src/ydata_profiling/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/controller/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/controller/pandas_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/expectations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.208625 ydata-profiling-4.7.0/src/ydata_profiling/model/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20409 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/description.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/expectation_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.212625 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/correlations_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_date_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_file_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_image_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_path_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_text_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_url_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/discretize_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/duplicates_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/imbalance_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/missing_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/sample_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/summary_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/table_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/timeseries_index_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/utils_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.216625 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/correlations_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/dataframe_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_boolean_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_categorical_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_counts_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_date_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_generic_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_numeric_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_supported_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_text_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/duplicates_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/missing_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/sample_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/summary_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/table_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/spark/timeseries_index_spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/summary_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/timeseries_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/typeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/model/typeset_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20108 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/profile_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.216625 ydata-profiling-4.7.0/src/ydata_profiling/report/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.216625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.220625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/item_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/renderable.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/root.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.220625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/flavours.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.224625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/root.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.224625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.228625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.228625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.228625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.232625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   121200 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   125618 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   127321 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    97163 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
--rw-r--r--   0 runner    (1001) docker     (127)   127551 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (127)   122851 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.236625 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/root.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/frequency_table_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.236625 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.236625 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/serialize_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/src/ydata_profiling/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/imghdr_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 18:30:06.000000 ydata-profiling-4.7.0/src/ydata_profiling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/missing.py
--rw-r--r--   0 runner    (1001) docker     (127)    33810 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/src/ydata_profiling/visualisation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.208625 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19877 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 18:30:07.000000 ydata-profiling-4.7.0/src/ydata_profiling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 18:30:07.240625 ydata-profiling-4.7.0/venv/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-18 18:22:52.000000 ydata-profiling-4.7.0/venv/spark.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/requirements-spark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.056603 ydata-profiling-4.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.060603 ydata-profiling-4.8.3/src/pandas_profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/pandas_profiling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.060603 ydata-profiling-4.8.3/src/ydata_profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/compare_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/config_minimal.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.060603 ydata-profiling-4.8.3/src/ydata_profiling/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/controller/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/controller/pandas_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/expectations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.064602 ydata-profiling-4.8.3/src/ydata_profiling/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20409 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/expectation_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.068602 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/correlations_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_boolean_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_categorical_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_counts_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_date_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_file_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_generic_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_image_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_numeric_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_path_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_supported_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_text_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_url_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/discretize_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/duplicates_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/imbalance_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/missing_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/sample_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/summary_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/table_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/timeseries_index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/utils_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.072603 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/correlations_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/dataframe_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_boolean_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_categorical_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_counts_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_date_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_generic_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_numeric_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_supported_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_text_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/duplicates_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/missing_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/sample_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/summary_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/table_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/spark/timeseries_index_spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/summary_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/timeseries_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/typeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/model/typeset_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20348 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/profile_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.072603 ydata-profiling-4.8.3/src/ydata_profiling/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.072603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.072603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/item_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/renderable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.072603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/flavours.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.076603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.080603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.080603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_constant_length.html
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_duplicates.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_empty.html
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_cardinality.html
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_high_correlation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_imbalance.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_infinite.html
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_missing.html
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_non_stationary.html
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_seasonal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_skewed.html
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_truncated.html
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_type_date.html
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_uniform.html
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unique.html
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_unsupported.html
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts/alert_zeros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/correlation_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/diagram.html
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/duplicate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sample.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.080603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/named_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/sections.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/variable.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.084602 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.084602 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121200 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   125618 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   127321 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    97163 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)   127551 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)   122851 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/variable_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.088603 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/correlation_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/variable_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/frequency_table_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.088603 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.088603 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/serialize_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/src/ydata_profiling/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/imghdr_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33810 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/src/ydata_profiling/visualisation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.060603 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20015 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14422 2024-05-07 20:05:24.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:05:23.000000 ydata-profiling-4.8.3/src/ydata_profiling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:05:24.092603 ydata-profiling-4.8.3/venv/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 20:04:21.000000 ydata-profiling-4.8.3/venv/spark.yml
```

### Comparing `ydata-profiling-4.7.0/CONTRIBUTING.md` & `ydata-profiling-4.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/LICENSE` & `ydata-profiling-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/MANIFEST.in` & `ydata-profiling-4.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/Makefile` & `ydata-profiling-4.8.3/Makefile`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/PKG-INFO` & `ydata-profiling-4.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.7.0
+Version: 4.8.3
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Keywords: pandas data-science data-analysis python jupyter ipython
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,14 +36,15 @@
 [![Build Status](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml)
 [![PyPI download month](https://img.shields.io/pypi/dm/ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/)
 [![](https://pepy.tech/badge/pandas-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code Coverage](https://codecov.io/gh/ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/ydataai/pandas-profiling)
 [![Release Version](https://img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://github.com/ydataai/pandas-profiling/releases)
 [![Python Version](https://img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc" />
 
 <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-profiling_black.png" alt="YData Profiling Logo"></p>
 
 <p align="center">
   <a href="https://ydata-profiling.ydata.ai/docs/master/">Documentation</a>
   |
   <a href="https://tiny.ydata.ai/dcai-ydata-profiling">Discord</a>
@@ -249,15 +250,15 @@
 
 ```sh
 pip install -e .
 ```
 
 The profiling report is written in HTML and CSS, which means a modern browser is required. 
 
-You need [Python 3](https://python3statement.org/) to run the package. Other dependencies can be found in the requirements files:
+You need [Python 3](https://python3statement.github.io/) to run the package. Other dependencies can be found in the requirements files:
 
 | Filename | Requirements|
 |----------|-------------|
 | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
 | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
 | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
 | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.7.0 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.8.3 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Keywords: pandas data-science data-analysis python jupyter ipython
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Build Tools Classifier: License :: OSI Approved :: MIT
 License Classifier: Environment :: Console Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Science/Research Classifier:
@@ -24,15 +24,16 @@
 pypi.org/project/ydata-profiling/) [![Code Coverage](https://codecov.io/gh/
 ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)]
 (https://codecov.io/gh/ydataai/pandas-profiling) [![Release Version](https://
 img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://
 github.com/ydataai/pandas-profiling/releases) [![Python Version](https://
 img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/
 ydata-profiling/) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/python/black)
+code%20style-black-000000.svg)](https://github.com/python/black)[https://
+static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc]
                             [YData Profiling Logo]
           _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d | _S_t_a_c_k_ _O_v_e_r_f_l_o_w | _L_a_t_e_s_t_ _c_h_a_n_g_e_l_o_g
         Do you like this project? Show us your love and _g_i_v_e_ _f_e_e_d_b_a_c_k_!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
@@ -196,18 +197,18 @@
 (https://anaconda.org/conda-forge/pandas-profiling) You can install using the
 `conda` package manager by running: ```sh conda install -c conda-forge ydata-
 profiling ``` ### From source (development) Download the source code by cloning
 the repository or click on [Download ZIP](https://github.com/ydataai/pandas-
 profiling/archive/master.zip) to download the latest stable version. Install it
 by navigating to the proper directory and running: ```sh pip install -e . ```
 The profiling report is written in HTML and CSS, which means a modern browser
-is required. You need [Python 3](https://python3statement.org/) to run the
-package. Other dependencies can be found in the requirements files: | Filename
-| Requirements| |----------|-------------| | [requirements.txt](https://
-github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
+is required. You need [Python 3](https://python3statement.github.io/) to run
+the package. Other dependencies can be found in the requirements files: |
+Filename | Requirements| |----------|-------------| | [requirements.txt](https:
+//github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
 contexts, `ydata-profiling` has a set of implicit and explicit integrations
```

### Comparing `ydata-profiling-4.7.0/README.md` & `ydata-profiling-4.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![Build Status](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml)
 [![PyPI download month](https://img.shields.io/pypi/dm/ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/)
 [![](https://pepy.tech/badge/pandas-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code Coverage](https://codecov.io/gh/ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/ydataai/pandas-profiling)
 [![Release Version](https://img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://github.com/ydataai/pandas-profiling/releases)
 [![Python Version](https://img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc" />
 
 <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-profiling_black.png" alt="YData Profiling Logo"></p>
 
 <p align="center">
   <a href="https://ydata-profiling.ydata.ai/docs/master/">Documentation</a>
   |
   <a href="https://tiny.ydata.ai/dcai-ydata-profiling">Discord</a>
@@ -216,15 +217,15 @@
 
 ```sh
 pip install -e .
 ```
 
 The profiling report is written in HTML and CSS, which means a modern browser is required. 
 
-You need [Python 3](https://python3statement.org/) to run the package. Other dependencies can be found in the requirements files:
+You need [Python 3](https://python3statement.github.io/) to run the package. Other dependencies can be found in the requirements files:
 
 | Filename | Requirements|
 |----------|-------------|
 | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
 | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
 | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
 | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
```

#### html2text {}

```diff
@@ -6,15 +6,16 @@
 pypi.org/project/ydata-profiling/) [![Code Coverage](https://codecov.io/gh/
 ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)]
 (https://codecov.io/gh/ydataai/pandas-profiling) [![Release Version](https://
 img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://
 github.com/ydataai/pandas-profiling/releases) [![Python Version](https://
 img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/
 ydata-profiling/) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/python/black)
+code%20style-black-000000.svg)](https://github.com/python/black)[https://
+static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc]
                             [YData Profiling Logo]
           _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d | _S_t_a_c_k_ _O_v_e_r_f_l_o_w | _L_a_t_e_s_t_ _c_h_a_n_g_e_l_o_g
         Do you like this project? Show us your love and _g_i_v_e_ _f_e_e_d_b_a_c_k_!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
@@ -178,18 +179,18 @@
 (https://anaconda.org/conda-forge/pandas-profiling) You can install using the
 `conda` package manager by running: ```sh conda install -c conda-forge ydata-
 profiling ``` ### From source (development) Download the source code by cloning
 the repository or click on [Download ZIP](https://github.com/ydataai/pandas-
 profiling/archive/master.zip) to download the latest stable version. Install it
 by navigating to the proper directory and running: ```sh pip install -e . ```
 The profiling report is written in HTML and CSS, which means a modern browser
-is required. You need [Python 3](https://python3statement.org/) to run the
-package. Other dependencies can be found in the requirements files: | Filename
-| Requirements| |----------|-------------| | [requirements.txt](https://
-github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
+is required. You need [Python 3](https://python3statement.github.io/) to run
+the package. Other dependencies can be found in the requirements files: |
+Filename | Requirements| |----------|-------------| | [requirements.txt](https:
+//github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
 contexts, `ydata-profiling` has a set of implicit and explicit integrations
```

### Comparing `ydata-profiling-4.7.0/make.bat` & `ydata-profiling-4.8.3/make.bat`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/setup.py` & `ydata-profiling-4.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/pandas_profiling/__init__.py` & `ydata-profiling-4.8.3/src/pandas_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/compare_reports.py` & `ydata-profiling-4.8.3/src/ydata_profiling/compare_reports.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/config.py` & `ydata-profiling-4.8.3/src/ydata_profiling/config.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/config_default.yaml` & `ydata-profiling-4.8.3/src/ydata_profiling/config_default.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/config_minimal.yaml` & `ydata-profiling-4.8.3/src/ydata_profiling/config_minimal.yaml`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/controller/console.py` & `ydata-profiling-4.8.3/src/ydata_profiling/controller/console.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/expectations_report.py` & `ydata-profiling-4.8.3/src/ydata_profiling/expectations_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/alerts.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/correlations.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/describe.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/describe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/description.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/description.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             return self.date_end - self.date_start
         if isinstance(self.date_start, list) and isinstance(self.date_end, list):
             return [
                 self.date_end[i] - self.date_start[i]
                 for i in range(len(self.date_start))
             ]
         else:
-            raise ValueError()
+            raise TypeError()
 
 
 @dataclass
 class TimeIndexAnalysis:
     """Description of timeseries index analysis module of report.
 
     Attributes:
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/expectation_algorithms.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/expectation_algorithms.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/handler.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/handler.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/missing.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pairwise.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pairwise.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/correlations_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/correlations_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/dataframe_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/dataframe_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_boolean_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_boolean_pandas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Tuple
 
+import numpy as np
 import pandas as pd
 
 from ydata_profiling.config import Settings
 from ydata_profiling.model.pandas.imbalance_pandas import column_imbalance_score
 from ydata_profiling.model.summary_algorithms import (
     describe_boolean_1d,
     series_hashable,
@@ -22,13 +23,21 @@
         series: The Series to describe.
         summary: The dict containing the series description so far.
 
     Returns:
         A dict containing calculated series description values.
     """
 
-    value_counts = summary["value_counts_without_nan"]
-    summary.update({"top": value_counts.index[0], "freq": value_counts.iloc[0]})
-
-    summary["imbalance"] = column_imbalance_score(value_counts, len(value_counts))
+    value_counts: pd.Series = summary["value_counts_without_nan"]
+    if not value_counts.empty:
+        summary.update({"top": value_counts.index[0], "freq": value_counts.iloc[0]})
+        summary["imbalance"] = column_imbalance_score(value_counts, len(value_counts))
+    else:
+        summary.update(
+            {
+                "top": np.nan,
+                "freq": 0,
+                "imbalance": 0,
+            }
+        )
 
     return config, series, summary
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_categorical_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_categorical_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,18 +191,22 @@
     length = series.str.len()
     length_counts = pd.Series(length.index, index=length)
     length_counts = length_counts.groupby(level=0, sort=False).sum()
     length_counts = length_counts.sort_values(ascending=False)
 
     summary = {
         "max_length": np.max(length_counts.index),
-        "mean_length": np.average(length_counts.index, weights=length_counts.values),
+        "mean_length": np.average(length_counts.index, weights=length_counts.values)
+        if not length_counts.empty
+        else np.nan,
         "median_length": weighted_median(
             length_counts.index.values, weights=length_counts.values
-        ),
+        )
+        if not length_counts.empty
+        else np.nan,
         "min_length": np.min(length_counts.index),
         "length_histogram": length_counts,
     }
 
     return summary
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_counts_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_counts_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_date_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_date_pandas.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,23 +25,33 @@
         config: report Settings object
         series: The Series to describe.
         summary: The dict containing the series description so far.
 
     Returns:
         A dict containing calculated series description values.
     """
-    summary.update(
-        {
-            "min": pd.Timestamp.to_pydatetime(series.min()),
-            "max": pd.Timestamp.to_pydatetime(series.max()),
-        }
-    )
+    if summary["value_counts_without_nan"].empty:
+        values = series.values
+        summary.update(
+            {
+                "min": pd.NaT,
+                "max": pd.NaT,
+                "range": 0,
+            }
+        )
+    else:
+        summary.update(
+            {
+                "min": pd.Timestamp.to_pydatetime(series.min()),
+                "max": pd.Timestamp.to_pydatetime(series.max()),
+            }
+        )
 
-    summary["range"] = summary["max"] - summary["min"]
+        summary["range"] = summary["max"] - summary["min"]
 
-    values = series.values.astype(np.int64) // 10**9
+        values = series.values.astype(np.int64) // 10**9
 
     if config.vars.num.chi_squared_threshold > 0.0:
         summary["chi_squared"] = chi_square(values)
 
     summary.update(histogram_compute(config, values, summary["n_distinct"]))
     return config, values, summary
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_file_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_file_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_generic_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_generic_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_image_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_image_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_numeric_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_numeric_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_path_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_path_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_supported_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_supported_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_text_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_text_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_timeseries_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/describe_url_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/describe_url_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/discretize_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/discretize_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/duplicates_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/duplicates_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/imbalance_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/imbalance_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/missing_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/missing_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/sample_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/sample_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/summary_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/summary_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/table_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/table_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/timeseries_index_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/timeseries_index_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/pandas/utils_pandas.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/pandas/utils_pandas.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/sample.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/correlations_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/correlations_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/dataframe_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/dataframe_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_boolean_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_boolean_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_categorical_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_categorical_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_counts_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_counts_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_date_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_date_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_generic_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_generic_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_numeric_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_numeric_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_supported_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_supported_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/describe_text_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/describe_text_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/duplicates_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/duplicates_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/missing_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/missing_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/sample_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/sample_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/summary_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/summary_spark.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,25 +83,31 @@
 
         Returns:
             A tuple with column and the series description.
         """
         column, df = args
         return column, describe_1d(config, df.select(column), summarizer, typeset)
 
+    # Rename the df column names to prevent potential conflicts
+    for col in df.columns:
+        df = df.withColumnRenamed(col, f"{col}_customer")
+
     args = [(name, df) for name in df.columns]
     with multiprocessing.pool.ThreadPool(12) as executor:
         for i, (column, description) in enumerate(
             executor.imap_unordered(multiprocess_1d, args)
         ):
+            if column.endswith("_customer"):
+                column = column[:-9]
             pbar.set_postfix_str(f"Describe variable:{column}")
 
             # summary clean up for spark
             description.pop("value_counts")
 
             series_description[column] = description
             pbar.update()
-        series_description = {k: series_description[k] for k in df.columns}
+        series_description = {k[:-9]: series_description[k[:-9]] for k in df.columns}
 
     # Mapping from column name to variable type
     series_description = sort_column_names(series_description, config.sort)
 
     return series_description
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/spark/table_spark.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/spark/table_spark.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/summarizer.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/summarizer.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/summary.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/summary.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/summary_algorithms.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/summary_algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     config: Settings,
     finite_values: np.ndarray,
     n_unique: int,
     name: str = "histogram",
     weights: Optional[np.ndarray] = None,
 ) -> dict:
     stats = {}
+    if len(finite_values) == 0:
+        return {name: []}
     hist_config = config.plot.histogram
     bins_arg = "auto" if hist_config.bins == 0 else min(hist_config.bins, n_unique)
     bins = np.histogram_bin_edges(finite_values, bins=bins_arg)
     if len(bins) > hist_config.max_bins:
         bins = np.histogram_bin_edges(finite_values, bins=hist_config.max_bins)
         weights = weights if weights and len(weights) == hist_config.max_bins else None
 
@@ -50,14 +52,16 @@
 
 def chi_square(
     values: Optional[np.ndarray] = None, histogram: Optional[np.ndarray] = None
 ) -> dict:
     if histogram is None:
         bins = np.histogram_bin_edges(values, bins="auto")
         histogram, _ = np.histogram(values, bins=bins)
+    if len(histogram) == 0 or np.sum(histogram) == 0:
+        return {"statistic": 0, "pvalue": 0}
     return dict(chisquare(histogram)._asdict())
 
 
 def series_hashable(
     fn: Callable[[Settings, pd.Series, dict], Tuple[Settings, pd.Series, dict]]
 ) -> Callable[[Settings, pd.Series, dict], Tuple[Settings, pd.Series, dict]]:
     @functools.wraps(fn)
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/typeset.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/typeset.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/model/typeset_relations.py` & `ydata-profiling-4.8.3/src/ydata_profiling/model/typeset_relations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/profile_report.py` & `ydata-profiling-4.8.3/src/ydata_profiling/profile_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,19 @@
 from ydata_profiling.report import get_report_structure
 from ydata_profiling.report.presentation.core import Root
 from ydata_profiling.report.presentation.flavours.html.templates import (
     create_html_assets,
 )
 from ydata_profiling.serialize_report import SerializeReport
 from ydata_profiling.utils.dataframe import hash_dataframe
+from ydata_profiling.utils.logger import ProfilingLogger
 from ydata_profiling.utils.paths import get_config
 
+logger = ProfilingLogger(name="ReportLogger")
+
 
 @typechecked
 class ProfileReport(SerializeReport, ExpectationsReport):
     """Generate a profile report from a Dataset stored as a pandas `DataFrame`.
 
     Used as is, it will output its content as an HTML report in a Jupyter notebook.
     """
@@ -87,15 +90,16 @@
         - config groups (e.g. `explorative` and `sensitive` arguments)
         - custom settings (e.g. `config` argument)
         - custom settings **kwargs (e.g. `title`)
 
         Args:
             df: a pandas or spark.sql DataFrame
             minimal: minimal mode is a default configuration with minimal computation
-            ts_mode: activates time-series analysis for all the numerical variables from the dataset. Only available for pd.DataFrame
+            ts_mode: activates time-series analysis for all the numerical variables from the dataset.
+            Only available for pd.DataFrame
             sort_by: ignored if ts_mode=False. Order the dataset by a provided column.
             sensitive: hides the values for categorical and text variables for report privacy
             config_file: a config file (.yml), mutually exclusive with `minimal`
             lazy: compute when needed
             sample: optional dict(name="Sample title", caption="Caption", data=pd.DataFrame())
             typeset: optional user typeset to use for type inference
             summarizer: optional user summarizer to generate custom summary output
@@ -195,14 +199,19 @@
                     "DataFrame is empty. Please" "provide a non-empty DataFrame."
                 )
 
     @staticmethod
     def __initialize_dataframe(
         df: Optional[Union[pd.DataFrame, sDataFrame]], report_config: Settings
     ) -> Optional[Union[pd.DataFrame, sDataFrame]]:
+
+        logger.info_def_report(
+            dataframe=type(df), timeseries=report_config.vars.timeseries.active
+        )
+
         if (
             df is not None
             and isinstance(df, pd.DataFrame)
             and report_config.vars.timeseries.active
         ):
             if report_config.vars.timeseries.sortby:
                 df = df.sort_values(by=report_config.vars.timeseries.sortby)
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/formatters.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/formatters.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/alerts.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/collapse.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/container.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/correlation_table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/dropdown.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/image.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/renderable.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/renderable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/root.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/root.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/sample.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/sample.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/variable.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/variable.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/core/variable_info.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/core/variable_info.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/flavours.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/flavours.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/alerts.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/container.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/correlation_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/duplicate.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/duplicate.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/frequency_table_small.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/report.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/report.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/batch_grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/grid.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/select.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/sequence/tabs.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/table.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/table.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/toggle_button.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/variable_info.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/cosmo.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/flatly.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/script.js`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/simplex.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/style.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/assets/united.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/javascript.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/navigation.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates/wrapper/style.html`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/html/templates.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/html/templates.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/alerts.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/alerts.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/collapse.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/collapse.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/container.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/container.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/dropdown.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/frequency_table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/frequency_table_small.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/image.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/notebook.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/notebook.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/table.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/table.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/flavours/widget/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/presentation/frequency_table_utils.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/presentation/frequency_table_utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/correlations.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/correlations.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/overview.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/overview.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/report.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/__init__.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_boolean.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_boolean.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_categorical.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_categorical.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_common.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_common.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_complex.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_complex.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_count.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_count.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_date.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,21 +99,22 @@
         )
     else:
         hist_data = histogram(
             config, summary["histogram"][0], summary["histogram"][1], date=True
         )
 
     # Bottom
+    n_bins = len(summary["histogram"][1]) - 1 if summary["histogram"] else 0
     bottom = Container(
         [
             Image(
                 hist_data,
                 image_format=image_format,
                 alt="Histogram",
-                caption=f"<strong>Histogram with fixed size bins</strong> (bins={len(summary['histogram'][1]) - 1})",
+                caption=f"<strong>Histogram with fixed size bins</strong> (bins={n_bins})",
                 name="Histogram",
                 anchor_id=f"{varid}histogram",
             )
         ],
         sequence_type="tabs",
         anchor_id=summary["varid"],
     )
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_file.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_file.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_generic.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_generic.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_image.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_image.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_path.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_path.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_real.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_real.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_text.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_text.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_timeseries.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_timeseries.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/report/structure/variables/render_url.py` & `ydata-profiling-4.8.3/src/ydata_profiling/report/structure/variables/render_url.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/serialize_report.py` & `ydata-profiling-4.8.3/src/ydata_profiling/serialize_report.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/utils/cache.py` & `ydata-profiling-4.8.3/src/ydata_profiling/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/utils/dataframe.py` & `ydata-profiling-4.8.3/src/ydata_profiling/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/utils/imghdr_patch.py` & `ydata-profiling-4.8.3/src/ydata_profiling/utils/imghdr_patch.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/utils/paths.py` & `ydata-profiling-4.8.3/src/ydata_profiling/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/visualisation/context.py` & `ydata-profiling-4.8.3/src/ydata_profiling/visualisation/context.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/visualisation/missing.py` & `ydata-profiling-4.8.3/src/ydata_profiling/visualisation/missing.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/visualisation/plot.py` & `ydata-profiling-4.8.3/src/ydata_profiling/visualisation/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,15 +739,15 @@
         method="ywm",
         color=color,
         vlines_kwargs={"colors": color},
     )
 
     for ax in axes:
         for item in ax.collections:
-            if type(item) == PolyCollection:
+            if type(item) is PolyCollection:
                 item.set_facecolor(color)
 
     return plot_360_n0sc0pe(config)
 
 
 def _plot_acf_pacf_comparison(
     config: Settings, series: List[pd.Series], figsize: tuple = (15, 5)
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling/visualisation/utils.py` & `ydata-profiling-4.8.3/src/ydata_profiling/visualisation/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling.egg-info/PKG-INFO` & `ydata-profiling-4.8.3/src/ydata_profiling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydata-profiling
-Version: 4.7.0
+Version: 4.8.3
 Summary: Generate profile report for pandas DataFrame
 Home-page: https://github.com/ydataai/ydata-profiling
 Author: YData Labs Inc
 Author-email: opensource@ydata.ai
 License: MIT
 Keywords: pandas data-science data-analysis python jupyter ipython
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,14 +36,15 @@
 [![Build Status](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/ydataai/pandas-profiling/actions/workflows/tests.yml)
 [![PyPI download month](https://img.shields.io/pypi/dm/ydata-profiling.svg)](https://pypi.python.org/pypi/ydata-profiling/)
 [![](https://pepy.tech/badge/pandas-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code Coverage](https://codecov.io/gh/ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)](https://codecov.io/gh/ydataai/pandas-profiling)
 [![Release Version](https://img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://github.com/ydataai/pandas-profiling/releases)
 [![Python Version](https://img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/ydata-profiling/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc" />
 
 <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-profiling_black.png" alt="YData Profiling Logo"></p>
 
 <p align="center">
   <a href="https://ydata-profiling.ydata.ai/docs/master/">Documentation</a>
   |
   <a href="https://tiny.ydata.ai/dcai-ydata-profiling">Discord</a>
@@ -249,15 +250,15 @@
 
 ```sh
 pip install -e .
 ```
 
 The profiling report is written in HTML and CSS, which means a modern browser is required. 
 
-You need [Python 3](https://python3statement.org/) to run the package. Other dependencies can be found in the requirements files:
+You need [Python 3](https://python3statement.github.io/) to run the package. Other dependencies can be found in the requirements files:
 
 | Filename | Requirements|
 |----------|-------------|
 | [requirements.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package requirements|
 | [requirements-dev.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-dev.txt)  |  Requirements for development|
 | [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/master/requirements-test.txt) | Requirements for testing|
 | [setup.py](https://github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for widgets etc. |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ydata-profiling Version: 4.7.0 Summary: Generate
+Metadata-Version: 2.1 Name: ydata-profiling Version: 4.8.3 Summary: Generate
 profile report for pandas DataFrame Home-page: https://github.com/ydataai/
 ydata-profiling Author: YData Labs Inc Author-email: opensource@ydata.ai
 License: MIT Keywords: pandas data-science data-analysis python jupyter ipython
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Build Tools Classifier: License :: OSI Approved :: MIT
 License Classifier: Environment :: Console Classifier: Operating System :: OS
 Independent Classifier: Intended Audience :: Science/Research Classifier:
@@ -24,15 +24,16 @@
 pypi.org/project/ydata-profiling/) [![Code Coverage](https://codecov.io/gh/
 ydataai/pandas-profiling/branch/master/graph/badge.svg?token=gMptB4YUnF)]
 (https://codecov.io/gh/ydataai/pandas-profiling) [![Release Version](https://
 img.shields.io/github/release/ydataai/pandas-profiling.svg)](https://
 github.com/ydataai/pandas-profiling/releases) [![Python Version](https://
 img.shields.io/pypi/pyversions/ydata-profiling)](https://pypi.org/project/
 ydata-profiling/) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/python/black)
+code%20style-black-000000.svg)](https://github.com/python/black)[https://
+static.scarf.sh/a.png?x-pxid=cb7e69df-af81-4352-809a-d4251756affc]
                             [YData Profiling Logo]
           _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d | _S_t_a_c_k_ _O_v_e_r_f_l_o_w | _L_a_t_e_s_t_ _c_h_a_n_g_e_l_o_g
         Do you like this project? Show us your love and _g_i_v_e_ _f_e_e_d_b_a_c_k_!
 `ydata-profiling` primary goal is to provide a one-line Exploratory Data
 Analysis (EDA) experience in a consistent and fast solution. Like pandas
 `df.describe()` function, that is so handy, ydata-profiling delivers an
 extended analysis of a DataFrame while allowing the data analysis to be
@@ -196,18 +197,18 @@
 (https://anaconda.org/conda-forge/pandas-profiling) You can install using the
 `conda` package manager by running: ```sh conda install -c conda-forge ydata-
 profiling ``` ### From source (development) Download the source code by cloning
 the repository or click on [Download ZIP](https://github.com/ydataai/pandas-
 profiling/archive/master.zip) to download the latest stable version. Install it
 by navigating to the proper directory and running: ```sh pip install -e . ```
 The profiling report is written in HTML and CSS, which means a modern browser
-is required. You need [Python 3](https://python3statement.org/) to run the
-package. Other dependencies can be found in the requirements files: | Filename
-| Requirements| |----------|-------------| | [requirements.txt](https://
-github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
+is required. You need [Python 3](https://python3statement.github.io/) to run
+the package. Other dependencies can be found in the requirements files: |
+Filename | Requirements| |----------|-------------| | [requirements.txt](https:
+//github.com/ydataai/pandas-profiling/blob/master/requirements.txt) | Package
 requirements| | [requirements-dev.txt](https://github.com/ydataai/pandas-
 profiling/blob/master/requirements-dev.txt) | Requirements for development| |
 [requirements-test.txt](https://github.com/ydataai/pandas-profiling/blob/
 master/requirements-test.txt) | Requirements for testing| | [setup.py](https://
 github.com/ydataai/pandas-profiling/blob/master/setup.py) | Requirements for
 widgets etc. | ## ð Integrations To maximize its usefulness in real world
 contexts, `ydata-profiling` has a set of implicit and explicit integrations
```

### Comparing `ydata-profiling-4.7.0/src/ydata_profiling.egg-info/SOURCES.txt` & `ydata-profiling-4.8.3/src/ydata_profiling.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -225,14 +225,15 @@
 src/ydata_profiling/report/structure/variables/render_url.py
 src/ydata_profiling/utils/__init__.py
 src/ydata_profiling/utils/cache.py
 src/ydata_profiling/utils/common.py
 src/ydata_profiling/utils/compat.py
 src/ydata_profiling/utils/dataframe.py
 src/ydata_profiling/utils/imghdr_patch.py
+src/ydata_profiling/utils/logger.py
 src/ydata_profiling/utils/notebook.py
 src/ydata_profiling/utils/paths.py
 src/ydata_profiling/utils/progress_bar.py
 src/ydata_profiling/utils/versions.py
 src/ydata_profiling/visualisation/__init__.py
 src/ydata_profiling/visualisation/context.py
 src/ydata_profiling/visualisation/missing.py
```

