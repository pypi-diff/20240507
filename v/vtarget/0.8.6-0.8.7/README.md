# Comparing `tmp/vtarget-0.8.6.tar.gz` & `tmp/vtarget-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtarget-0.8.6.tar", last modified: Wed Apr 10 13:56:00 2024, max compression
+gzip compressed data, was "vtarget-0.8.7.tar", last modified: Tue May  7 17:48:05 2024, max compression
```

## Comparing `vtarget-0.8.6.tar` & `vtarget-0.8.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.401853 vtarget-0.8.6/
--rw-rw-rw-   0        0        0     1494 2024-03-25 15:35:40.000000 vtarget-0.8.6/LICENSE
--rw-rw-rw-   0        0        0       58 2024-03-25 15:35:40.000000 vtarget-0.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2144 2024-04-10 13:56:00.399855 vtarget-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      806 2024-03-25 15:35:52.000000 vtarget-0.8.6/README.md
--rw-rw-rw-   0        0        0      100 2024-03-25 15:35:41.000000 vtarget-0.8.6/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-03-25 15:35:52.000000 vtarget-0.8.6/requirements.txt
--rw-rw-rw-   0        0        0       96 2024-04-10 13:56:00.403852 vtarget-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      826 2024-04-10 13:55:35.000000 vtarget-0.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.187866 vtarget-0.8.6/vtarget/
--rw-rw-rw-   0        0        0      146 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.217867 vtarget-0.8.6/vtarget/dataprep/
--rw-rw-rw-   0        0        0     2635 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/__init__.py
--rw-rw-rw-   0        0        0    37512 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/builder.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.338857 vtarget-0.8.6/vtarget/dataprep/nodes/
--rw-rw-rw-   0        0        0     2756 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/api_rest.py
--rw-rw-rw-   0        0        0     4933 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/code.py
--rw-rw-rw-   0        0        0     4148 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/column.py
--rw-rw-rw-   0        0        0     3232 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/concat.py
--rw-rw-rw-   0        0        0     3304 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cross_join.py
--rw-rw-rw-   0        0        0     3798 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cumsum.py
--rw-rw-rw-   0        0        0     2318 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cut.py
--rw-rw-rw-   0        0        0     5935 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/data_cleansing.py
--rw-rw-rw-   0        0        0     9143 2024-03-25 18:33:04.000000 vtarget-0.8.6/vtarget/dataprep/nodes/database.py
--rw-rw-rw-   0        0        0     7215 2024-03-25 18:33:04.000000 vtarget-0.8.6/vtarget/dataprep/nodes/database_write.py
--rw-rw-rw-   0        0        0     2384 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_extract.py
--rw-rw-rw-   0        0        0     2617 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_fill.py
--rw-rw-rw-   0        0        0     4681 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_formatter.py
--rw-rw-rw-   0        0        0     2465 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_range.py
--rw-rw-rw-   0        0        0     3612 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/describe.py
--rw-rw-rw-   0        0        0     1842 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/df_maker.py
--rw-rw-rw-   0        0        0     1792 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/drop_duplicates.py
--rw-rw-rw-   0        0        0     7409 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/dtype.py
--rw-rw-rw-   0        0        0     6583 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/email.py
--rw-rw-rw-   0        0        0     5993 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/excel.py
--rw-rw-rw-   0        0        0     9424 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/filter.py
--rw-rw-rw-   0        0        0     3392 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/formula.py
--rw-rw-rw-   0        0        0     5411 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/groupby.py
--rw-rw-rw-   0        0        0     6755 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/dataprep/nodes/input_data.py
--rw-rw-rw-   0        0        0     4160 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/inter_row.py
--rw-rw-rw-   0        0        0     2810 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/isin.py
--rw-rw-rw-   0        0        0     1820 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/melt.py
--rw-rw-rw-   0        0        0     6490 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/merge.py
--rw-rw-rw-   0        0        0     3112 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/output.py
--rw-rw-rw-   0        0        0     4404 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/pivot.py
--rw-rw-rw-   0        0        0     3133 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/rolling.py
--rw-rw-rw-   0        0        0     3151 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/sample.py
--rw-rw-rw-   0        0        0     1212 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/shape.py
--rw-rw-rw-   0        0        0     2024 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/sort.py
--rw-rw-rw-   0        0        0     3122 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/split.py
--rw-rw-rw-   0        0        0     8644 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/switch.py
--rw-rw-rw-   0        0        0     1513 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/unique.py
--rw-rw-rw-   0        0        0      616 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/v_output.py
--rw-rw-rw-   0        0        0     2500 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/value_counts.py
--rw-rw-rw-   0        0        0     8894 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/pipeline.py
--rw-rw-rw-   0        0        0     1542 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/types.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.360857 vtarget-0.8.6/vtarget/handlers/
--rw-rw-rw-   0        0        0     5301 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/automl_cache.py
--rw-rw-rw-   0        0        0     6508 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/autots_cache.py
--rw-rw-rw-   0        0        0     1856 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/bug_handler.py
--rw-rw-rw-   0        0        0     9116 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/cache_handler.py
--rw-rw-rw-   0        0        0     1449 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/event_handler.py
--rw-rw-rw-   0        0        0      464 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/log_handler.py
--rw-rw-rw-   0        0        0      172 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/script_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.366855 vtarget-0.8.6/vtarget/language/
--rw-rw-rw-   0        0        0    35956 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/language/app_message.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.384855 vtarget-0.8.6/vtarget/utils/
--rw-rw-rw-   0        0        0     4125 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/__init__.py
--rw-rw-rw-   0        0        0     1570 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/calc_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.393851 vtarget-0.8.6/vtarget/utils/database_connection/
--rw-rw-rw-   0        0        0     3311 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/database_connection/field_validation.py
--rw-rw-rw-   0        0        0     7400 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/database_connection/utilities.py
--rw-rw-rw-   0        0        0     3516 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/email_sender.py
--rw-rw-rw-   0        0        0      838 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/encrypter.py
--rw-rw-rw-   0        0        0    20811 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/modeling.py
--rw-rw-rw-   0        0        0    13591 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.397860 vtarget-0.8.6/vtarget.egg-info/
--rw-rw-rw-   0        0        0     2144 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2259 2024-04-10 13:56:00.000000 vtarget-0.8.6/vtarget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      531 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.569144 vtarget-0.8.7/
+-rw-rw-rw-   0        0        0     1522 2023-09-06 13:09:46.000000 vtarget-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-10-12 15:12:24.000000 vtarget-0.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2144 2024-05-07 17:48:05.569144 vtarget-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-05-07 15:58:06.000000 vtarget-0.8.7/README.md
+-rw-rw-rw-   0        0        0      102 2023-09-06 13:09:46.000000 vtarget-0.8.7/pyproject.toml
+-rw-rw-rw-   0        0        0      565 2024-05-07 15:58:06.000000 vtarget-0.8.7/requirements.txt
+-rw-rw-rw-   0        0        0       96 2024-05-07 17:48:05.570144 vtarget-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      858 2024-05-07 17:46:13.000000 vtarget-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.415104 vtarget-0.8.7/vtarget/
+-rw-rw-rw-   0        0        0      150 2024-02-20 16:12:28.000000 vtarget-0.8.7/vtarget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.441611 vtarget-0.8.7/vtarget/dataprep/
+-rw-rw-rw-   0        0        0     2795 2024-05-07 17:37:18.000000 vtarget-0.8.7/vtarget/dataprep/__init__.py
+-rw-rw-rw-   0        0        0    38254 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/builder.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.533682 vtarget-0.8.7/vtarget/dataprep/nodes/
+-rw-rw-rw-   0        0        0     2825 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/api_rest.py
+-rw-rw-rw-   0        0        0     5052 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/dataprep/nodes/code.py
+-rw-rw-rw-   0        0        0     4253 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/column.py
+-rw-rw-rw-   0        0        0     3307 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/concat.py
+-rw-rw-rw-   0        0        0     3379 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/cross_join.py
+-rw-rw-rw-   0        0        0     3878 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/cumsum.py
+-rw-rw-rw-   0        0        0     2378 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/cut.py
+-rw-rw-rw-   0        0        0     6040 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/data_cleansing.py
+-rw-rw-rw-   0        0        0     9332 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/database.py
+-rw-rw-rw-   0        0        0     7379 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/database_write.py
+-rw-rw-rw-   0        0        0     2436 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/datetime_extract.py
+-rw-rw-rw-   0        0        0     2671 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/datetime_fill.py
+-rw-rw-rw-   0        0        0     4771 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/datetime_formatter.py
+-rw-rw-rw-   0        0        0     2519 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/datetime_range.py
+-rw-rw-rw-   0        0        0     3688 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/dataprep/nodes/describe.py
+-rw-rw-rw-   0        0        0     1895 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/df_maker.py
+-rw-rw-rw-   0        0        0     1841 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/drop_duplicates.py
+-rw-rw-rw-   0        0        0     7560 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/dtype.py
+-rw-rw-rw-   0        0        0     6710 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/email.py
+-rw-rw-rw-   0        0        0     6114 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/excel.py
+-rw-rw-rw-   0        0        0     9615 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/filter.py
+-rw-rw-rw-   0        0        0     3479 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/formula.py
+-rw-rw-rw-   0        0        0     5536 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/groupby.py
+-rw-rw-rw-   0        0        0     6896 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/input_data.py
+-rw-rw-rw-   0        0        0     4248 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/dataprep/nodes/inter_row.py
+-rw-rw-rw-   0        0        0     2873 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/isin.py
+-rw-rw-rw-   0        0        0     1866 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/melt.py
+-rw-rw-rw-   0        0        0     6619 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/merge.py
+-rw-rw-rw-   0        0        0     3188 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/output.py
+-rw-rw-rw-   0        0        0     4501 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/pivot.py
+-rw-rw-rw-   0        0        0     3205 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/rolling.py
+-rw-rw-rw-   0        0        0     3222 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/sample.py
+-rw-rw-rw-   0        0        0     1248 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/shape.py
+-rw-rw-rw-   0        0        0     2078 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/dataprep/nodes/sort.py
+-rw-rw-rw-   0        0        0     3188 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/split.py
+-rw-rw-rw-   0        0        0     8801 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/switch.py
+-rw-rw-rw-   0        0        0     1556 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/dataprep/nodes/unique.py
+-rw-rw-rw-   0        0        0      640 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/dataprep/nodes/v_output.py
+-rw-rw-rw-   0        0        0     2560 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/nodes/value_counts.py
+-rw-rw-rw-   0        0        0     9076 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/pipeline.py
+-rw-rw-rw-   0        0        0     1601 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/dataprep/types.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.548570 vtarget-0.8.7/vtarget/handlers/
+-rw-rw-rw-   0        0        0     5475 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/handlers/automl_cache.py
+-rw-rw-rw-   0        0        0     6710 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/handlers/autots_cache.py
+-rw-rw-rw-   0        0        0     1925 2024-02-28 15:31:48.000000 vtarget-0.8.7/vtarget/handlers/bug_handler.py
+-rw-rw-rw-   0        0        0     9333 2024-02-20 16:12:28.000000 vtarget-0.8.7/vtarget/handlers/cache_handler.py
+-rw-rw-rw-   0        0        0     1499 2023-10-25 21:29:28.000000 vtarget-0.8.7/vtarget/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      483 2023-09-06 13:09:46.000000 vtarget-0.8.7/vtarget/handlers/log_handler.py
+-rw-rw-rw-   0        0        0      181 2023-09-06 13:09:46.000000 vtarget-0.8.7/vtarget/handlers/script_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.549571 vtarget-0.8.7/vtarget/language/
+-rw-rw-rw-   0        0        0    36540 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/language/app_message.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.562544 vtarget-0.8.7/vtarget/utils/
+-rw-rw-rw-   0        0        0     4252 2024-05-07 15:57:39.000000 vtarget-0.8.7/vtarget/utils/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-09-06 13:09:46.000000 vtarget-0.8.7/vtarget/utils/calc_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.565631 vtarget-0.8.7/vtarget/utils/database_connection/
+-rw-rw-rw-   0        0        0     3382 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/utils/database_connection/field_validation.py
+-rw-rw-rw-   0        0        0     7526 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/utils/database_connection/utilities.py
+-rw-rw-rw-   0        0        0     3623 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/utils/email_sender.py
+-rw-rw-rw-   0        0        0      861 2023-12-22 16:11:36.000000 vtarget-0.8.7/vtarget/utils/encrypter.py
+-rw-rw-rw-   0        0        0    21252 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/utils/modeling.py
+-rw-rw-rw-   0        0        0    13896 2024-05-07 15:58:07.000000 vtarget-0.8.7/vtarget/utils/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:48:05.566632 vtarget-0.8.7/vtarget.egg-info/
+-rw-rw-rw-   0        0        0     2144 2024-05-07 17:48:05.000000 vtarget-0.8.7/vtarget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2259 2024-05-07 17:48:05.000000 vtarget-0.8.7/vtarget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:48:05.000000 vtarget-0.8.7/vtarget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      531 2024-05-07 17:48:05.000000 vtarget-0.8.7/vtarget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 17:48:05.000000 vtarget-0.8.7/vtarget.egg-info/top_level.txt
```

### Comparing `vtarget-0.8.6/LICENSE` & `vtarget-0.8.7/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, vTarget
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, vTarget
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `vtarget-0.8.6/PKG-INFO` & `vtarget-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtarget
-Version: 0.8.6
+Version: 0.8.7
 Summary: vtarget lib
 Author: vTarget Team
 Author-email: contact@vtarget.ai
 License: BSD
 Keywords: vtarget,dataprep
 Requires-Python: >=3.9.0,<3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `vtarget-0.8.6/requirements.txt` & `vtarget-0.8.7/vtarget.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 numpy>=1.21.0
-pandas>=1.5.0,<2.0.0
+pandas<2.0.0,>=1.5.0
 scipy>=1.5.0
 scikit-learn>=1.2.1
 scikit-optimize>=0.9.0
 pyzmq>=20.0.0
 colorama>=0.4.4
 cloudpickle>=1.5.0
 click>=7.1.2
 shap>=0.40.0
 statsmodels>=0.12.2
 texttable>=1.6.2
-woodwork>= 0.21.1
-dask>=2022.2.0,!=2022.10.1
+woodwork>=0.21.1
+dask!=2022.10.1,>=2022.2.0
 nlp-primitives>=2.9.0
 featuretools>=1.16.0
-networkx>=2.5,<2.6
-
+networkx<2.6,>=2.5
 distributed==2023.5.0
 matplotlib>=3.7.1
 seaborn>=0.12.2
 termcolor
 pycryptodome>=3.18.0
 google-cloud-bigquery
 pyodbc
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/__init__.py` & `vtarget-0.8.7/vtarget/dataprep/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,95 @@
-from typing import Any, Dict
-
-
-def run_flow(path: str) -> Dict[str, Any]:
-    import gc
-    import json
-    import os
-
-    from vtarget.dataprep.builder import Builder
-    from vtarget.handlers.bug_handler import bug_handler
-    from vtarget.handlers.cache_handler import cache_handler
-    from vtarget.handlers.log_handler import log_handler
-
-    with open(path, "r") as content:
-        data = json.loads(content.read())
-
-    builder = Builder()
-
-    builder.init_pipeline()
-
-    flow_id = data["id"]
-
-    deploy_enabled = data["deployEnabled"] if "deployEnabled" in data else False
-
-    builder.analyzer(
-        data["model"],
-        True,
-        flow_id,
-        os.path.basename(path),
-        False,
-        False,
-        deploy_enabled,
-    )
-
-    del builder.pipeline
-
-    result = {
-        "status": True,
-        "flow_id": flow_id,
-        "nodes": {
-            # node_key: {
-            #     "status": True/False
-            #     "bugs":
-            # }
-        },
-        "logs": [],
-        "bugs": [],
-        "v_output": {
-            # node_key: dataframe
-        },
-        "message": "",
-    }
-
-    cache_handler.load_settings(flow_id)
-
-    for node_key in cache_handler.settings[flow_id]:
-        if node_key not in result["nodes"]:
-            result["nodes"][node_key] = dict()
-        result["nodes"][node_key]["status"] = True
-        result["nodes"][node_key]["bugs"] = []
-        result["nodes"][node_key]["logs"] = []
-        if "type" not in cache_handler.settings[flow_id][node_key]:
-            continue
-        if cache_handler.settings[flow_id][node_key]["type"] != "V_Output":
-            continue
-        if node_key not in result["v_output"]:
-            result["v_output"][node_key] = dict()
-        for port_name in cache_handler.settings[flow_id][node_key]["pout"]:
-            cache_handler.load(flow_id, node_key, port_name)
-            port = cache_handler.cache[flow_id][node_key]["pout"][port_name]
-            result["v_output"][node_key][port_name] = port
-
-    cache_handler.reset(flow_id)
-
-    gc.collect()
-
-    for bug in bug_handler.bug:
-        node_key = bug["node_key"] if "node_key" in bug else None
-        if node_key:
-            result["status"] = False
-            result["nodes"][node_key]["status"] = False
-            result["nodes"][node_key]["bugs"].append(bug)
-        else:
-            result["bugs"].append(bug)
-
-    for log in log_handler.log:
-        node_key = log["node_key"] if "node_key" in log else None
-        if node_key:
-            result["nodes"][node_key]["logs"].append(log)
-        else:
-            result["logs"].append(log)
-
-    return result
+from typing import Any, Dict
+
+
+def run_flow(path: str, enable_dump=False) -> Dict[str, Any]:
+    import gc
+    import json
+    import os
+
+    from vtarget.dataprep.builder import Builder
+    from vtarget.handlers.bug_handler import bug_handler
+    from vtarget.handlers.cache_handler import cache_handler
+    from vtarget.handlers.log_handler import log_handler
+
+    with open(path, "r") as content:
+        data = json.loads(content.read())
+
+    builder = Builder()
+
+    builder.init_pipeline()
+
+    flow_id = data["id"]
+
+    deploy_enabled = data["deployEnabled"] if "deployEnabled" in data else False
+
+    cache_handler.dump_enabled = enable_dump
+
+    builder.analyzer(
+        data["model"],
+        True,
+        flow_id,
+        os.path.basename(path),
+        False,
+        False,
+        deploy_enabled,
+    )
+
+    del builder.pipeline
+
+    result = {
+        "status": True,
+        "flow_id": flow_id,
+        "nodes": {
+            # node_key: {
+            #     "status": True/False
+            #     "bugs":
+            # }
+        },
+        "logs": [],
+        "bugs": [],
+        "v_output": {
+            # node_key: dataframe
+        },
+        "message": "",
+    }
+
+    cache_handler.load_settings(flow_id)
+
+    for node_key in cache_handler.settings[flow_id]:
+        if node_key not in result["nodes"]:
+            result["nodes"][node_key] = dict()
+        result["nodes"][node_key]["status"] = True
+        result["nodes"][node_key]["bugs"] = []
+        result["nodes"][node_key]["logs"] = []
+        if "type" not in cache_handler.settings[flow_id][node_key]:
+            continue
+        if cache_handler.settings[flow_id][node_key]["type"] != "V_Output":
+            continue
+        if node_key not in result["v_output"]:
+            result["v_output"][node_key] = dict()
+        for port_name in cache_handler.settings[flow_id][node_key]["pout"]:
+            cache_handler.load(flow_id, node_key, port_name)
+            port = cache_handler.cache[flow_id][node_key]["pout"][port_name]
+            result["v_output"][node_key][port_name] = port
+
+    cache_handler.reset(flow_id)
+
+    gc.collect()
+
+    for bug in bug_handler.bug:
+        node_key = bug["node_key"] if "node_key" in bug else None
+        if node_key:
+            result["status"] = False
+            result["nodes"][node_key]["status"] = False
+            result["nodes"][node_key]["bugs"].append(bug)
+        else:
+            result["bugs"].append(bug)
+
+    for log in log_handler.log:
+        node_key = log["node_key"] if "node_key" in log else None
+        if node_key:
+            result["nodes"][node_key]["logs"].append(log)
+        else:
+            result["logs"].append(log)
+
+    return result
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/builder.py` & `vtarget-0.8.7/vtarget/dataprep/builder.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,742 +1,742 @@
-from vtarget.language.app_message import app_message
-
-
-class Builder:
-    import pandas as pd
-
-    def __init__(self):
-        # self.compute_node_counter = 0
-        self.nodes: dict = {}
-        self.script: str = ""
-        self.init_script()  # resetea el script
-        self.cur_node_key: str = None
-        self.dumpings = 0
-        self.execution = 0
-        self.runnable = False
-        # self.ultra = None
-
-    def init_pipeline(self):
-        from vtarget.dataprep.pipeline import Pipeline
-
-        self.pipeline = Pipeline()
-
-    def init_script(self):
-        from vtarget.handlers.script_handler import script_handler
-
-        # Headers del script
-        script_handler.script.append("#!/usr/bin/env python")
-        script_handler.script.append("# coding: utf-8\n")
-        script_handler.script.append("import pandas as pd")
-        script_handler.script.append("import numpy as np")
-
-    def set_nodes(self, flow_id: str, data: dict):
-        from vtarget.handlers.bug_handler import bug_handler
-
-        self.nodes = {}  # Diccionario con los nodos del flujo cuya clave es el atributo "key" del nodo
-        for idx, nd in enumerate(data["nodeDataArray"]):
-            if not ("isGroup" in nd and nd["isGroup"]) and (nd["type"] not in ["Comment"]):  # and (nd["categoryId"] not in ["chart"]):  # no es grupo  # no es comment  # no es chart
-                self.nodes[nd["key"]] = {
-                    "idx": idx,
-                    "key": nd["key"],
-                    "skip": False,
-                    "name": nd["name"],
-                    "type": nd["type"],
-                    "output": None,
-                    "loaded": False,
-                    "childs": [],
-                    "parents": [],
-                    "disabled": True if "meta" in nd and "disabled" in nd["meta"] and nd["meta"]["disabled"] else False,
-                }
-
-        # * Recorre los links para obtener los padres e hijos por nodo
-        for ld in data["linkDataArray"]:
-            # if "_chart" in ld["to"]:
-            #     continue
-
-            # ! Valida que el nodo existe
-            if ld["to"] not in self.nodes:
-                # TODO: Agregar al diccionario
-                msg = f'link {ld["key"]} to {ld["to"]}: hace referencia a nodo inexistente ({ld["to"]})'
-                bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="warning", success=True)
-                continue
-
-            # ! Valida que el nodo existe
-            if ld["from"] not in self.nodes:
-                # TODO: Agregar al diccionario
-                msg = f'link {ld["key"]} from {ld["from"]}: hace referencia a nodo inexistente ({ld["from"]})'
-                bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="warning", success=True)
-                continue
-
-            # * Agrega los padres
-            parent = {"from": ld["from"], "frompid": ld["frompid"], "topid": ld["topid"]}
-            if not self.nodes[ld["to"]]["parents"]:
-                self.nodes[ld["to"]]["parents"] = [parent]
-            else:
-                self.nodes[ld["to"]]["parents"].append(parent)
-
-            # * Agrega los hijos
-            child = {"to": ld["to"], "topid": ld["topid"], "frompid": ld["frompid"], "to_idx": self.nodes[ld["to"]]["idx"]}
-            if not self.nodes[ld["from"]]["childs"]:
-                self.nodes[ld["from"]]["childs"] = [child]
-            else:
-                self.nodes[ld["from"]]["childs"].append(child)
-
-    def reset_childs_recursive(self, flow_id: str, node_key: str, reseted_nodes: list):
-        """Resetea todos los nodos hijos cuando cambia la configuración de un padre"""
-        
-        import gc
-
-        from vtarget.handlers.cache_handler import cache_handler
-
-        for child in self.nodes[node_key]["childs"]:
-            if child["to"] in cache_handler.settings[flow_id]:
-                print(node_key, "reset_childs_recursive")
-                del cache_handler.settings[flow_id][child["to"]]
-                reseted_nodes.append(child["to"])
-            self.reset_childs_recursive(flow_id, child["to"], reseted_nodes)
-        gc.collect()
-        return reseted_nodes
-
-    def set_skip_childs_recursive(self, flow_id: str, node_key: str, data: dict):
-        """Setea a True el parámetro para saltar (no-procesar) los nodos hijos cuando existe un error"""
-        
-        for child in self.nodes[node_key]["childs"]:
-            # Habilita la bandera para saltarse el nodo
-            self.nodes[child["to"]]["skip"] = True
-            # Resetea el df completo almacenado en RAM
-            self.nodes[child["to"]]["output"] = None
-            # Resetea el nodo de gojs
-            for port_name in data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"]:
-                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["head"] = []
-                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["rows"] = 0
-                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["cols"] = 0
-            data["nodeDataArray"][child["to_idx"]]["meta"]["skipped"] = True
-            print("=================> se saltará el nodo", child["to"])
-            self.set_skip_childs_recursive(flow_id, child["to"], data)
-        return True
-
-    def check_childs_loaded(self, node_key: str):
-        """Checkea si todos los hijos están listos"""
-        
-        loaded = True
-        for child in self.nodes[node_key]["childs"]:
-            if not self.nodes[child["to"]]["loaded"]:
-                loaded = False
-                break
-        return loaded
-
-    def dump_parents(self, flow_id, node_key):
-        """Manda a almacenar y liberar los padres que ya están listos"""
-        
-        import time
-
-        from vtarget.handlers.cache_handler import cache_handler
-
-        if not cache_handler.dump_enabled:
-            return
-
-        t = time.time()
-        if not self.nodes[node_key]["loaded"]:
-            return
-        for parent in self.nodes[node_key]["parents"]:
-            if self.check_childs_loaded(parent["from"]):
-                cache_handler.dump(flow_id, parent["from"])
-        if len(self.nodes[node_key]["childs"]) == 0:
-            cache_handler.dump(flow_id, node_key)
-        self.dumpings += time.time() - t
-
-    def stop_model(self):
-        self.runnable = False
-
-    def analyzer(
-        self,
-        data: dict,
-        reset_cache: bool,
-        flow_id: str,
-        flow_name: str,
-        disable_all_write_nodes: bool,
-        disable_all_email_nodes: bool,
-        deploy_enabled: bool = False,
-    ):
-        import gc
-        import json
-        import time
-        from typing import Any, Dict
-
-        import pandas as pd
-
-        from vtarget.dataprep.types import NodeType
-        from vtarget.handlers.bug_handler import bug_handler
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.handlers.event_handler import event_handler
-        from vtarget.handlers.log_handler import log_handler
-        from vtarget.handlers.script_handler import script_handler
-        import math
-
-        print("deploy_enabled", deploy_enabled)
-        
-        self.runnable = True
-        self.dumpings = 0
-        self.execution = 0
-
-        # * Reseteo de variables singleton para cada ejecución
-        log_handler.log = []
-        bug_handler.bug = []
-        script_handler.script = []
-
-        # * Si se corre el flujo reseteando la cache
-        if reset_cache:
-            msg = app_message.dataprep["builder"]["reset_cache"](flow_name)
-            bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
-            cache_handler.reset(flow_id)
-
-        # * Inicializa la caché para el flujo si es que aún no existe
-        cache_handler.load_settings(flow_id)
-        if flow_id not in cache_handler.cache:
-            cache_handler.cache[flow_id] = dict()
-
-        cache_nodes_keys = list(cache_handler.cache[flow_id].keys())
-        msg = app_message.dataprep["builder"]["nodes_in_cache"](str(len(cache_nodes_keys)))
-        bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
-
-        # * Hace una copia local de los nodos y su metadata
-        self.set_nodes(flow_id, data)
-
-        completed_nodes: list = []
-        num_nodes_ok: int = 0  # conteo del número de nodos procesados
-        attemps: int = 0  # contador de intentos del while para procesar el flujo completo
-        t1 = time.time()  # inicializa el tiempo total de procesamiento de los nodos
-
-        # * Itera mientras no estén todos los nodos procesados (prop loaded == True)
-        while self.runnable and num_nodes_ok < len(self.nodes):
-            # print(num_nodes_ok, "<", len(self.nodes))
-            attemps += 1
-            for node_key, node_data in self.nodes.items():
-                node_idx: int = self.nodes[node_key]["idx"]
-                
-                if not self.runnable:
-                    msg = app_message.dataprep["builder"]["stopped_flow"]
-                    bug_handler.default_node_log(flow_id, None, msg, console_level="error", bug_level="warning", success=True)
-                    break
-                
-                # * Salta los nodos que ya han sido procesados
-                if self.nodes[node_key]["loaded"]:
-                    continue
-
-                # * Salta los nodos output y email cuando el check de deshabilitar está activado
-                if (
-                    (disable_all_write_nodes and (node_data["type"] in [NodeType.OUTPUTDATA.value, NodeType.EXCEL.value, NodeType.DATABASEWRITE.value])) 
-                    or
-                    (disable_all_email_nodes and (node_data["type"] in [NodeType.EMAIL.value]))
-                    ):
-                    
-                    if node_data["type"] in [NodeType.EMAIL.value]:
-                        msg = app_message.dataprep["builder"]["not_send"](node_key)
-                    else:
-                        msg = app_message.dataprep["builder"]["skip_writing"](node_key)
-                    bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
-
-                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
-                    self.nodes[node_key]["loaded"] = True
-                    data["nodeDataArray"][node_idx]["meta"]["skipped"] = False
-                    self.dump_parents(flow_id, node_key)
-                    # * Agrega nodo a lista de completados
-                    if node_key not in completed_nodes:
-                        num_nodes_ok += 1
-                        completed_nodes.append(node_key)
-                    continue
-
-                # * Omitir el procesamiento de nodos saltados por un error en el nodo padre
-                if self.nodes[node_key]["skip"]:
-                    # TODO: Pancho aquí te falto traducción
-                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
-                    self.nodes[node_key]["loaded"] = True
-                    bug_handler.console("Nodo {} saltado".format(node_key), "trace", flow_id)
-                    # * Agrega nodo a lista de completados
-                    if node_key not in completed_nodes:
-                        num_nodes_ok += 1
-                        completed_nodes.append(node_key)
-                    continue
-                
-                # * Omitir el procesamiento de nodos deshabilitados desde la vista
-                if self.nodes[node_key]["disabled"]:
-                    # TODO: Pancho aquí te falto traducción
-                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
-                    self.nodes[node_key]["loaded"] = True
-                    bug_handler.console("Nodo {} dehabilitado".format(node_key), "trace", flow_id)
-                    # * Agrega nodo a lista de completados
-                    if node_key not in completed_nodes:
-                        num_nodes_ok += 1
-                        completed_nodes.append(node_key)
-                    continue
-
-                # * --------------------------------------------------
-                # * Determina si el nodo puede ser procesado
-                # * --------------------------------------------------
-                ready_to_exec = False # * Solo es verdadero cuando todos los nodos padres han sido procesados
-                to_load_input_port: Dict[str, Dict[str, Any]] = {}
-                # * Almacena los df del mapeo de los puertos de entrada
-                input_port: Dict[str, pd.DataFrame] = {}
-                
-                # * Si el nodo no posee padres, se puede procesar
-                if not node_data["parents"]:
-                    # * Nodos de entrada pueden procesarse inmediatamente ya que no tienen registro de nodos padres
-                    if node_data["type"] in [
-                        NodeType.INPUTDATA.value,
-                        NodeType.DFMAKER.value,
-                        NodeType.DATABASE.value,
-                        NodeType.SOURCE.value,
-                        NodeType.DATETIMERANGE.value,
-                        NodeType.APIREST.value,
-                    ]:
-                        ready_to_exec = True
-                    else:
-                        # * Error si el nodo no tiene registro de padres, pero debería tenerlos
-                        msg = app_message.dataprep["builder"]["parent_without_entry"](node_key)
-                        bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
-
-                        # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
-                        self.nodes[node_key]["loaded"] = True
-                        self.dump_parents(flow_id, node_key)
-                        # * Agrega nodo a lista de completados
-                        if node_key not in completed_nodes:
-                            num_nodes_ok += 1
-                            completed_nodes.append(node_key)
-                            
-                        # * Saltar rama del nodo
-                        self.set_skip_childs_recursive(flow_id, node_key, data)
-                        continue
-                    
-                else:  # * Si el nodo tiene padres
-                    # * Verificar que todos los padres tienen sus salidas cargadas (que han sido procesados)
-                    for parent in node_data["parents"]:
-                        ready_to_exec = True  # inicializo la carga en verdadero
-                        # * Si el nodo padre posee salida
-                        if self.nodes[parent["from"]]["output"] != None:
-                            # Almacena temporalmente la salida del padre para cargarla posteriomente como entrada del nodo hijo
-                            to_load_input_port[parent["topid"]] = {"node_key": parent["from"], "port_name": parent["frompid"]}
-                        else: 
-                            # *Si al menos un padre no está procesado, entonces termina la iteración
-                            ready_to_exec = False
-                            break
-
-                # * --------------------------------------------------
-                # * Si el nodo se puede procesar, inicia el procesamiento
-                # * --------------------------------------------------
-                if ready_to_exec:
-                    # node_key: str = data["nodeDataArray"][node_idx]["key"]
-                    # node_name: str = data["nodeDataArray"][node_idx]["name"]
-                    node_name: str = node_data["name"]
-                    has_error: bool = False
-                    self.cur_node_key = node_key
-
-                    node_settings = cache_handler.settings[flow_id][node_key] if node_key in cache_handler.settings[flow_id] else dict()
-                    node_in_cache = len(node_settings) > 0 and node_key in cache_handler.cache[flow_id]
-
-                    # * --------------------------------------------------
-                    # * Si el nodo actual está en caché y su config no ha cambiado, entonces no lo procesa
-                    # * --------------------------------------------------
-                    if (
-                        node_in_cache
-                        and "config" in node_settings
-                        and node_settings["config"] == json.dumps(data["nodeDataArray"][node_idx]["meta"]["config"], sort_keys=True)
-                        and (
-                            "ports_config" not in node_settings  # no existe ports_config en cache
-                            or (
-                                "ports_config" in node_settings  # existe ports_config en cache
-                                and node_settings["ports_config"]
-                                == json.dumps(
-                                    data["nodeDataArray"][node_idx]["meta"]["ports_config"],
-                                    sort_keys=True,
-                                )  # y ports_config no ha cambiado
-                            )
-                        )
-                    ):
-                        data["nodeDataArray"][node_idx]["meta"]["readed_from_cache"] = True
-                        data["nodeDataArray"][node_idx]["meta"]["processed"] = True
-                        script_handler.script += node_settings["script"]
-                    # * --------------------------------------------------
-                    # * De lo contrario, procesa y actualiza los valores de los df de salida
-                    # * --------------------------------------------------
-                    else:
-                        if node_data["type"] not in [
-                            NodeType.INPUTDATA.value,
-                            NodeType.DFMAKER.value,
-                            NodeType.DATABASE.value,
-                            NodeType.SOURCE.value,
-                            NodeType.DATETIMERANGE.value,
-                            NodeType.APIREST.value,
-                        ]:
-                            # * Recorre los puertos del entrada del nodo
-                            for _, pin_name in enumerate(data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"]):
-                                if "dtypes" in data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name] and pin_name in to_load_input_port:
-                                    # * Carga salida del padre desde caché
-                                    to_load = to_load_input_port[pin_name]
-                                    cache_handler.load(flow_id, to_load["node_key"], to_load["port_name"])
-                                    parent_key = to_load["node_key"]
-                                    parent_port = to_load["port_name"]
-                                    parent_cache = (
-                                        cache_handler.cache[flow_id][parent_key] if flow_id in cache_handler.cache and parent_key in cache_handler.cache[flow_id] else dict()
-                                    )
-                                    
-                                    # * Actualiza los dtypes de la entrada del nodo con el dataframe de la salida del nodo anterior
-                                    if parent_cache and "pout" in parent_cache and parent_port in parent_cache["pout"]:
-                                        input_port[pin_name] = parent_cache["pout"][parent_port]
-                                        dtypes_list = data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name]["dtypes"]
-                                        
-                                        # NOTE: ¿Esto se ejecuta siempre o solo la primera vez que se carga el nodo?
-                                        u_dtypes = self.update_inputs_dtypes(node_name, node_key, dtypes_list, input_port[pin_name])
-                                        data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name]["dtypes"] = u_dtypes
-                                        # print(pin_index, 'fin')
-
-                        # * --------------------------------------------------
-                        # * Verifica si el nodo existía en caché, pero su config se modificó
-                        # * --------------------------------------------------
-                        bug_handler.console(f"PROCESANDO NODO {node_key}", "-", flow_id)
-                        if node_settings and (
-                            (
-                                "config" in node_settings and node_settings["config"] != json.dumps(data["nodeDataArray"][node_idx]["meta"]["config"], sort_keys=True)
-                            )  # node config ha cambiado
-                            or (
-                                "ports_config" in node_settings  # existe ports_config en cache
-                                # and "ports_config" in data["nodeDataArray"][node_idx]["meta"]
-                                and node_settings["ports_config"] != json.dumps(data["nodeDataArray"][node_idx]["meta"]["ports_config"], sort_keys=True)
-                            )  # node ports_config ha cambiado
-                        ):
-                            # * Resetea la rama completa del nodo y envia lista de nodos a la vista
-                            reseted_nodes = self.reset_childs_recursive(flow_id, node_key, [node_key])
-                            event_handler.emit_queue.put(
-                                {
-                                    "name": "dataprep.reseted_nodes",
-                                    "data": {
-                                        "flow_id": flow_id,
-                                        "reseted_nodes": reseted_nodes,
-                                    },
-                                }
-                            )
-
-                        t = time.time()
-
-                        # ! Agrega parametro de despliegue a la config de cada nodo
-                        if "meta" in data["nodeDataArray"][node_idx] and "config" in data["nodeDataArray"][node_idx]["meta"]:
-                            data["nodeDataArray"][node_idx]["meta"]["config"]["deploy_enabled"] = deploy_enabled
-
-                        # * Procesa todos los nodos excepto los de tipo chart
-                        if "categoryId" in data["nodeDataArray"][node_idx] and data["nodeDataArray"][node_idx]["categoryId"] != "chart":
-                            # ! restea paginacion a 1
-                            if "ports_config" in data["nodeDataArray"][node_idx]["meta"] and data["nodeDataArray"][node_idx]["meta"]["ports_config"] is not None:
-                                for port in data["nodeDataArray"][node_idx]["meta"]["ports_config"]:
-                                    data["nodeDataArray"][node_idx]["meta"]["ports_config"][port]["page"] = 1
-                                    
-                            # * Ejecucion individual de cada nodo
-                            data["nodeDataArray"][node_idx] = self.pipeline.exec(flow_id, data["nodeDataArray"][node_idx], input_port)
-                        else:
-                            print(f'{data["nodeDataArray"][node_idx]["type"]} no se procesa')
-
-                        self.execution += time.time() - t
-                        # print(self.execution)
-
-                        has_error = (
-                            next(
-                                (x for x in bug_handler.bug if x["node_key"] == node_key and x["level"] == "error"),
-                                None,
-                            )
-                            != None
-                        )
-
-                        data["nodeDataArray"][node_idx]["meta"]["processed"] = True
-                        data["nodeDataArray"][node_idx]["meta"]["has_error"] = has_error
-
-                        # * Envía nodos procesado a la vista
-                        event_handler.emit_queue.put(
-                            {
-                                "name": "dataprep.node_processed",
-                                "data": {
-                                    "flow_id": flow_id,
-                                    "key": node_key,
-                                    "node": json.dumps(data["nodeDataArray"][node_idx], default=str),
-                                    "progress": math.floor(((num_nodes_ok+1) / len(self.nodes)) * 100) if len(self.nodes) > 0 else 0
-                                    # 'log': log_handler.log, # TODO: Hacer el log del nodo correspondiente
-                                },
-                            }
-                        )
-
-                    # * Establece que el nodo se ha procesado y se ha generado una salida
-                    self.nodes[node_key]["output"] = True
-                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
-                    self.nodes[node_key]["loaded"] = True
-                    self.dump_parents(flow_id, node_key)
-                    # * Agrega nodo a lista de completados
-                    if node_key not in completed_nodes:
-                        num_nodes_ok += 1
-                        completed_nodes.append(node_key)
-
-                    # * Verifica si el nodo fue procesado con error
-                    data["nodeDataArray"][node_idx]["meta"]["skipped"] = False
-                    if has_error:
-                        print("\n\n\n----------- has_error", has_error)
-                        cache_handler.delete_node(flow_id, node_key)
-                        data["nodeDataArray"][node_idx]["meta"]["has_error"] = True # * Marca nodo como error
-                        self.set_skip_childs_recursive(flow_id, node_key, data) # * Saltar rama del nodo
-
-        # * --------------------------------------------------
-        # * Fin del while y for principal
-        # * --------------------------------------------------
-        
-        cache_nodes_keys = list(cache_handler.settings[flow_id].keys())
-        msg = app_message.dataprep["builder"]["save_cache"](len(cache_nodes_keys))
-        bug_handler.default_node_log(flow_id, None, msg, console_level="debug", bug_level="info", success=True)
-
-        msg = app_message.dataprep["builder"]["processed_flow"](str(round(time.time() - t1, 3)))
-        bug_handler.default_node_log(flow_id, None, msg, console_level="debug", bug_level="info", success=True)
-
-        print(self.dumpings, "dumpings")
-        print(self.execution, "execution")
-
-        # Una vez que acaba la ejecución del flujo se conforma el script
-        self.script = "\n".join(script_handler.script)
-        cache_handler.dump_settings(flow_id)
-        del self.nodes
-        gc.collect()
-
-        return data
-
-    # ---------------------------------------------------------------------------------------
-    # Actualiza los dtypes utilizando el df que se está recibiendo de entrada
-    # y compara con lo que se tenía en la configuración, manejando tanto la
-    # creación de campos que antes no existían, como la eliminación de campos que fueron eliminados
-
-    def update_inputs_dtypes(self, node_name, node_key, current_dtypes, input_df: pd.DataFrame):
-        res = input_df.dtypes.to_frame("dtypes")
-        res = res["dtypes"].astype(str).reset_index()
-        updated_dtypes = {}
-        for i, x in res.iterrows():
-            updated_dtypes[x["index"]] = {
-                "dtype": x["dtypes"],
-                "selected": True,
-                "order": i,
-            }
-
-        return updated_dtypes
-        """
-        if not len(current_dtypes):
-            return current_dtypes
-
-        # Si hay que crear campos nuevos se agregarán al final
-        try:
-            max_order =  max(list(map(lambda x: x['order'], current_dtypes.values())))
-        except Exception as e:
-            print('Error (builder): ', e)
-            bug_handler.append({'flow_id':flow_id, 'success': False, 'node_key': None, 'level': 'error',
-                                        'msg': 'No fue obtener el max de la lista de dtypes', 'exception': str(e)})
-            return current_dtypes
-
-        for i,x in res.iterrows():
-            if x['index'] in current_dtypes: # si el campo en la salida está en el pin de entrada, sólo actualizo el tipo de dato
-                if node_name != 'Select': # los select, al permitir cambiar los datatypes no deben actualizarse
-                    current_dtypes[x['index']]['dtype'] = x['dtypes']
-            else: # si el campo no está, es porque se editó el flujo en algun punto intermedio y se debe crear el campo
-                # del current_dtypes[x['index']]
-                max_order += 1
-                current_dtypes[x['index']] = {'dtype': x['dtypes'], 'selected': True, 'order': max_order}
-                print('previamente no existía el campo "{}" en el nodo "{}", se agrega'.format(x['index'], node_name))
-                bug_handler.append({'flow_id':flow_id, 'success': True, 'node_key': node_key, 'level': 'info',
-                                        'msg': 'Campo "{}" no existía en el nodo "{}" previamente, se agrega'.format(x['index'], node_name), 'exception': ''})
-                # print('Campo "{}" no existe en nodo "{}" será omitido'.format(x['index'], node_name))
-        # print('\n\n\ncurrent_dtypes:\n')
-        # print(current_dtypes)
-        # Extraigo los campos que antes existían y ya no
-        removed_fields = list(set(current_dtypes.keys()) - set(res['index'].tolist()))
-        # Remuevo los campos que ya no existen
-        # current_dtypes = dict(filter(lambda i: i[0] in res['index'].tolist(), current_dtypes.items()))
-        for rf in removed_fields:
-            to_remove = current_dtypes[rf]
-            # print(rf, to_remove)
-            bug_handler.append({'flow_id':flow_id, 'success': True, 'node_key': node_key, 'level': 'warning',
-                                        'msg': 'Ya no existe el campo "{}" en el nodo "{}", se elimina de sus dtypes'.format(rf, node_name), 'exception': ''})
-            del current_dtypes[rf]
-
-        # print('\ncurrent_dtypes (modified):')
-        # print(current_dtypes)
-        return current_dtypes
-        """
-
-    def remove_flow_from_cache(self, flow_id: str):
-        """DEPRECATED"""
-        import gc
-
-        from vtarget.handlers.cache_handler import cache_handler
-
-        if flow_id in cache_handler.settings:
-            print("remove_flow_from_cache")
-            del cache_handler.settings[flow_id]
-        gc.collect()
-
-    def remove_nodes_from_cache(self, flow_id: str, node_keys: list[str]):
-        import gc
-
-        from vtarget.handlers.cache_handler import cache_handler
-
-        removeds = []
-        if flow_id in cache_handler.settings:
-            for node_key in node_keys:
-                if node_key in cache_handler.settings[flow_id]:
-                    if node_key not in removeds:
-                        removeds.append(node_key)
-                    del cache_handler.settings[flow_id][node_key]
-                    print("remove_nodes_from_cache")
-        if flow_id in cache_handler.cache:
-            for node_key in node_keys:
-                if node_key in cache_handler.cache[flow_id]:
-                    if node_key not in removeds:
-                        removeds.append(node_key)
-                    del cache_handler.cache[flow_id][node_key]
-
-        cache_handler.dump_settings(flow_id)
-        gc.collect()
-        return removeds
-
-    # Actualiza node['meta']['ports_map']['pout'][port_name]['summary']
-    def load_detailed_view(self, flow_id: str, node_key: str, port_name: str):
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.utils.utilities import utilities
-
-        # NOTE: No sé cuantas veces se ejecuta esta carga
-        cache_handler.load(flow_id, node_key, port_name)
-        if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
-            df = cache_handler.cache[flow_id][node_key]["pout"][port_name]
-            return utilities.viz_summary(df)
-        return {}
-
-    # Actualiza node['meta']['ports_map']['pout'][port_name]['describe']
-    def load_column_view(self, flow_id: str, node_key: str, port_name: str):
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.utils.utilities import utilities
-
-        # NOTE: No sé cuantas veces se ejecuta esta carga
-        cache_handler.load(flow_id, node_key, port_name)
-        if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
-            df = cache_handler.cache[flow_id][node_key]["pout"][port_name]
-            return utilities.get_central_tendency_measures(df)
-        return {}
-
-    def modify_node(self, flow_id: str, node_key: str, node: dict, port_name: str):
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.utils.utilities import utilities
-
-        try:
-            cache_handler.load(flow_id, node_key, port_name)
-            if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
-                cached_node = cache_handler.cache[flow_id][node_key]
-                if "pout" in cached_node and port_name in cached_node["pout"]:
-                    port_df = cached_node["pout"][port_name]
-                    port_config = utilities.get_table_config(node["meta"], port_name)
-                    head = utilities.get_head_of_df_as_list(port_df, port_config, flow_id, node_key, port_name)
-                    node["meta"]["ports_map"]["pout"][port_name]["head"] = head
-                else:
-                    msg = app_message.dataprep["builder"]["exec_flow"]
-                    return {
-                        "flow_id": flow_id,
-                        "node_key": node_key,
-                        "node": node,
-                        "success": False,
-                        "error": msg,
-                    }
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return {
-                "flow_id": flow_id,
-                "node_key": node_key,
-                "node": node,
-                "success": False,
-                "error": str(e),
-            }
-
-        return {"flow_id": flow_id, "node_key": node_key, "node": node, "success": True}
-
-    def run_node(self, flow_id: str, node_key: str, node: dict, links_to: list):
-        if "CHART" in node_key.upper():
-            return
-
-        import json
-        from typing import Dict
-
-        import pandas as pd
-
-        from vtarget.handlers.bug_handler import bug_handler
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.handlers.event_handler import event_handler
-
-        print("run node", node_key)
-
-        # Resetea los bug
-        bug_handler.bug = []
-
-        # Incializa la caché para el nodo si es que aún no existe
-        cache_handler.load_settings(flow_id)
-
-        # Almancena los df del mapeo de los puertos de entrada
-        input_port: Dict[str, pd.DataFrame] = {}
-
-        # Cargar la cache de los padres en los puertos de entrada del nodo
-        for ld in links_to:
-            if "_chart" in ld["to"]:
-                continue
-            parent_port = ld["frompid"]
-            parent_key = ld["from"]
-            node_port = ld["topid"]
-
-            cache_handler.load(flow_id, parent_key, parent_port)  # carga la cache del padre
-            parent_cache = cache_handler.cache[flow_id][parent_key] if flow_id in cache_handler.cache and parent_key in cache_handler.cache[flow_id] else dict()
-
-            if parent_cache and "pout" in parent_cache and parent_port in parent_cache["pout"]:
-                input_port[node_port] = parent_cache["pout"][parent_port]  # actualiza pin del nodo con la salida correspondiente del padre
-
-        # ! restea paginacion a 1
-        if "ports_config" in node["meta"] and node["meta"]["ports_config"] is not None:
-            for port in node["meta"]["ports_config"]:
-                node["meta"]["ports_config"][port]["page"] = 1
-
-        node = self.pipeline.exec(flow_id, node, input_port)
-
-        # Valida si la ejecucion del nodo tuvo algun error
-        has_error = (
-            next(
-                (x for x in bug_handler.bug if x["node_key"] == node_key and x["level"] == "error"),
-                None,
-            )
-            != None
-        )
-        node["meta"]["skipped"] = False
-        node["meta"]["processed"] = True
-        node["meta"]["has_error"] = has_error
-
-        event_handler.emit_queue.put(
-            {
-                "name": "dataprep.node_processed",
-                "data": {
-                    "flow_id": flow_id,
-                    "key": node_key,
-                    "node": json.dumps(node, default=str),
-                    "progress": 100
-                },
-            }
-        )
-
-        if has_error:
-            cache_handler.delete_node(flow_id, node_key)
-
-        # TODO: deberia guardarse el resultado en cache
-        cache_handler.dump_settings(flow_id)
-
-        return {
-            "flow_id": flow_id,
-            "key": node_key,
-            "node": json.dumps(node, default=str),
-        }
-
-
-if __name__ == "__main__":
-    b = Builder()
-    m = b.load_model()
-    print(m)
+from vtarget.language.app_message import app_message
+
+
+class Builder:
+    import pandas as pd
+
+    def __init__(self):
+        # self.compute_node_counter = 0
+        self.nodes: dict = {}
+        self.script: str = ""
+        self.init_script()  # resetea el script
+        self.cur_node_key: str = None
+        self.dumpings = 0
+        self.execution = 0
+        self.runnable = False
+        # self.ultra = None
+
+    def init_pipeline(self):
+        from vtarget.dataprep.pipeline import Pipeline
+
+        self.pipeline = Pipeline()
+
+    def init_script(self):
+        from vtarget.handlers.script_handler import script_handler
+
+        # Headers del script
+        script_handler.script.append("#!/usr/bin/env python")
+        script_handler.script.append("# coding: utf-8\n")
+        script_handler.script.append("import pandas as pd")
+        script_handler.script.append("import numpy as np")
+
+    def set_nodes(self, flow_id: str, data: dict):
+        from vtarget.handlers.bug_handler import bug_handler
+
+        self.nodes = {}  # Diccionario con los nodos del flujo cuya clave es el atributo "key" del nodo
+        for idx, nd in enumerate(data["nodeDataArray"]):
+            if not ("isGroup" in nd and nd["isGroup"]) and (nd["type"] not in ["Comment"]):  # and (nd["categoryId"] not in ["chart"]):  # no es grupo  # no es comment  # no es chart
+                self.nodes[nd["key"]] = {
+                    "idx": idx,
+                    "key": nd["key"],
+                    "skip": False,
+                    "name": nd["name"],
+                    "type": nd["type"],
+                    "output": None,
+                    "loaded": False,
+                    "childs": [],
+                    "parents": [],
+                    "disabled": True if "meta" in nd and "disabled" in nd["meta"] and nd["meta"]["disabled"] else False,
+                }
+
+        # * Recorre los links para obtener los padres e hijos por nodo
+        for ld in data["linkDataArray"]:
+            # if "_chart" in ld["to"]:
+            #     continue
+
+            # ! Valida que el nodo existe
+            if ld["to"] not in self.nodes:
+                # TODO: Agregar al diccionario
+                msg = f'link {ld["key"]} to {ld["to"]}: hace referencia a nodo inexistente ({ld["to"]})'
+                bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="warning", success=True)
+                continue
+
+            # ! Valida que el nodo existe
+            if ld["from"] not in self.nodes:
+                # TODO: Agregar al diccionario
+                msg = f'link {ld["key"]} from {ld["from"]}: hace referencia a nodo inexistente ({ld["from"]})'
+                bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="warning", success=True)
+                continue
+
+            # * Agrega los padres
+            parent = {"from": ld["from"], "frompid": ld["frompid"], "topid": ld["topid"]}
+            if not self.nodes[ld["to"]]["parents"]:
+                self.nodes[ld["to"]]["parents"] = [parent]
+            else:
+                self.nodes[ld["to"]]["parents"].append(parent)
+
+            # * Agrega los hijos
+            child = {"to": ld["to"], "topid": ld["topid"], "frompid": ld["frompid"], "to_idx": self.nodes[ld["to"]]["idx"]}
+            if not self.nodes[ld["from"]]["childs"]:
+                self.nodes[ld["from"]]["childs"] = [child]
+            else:
+                self.nodes[ld["from"]]["childs"].append(child)
+
+    def reset_childs_recursive(self, flow_id: str, node_key: str, reseted_nodes: list):
+        """Resetea todos los nodos hijos cuando cambia la configuración de un padre"""
+        
+        import gc
+
+        from vtarget.handlers.cache_handler import cache_handler
+
+        for child in self.nodes[node_key]["childs"]:
+            if child["to"] in cache_handler.settings[flow_id]:
+                print(node_key, "reset_childs_recursive")
+                del cache_handler.settings[flow_id][child["to"]]
+                reseted_nodes.append(child["to"])
+            self.reset_childs_recursive(flow_id, child["to"], reseted_nodes)
+        gc.collect()
+        return reseted_nodes
+
+    def set_skip_childs_recursive(self, flow_id: str, node_key: str, data: dict):
+        """Setea a True el parámetro para saltar (no-procesar) los nodos hijos cuando existe un error"""
+        
+        for child in self.nodes[node_key]["childs"]:
+            # Habilita la bandera para saltarse el nodo
+            self.nodes[child["to"]]["skip"] = True
+            # Resetea el df completo almacenado en RAM
+            self.nodes[child["to"]]["output"] = None
+            # Resetea el nodo de gojs
+            for port_name in data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"]:
+                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["head"] = []
+                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["rows"] = 0
+                data["nodeDataArray"][child["to_idx"]]["meta"]["ports_map"]["pout"][port_name]["cols"] = 0
+            data["nodeDataArray"][child["to_idx"]]["meta"]["skipped"] = True
+            print("=================> se saltará el nodo", child["to"])
+            self.set_skip_childs_recursive(flow_id, child["to"], data)
+        return True
+
+    def check_childs_loaded(self, node_key: str):
+        """Checkea si todos los hijos están listos"""
+        
+        loaded = True
+        for child in self.nodes[node_key]["childs"]:
+            if not self.nodes[child["to"]]["loaded"]:
+                loaded = False
+                break
+        return loaded
+
+    def dump_parents(self, flow_id, node_key):
+        """Manda a almacenar y liberar los padres que ya están listos"""
+        
+        import time
+
+        from vtarget.handlers.cache_handler import cache_handler
+
+        if not cache_handler.dump_enabled:
+            return
+
+        t = time.time()
+        if not self.nodes[node_key]["loaded"]:
+            return
+        for parent in self.nodes[node_key]["parents"]:
+            if self.check_childs_loaded(parent["from"]):
+                cache_handler.dump(flow_id, parent["from"])
+        if len(self.nodes[node_key]["childs"]) == 0:
+            cache_handler.dump(flow_id, node_key)
+        self.dumpings += time.time() - t
+
+    def stop_model(self):
+        self.runnable = False
+
+    def analyzer(
+        self,
+        data: dict,
+        reset_cache: bool,
+        flow_id: str,
+        flow_name: str,
+        disable_all_write_nodes: bool,
+        disable_all_email_nodes: bool,
+        deploy_enabled: bool = False,
+    ):
+        import gc
+        import json
+        import time
+        from typing import Any, Dict
+
+        import pandas as pd
+
+        from vtarget.dataprep.types import NodeType
+        from vtarget.handlers.bug_handler import bug_handler
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.handlers.event_handler import event_handler
+        from vtarget.handlers.log_handler import log_handler
+        from vtarget.handlers.script_handler import script_handler
+        import math
+
+        print("deploy_enabled", deploy_enabled)
+        
+        self.runnable = True
+        self.dumpings = 0
+        self.execution = 0
+
+        # * Reseteo de variables singleton para cada ejecución
+        log_handler.log = []
+        bug_handler.bug = []
+        script_handler.script = []
+
+        # * Si se corre el flujo reseteando la cache
+        if reset_cache:
+            msg = app_message.dataprep["builder"]["reset_cache"](flow_name)
+            bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
+            cache_handler.reset(flow_id)
+
+        # * Inicializa la caché para el flujo si es que aún no existe
+        cache_handler.load_settings(flow_id)
+        if flow_id not in cache_handler.cache:
+            cache_handler.cache[flow_id] = dict()
+
+        cache_nodes_keys = list(cache_handler.cache[flow_id].keys())
+        msg = app_message.dataprep["builder"]["nodes_in_cache"](str(len(cache_nodes_keys)))
+        bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
+
+        # * Hace una copia local de los nodos y su metadata
+        self.set_nodes(flow_id, data)
+
+        completed_nodes: list = []
+        num_nodes_ok: int = 0  # conteo del número de nodos procesados
+        attemps: int = 0  # contador de intentos del while para procesar el flujo completo
+        t1 = time.time()  # inicializa el tiempo total de procesamiento de los nodos
+
+        # * Itera mientras no estén todos los nodos procesados (prop loaded == True)
+        while self.runnable and num_nodes_ok < len(self.nodes):
+            # print(num_nodes_ok, "<", len(self.nodes))
+            attemps += 1
+            for node_key, node_data in self.nodes.items():
+                node_idx: int = self.nodes[node_key]["idx"]
+                
+                if not self.runnable:
+                    msg = app_message.dataprep["builder"]["stopped_flow"]
+                    bug_handler.default_node_log(flow_id, None, msg, console_level="error", bug_level="warning", success=True)
+                    break
+                
+                # * Salta los nodos que ya han sido procesados
+                if self.nodes[node_key]["loaded"]:
+                    continue
+
+                # * Salta los nodos output y email cuando el check de deshabilitar está activado
+                if (
+                    (disable_all_write_nodes and (node_data["type"] in [NodeType.OUTPUTDATA.value, NodeType.EXCEL.value, NodeType.DATABASEWRITE.value])) 
+                    or
+                    (disable_all_email_nodes and (node_data["type"] in [NodeType.EMAIL.value]))
+                    ):
+                    
+                    if node_data["type"] in [NodeType.EMAIL.value]:
+                        msg = app_message.dataprep["builder"]["not_send"](node_key)
+                    else:
+                        msg = app_message.dataprep["builder"]["skip_writing"](node_key)
+                    bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
+
+                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
+                    self.nodes[node_key]["loaded"] = True
+                    data["nodeDataArray"][node_idx]["meta"]["skipped"] = False
+                    self.dump_parents(flow_id, node_key)
+                    # * Agrega nodo a lista de completados
+                    if node_key not in completed_nodes:
+                        num_nodes_ok += 1
+                        completed_nodes.append(node_key)
+                    continue
+
+                # * Omitir el procesamiento de nodos saltados por un error en el nodo padre
+                if self.nodes[node_key]["skip"]:
+                    # TODO: Pancho aquí te falto traducción
+                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
+                    self.nodes[node_key]["loaded"] = True
+                    bug_handler.console("Nodo {} saltado".format(node_key), "trace", flow_id)
+                    # * Agrega nodo a lista de completados
+                    if node_key not in completed_nodes:
+                        num_nodes_ok += 1
+                        completed_nodes.append(node_key)
+                    continue
+                
+                # * Omitir el procesamiento de nodos deshabilitados desde la vista
+                if self.nodes[node_key]["disabled"]:
+                    # TODO: Pancho aquí te falto traducción
+                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
+                    self.nodes[node_key]["loaded"] = True
+                    bug_handler.console("Nodo {} dehabilitado".format(node_key), "trace", flow_id)
+                    # * Agrega nodo a lista de completados
+                    if node_key not in completed_nodes:
+                        num_nodes_ok += 1
+                        completed_nodes.append(node_key)
+                    continue
+
+                # * --------------------------------------------------
+                # * Determina si el nodo puede ser procesado
+                # * --------------------------------------------------
+                ready_to_exec = False # * Solo es verdadero cuando todos los nodos padres han sido procesados
+                to_load_input_port: Dict[str, Dict[str, Any]] = {}
+                # * Almacena los df del mapeo de los puertos de entrada
+                input_port: Dict[str, pd.DataFrame] = {}
+                
+                # * Si el nodo no posee padres, se puede procesar
+                if not node_data["parents"]:
+                    # * Nodos de entrada pueden procesarse inmediatamente ya que no tienen registro de nodos padres
+                    if node_data["type"] in [
+                        NodeType.INPUTDATA.value,
+                        NodeType.DFMAKER.value,
+                        NodeType.DATABASE.value,
+                        NodeType.SOURCE.value,
+                        NodeType.DATETIMERANGE.value,
+                        NodeType.APIREST.value,
+                    ]:
+                        ready_to_exec = True
+                    else:
+                        # * Error si el nodo no tiene registro de padres, pero debería tenerlos
+                        msg = app_message.dataprep["builder"]["parent_without_entry"](node_key)
+                        bug_handler.default_node_log(flow_id, None, msg, console_level="trace", bug_level="info", success=True)
+
+                        # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
+                        self.nodes[node_key]["loaded"] = True
+                        self.dump_parents(flow_id, node_key)
+                        # * Agrega nodo a lista de completados
+                        if node_key not in completed_nodes:
+                            num_nodes_ok += 1
+                            completed_nodes.append(node_key)
+                            
+                        # * Saltar rama del nodo
+                        self.set_skip_childs_recursive(flow_id, node_key, data)
+                        continue
+                    
+                else:  # * Si el nodo tiene padres
+                    # * Verificar que todos los padres tienen sus salidas cargadas (que han sido procesados)
+                    for parent in node_data["parents"]:
+                        ready_to_exec = True  # inicializo la carga en verdadero
+                        # * Si el nodo padre posee salida
+                        if self.nodes[parent["from"]]["output"] != None:
+                            # Almacena temporalmente la salida del padre para cargarla posteriomente como entrada del nodo hijo
+                            to_load_input_port[parent["topid"]] = {"node_key": parent["from"], "port_name": parent["frompid"]}
+                        else: 
+                            # *Si al menos un padre no está procesado, entonces termina la iteración
+                            ready_to_exec = False
+                            break
+
+                # * --------------------------------------------------
+                # * Si el nodo se puede procesar, inicia el procesamiento
+                # * --------------------------------------------------
+                if ready_to_exec:
+                    # node_key: str = data["nodeDataArray"][node_idx]["key"]
+                    # node_name: str = data["nodeDataArray"][node_idx]["name"]
+                    node_name: str = node_data["name"]
+                    has_error: bool = False
+                    self.cur_node_key = node_key
+
+                    node_settings = cache_handler.settings[flow_id][node_key] if node_key in cache_handler.settings[flow_id] else dict()
+                    node_in_cache = len(node_settings) > 0 and node_key in cache_handler.cache[flow_id]
+
+                    # * --------------------------------------------------
+                    # * Si el nodo actual está en caché y su config no ha cambiado, entonces no lo procesa
+                    # * --------------------------------------------------
+                    if (
+                        node_in_cache
+                        and "config" in node_settings
+                        and node_settings["config"] == json.dumps(data["nodeDataArray"][node_idx]["meta"]["config"], sort_keys=True)
+                        and (
+                            "ports_config" not in node_settings  # no existe ports_config en cache
+                            or (
+                                "ports_config" in node_settings  # existe ports_config en cache
+                                and node_settings["ports_config"]
+                                == json.dumps(
+                                    data["nodeDataArray"][node_idx]["meta"]["ports_config"],
+                                    sort_keys=True,
+                                )  # y ports_config no ha cambiado
+                            )
+                        )
+                    ):
+                        data["nodeDataArray"][node_idx]["meta"]["readed_from_cache"] = True
+                        data["nodeDataArray"][node_idx]["meta"]["processed"] = True
+                        script_handler.script += node_settings["script"]
+                    # * --------------------------------------------------
+                    # * De lo contrario, procesa y actualiza los valores de los df de salida
+                    # * --------------------------------------------------
+                    else:
+                        if node_data["type"] not in [
+                            NodeType.INPUTDATA.value,
+                            NodeType.DFMAKER.value,
+                            NodeType.DATABASE.value,
+                            NodeType.SOURCE.value,
+                            NodeType.DATETIMERANGE.value,
+                            NodeType.APIREST.value,
+                        ]:
+                            # * Recorre los puertos del entrada del nodo
+                            for _, pin_name in enumerate(data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"]):
+                                if "dtypes" in data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name] and pin_name in to_load_input_port:
+                                    # * Carga salida del padre desde caché
+                                    to_load = to_load_input_port[pin_name]
+                                    cache_handler.load(flow_id, to_load["node_key"], to_load["port_name"])
+                                    parent_key = to_load["node_key"]
+                                    parent_port = to_load["port_name"]
+                                    parent_cache = (
+                                        cache_handler.cache[flow_id][parent_key] if flow_id in cache_handler.cache and parent_key in cache_handler.cache[flow_id] else dict()
+                                    )
+                                    
+                                    # * Actualiza los dtypes de la entrada del nodo con el dataframe de la salida del nodo anterior
+                                    if parent_cache and "pout" in parent_cache and parent_port in parent_cache["pout"]:
+                                        input_port[pin_name] = parent_cache["pout"][parent_port]
+                                        dtypes_list = data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name]["dtypes"]
+                                        
+                                        # NOTE: ¿Esto se ejecuta siempre o solo la primera vez que se carga el nodo?
+                                        u_dtypes = self.update_inputs_dtypes(node_name, node_key, dtypes_list, input_port[pin_name])
+                                        data["nodeDataArray"][node_idx]["meta"]["ports_map"]["pin"][pin_name]["dtypes"] = u_dtypes
+                                        # print(pin_index, 'fin')
+
+                        # * --------------------------------------------------
+                        # * Verifica si el nodo existía en caché, pero su config se modificó
+                        # * --------------------------------------------------
+                        bug_handler.console(f"PROCESANDO NODO {node_key}", "-", flow_id)
+                        if node_settings and (
+                            (
+                                "config" in node_settings and node_settings["config"] != json.dumps(data["nodeDataArray"][node_idx]["meta"]["config"], sort_keys=True)
+                            )  # node config ha cambiado
+                            or (
+                                "ports_config" in node_settings  # existe ports_config en cache
+                                # and "ports_config" in data["nodeDataArray"][node_idx]["meta"]
+                                and node_settings["ports_config"] != json.dumps(data["nodeDataArray"][node_idx]["meta"]["ports_config"], sort_keys=True)
+                            )  # node ports_config ha cambiado
+                        ):
+                            # * Resetea la rama completa del nodo y envia lista de nodos a la vista
+                            reseted_nodes = self.reset_childs_recursive(flow_id, node_key, [node_key])
+                            event_handler.emit_queue.put(
+                                {
+                                    "name": "dataprep.reseted_nodes",
+                                    "data": {
+                                        "flow_id": flow_id,
+                                        "reseted_nodes": reseted_nodes,
+                                    },
+                                }
+                            )
+
+                        t = time.time()
+
+                        # ! Agrega parametro de despliegue a la config de cada nodo
+                        if "meta" in data["nodeDataArray"][node_idx] and "config" in data["nodeDataArray"][node_idx]["meta"]:
+                            data["nodeDataArray"][node_idx]["meta"]["config"]["deploy_enabled"] = deploy_enabled
+
+                        # * Procesa todos los nodos excepto los de tipo chart
+                        if "categoryId" in data["nodeDataArray"][node_idx] and data["nodeDataArray"][node_idx]["categoryId"] != "chart":
+                            # ! restea paginacion a 1
+                            if "ports_config" in data["nodeDataArray"][node_idx]["meta"] and data["nodeDataArray"][node_idx]["meta"]["ports_config"] is not None:
+                                for port in data["nodeDataArray"][node_idx]["meta"]["ports_config"]:
+                                    data["nodeDataArray"][node_idx]["meta"]["ports_config"][port]["page"] = 1
+                                    
+                            # * Ejecucion individual de cada nodo
+                            data["nodeDataArray"][node_idx] = self.pipeline.exec(flow_id, data["nodeDataArray"][node_idx], input_port)
+                        else:
+                            print(f'{data["nodeDataArray"][node_idx]["type"]} no se procesa')
+
+                        self.execution += time.time() - t
+                        # print(self.execution)
+
+                        has_error = (
+                            next(
+                                (x for x in bug_handler.bug if x["node_key"] == node_key and x["level"] == "error"),
+                                None,
+                            )
+                            != None
+                        )
+
+                        data["nodeDataArray"][node_idx]["meta"]["processed"] = True
+                        data["nodeDataArray"][node_idx]["meta"]["has_error"] = has_error
+
+                        # * Envía nodos procesado a la vista
+                        event_handler.emit_queue.put(
+                            {
+                                "name": "dataprep.node_processed",
+                                "data": {
+                                    "flow_id": flow_id,
+                                    "key": node_key,
+                                    "node": json.dumps(data["nodeDataArray"][node_idx], default=str),
+                                    "progress": math.floor(((num_nodes_ok+1) / len(self.nodes)) * 100) if len(self.nodes) > 0 else 0
+                                    # 'log': log_handler.log, # TODO: Hacer el log del nodo correspondiente
+                                },
+                            }
+                        )
+
+                    # * Establece que el nodo se ha procesado y se ha generado una salida
+                    self.nodes[node_key]["output"] = True
+                    # * Se establece como loaded = True para que no entre nuevamente en caso que el while haga mas de un intento
+                    self.nodes[node_key]["loaded"] = True
+                    self.dump_parents(flow_id, node_key)
+                    # * Agrega nodo a lista de completados
+                    if node_key not in completed_nodes:
+                        num_nodes_ok += 1
+                        completed_nodes.append(node_key)
+
+                    # * Verifica si el nodo fue procesado con error
+                    data["nodeDataArray"][node_idx]["meta"]["skipped"] = False
+                    if has_error:
+                        print("\n\n\n----------- has_error", has_error)
+                        cache_handler.delete_node(flow_id, node_key)
+                        data["nodeDataArray"][node_idx]["meta"]["has_error"] = True # * Marca nodo como error
+                        self.set_skip_childs_recursive(flow_id, node_key, data) # * Saltar rama del nodo
+
+        # * --------------------------------------------------
+        # * Fin del while y for principal
+        # * --------------------------------------------------
+        
+        cache_nodes_keys = list(cache_handler.settings[flow_id].keys())
+        msg = app_message.dataprep["builder"]["save_cache"](len(cache_nodes_keys))
+        bug_handler.default_node_log(flow_id, None, msg, console_level="debug", bug_level="info", success=True)
+
+        msg = app_message.dataprep["builder"]["processed_flow"](str(round(time.time() - t1, 3)))
+        bug_handler.default_node_log(flow_id, None, msg, console_level="debug", bug_level="info", success=True)
+
+        print(self.dumpings, "dumpings")
+        print(self.execution, "execution")
+
+        # Una vez que acaba la ejecución del flujo se conforma el script
+        self.script = "\n".join(script_handler.script)
+        cache_handler.dump_settings(flow_id)
+        del self.nodes
+        gc.collect()
+
+        return data
+
+    # ---------------------------------------------------------------------------------------
+    # Actualiza los dtypes utilizando el df que se está recibiendo de entrada
+    # y compara con lo que se tenía en la configuración, manejando tanto la
+    # creación de campos que antes no existían, como la eliminación de campos que fueron eliminados
+
+    def update_inputs_dtypes(self, node_name, node_key, current_dtypes, input_df: pd.DataFrame):
+        res = input_df.dtypes.to_frame("dtypes")
+        res = res["dtypes"].astype(str).reset_index()
+        updated_dtypes = {}
+        for i, x in res.iterrows():
+            updated_dtypes[x["index"]] = {
+                "dtype": x["dtypes"],
+                "selected": True,
+                "order": i,
+            }
+
+        return updated_dtypes
+        """
+        if not len(current_dtypes):
+            return current_dtypes
+
+        # Si hay que crear campos nuevos se agregarán al final
+        try:
+            max_order =  max(list(map(lambda x: x['order'], current_dtypes.values())))
+        except Exception as e:
+            print('Error (builder): ', e)
+            bug_handler.append({'flow_id':flow_id, 'success': False, 'node_key': None, 'level': 'error',
+                                        'msg': 'No fue obtener el max de la lista de dtypes', 'exception': str(e)})
+            return current_dtypes
+
+        for i,x in res.iterrows():
+            if x['index'] in current_dtypes: # si el campo en la salida está en el pin de entrada, sólo actualizo el tipo de dato
+                if node_name != 'Select': # los select, al permitir cambiar los datatypes no deben actualizarse
+                    current_dtypes[x['index']]['dtype'] = x['dtypes']
+            else: # si el campo no está, es porque se editó el flujo en algun punto intermedio y se debe crear el campo
+                # del current_dtypes[x['index']]
+                max_order += 1
+                current_dtypes[x['index']] = {'dtype': x['dtypes'], 'selected': True, 'order': max_order}
+                print('previamente no existía el campo "{}" en el nodo "{}", se agrega'.format(x['index'], node_name))
+                bug_handler.append({'flow_id':flow_id, 'success': True, 'node_key': node_key, 'level': 'info',
+                                        'msg': 'Campo "{}" no existía en el nodo "{}" previamente, se agrega'.format(x['index'], node_name), 'exception': ''})
+                # print('Campo "{}" no existe en nodo "{}" será omitido'.format(x['index'], node_name))
+        # print('\n\n\ncurrent_dtypes:\n')
+        # print(current_dtypes)
+        # Extraigo los campos que antes existían y ya no
+        removed_fields = list(set(current_dtypes.keys()) - set(res['index'].tolist()))
+        # Remuevo los campos que ya no existen
+        # current_dtypes = dict(filter(lambda i: i[0] in res['index'].tolist(), current_dtypes.items()))
+        for rf in removed_fields:
+            to_remove = current_dtypes[rf]
+            # print(rf, to_remove)
+            bug_handler.append({'flow_id':flow_id, 'success': True, 'node_key': node_key, 'level': 'warning',
+                                        'msg': 'Ya no existe el campo "{}" en el nodo "{}", se elimina de sus dtypes'.format(rf, node_name), 'exception': ''})
+            del current_dtypes[rf]
+
+        # print('\ncurrent_dtypes (modified):')
+        # print(current_dtypes)
+        return current_dtypes
+        """
+
+    def remove_flow_from_cache(self, flow_id: str):
+        """DEPRECATED"""
+        import gc
+
+        from vtarget.handlers.cache_handler import cache_handler
+
+        if flow_id in cache_handler.settings:
+            print("remove_flow_from_cache")
+            del cache_handler.settings[flow_id]
+        gc.collect()
+
+    def remove_nodes_from_cache(self, flow_id: str, node_keys: list[str]):
+        import gc
+
+        from vtarget.handlers.cache_handler import cache_handler
+
+        removeds = []
+        if flow_id in cache_handler.settings:
+            for node_key in node_keys:
+                if node_key in cache_handler.settings[flow_id]:
+                    if node_key not in removeds:
+                        removeds.append(node_key)
+                    del cache_handler.settings[flow_id][node_key]
+                    print("remove_nodes_from_cache")
+        if flow_id in cache_handler.cache:
+            for node_key in node_keys:
+                if node_key in cache_handler.cache[flow_id]:
+                    if node_key not in removeds:
+                        removeds.append(node_key)
+                    del cache_handler.cache[flow_id][node_key]
+
+        cache_handler.dump_settings(flow_id)
+        gc.collect()
+        return removeds
+
+    # Actualiza node['meta']['ports_map']['pout'][port_name]['summary']
+    def load_detailed_view(self, flow_id: str, node_key: str, port_name: str):
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.utils.utilities import utilities
+
+        # NOTE: No sé cuantas veces se ejecuta esta carga
+        cache_handler.load(flow_id, node_key, port_name)
+        if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
+            df = cache_handler.cache[flow_id][node_key]["pout"][port_name]
+            return utilities.viz_summary(df)
+        return {}
+
+    # Actualiza node['meta']['ports_map']['pout'][port_name]['describe']
+    def load_column_view(self, flow_id: str, node_key: str, port_name: str):
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.utils.utilities import utilities
+
+        # NOTE: No sé cuantas veces se ejecuta esta carga
+        cache_handler.load(flow_id, node_key, port_name)
+        if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
+            df = cache_handler.cache[flow_id][node_key]["pout"][port_name]
+            return utilities.get_central_tendency_measures(df)
+        return {}
+
+    def modify_node(self, flow_id: str, node_key: str, node: dict, port_name: str):
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.utils.utilities import utilities
+
+        try:
+            cache_handler.load(flow_id, node_key, port_name)
+            if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id]:
+                cached_node = cache_handler.cache[flow_id][node_key]
+                if "pout" in cached_node and port_name in cached_node["pout"]:
+                    port_df = cached_node["pout"][port_name]
+                    port_config = utilities.get_table_config(node["meta"], port_name)
+                    head = utilities.get_head_of_df_as_list(port_df, port_config, flow_id, node_key, port_name)
+                    node["meta"]["ports_map"]["pout"][port_name]["head"] = head
+                else:
+                    msg = app_message.dataprep["builder"]["exec_flow"]
+                    return {
+                        "flow_id": flow_id,
+                        "node_key": node_key,
+                        "node": node,
+                        "success": False,
+                        "error": msg,
+                    }
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return {
+                "flow_id": flow_id,
+                "node_key": node_key,
+                "node": node,
+                "success": False,
+                "error": str(e),
+            }
+
+        return {"flow_id": flow_id, "node_key": node_key, "node": node, "success": True}
+
+    def run_node(self, flow_id: str, node_key: str, node: dict, links_to: list):
+        if "CHART" in node_key.upper():
+            return
+
+        import json
+        from typing import Dict
+
+        import pandas as pd
+
+        from vtarget.handlers.bug_handler import bug_handler
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.handlers.event_handler import event_handler
+
+        print("run node", node_key)
+
+        # Resetea los bug
+        bug_handler.bug = []
+
+        # Incializa la caché para el nodo si es que aún no existe
+        cache_handler.load_settings(flow_id)
+
+        # Almancena los df del mapeo de los puertos de entrada
+        input_port: Dict[str, pd.DataFrame] = {}
+
+        # Cargar la cache de los padres en los puertos de entrada del nodo
+        for ld in links_to:
+            if "_chart" in ld["to"]:
+                continue
+            parent_port = ld["frompid"]
+            parent_key = ld["from"]
+            node_port = ld["topid"]
+
+            cache_handler.load(flow_id, parent_key, parent_port)  # carga la cache del padre
+            parent_cache = cache_handler.cache[flow_id][parent_key] if flow_id in cache_handler.cache and parent_key in cache_handler.cache[flow_id] else dict()
+
+            if parent_cache and "pout" in parent_cache and parent_port in parent_cache["pout"]:
+                input_port[node_port] = parent_cache["pout"][parent_port]  # actualiza pin del nodo con la salida correspondiente del padre
+
+        # ! restea paginacion a 1
+        if "ports_config" in node["meta"] and node["meta"]["ports_config"] is not None:
+            for port in node["meta"]["ports_config"]:
+                node["meta"]["ports_config"][port]["page"] = 1
+
+        node = self.pipeline.exec(flow_id, node, input_port)
+
+        # Valida si la ejecucion del nodo tuvo algun error
+        has_error = (
+            next(
+                (x for x in bug_handler.bug if x["node_key"] == node_key and x["level"] == "error"),
+                None,
+            )
+            != None
+        )
+        node["meta"]["skipped"] = False
+        node["meta"]["processed"] = True
+        node["meta"]["has_error"] = has_error
+
+        event_handler.emit_queue.put(
+            {
+                "name": "dataprep.node_processed",
+                "data": {
+                    "flow_id": flow_id,
+                    "key": node_key,
+                    "node": json.dumps(node, default=str),
+                    "progress": 100
+                },
+            }
+        )
+
+        if has_error:
+            cache_handler.delete_node(flow_id, node_key)
+
+        # TODO: deberia guardarse el resultado en cache
+        cache_handler.dump_settings(flow_id)
+
+        return {
+            "flow_id": flow_id,
+            "key": node_key,
+            "node": json.dumps(node, default=str),
+        }
+
+
+if __name__ == "__main__":
+    b = Builder()
+    m = b.load_model()
+    print(m)
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/api_rest.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/api_rest.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import json
-import pprint
-
-import numpy as np
-import pandas as pd
-import requests
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class ApiRest:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# APIREST")
-        method: str = settings["method"] if "method" in settings and settings["method"] else None
-        url: str = settings["url"] if "url" in settings and settings["url"] else None
-        headers: list = settings["headers"] if "headers" in settings and settings["headers"] else []
-        params: list = settings["params"] if "params" in settings and settings["params"] else []
-        items: str = settings["items"] if "items" in settings and settings["items"] else "data.items"
-
-        if not method:
-            msg = app_message["nodes"]["api-rest"]["no_method"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if not url:
-            msg = app_message["nodes"]["api-rest"]["no_url"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            # method = "GET"
-            # url = "https://api.clay.cl/v1/cuentas_bancarias/movimientos/"
-
-            headers = {item["prop"]: item["value"] for item in headers}
-            params = {item["prop"]: item["value"] for item in params}
-            print('0')
-            response = requests.request(
-                method,
-                url,
-                headers=headers,
-                params=params,
-            )
-            print('1')
-            script.append(
-                f"import requests\n\nresponse = requests.request(\n\t'{method}', \n\t'{url}', \n\theaders={headers}, \n\tparams={params}\n)\n\nresponse = response.json()"
-            )
-
-            response_json = response.json()
-            new_items = "".join([f'["{i}"]' for i in items.split(".")])
-            df = eval(f"pd.DataFrame(response_json{new_items})")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+import pprint
+
+import numpy as np
+import pandas as pd
+import requests
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class ApiRest:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# APIREST")
+        method: str = settings["method"] if "method" in settings and settings["method"] else None
+        url: str = settings["url"] if "url" in settings and settings["url"] else None
+        headers: list = settings["headers"] if "headers" in settings and settings["headers"] else []
+        params: list = settings["params"] if "params" in settings and settings["params"] else []
+        items: str = settings["items"] if "items" in settings and settings["items"] else "data.items"
+
+        if not method:
+            msg = app_message["nodes"]["api-rest"]["no_method"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if not url:
+            msg = app_message["nodes"]["api-rest"]["no_url"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            # method = "GET"
+            # url = "https://api.clay.cl/v1/cuentas_bancarias/movimientos/"
+
+            headers = {item["prop"]: item["value"] for item in headers}
+            params = {item["prop"]: item["value"] for item in params}
+            print('0')
+            response = requests.request(
+                method,
+                url,
+                headers=headers,
+                params=params,
+            )
+            print('1')
+            script.append(
+                f"import requests\n\nresponse = requests.request(\n\t'{method}', \n\t'{url}', \n\theaders={headers}, \n\tparams={params}\n)\n\nresponse = response.json()"
+            )
+
+            response_json = response.json()
+            new_items = "".join([f'["{i}"]' for i in items.split(".")])
+            df = eval(f"pd.DataFrame(response_json{new_items})")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/code.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/code.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import importlib
-import json
-from contextlib import redirect_stdout
-from io import StringIO
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.utilities import utilities
-
-
-class Code:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        code_snippet: str = settings["code"] if "code" in settings else ""
-        node_type: str = "CODE" if "code" in node_key.lower() else "SOURCE"
-        script.append(f"\n# {node_type}")
-
-        # Agrego los modulos y alias al entorno de variables globales
-        used_modules = utilities.find_imports(code_snippet)
-
-        for m in used_modules:
-            try:
-                if m["alias"]:
-                    globals()[m["alias"]] = importlib.import_module(m["name"])
-                else:
-                    globals().update(importlib.import_module(m["name"]).__dict__)
-
-            except ModuleNotFoundError as e:
-                import os
-                import subprocess
-
-                current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
-                python_path = os.path.join(current_path, "python", "python.exe")
-                if os.path.exists(python_path):
-                    subprocess.run(
-                        [
-                            python_path,
-                            "-m",
-                            "pipenv",
-                            "install",
-                            "--skip-lock",
-                            m["name"].split(".")[0],
-                        ]
-                    )
-
-                else:
-                    import pip
-
-                    pip.main(["install", m["name"].split(".")[0]])
-                if m["alias"]:
-                    globals()[m["alias"]] = importlib.import_module(m["name"])
-                else:
-                    globals().update(importlib.import_module(m["name"]).__dict__)
-
-        def vtg_codeout(x):
-            global vtg_df, vtg_metacode
-            vtg_df = x.copy()
-
-        loc = {f"df_{k.lower()}": v.copy() for k, v in pin.items()}
-        loc["vtg_codeout"] = vtg_codeout
-        stdout = ""
-
-        try:
-            out = StringIO()
-            with redirect_stdout(out):
-                # NOTE: Antes estaba como exec(code_snippet, None, loc).
-                # NOTE: Tener en cuenta en caso de que se encuentre algun fallo
-                exec(code_snippet, loc)
-            stdout = out.getvalue()
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            default = bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            default["STDOUT"] = stdout
-            default["STDOUT"] += str(e)
-            return default
-        else:
-            script.append(code_snippet)
-            df_out = globals()["vtg_df"] if "vtg_df" in globals() else []
-            globals()["vtg_df"] = []
-            if not isinstance(df_out, pd.DataFrame):
-                msg = app_message.dataprep["nodes"]["code"]["no_vtg_codeout"](node_key)
-                default = bug_handler.default_node_log(flow_id, node_key, msg, "", "error")
-                default["STDOUT"] = stdout
-                return default
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {"pout": {"Out": df_out}, "config": json.dumps(settings, sort_keys=True), "script": script},
-        )
-
-        script_handler.script += script
-        return {"Out": df_out, "STDOUT": stdout}
-
-    # def find_imports(self, code_snippet):
-    #     # Busco los modulos que tienen la forma ['import * as *']
-    #     matchs = re.findall("import (.*?) as (.*?)$", code_snippet, flags=re.MULTILINE)
-    #     # print(matchs)
-    #     out = [{"name": m[0].strip(), "alias": m[1].strip(), "objects": []} for m in matchs]
-    #     # print(out)
-    #     # Busco los ['from * import *', 'import *']
-    #     # modules = []
-    #     for node in ast.iter_child_nodes(ast.parse(code_snippet)):
-    #         if isinstance(node, ast.ImportFrom):
-    #             objects = [node.names[i].name for i in range(len(node.names))]
-    #             if not node.names[0].asname:  # excluding the 'as' part of import
-    #                 # modules.append(node.module)
-    #                 out.append({"name": node.module, "alias": None, "objects": objects})
-    #         elif isinstance(node, ast.Import):  # excluding the 'as' part of import
-    #             if not node.names[0].asname:
-    #                 out.append({"name": node.names[0].name, "alias": None, "objects": []})
-    #                 # modules.append(node.names[0].name)
-    #     return out
+import importlib
+import json
+from contextlib import redirect_stdout
+from io import StringIO
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.utilities import utilities
+
+
+class Code:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        code_snippet: str = settings["code"] if "code" in settings else ""
+        node_type: str = "CODE" if "code" in node_key.lower() else "SOURCE"
+        script.append(f"\n# {node_type}")
+
+        # Agrego los modulos y alias al entorno de variables globales
+        used_modules = utilities.find_imports(code_snippet)
+
+        for m in used_modules:
+            try:
+                if m["alias"]:
+                    globals()[m["alias"]] = importlib.import_module(m["name"])
+                else:
+                    globals().update(importlib.import_module(m["name"]).__dict__)
+
+            except ModuleNotFoundError as e:
+                import os
+                import subprocess
+
+                current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+                python_path = os.path.join(current_path, "python", "python.exe")
+                if os.path.exists(python_path):
+                    subprocess.run(
+                        [
+                            python_path,
+                            "-m",
+                            "pipenv",
+                            "install",
+                            "--skip-lock",
+                            m["name"].split(".")[0],
+                        ]
+                    )
+
+                else:
+                    import pip
+
+                    pip.main(["install", m["name"].split(".")[0]])
+                if m["alias"]:
+                    globals()[m["alias"]] = importlib.import_module(m["name"])
+                else:
+                    globals().update(importlib.import_module(m["name"]).__dict__)
+
+        def vtg_codeout(x):
+            global vtg_df, vtg_metacode
+            vtg_df = x.copy()
+
+        loc = {f"df_{k.lower()}": v.copy() for k, v in pin.items()}
+        loc["vtg_codeout"] = vtg_codeout
+        stdout = ""
+
+        try:
+            out = StringIO()
+            with redirect_stdout(out):
+                # NOTE: Antes estaba como exec(code_snippet, None, loc).
+                # NOTE: Tener en cuenta en caso de que se encuentre algun fallo
+                exec(code_snippet, loc)
+            stdout = out.getvalue()
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            default = bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            default["STDOUT"] = stdout
+            default["STDOUT"] += str(e)
+            return default
+        else:
+            script.append(code_snippet)
+            df_out = globals()["vtg_df"] if "vtg_df" in globals() else []
+            globals()["vtg_df"] = []
+            if not isinstance(df_out, pd.DataFrame):
+                msg = app_message.dataprep["nodes"]["code"]["no_vtg_codeout"](node_key)
+                default = bug_handler.default_node_log(flow_id, node_key, msg, "", "error")
+                default["STDOUT"] = stdout
+                return default
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {"pout": {"Out": df_out}, "config": json.dumps(settings, sort_keys=True), "script": script},
+        )
+
+        script_handler.script += script
+        return {"Out": df_out, "STDOUT": stdout}
+
+    # def find_imports(self, code_snippet):
+    #     # Busco los modulos que tienen la forma ['import * as *']
+    #     matchs = re.findall("import (.*?) as (.*?)$", code_snippet, flags=re.MULTILINE)
+    #     # print(matchs)
+    #     out = [{"name": m[0].strip(), "alias": m[1].strip(), "objects": []} for m in matchs]
+    #     # print(out)
+    #     # Busco los ['from * import *', 'import *']
+    #     # modules = []
+    #     for node in ast.iter_child_nodes(ast.parse(code_snippet)):
+    #         if isinstance(node, ast.ImportFrom):
+    #             objects = [node.names[i].name for i in range(len(node.names))]
+    #             if not node.names[0].asname:  # excluding the 'as' part of import
+    #                 # modules.append(node.module)
+    #                 out.append({"name": node.module, "alias": None, "objects": objects})
+    #         elif isinstance(node, ast.Import):  # excluding the 'as' part of import
+    #             if not node.names[0].asname:
+    #                 out.append({"name": node.names[0].name, "alias": None, "objects": []})
+    #                 # modules.append(node.names[0].name)
+    #     return out
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/column.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/column.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Column:
-    def __init__(self):
-        self.script = []
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        df = pin["In"].copy()
-
-        self.script.append("\n# COLUMN")
-        if "items" not in settings or not settings["items"]:
-            msg = app_message["nodes"]["column"]["no_columns_selected"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        # Obtener df con las columnas seleccionadas y su orden, dtypes actualizados, lista con los nuevos nombres de las columnas
-        df, _, rename_cols = self.select_types_and_fields(flow_id, node_key, df, settings["items"])
-
-        # Si hay alguna columna para renombrar en las seleccionadas
-        if rename_cols:
-            try:
-                df = df.rename(columns=rename_cols)
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["column"]["rename_columns"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            
-            self.script.append("\n# Rename columns")
-            self.script.append("df = df.rename(columns={})".format(rename_cols))
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": self.script,
-            },
-        )
-
-        script_handler.script += self.script.copy()
-        self.script = []
-
-        return {"Out": df}
-
-    def select_types_and_fields(self, flow_id: str, node_key: str, df: pd.DataFrame, dtypes: dict):
-        """Retorna el df con las columnas seleccionadas y el orden dado
-
-        Args:
-            flow_id (str): id del flujo
-            node_key (str): id del nodo
-            df (pd.DataFrame): dataframe de entrada
-            dtypes (dict): configuracion de las columnas (selected, order)
-
-        Returns:
-            tuple: df, dtypes, rename_cols
-        """
-        
-        # https://pbpython.com/pandas_dtypes.html
-        # Obtener solo las columnas seleccionadas de la lista inicial (selected==True)
-        selected = dict(
-            filter(
-                lambda x: True if "selected" in x[1] and x[1]["selected"] else False,
-                dtypes.items(),
-            )
-        )
-
-        # Existe la posibilidad de que ya no existan columnas que previamente fueron creadas
-        available_cols = []
-        removed_cols = []
-        for field, _ in selected.items():
-            if field in df.columns:
-                available_cols.append(field)
-            else:
-                removed_cols.append(field)
-                del dtypes[field]  # dado que no existe la eliminamos de dtypes
-                msg = app_message.dataprep["nodes"]["column"]["column_not_in_df"](node_key, field)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
-
-        # Remover las columnas que ya no existen
-        for del_key in removed_cols:
-            del selected[del_key]
-
-        # Mantener solamente columnas existentes y seleccionadas
-        df = df[available_cols]
-        
-        self.script.append("df = df[{}]".format(available_cols))
-        self.script.append("\n# DATA TYPES")
-
-        # Diccionario para el renombrado de columnas
-        rename_cols = {}
-        for field, _ in selected.items():
-            if "rename" in dtypes[field] and dtypes[field]["rename"]:
-                rename_cols[field] = dtypes[field]["rename"]
-
-        # Ordena las columnas segun el orden dado en la configuracion del nodo
-        order_cols = list(dict(sorted(selected.items(), key=lambda item: item[1]["order"])).keys())
-
-        return df[order_cols], dtypes, rename_cols
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Column:
+    def __init__(self):
+        self.script = []
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        df = pin["In"].copy()
+
+        self.script.append("\n# COLUMN")
+        if "items" not in settings or not settings["items"]:
+            msg = app_message["nodes"]["column"]["no_columns_selected"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        # Obtener df con las columnas seleccionadas y su orden, dtypes actualizados, lista con los nuevos nombres de las columnas
+        df, _, rename_cols = self.select_types_and_fields(flow_id, node_key, df, settings["items"])
+
+        # Si hay alguna columna para renombrar en las seleccionadas
+        if rename_cols:
+            try:
+                df = df.rename(columns=rename_cols)
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["column"]["rename_columns"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            
+            self.script.append("\n# Rename columns")
+            self.script.append("df = df.rename(columns={})".format(rename_cols))
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": self.script,
+            },
+        )
+
+        script_handler.script += self.script.copy()
+        self.script = []
+
+        return {"Out": df}
+
+    def select_types_and_fields(self, flow_id: str, node_key: str, df: pd.DataFrame, dtypes: dict):
+        """Retorna el df con las columnas seleccionadas y el orden dado
+
+        Args:
+            flow_id (str): id del flujo
+            node_key (str): id del nodo
+            df (pd.DataFrame): dataframe de entrada
+            dtypes (dict): configuracion de las columnas (selected, order)
+
+        Returns:
+            tuple: df, dtypes, rename_cols
+        """
+        
+        # https://pbpython.com/pandas_dtypes.html
+        # Obtener solo las columnas seleccionadas de la lista inicial (selected==True)
+        selected = dict(
+            filter(
+                lambda x: True if "selected" in x[1] and x[1]["selected"] else False,
+                dtypes.items(),
+            )
+        )
+
+        # Existe la posibilidad de que ya no existan columnas que previamente fueron creadas
+        available_cols = []
+        removed_cols = []
+        for field, _ in selected.items():
+            if field in df.columns:
+                available_cols.append(field)
+            else:
+                removed_cols.append(field)
+                del dtypes[field]  # dado que no existe la eliminamos de dtypes
+                msg = app_message.dataprep["nodes"]["column"]["column_not_in_df"](node_key, field)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
+
+        # Remover las columnas que ya no existen
+        for del_key in removed_cols:
+            del selected[del_key]
+
+        # Mantener solamente columnas existentes y seleccionadas
+        df = df[available_cols]
+        
+        self.script.append("df = df[{}]".format(available_cols))
+        self.script.append("\n# DATA TYPES")
+
+        # Diccionario para el renombrado de columnas
+        rename_cols = {}
+        for field, _ in selected.items():
+            if "rename" in dtypes[field] and dtypes[field]["rename"]:
+                rename_cols[field] = dtypes[field]["rename"]
+
+        # Ordena las columnas segun el orden dado en la configuracion del nodo
+        order_cols = list(dict(sorted(selected.items(), key=lambda item: item[1]["order"])).keys())
+
+        return df[order_cols], dtypes, rename_cols
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/concat.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/concat.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Concat:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        
-        # Validar que exista df de entrada en el puerto A
-        if "A" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "A")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-        # Validar que exista df de entrada en el puerto B
-        if "B" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "B")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        script.append("\n# CONCAT")
-        df_A: pd.DataFrame = pin["A"].copy() if "A" in pin else pd.DataFrame()
-        df_B: pd.DataFrame = pin["B"].copy() if "B" in pin else pd.DataFrame()
-
-        # Advertir si el dataframe está vacío
-        if df_A.empty:
-            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "A")
-            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
-
-        # Advertir si el dataframe está vacío
-        if df_B.empty:
-            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "B")
-            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
-
-        # Validar que exista columnas seleccionadas en la config de ambos Dataframes
-        selected_A: list = settings["a"] if "a" in settings and settings["a"] else None
-        selected_B: list = settings["b"] if "b" in settings and settings["b"] else None
-        
-        if not selected_A:
-            msg = app_message.dataprep["nodes"]["concat"]["column_required"](node_key, "A")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not selected_B:
-            msg = app_message.dataprep["nodes"]["concat"]["column_required"](node_key, "B")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        df_A = df_A[selected_A]
-        script.append("df_A = df_A[{}]".format(selected_A))
-        
-        df_B = df_B[selected_B]
-        script.append("df_B = df_B[{}]".format(selected_B))
-
-        try:
-            df = pd.concat([df_A, df_B], ignore_index=True)
-            script.append("df = pd.concat([df_A, df_B], ignore_index=True)")
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Concat:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        
+        # Validar que exista df de entrada en el puerto A
+        if "A" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "A")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+        # Validar que exista df de entrada en el puerto B
+        if "B" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "B")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        script.append("\n# CONCAT")
+        df_A: pd.DataFrame = pin["A"].copy() if "A" in pin else pd.DataFrame()
+        df_B: pd.DataFrame = pin["B"].copy() if "B" in pin else pd.DataFrame()
+
+        # Advertir si el dataframe está vacío
+        if df_A.empty:
+            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "A")
+            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
+
+        # Advertir si el dataframe está vacío
+        if df_B.empty:
+            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "B")
+            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
+
+        # Validar que exista columnas seleccionadas en la config de ambos Dataframes
+        selected_A: list = settings["a"] if "a" in settings and settings["a"] else None
+        selected_B: list = settings["b"] if "b" in settings and settings["b"] else None
+        
+        if not selected_A:
+            msg = app_message.dataprep["nodes"]["concat"]["column_required"](node_key, "A")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not selected_B:
+            msg = app_message.dataprep["nodes"]["concat"]["column_required"](node_key, "B")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        df_A = df_A[selected_A]
+        script.append("df_A = df_A[{}]".format(selected_A))
+        
+        df_B = df_B[selected_B]
+        script.append("df_B = df_B[{}]".format(selected_B))
+
+        try:
+            df = pd.concat([df_A, df_B], ignore_index=True)
+            script.append("df = pd.concat([df_A, df_B], ignore_index=True)")
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/cross_join.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/cross_join.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class CrossJoin:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        
-        # Validar que exista df de entrada en el puerto Tgt
-        if "Tgt" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Tgt")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-        # Validar que exista df de entrada en el puerto Src
-        if "Src" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Src")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        script.append("\n# CROSS_JOIN")
-        df_T: pd.DataFrame = pin["Tgt"].copy() if "Tgt" in pin else pd.DataFrame()
-        df_S: pd.DataFrame = pin["Src"].copy() if "Src" in pin else pd.DataFrame()
-        
-        # Advertir si el dataframe está vacío
-        if df_T.empty:
-            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "Tgt")
-            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
-
-        # Advertir si el dataframe está vacío
-        if df_S.empty:
-            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "Src")
-            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
-
-        # Validar que exista columnas seleccionadas en la config de ambos Dataframes
-        selected_T: list = settings["tgt"] if "tgt" in settings and settings["tgt"] else None
-        selected_S: list = settings["src"] if "src" in settings and settings["src"] else None
-        
-        if not selected_T:
-            msg = app_message.dataprep["nodes"]["cross_join"]["column_required"](node_key, "Target")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if not selected_S:
-            msg = app_message.dataprep["nodes"]["cross_join"]["column_required"](node_key, "Source")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        df_T = df_T[selected_T]
-        script.append("df_T = df_T[{}]".format(selected_T))
-        
-        df_S = df_S[selected_S]
-        script.append("df_S = df_S[{}]".format(selected_S))
-
-        try:
-            df = pd.merge(df_T, df_S, how="cross")  # , validate="many_to_one")
-            script.append("df = pd.merge(df_T, df_S, how='cross')")
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class CrossJoin:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        
+        # Validar que exista df de entrada en el puerto Tgt
+        if "Tgt" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Tgt")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+        # Validar que exista df de entrada en el puerto Src
+        if "Src" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Src")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        script.append("\n# CROSS_JOIN")
+        df_T: pd.DataFrame = pin["Tgt"].copy() if "Tgt" in pin else pd.DataFrame()
+        df_S: pd.DataFrame = pin["Src"].copy() if "Src" in pin else pd.DataFrame()
+        
+        # Advertir si el dataframe está vacío
+        if df_T.empty:
+            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "Tgt")
+            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
+
+        # Advertir si el dataframe está vacío
+        if df_S.empty:
+            msg = app_message.dataprep["nodes"]["empty_df"](node_key, "Src")
+            bug_handler.default_node_log(flow_id, node_key, msg, bug_level="warning", console_level="WARN")
+
+        # Validar que exista columnas seleccionadas en la config de ambos Dataframes
+        selected_T: list = settings["tgt"] if "tgt" in settings and settings["tgt"] else None
+        selected_S: list = settings["src"] if "src" in settings and settings["src"] else None
+        
+        if not selected_T:
+            msg = app_message.dataprep["nodes"]["cross_join"]["column_required"](node_key, "Target")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if not selected_S:
+            msg = app_message.dataprep["nodes"]["cross_join"]["column_required"](node_key, "Source")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        df_T = df_T[selected_T]
+        script.append("df_T = df_T[{}]".format(selected_T))
+        
+        df_S = df_S[selected_S]
+        script.append("df_S = df_S[{}]".format(selected_S))
+
+        try:
+            df = pd.merge(df_T, df_S, how="cross")  # , validate="many_to_one")
+            script.append("df = pd.merge(df_T, df_S, how='cross')")
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/cumsum.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/cumsum.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Cumsum:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# CUMSUM")
-
-        groupby: list = settings["groupby"] if "groupby" in settings and settings["groupby"] else []
-        cumcount: bool = settings["cumcount"] if "cumcount" in settings else False
-        cumsum: bool = settings["cumsum"] if "cumsum" in settings else False
-        cumpct: bool = settings["cumpct"] if "cumpct" in settings else False
-        axis: str = settings["axis"] if "axis" in settings and settings["axis"] else None
-        pct: bool = settings["pct"] if "pct" in settings else False
-
-        if not axis:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        prefix = axis[:3]
-        script.append(f"prefix = '{prefix}'")
-
-        if not (cumcount or cumsum or cumpct or pct):
-            msg = app_message.dataprep["nodes"]["cumsum"]["aggregation_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
-
-        try:
-            if groupby:
-                df_obj = df.groupby(groupby)
-                script.append(f"df_obj = df.groupby({groupby})['{axis}']")
-                if cumcount:
-                    df[prefix + "_cumcount"] = df_obj.cumcount() + 1
-                    script.append(f"df[prefix+'_cumcount'] = df_obj.cumcount()+1")
-                if cumsum:
-                    df[prefix + "_cumsum"] = df_obj[axis].apply(lambda x: x.cumsum())
-                    script.append(f"df[prefix+'_cumsum'] = df_obj.apply(lambda x: x.cumsum())")
-                if pct:
-                    df[prefix + "_pct"] = df_obj[axis].apply(lambda x: x / x.sum())
-                    script.append(f"df[prefix+'_pct'] = df_obj.apply(lambda x: x/x.sum())")
-                if cumpct:
-                    df[prefix + "_cumpct"] = df_obj[axis].apply(lambda x: (x / x.sum()).cumsum())
-                    script.append(f"df[prefix+'_cumpct'] = df_obj.apply(lambda x: (x/x.sum()).cumsum())")
-            else:
-                if cumcount:
-                    df[prefix + "_cumcount"] = range(1, 1 + len(df))
-                    script.append(f"df[prefix+'_cumcount'] = range(1, 1 + len(df))")
-                if cumsum:
-                    df[prefix + "_cumsum"] = df[axis].cumsum()
-                    script.append(f"df[prefix+'_cumsum'] = df['{axis}'].cumsum()")
-                if pct:
-                    df[prefix + "_pct"] = df[axis] / df[axis].sum()
-                    script.append(f"df[prefix+'_pct'] = df['{axis}']/df[axis].sum()")
-                if cumpct:
-                    df[prefix + "_cumpct"] = df[axis].cumsum() / df[axis].sum()
-                    script.append(f"df[prefix+'_cumpct'] = df['{axis}'].cumsum()/df['{axis}'].sum()")
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Cumsum:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# CUMSUM")
+
+        groupby: list = settings["groupby"] if "groupby" in settings and settings["groupby"] else []
+        cumcount: bool = settings["cumcount"] if "cumcount" in settings else False
+        cumsum: bool = settings["cumsum"] if "cumsum" in settings else False
+        cumpct: bool = settings["cumpct"] if "cumpct" in settings else False
+        axis: str = settings["axis"] if "axis" in settings and settings["axis"] else None
+        pct: bool = settings["pct"] if "pct" in settings else False
+
+        if not axis:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        prefix = axis[:3]
+        script.append(f"prefix = '{prefix}'")
+
+        if not (cumcount or cumsum or cumpct or pct):
+            msg = app_message.dataprep["nodes"]["cumsum"]["aggregation_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
+
+        try:
+            if groupby:
+                df_obj = df.groupby(groupby)
+                script.append(f"df_obj = df.groupby({groupby})['{axis}']")
+                if cumcount:
+                    df[prefix + "_cumcount"] = df_obj.cumcount() + 1
+                    script.append(f"df[prefix+'_cumcount'] = df_obj.cumcount()+1")
+                if cumsum:
+                    df[prefix + "_cumsum"] = df_obj[axis].apply(lambda x: x.cumsum())
+                    script.append(f"df[prefix+'_cumsum'] = df_obj.apply(lambda x: x.cumsum())")
+                if pct:
+                    df[prefix + "_pct"] = df_obj[axis].apply(lambda x: x / x.sum())
+                    script.append(f"df[prefix+'_pct'] = df_obj.apply(lambda x: x/x.sum())")
+                if cumpct:
+                    df[prefix + "_cumpct"] = df_obj[axis].apply(lambda x: (x / x.sum()).cumsum())
+                    script.append(f"df[prefix+'_cumpct'] = df_obj.apply(lambda x: (x/x.sum()).cumsum())")
+            else:
+                if cumcount:
+                    df[prefix + "_cumcount"] = range(1, 1 + len(df))
+                    script.append(f"df[prefix+'_cumcount'] = range(1, 1 + len(df))")
+                if cumsum:
+                    df[prefix + "_cumsum"] = df[axis].cumsum()
+                    script.append(f"df[prefix+'_cumsum'] = df['{axis}'].cumsum()")
+                if pct:
+                    df[prefix + "_pct"] = df[axis] / df[axis].sum()
+                    script.append(f"df[prefix+'_pct'] = df['{axis}']/df[axis].sum()")
+                if cumpct:
+                    df[prefix + "_cumpct"] = df[axis].cumsum() / df[axis].sum()
+                    script.append(f"df[prefix+'_cumpct'] = df['{axis}'].cumsum()/df['{axis}'].sum()")
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/cut.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/cut.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Cut:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        df_A: pd.DataFrame = pd.DataFrame()
-        df_B: pd.DataFrame = pd.DataFrame()
-
-        script.append("\n# CUT")
-
-        field: str = settings["field"] if "field" in settings else None
-        first_n: float = settings["first_n"] if "first_n" in settings else None
-        last_n: float = settings["last_n"] if "last_n" in settings else None
-        n_to_last: float = settings["n_to_last"] if "n_to_last" in settings else None
-
-        if not field:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if not first_n and not last_n and not n_to_last:
-            msg = app_message.dataprep["nodes"]["cut"]["no_cutting_parameter"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            if first_n:
-                df["first_n"] = df[field].str[:first_n]
-            elif last_n:
-                df["last_n"] = df[field].str[-last_n:]
-            elif n_to_last:
-                df["n_to_last"] = df[field].str[n_to_last:]
-            else:
-                msg = app_message.dataprep["nodes"]["cut"]["no_type_cut"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Cut:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        df_A: pd.DataFrame = pd.DataFrame()
+        df_B: pd.DataFrame = pd.DataFrame()
+
+        script.append("\n# CUT")
+
+        field: str = settings["field"] if "field" in settings else None
+        first_n: float = settings["first_n"] if "first_n" in settings else None
+        last_n: float = settings["last_n"] if "last_n" in settings else None
+        n_to_last: float = settings["n_to_last"] if "n_to_last" in settings else None
+
+        if not field:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if not first_n and not last_n and not n_to_last:
+            msg = app_message.dataprep["nodes"]["cut"]["no_cutting_parameter"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            if first_n:
+                df["first_n"] = df[field].str[:first_n]
+            elif last_n:
+                df["last_n"] = df[field].str[-last_n:]
+            elif n_to_last:
+                df["n_to_last"] = df[field].str[n_to_last:]
+            else:
+                msg = app_message.dataprep["nodes"]["cut"]["no_type_cut"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/data_cleansing.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/data_cleansing.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DataCleansing:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# Data Cleansing")
-
-        selected_columns: list = settings["columns"] if "columns" in settings and settings["columns"] else []
-        replace_blanks: bool = settings["replace_blanks"] if "replace_blanks" in settings else False
-        replace_zeros: bool = settings["replace_zeros"] if "replace_zeros" in settings else False
-        remove_leading_trailing: bool = settings["remove_leading_trailing"] if "remove_leading_trailing" in settings else False
-        remove_tabs_line_breaks: bool = settings["remove_tabs_line_breaks"] if "remove_tabs_line_breaks" in settings else False
-        remove_all_whitespaces: bool = settings["remove_all_whitespaces"] if "remove_all_whitespaces" in settings else False
-        remove_punctuation: bool = settings["remove_punctuation"] if "remove_punctuation" in settings else False
-        remove_letters: bool = settings["remove_letters"] if "remove_letters" in settings else False
-        remove_numbers: bool = settings["remove_numbers"] if "remove_numbers" in settings else False
-        remove_nulls: bool = settings["remove_nulls"] if "remove_nulls" in settings else False
-        modify_case_type: str = settings["modify_case_type"] if "modify_case_type" in settings and settings["modify_case_type"] else None
-
-        try:
-            columns = selected_columns if selected_columns else df.columns
-            for column in columns:
-                if replace_blanks and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].fillna("")
-                    script.append(f'# replace_blanks')
-                    script.append(f'df["{column}"] = df["{column}"].fillna("")')
-                    
-                if replace_zeros and pd.api.types.is_numeric_dtype(df[column]):
-                    df[column] = df[column].fillna(0)
-                    script.append(f'# replace_zeros')
-                    script.append(f'df["{column}"] = df["{column}"].fillna(0)')
-                    
-                if remove_leading_trailing and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.strip()
-                    script.append(f'# remove_leading_trailing')
-                    script.append(f'df["{column}"].str.strip()')
-                    
-                if remove_tabs_line_breaks and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.replace(r"[ \r\t\n]+", " ")
-                    script.append(f'# remove_tabs_line_breaks')
-                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[ \\r\\t\\n]+", " ")')
-                    
-                if remove_all_whitespaces and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.replace(" ", "")
-                    script.append(f'# remove_all_whitespaces')
-                    script.append(f'df["{column}"] = df["{column}"].str.replace(" ", "")')
-                    
-                if remove_letters and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.replace(r"[a-zA-Z]", "")
-                    script.append(f'# remove_letters')
-                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[a-zA-Z]", "")')
-                    
-                if remove_numbers and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.replace(r"\d", "")
-                    script.append(f'# remove_numbers')
-                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"\d", "")')
-                    
-                if remove_punctuation and pd.api.types.is_string_dtype(df[column]):
-                    df[column] = df[column].str.replace(r"[^\w\s]", "")
-                    script.append(f'# remove_punctuation')
-                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[^\w\s]", "")')
-                    
-                if remove_nulls:
-                    df = df.dropna(subset=[column])
-                    script.append(f'# remove_nulls')
-                    script.append(f'df = df.dropna(subset=["{column}"])')
-                    
-                if modify_case_type and pd.api.types.is_string_dtype(df[column]):
-                    script.append(f'# modify_case_type {modify_case_type}')
-                    if modify_case_type == "upper_case":
-                        df[column] = df[column].str.upper()
-                        script.append(f'df["{column}"] = df["{column}"].str.upper()')
-                    if modify_case_type == "lower_case":
-                        df[column] = df[column].str.lower()
-                        script.append(f'df["{column}"] = df["{column}"].str.lower()')
-                    if modify_case_type == "title_case":
-                        df[column] = df[column].str.title()
-                        script.append(f'df["{column}"] = df["{column}"].str.title()')
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DataCleansing:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# Data Cleansing")
+
+        selected_columns: list = settings["columns"] if "columns" in settings and settings["columns"] else []
+        replace_blanks: bool = settings["replace_blanks"] if "replace_blanks" in settings else False
+        replace_zeros: bool = settings["replace_zeros"] if "replace_zeros" in settings else False
+        remove_leading_trailing: bool = settings["remove_leading_trailing"] if "remove_leading_trailing" in settings else False
+        remove_tabs_line_breaks: bool = settings["remove_tabs_line_breaks"] if "remove_tabs_line_breaks" in settings else False
+        remove_all_whitespaces: bool = settings["remove_all_whitespaces"] if "remove_all_whitespaces" in settings else False
+        remove_punctuation: bool = settings["remove_punctuation"] if "remove_punctuation" in settings else False
+        remove_letters: bool = settings["remove_letters"] if "remove_letters" in settings else False
+        remove_numbers: bool = settings["remove_numbers"] if "remove_numbers" in settings else False
+        remove_nulls: bool = settings["remove_nulls"] if "remove_nulls" in settings else False
+        modify_case_type: str = settings["modify_case_type"] if "modify_case_type" in settings and settings["modify_case_type"] else None
+
+        try:
+            columns = selected_columns if selected_columns else df.columns
+            for column in columns:
+                if replace_blanks and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].fillna("")
+                    script.append(f'# replace_blanks')
+                    script.append(f'df["{column}"] = df["{column}"].fillna("")')
+                    
+                if replace_zeros and pd.api.types.is_numeric_dtype(df[column]):
+                    df[column] = df[column].fillna(0)
+                    script.append(f'# replace_zeros')
+                    script.append(f'df["{column}"] = df["{column}"].fillna(0)')
+                    
+                if remove_leading_trailing and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.strip()
+                    script.append(f'# remove_leading_trailing')
+                    script.append(f'df["{column}"].str.strip()')
+                    
+                if remove_tabs_line_breaks and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.replace(r"[ \r\t\n]+", " ")
+                    script.append(f'# remove_tabs_line_breaks')
+                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[ \\r\\t\\n]+", " ")')
+                    
+                if remove_all_whitespaces and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.replace(" ", "")
+                    script.append(f'# remove_all_whitespaces')
+                    script.append(f'df["{column}"] = df["{column}"].str.replace(" ", "")')
+                    
+                if remove_letters and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.replace(r"[a-zA-Z]", "")
+                    script.append(f'# remove_letters')
+                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[a-zA-Z]", "")')
+                    
+                if remove_numbers and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.replace(r"\d", "")
+                    script.append(f'# remove_numbers')
+                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"\d", "")')
+                    
+                if remove_punctuation and pd.api.types.is_string_dtype(df[column]):
+                    df[column] = df[column].str.replace(r"[^\w\s]", "")
+                    script.append(f'# remove_punctuation')
+                    script.append(f'df["{column}"] = df["{column}"].str.replace(r"[^\w\s]", "")')
+                    
+                if remove_nulls:
+                    df = df.dropna(subset=[column])
+                    script.append(f'# remove_nulls')
+                    script.append(f'df = df.dropna(subset=["{column}"])')
+                    
+                if modify_case_type and pd.api.types.is_string_dtype(df[column]):
+                    script.append(f'# modify_case_type {modify_case_type}')
+                    if modify_case_type == "upper_case":
+                        df[column] = df[column].str.upper()
+                        script.append(f'df["{column}"] = df["{column}"].str.upper()')
+                    if modify_case_type == "lower_case":
+                        df[column] = df[column].str.lower()
+                        script.append(f'df["{column}"] = df["{column}"].str.lower()')
+                    if modify_case_type == "title_case":
+                        df[column] = df[column].str.title()
+                        script.append(f'df["{column}"] = df["{column}"].str.title()')
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/database.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/database.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import json
-import time
-
-import numpy as np
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.database_connection.utilities import database_utilities
-
-import snowflake.connector
-from google.cloud import bigquery
-from google.oauth2 import service_account
-from pymongo import MongoClient
-from sqlalchemy import create_engine, text
-
-class Database:
-    def exec(self, flow_id, node_key, pin, settings):
-
-        script = []
-        script.append("\n# DATABASE")
-
-        try:
-            # * Valida que existan todos los campos requeridos y que no estén vacíos dependiendo del tipo de conexion
-            checked, msg = database_utilities.check_fields(settings, tier="data")
-            if not checked:
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            prefix: str = ""
-            deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-
-            if deploy_enabled:
-                prefix = "deploy_"
-
-            source = settings[f"{prefix}source"]
-
-            if source == "postgresql" or source == "mysql" or source == "sqlite" or source == "mariadb" or source == "oracle":
-                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
-                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
-
-                connection = database_utilities.get_url_connection(flow_id, settings, with_database=True)
-                engine = create_engine(connection)
-                df = pd.read_sql(text(query if query else f'SELECT * FROM "{table}"'), con=engine.connect())
-                engine.dispose()
-
-            elif source == "sqlserver_2000":
-                import pyodbc
-                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
-                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
-
-                connection = database_utilities.get_url_connection(flow_id, settings, True)
-                try:
-                    engine = pyodbc.connect(connection)
-                except Exception as e:
-                    # TODO: Agregar a la lista de opciones de la vista
-                    settings[f"{prefix}source"] = "sqlserver_2000_v2"
-                    connection = database_utilities.get_url_connection(flow_id, settings, True)
-                    engine = pyodbc.connect(connection)
-                cursor = engine.cursor()
-                cursor.execute(query if query else f"SELECT * FROM [{table}]")
-                results = np.array(cursor.fetchall())
-                column_names = [str(column[0]) for column in cursor.description]
-                df = pd.DataFrame(results, columns=column_names)
-                cursor.close()
-                engine.close()
-
-            elif source == "bigquery":
-                service_account_host = settings[f"{prefix}service_account_host"]
-                database = settings[f"{prefix}database"]
-                project = settings[f"{prefix}project"]
-                table = settings[f"{prefix}table"]
-
-                with open(service_account_host) as file:
-                    service_account_host = json.load(file)
-                    credentials = service_account.Credentials.from_service_account_info(service_account_host)
-                    client = bigquery.Client(credentials=credentials)
-                    table_ref = client.dataset(database, project=project).table(table)
-                    table_type = client.get_table(table_ref).table_type
-                    client.close()
-
-                    if table_type == 'TABLE':
-                        rows = client.list_rows(table_ref)
-                        df = rows.to_dataframe()
-                    elif table_type == 'VIEW':
-                        query = f"SELECT * FROM `{project}.{database}.{table}`"
-                        query_job = client.query(query)
-                        df = query_job.to_dataframe()
-
-                        # batch_size = 2000000
-                        # total_results = 0
-                        # df_batches = []
-                        # while True:
-                        #     credentials = service_account.Credentials.from_service_account_info(service_account_host)
-                        #     client = bigquery.Client(credentials=credentials)
-                        #     query = f"""SELECT 
-                        #         sucursal, 
-                        #         rut, 
-                        #         cliente, 
-                        #         direccion, 
-                        #         comuna, 
-                        #         ciudad, 
-                        #         vendedor, 
-                        #         cod_vendedor, 
-                        #         dia_visita, 
-                        #         frecuencia_visita, 
-                        #         fecha_programada, 
-                        #         supervisor,
-                        #         region,
-                        #         tipo,
-                        #         nro_pedido,
-                        #         fecha_pedido,
-                        #         codigo_vendedor_realizado,
-                        #         codigo_vendedor_asignado_hoy
-                        #     FROM 
-                        #         espol-data.vistas.cartera_clientes_atendidos 
-                        #     WHERE
-                        #         region IS NOT NULL AND
-                        #         tipo IS NOT NULL AND
-                        #         nro_pedido IS NOT NULL AND
-                        #         fecha_pedido IS NOT NULL AND
-                        #         codigo_vendedor_realizado IS NOT NULL
-                        #     LIMIT {batch_size}
-                        #     OFFSET {total_results}
-                        #     """
-                        #     query_job = client.query(query)
-                        #     results = query_job.result(max_results=batch_size)
-
-                        #     df_batch = results.to_dataframe()
-                        #     df_batches.append(df_batch)
-
-                        #     total_results += batch_size
-                        #     if len(df_batch) < batch_size:
-                        #         break
-
-                        #     client.close()
-
-                        # df = pd.concat(df_batches, ignore_index=True)
-
-            elif source == "snowflake":
-                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
-                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
-
-                user = settings[f"{prefix}user"]
-                database = settings[f"{prefix}database"]
-                project = settings[f"{prefix}project"]
-                account = settings[f"{prefix}account"]
-                password = settings[f"{prefix}password"]
-
-                connection = snowflake.connector.connect(user=user, password=password, account=account, database=project, schema=database)
-                cursor = connection.cursor()
-                cursor.execute(query if query else f'SELECT * FROM "{table}"')
-                results = cursor.fetchall()
-                column_names = [desc[0] for desc in cursor.description]
-                df = pd.DataFrame(results, columns=column_names)
-                connection.close()
-                cursor.close()
-
-            elif source == "mongodb":
-                mongo_client = settings[f"{prefix}mongo_client"]
-                database = settings[f"{prefix}database"]
-                table = settings[f"{prefix}table"]
-
-                client = MongoClient(mongo_client)
-                db = client[database]
-                collection = db[table]
-                data = list(collection.find())
-                df = pd.DataFrame(data)
-                client.close()
-
-            else:
-                msg = app_message.dataprep["nodes"]["database"]["source_required"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+import time
+
+import numpy as np
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.database_connection.utilities import database_utilities
+
+import snowflake.connector
+from google.cloud import bigquery
+from google.oauth2 import service_account
+from pymongo import MongoClient
+from sqlalchemy import create_engine, text
+
+class Database:
+    def exec(self, flow_id, node_key, pin, settings):
+
+        script = []
+        script.append("\n# DATABASE")
+
+        try:
+            # * Valida que existan todos los campos requeridos y que no estén vacíos dependiendo del tipo de conexion
+            checked, msg = database_utilities.check_fields(settings, tier="data")
+            if not checked:
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+            prefix: str = ""
+            deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+
+            if deploy_enabled:
+                prefix = "deploy_"
+
+            source = settings[f"{prefix}source"]
+
+            if source == "postgresql" or source == "mysql" or source == "sqlite" or source == "mariadb" or source == "oracle":
+                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
+                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
+
+                connection = database_utilities.get_url_connection(flow_id, settings, with_database=True)
+                engine = create_engine(connection)
+                df = pd.read_sql(text(query if query else f'SELECT * FROM "{table}"'), con=engine.connect())
+                engine.dispose()
+
+            elif source == "sqlserver_2000":
+                import pyodbc
+                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
+                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
+
+                connection = database_utilities.get_url_connection(flow_id, settings, True)
+                try:
+                    engine = pyodbc.connect(connection)
+                except Exception as e:
+                    # TODO: Agregar a la lista de opciones de la vista
+                    settings[f"{prefix}source"] = "sqlserver_2000_v2"
+                    connection = database_utilities.get_url_connection(flow_id, settings, True)
+                    engine = pyodbc.connect(connection)
+                cursor = engine.cursor()
+                cursor.execute(query if query else f"SELECT * FROM [{table}]")
+                results = np.array(cursor.fetchall())
+                column_names = [str(column[0]) for column in cursor.description]
+                df = pd.DataFrame(results, columns=column_names)
+                cursor.close()
+                engine.close()
+
+            elif source == "bigquery":
+                service_account_host = settings[f"{prefix}service_account_host"]
+                database = settings[f"{prefix}database"]
+                project = settings[f"{prefix}project"]
+                table = settings[f"{prefix}table"]
+
+                with open(service_account_host) as file:
+                    service_account_host = json.load(file)
+                    credentials = service_account.Credentials.from_service_account_info(service_account_host)
+                    client = bigquery.Client(credentials=credentials)
+                    table_ref = client.dataset(database, project=project).table(table)
+                    table_type = client.get_table(table_ref).table_type
+                    client.close()
+
+                    if table_type == 'TABLE':
+                        rows = client.list_rows(table_ref)
+                        df = rows.to_dataframe()
+                    elif table_type == 'VIEW':
+                        query = f"SELECT * FROM `{project}.{database}.{table}`"
+                        query_job = client.query(query)
+                        df = query_job.to_dataframe()
+
+                        # batch_size = 2000000
+                        # total_results = 0
+                        # df_batches = []
+                        # while True:
+                        #     credentials = service_account.Credentials.from_service_account_info(service_account_host)
+                        #     client = bigquery.Client(credentials=credentials)
+                        #     query = f"""SELECT 
+                        #         sucursal, 
+                        #         rut, 
+                        #         cliente, 
+                        #         direccion, 
+                        #         comuna, 
+                        #         ciudad, 
+                        #         vendedor, 
+                        #         cod_vendedor, 
+                        #         dia_visita, 
+                        #         frecuencia_visita, 
+                        #         fecha_programada, 
+                        #         supervisor,
+                        #         region,
+                        #         tipo,
+                        #         nro_pedido,
+                        #         fecha_pedido,
+                        #         codigo_vendedor_realizado,
+                        #         codigo_vendedor_asignado_hoy
+                        #     FROM 
+                        #         espol-data.vistas.cartera_clientes_atendidos 
+                        #     WHERE
+                        #         region IS NOT NULL AND
+                        #         tipo IS NOT NULL AND
+                        #         nro_pedido IS NOT NULL AND
+                        #         fecha_pedido IS NOT NULL AND
+                        #         codigo_vendedor_realizado IS NOT NULL
+                        #     LIMIT {batch_size}
+                        #     OFFSET {total_results}
+                        #     """
+                        #     query_job = client.query(query)
+                        #     results = query_job.result(max_results=batch_size)
+
+                        #     df_batch = results.to_dataframe()
+                        #     df_batches.append(df_batch)
+
+                        #     total_results += batch_size
+                        #     if len(df_batch) < batch_size:
+                        #         break
+
+                        #     client.close()
+
+                        # df = pd.concat(df_batches, ignore_index=True)
+
+            elif source == "snowflake":
+                table: str = settings[f"{prefix}table"] if (f"{prefix}table" in settings and settings[f"{prefix}table"] is not None) else None
+                query: str = settings[f"{prefix}query"] if (f"{prefix}query" in settings and settings[f"{prefix}query"] is not None) else None
+
+                user = settings[f"{prefix}user"]
+                database = settings[f"{prefix}database"]
+                project = settings[f"{prefix}project"]
+                account = settings[f"{prefix}account"]
+                password = settings[f"{prefix}password"]
+
+                connection = snowflake.connector.connect(user=user, password=password, account=account, database=project, schema=database)
+                cursor = connection.cursor()
+                cursor.execute(query if query else f'SELECT * FROM "{table}"')
+                results = cursor.fetchall()
+                column_names = [desc[0] for desc in cursor.description]
+                df = pd.DataFrame(results, columns=column_names)
+                connection.close()
+                cursor.close()
+
+            elif source == "mongodb":
+                mongo_client = settings[f"{prefix}mongo_client"]
+                database = settings[f"{prefix}database"]
+                table = settings[f"{prefix}table"]
+
+                client = MongoClient(mongo_client)
+                db = client[database]
+                collection = db[table]
+                data = list(collection.find())
+                df = pd.DataFrame(data)
+                client.close()
+
+            else:
+                msg = app_message.dataprep["nodes"]["database"]["source_required"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/database_write.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/database_write.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import json
-
-import numpy as np
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.database_connection.utilities import database_utilities
-
-import re
-
-import snowflake.connector
-from google.oauth2 import service_account
-from pymongo import MongoClient
-from snowflake.connector.pandas_tools import write_pandas
-from sqlalchemy import create_engine
-from sqlalchemy.exc import ProgrammingError
-
-class DatabaseWrite:
-    def exec(self, flow_id, node_key, pin, settings):
-
-        df: pd.DataFrame = pin["In"].copy()
-        script = []
-        script.append("\n# DATABASE WRITE")
-
-        try:
-            # * Valida que existan todos los campos requeridos y que no estén vacíos dependiendo del tipo de conexion
-            checked, msg = database_utilities.check_fields(settings, tier="write_data", node_key=node_key)
-            if not checked:
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            prefix: str = ""
-            deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-
-            if deploy_enabled:
-                prefix = "deploy_"
-
-            source = settings[f"{prefix}source"]
-
-            if source == "postgresql" or source == "mysql" or source == "sqlite" or source == "mariadb" or source == "oracle":
-                table = settings[f"{prefix}table"]
-                save_type = settings[f"{prefix}save_type"]
-
-                connection = database_utilities.get_url_connection(flow_id, settings, with_database=True)
-                engine = create_engine(connection)
-                df.to_sql(name=table, con=engine, if_exists=save_type, index=False)
-                engine.dispose()
-
-            elif source == "sqlserver_2000":
-                import pyodbc
-                table = settings[f"{prefix}table"]
-                save_type = settings[f"{prefix}save_type"]
-
-                connection = database_utilities.get_url_connection(flow_id, settings, True)
-                try:
-                    engine = pyodbc.connect(connection)
-                except Exception as e:
-                    #TODO: Agregar a la lista de opciones de la vista
-                    settings[f"{prefix}source"] = "sqlserver_2000_v2"
-                    connection = database_utilities.get_url_connection(flow_id, settings, True)
-                    engine = pyodbc.connect(connection)
-                cursor = engine.cursor()
-                # Preparación de datos
-                columns_name = ", ".join(df.columns)
-                values = ", ".join(["?" for _ in df.columns])
-                params = iter(np.asarray(df).tolist())
-                # Limpia o no la tabla seleccionada de la base de datos
-
-                if save_type == "replace":
-                    cursor.execute(f"TRUNCATE TABLE {table}")
-                # Inserción
-                cursor.executemany(f"INSERT INTO {table} ({columns_name}) VALUES ({values})", params)
-                cursor.commit()
-                cursor.close()
-                engine.close()
-
-            elif source == "bigquery":
-                service_account_host = settings[f"{prefix}service_account_host"]
-                database = settings[f"{prefix}database"]
-                project = settings[f"{prefix}project"]
-                table = settings[f"{prefix}table"]
-                save_type = settings[f"{prefix}save_type"]
-
-                with open(service_account_host) as file:
-                    service_account_host = json.load(file)
-                    credentials = service_account.Credentials.from_service_account_info(service_account_host)
-                    df.to_gbq(
-                        f"{database}.{table}",
-                        project_id=project,
-                        if_exists=save_type,
-                        credentials=credentials,
-                    )
-
-            elif source == "snowflake":
-                table = settings[f"{prefix}table"]
-                user = settings[f"{prefix}user"]
-                database = settings[f"{prefix}database"]
-                project = settings[f"{prefix}project"]
-                account = settings[f"{prefix}account"]
-                password = settings[f"{prefix}password"]
-                save_type = settings[f"{prefix}save_type"]
-
-                connection = snowflake.connector.connect(user=user, password=password, account=account, database=project, schema=database)
-                write_pandas(
-                    connection,
-                    df,
-                    table,
-                    project,
-                    database,
-                    overwrite=save_type == "replace",
-                    auto_create_table=False,
-                )
-                connection.close()
-
-            elif source == "mongodb":
-                mongo_client = settings[f"{prefix}mongo_client"]
-                database = settings[f"{prefix}database"]
-                table = settings[f"{prefix}table"]
-                save_type = settings[f"{prefix}save_type"]
-
-                client = MongoClient(mongo_client)
-                db = client[database]
-                collection = db[table]
-                if save_type == "replace":
-                    collection.drop()
-                collection.insert_many(df.to_dict("records"), ordered=True)
-                client.close()
-
-            else:
-                msg = app_message.dataprep["nodes"]["database_write"]["source_required"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        except ProgrammingError as e:
-            # Utiliza expresiones regulares para extraer el nombre de la columna y la tabla desde el mensaje de error
-            column_match = re.search(r'column "(.*?)" of relation', str(e.orig))
-            table_match = re.search(r'relation "(.*?)" does not exist', str(e.orig))
-
-            column_name = column_match.group(1) if column_match else None
-            table_name = table_match.group(1) if table_match else None
-            
-            if column_name and table_name:
-                msg = app_message.dataprep["nodes"]["database_write"]["no_column_in_table"](node_key, column_name, table_name)
-            else:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
+import json
+
+import numpy as np
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.database_connection.utilities import database_utilities
+
+import re
+
+import snowflake.connector
+from google.oauth2 import service_account
+from pymongo import MongoClient
+from snowflake.connector.pandas_tools import write_pandas
+from sqlalchemy import create_engine
+from sqlalchemy.exc import ProgrammingError
+
+class DatabaseWrite:
+    def exec(self, flow_id, node_key, pin, settings):
+
+        df: pd.DataFrame = pin["In"].copy()
+        script = []
+        script.append("\n# DATABASE WRITE")
+
+        try:
+            # * Valida que existan todos los campos requeridos y que no estén vacíos dependiendo del tipo de conexion
+            checked, msg = database_utilities.check_fields(settings, tier="write_data", node_key=node_key)
+            if not checked:
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+            prefix: str = ""
+            deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+
+            if deploy_enabled:
+                prefix = "deploy_"
+
+            source = settings[f"{prefix}source"]
+
+            if source == "postgresql" or source == "mysql" or source == "sqlite" or source == "mariadb" or source == "oracle":
+                table = settings[f"{prefix}table"]
+                save_type = settings[f"{prefix}save_type"]
+
+                connection = database_utilities.get_url_connection(flow_id, settings, with_database=True)
+                engine = create_engine(connection)
+                df.to_sql(name=table, con=engine, if_exists=save_type, index=False)
+                engine.dispose()
+
+            elif source == "sqlserver_2000":
+                import pyodbc
+                table = settings[f"{prefix}table"]
+                save_type = settings[f"{prefix}save_type"]
+
+                connection = database_utilities.get_url_connection(flow_id, settings, True)
+                try:
+                    engine = pyodbc.connect(connection)
+                except Exception as e:
+                    #TODO: Agregar a la lista de opciones de la vista
+                    settings[f"{prefix}source"] = "sqlserver_2000_v2"
+                    connection = database_utilities.get_url_connection(flow_id, settings, True)
+                    engine = pyodbc.connect(connection)
+                cursor = engine.cursor()
+                # Preparación de datos
+                columns_name = ", ".join(df.columns)
+                values = ", ".join(["?" for _ in df.columns])
+                params = iter(np.asarray(df).tolist())
+                # Limpia o no la tabla seleccionada de la base de datos
+
+                if save_type == "replace":
+                    cursor.execute(f"TRUNCATE TABLE {table}")
+                # Inserción
+                cursor.executemany(f"INSERT INTO {table} ({columns_name}) VALUES ({values})", params)
+                cursor.commit()
+                cursor.close()
+                engine.close()
+
+            elif source == "bigquery":
+                service_account_host = settings[f"{prefix}service_account_host"]
+                database = settings[f"{prefix}database"]
+                project = settings[f"{prefix}project"]
+                table = settings[f"{prefix}table"]
+                save_type = settings[f"{prefix}save_type"]
+
+                with open(service_account_host) as file:
+                    service_account_host = json.load(file)
+                    credentials = service_account.Credentials.from_service_account_info(service_account_host)
+                    df.to_gbq(
+                        f"{database}.{table}",
+                        project_id=project,
+                        if_exists=save_type,
+                        credentials=credentials,
+                    )
+
+            elif source == "snowflake":
+                table = settings[f"{prefix}table"]
+                user = settings[f"{prefix}user"]
+                database = settings[f"{prefix}database"]
+                project = settings[f"{prefix}project"]
+                account = settings[f"{prefix}account"]
+                password = settings[f"{prefix}password"]
+                save_type = settings[f"{prefix}save_type"]
+
+                connection = snowflake.connector.connect(user=user, password=password, account=account, database=project, schema=database)
+                write_pandas(
+                    connection,
+                    df,
+                    table,
+                    project,
+                    database,
+                    overwrite=save_type == "replace",
+                    auto_create_table=False,
+                )
+                connection.close()
+
+            elif source == "mongodb":
+                mongo_client = settings[f"{prefix}mongo_client"]
+                database = settings[f"{prefix}database"]
+                table = settings[f"{prefix}table"]
+                save_type = settings[f"{prefix}save_type"]
+
+                client = MongoClient(mongo_client)
+                db = client[database]
+                collection = db[table]
+                if save_type == "replace":
+                    collection.drop()
+                collection.insert_many(df.to_dict("records"), ordered=True)
+                client.close()
+
+            else:
+                msg = app_message.dataprep["nodes"]["database_write"]["source_required"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        except ProgrammingError as e:
+            # Utiliza expresiones regulares para extraer el nombre de la columna y la tabla desde el mensaje de error
+            column_match = re.search(r'column "(.*?)" of relation', str(e.orig))
+            table_match = re.search(r'relation "(.*?)" does not exist', str(e.orig))
+
+            column_name = column_match.group(1) if column_match else None
+            table_name = table_match.group(1) if table_match else None
+            
+            if column_name and table_name:
+                msg = app_message.dataprep["nodes"]["database_write"]["no_column_in_table"](node_key, column_name, table_name)
+            else:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
         return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_extract.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/datetime_extract.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DatetimeExtract:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# Datetime Extract")
-
-        items: list[str] = settings["items"] if ("items" in settings and settings["items"]) else None
-
-        if items:
-            for item in items:
-                # column_to_convert, new_column_name, to_extract
-                column_to_convert: str = item["column_to_convert"] if ("column_to_convert" in item and item["column_to_convert"]) else ""
-                to_extract: str = item["to_extract"] if ("to_extract" in item and item["to_extract"]) else ""
-                new_column_name: str = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else to_extract.replace("()", "")
-
-                if not to_extract or not column_to_convert:
-                    msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-                    return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-                try:
-                    df[new_column_name] = eval("df[column_to_convert].dt.{}".format(to_extract))
-                    script.append(f'df["{new_column_name}"] = df["{column_to_convert}"].dt.{to_extract}')
-
-                except Exception as e:
-                    msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                    return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-            cache_handler.update_node(
-                flow_id,
-                node_key,
-                {
-                    "pout": {"Out": df},
-                    "config": json.dumps(settings, sort_keys=True),
-                    "script": script,
-                },
-            )
-            script_handler.script += script
-            return {"Out": df}
-        else:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DatetimeExtract:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# Datetime Extract")
+
+        items: list[str] = settings["items"] if ("items" in settings and settings["items"]) else None
+
+        if items:
+            for item in items:
+                # column_to_convert, new_column_name, to_extract
+                column_to_convert: str = item["column_to_convert"] if ("column_to_convert" in item and item["column_to_convert"]) else ""
+                to_extract: str = item["to_extract"] if ("to_extract" in item and item["to_extract"]) else ""
+                new_column_name: str = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else to_extract.replace("()", "")
+
+                if not to_extract or not column_to_convert:
+                    msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+                    return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+                try:
+                    df[new_column_name] = eval("df[column_to_convert].dt.{}".format(to_extract))
+                    script.append(f'df["{new_column_name}"] = df["{column_to_convert}"].dt.{to_extract}')
+
+                except Exception as e:
+                    msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                    return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+            cache_handler.update_node(
+                flow_id,
+                node_key,
+                {
+                    "pout": {"Out": df},
+                    "config": json.dumps(settings, sort_keys=True),
+                    "script": script,
+                },
+            )
+            script_handler.script += script
+            return {"Out": df}
+        else:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_fill.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/datetime_fill.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DatetimeFill:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# DATETIME FILL")
-
-        time_column: str = settings["time_column"] if "time_column" in settings else None
-        key_columns: list = settings["key_columns"] if "key_columns" in settings else []
-        frequency = settings["frequency"] if "frequency" in settings else None
-        msg = ''
-
-        if not time_column:
-            msg = app_message.dataprep["nodes"]["datetime_fill"]["time_column_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        if not key_columns:
-            msg = app_message.dataprep["nodes"]["datetime_fill"]["key_column_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        if not frequency:
-            msg = app_message.dataprep["nodes"]["datetime_fill"]["frequency_column_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if time_column and key_columns and frequency:
-            try:
-                df = df.set_index([time_column] + key_columns).unstack(fill_value=0).asfreq(frequency, fill_value=0).stack().sort_index(level=1).reset_index()
-                script.append(f"df = df.set_index({[time_column] + key_columns}).unstack(fill_value=0).asfreq('{frequency}', fill_value=0).stack().sort_index(level=1).reset_index()")
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
-
-            cache_handler.update_node(
-                flow_id,
-                node_key,
-                {
-                    "pout": {"Out": df},
-                    "config": json.dumps(settings, sort_keys=True),
-                    "script": script,
-                },
-            )
-            script_handler.script += script
-            return {"Out": df}
-        else:
-            msg = app_message.dataprep["nodes"]["datetime_fill"]["properties_not_provided"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DatetimeFill:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# DATETIME FILL")
+
+        time_column: str = settings["time_column"] if "time_column" in settings else None
+        key_columns: list = settings["key_columns"] if "key_columns" in settings else []
+        frequency = settings["frequency"] if "frequency" in settings else None
+        msg = ''
+
+        if not time_column:
+            msg = app_message.dataprep["nodes"]["datetime_fill"]["time_column_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not key_columns:
+            msg = app_message.dataprep["nodes"]["datetime_fill"]["key_column_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not frequency:
+            msg = app_message.dataprep["nodes"]["datetime_fill"]["frequency_column_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if time_column and key_columns and frequency:
+            try:
+                df = df.set_index([time_column] + key_columns).unstack(fill_value=0).asfreq(frequency, fill_value=0).stack().sort_index(level=1).reset_index()
+                script.append(f"df = df.set_index({[time_column] + key_columns}).unstack(fill_value=0).asfreq('{frequency}', fill_value=0).stack().sort_index(level=1).reset_index()")
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
+
+            cache_handler.update_node(
+                flow_id,
+                node_key,
+                {
+                    "pout": {"Out": df},
+                    "config": json.dumps(settings, sort_keys=True),
+                    "script": script,
+                },
+            )
+            script_handler.script += script
+            return {"Out": df}
+        else:
+            msg = app_message.dataprep["nodes"]["datetime_fill"]["properties_not_provided"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_formatter.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/datetime_formatter.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import datetime
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DatetimeFormatter:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# Datetime Formatter")
-        items: list[str] = settings["items"] if ("items" in settings and settings["items"]) else None
-
-        if items:
-            for item in items:
-                # column_to_convert, new_column_name, pattern, custom_pattern
-                column_to_convert: str = item["column_to_convert"] if "column_to_convert" in item and item["column_to_convert"] else None
-                new_column_name: str = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else column_to_convert
-                preconfigured_pattern: str = item["preconfigured_pattern"] if "preconfigured_pattern" in item and item["preconfigured_pattern"] else None
-                custom_pattern: str = item["custom_pattern"] if "custom_pattern" in item and item["custom_pattern"] else None
-
-                if not column_to_convert:
-                    msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-                    return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-                if custom_pattern:
-                    if custom_pattern[0] not in ["'", '"'] or custom_pattern[-1] not in ["'", '"']:
-                        msg = app_message.dataprep["nodes"]["datetime_formatter"]["pattern_quotes"](node_key)
-                        return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-                    preconfigured_pattern = custom_pattern[1:-1]
-                else:
-                    if not preconfigured_pattern:
-                        msg = app_message.dataprep["nodes"]["datetime_formatter"]["pattern_required"](node_key)
-                        return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-                try:
-                    if df[column_to_convert].dtype == "object" or df[column_to_convert].dtype == "str":
-                        df[new_column_name] = pd.to_datetime(df[column_to_convert], format=preconfigured_pattern)
-                        script.append(f"df['{new_column_name}'] = pd.to_datetime(df['{column_to_convert}'], format='{preconfigured_pattern}')")
-                    else:
-                        df[new_column_name] = df[column_to_convert].dt.strftime(preconfigured_pattern)
-                        script.append(f"df['{new_column_name}'] = df['{column_to_convert}'].dt.strftime('{preconfigured_pattern}')")
-
-                except Exception as e:
-                    msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                    return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-            cache_handler.update_node(
-                flow_id,
-                node_key,
-                {
-                    "pout": {"Out": df},
-                    "config": json.dumps(settings, sort_keys=True),
-                    "script": script,
-                },
-            )
-            script_handler.script += script
-            return {"Out": df}
-        else:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-    # def process_datetime(self, _datetime, pattern, script):
-    #     # Hay que ver por qué ocurren estos 2 casos
-    #     # Cuando es string entra como None
-    #     if isinstance(_datetime, float):
-    #         return None
-    #     # Cuando es datetime entra como NaT
-    #     if pd.isnull(_datetime):
-    #         return None
-    #     if not _datetime:
-    #         return None
-
-    #     result = _datetime
-    #     # Es string
-    #     if isinstance(_datetime, str):
-    #         result = datetime.datetime.strptime(_datetime.lower(), pattern)
-    #         if len(script) == 2:
-    #             script.append(f"""def process_datetime(_datetime, pattern): \n\treturn datetime.datetime.strptime(_datetime.lower(), pattern)""")
-    #     else:
-    #         result = _datetime.strftime(pattern)
-    #         if len(script) == 2:
-    #             script.append(f"""def process_datetime(_datetime, pattern): \n\treturn _datetime.strftime(pattern)""")
-    #     return result
+import datetime
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DatetimeFormatter:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# Datetime Formatter")
+        items: list[str] = settings["items"] if ("items" in settings and settings["items"]) else None
+
+        if items:
+            for item in items:
+                # column_to_convert, new_column_name, pattern, custom_pattern
+                column_to_convert: str = item["column_to_convert"] if "column_to_convert" in item and item["column_to_convert"] else None
+                new_column_name: str = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else column_to_convert
+                preconfigured_pattern: str = item["preconfigured_pattern"] if "preconfigured_pattern" in item and item["preconfigured_pattern"] else None
+                custom_pattern: str = item["custom_pattern"] if "custom_pattern" in item and item["custom_pattern"] else None
+
+                if not column_to_convert:
+                    msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+                    return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+                if custom_pattern:
+                    if custom_pattern[0] not in ["'", '"'] or custom_pattern[-1] not in ["'", '"']:
+                        msg = app_message.dataprep["nodes"]["datetime_formatter"]["pattern_quotes"](node_key)
+                        return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+                    preconfigured_pattern = custom_pattern[1:-1]
+                else:
+                    if not preconfigured_pattern:
+                        msg = app_message.dataprep["nodes"]["datetime_formatter"]["pattern_required"](node_key)
+                        return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+                try:
+                    if df[column_to_convert].dtype == "object" or df[column_to_convert].dtype == "str":
+                        df[new_column_name] = pd.to_datetime(df[column_to_convert], format=preconfigured_pattern)
+                        script.append(f"df['{new_column_name}'] = pd.to_datetime(df['{column_to_convert}'], format='{preconfigured_pattern}')")
+                    else:
+                        df[new_column_name] = df[column_to_convert].dt.strftime(preconfigured_pattern)
+                        script.append(f"df['{new_column_name}'] = df['{column_to_convert}'].dt.strftime('{preconfigured_pattern}')")
+
+                except Exception as e:
+                    msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                    return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+            cache_handler.update_node(
+                flow_id,
+                node_key,
+                {
+                    "pout": {"Out": df},
+                    "config": json.dumps(settings, sort_keys=True),
+                    "script": script,
+                },
+            )
+            script_handler.script += script
+            return {"Out": df}
+        else:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+    # def process_datetime(self, _datetime, pattern, script):
+    #     # Hay que ver por qué ocurren estos 2 casos
+    #     # Cuando es string entra como None
+    #     if isinstance(_datetime, float):
+    #         return None
+    #     # Cuando es datetime entra como NaT
+    #     if pd.isnull(_datetime):
+    #         return None
+    #     if not _datetime:
+    #         return None
+
+    #     result = _datetime
+    #     # Es string
+    #     if isinstance(_datetime, str):
+    #         result = datetime.datetime.strptime(_datetime.lower(), pattern)
+    #         if len(script) == 2:
+    #             script.append(f"""def process_datetime(_datetime, pattern): \n\treturn datetime.datetime.strptime(_datetime.lower(), pattern)""")
+    #     else:
+    #         result = _datetime.strftime(pattern)
+    #         if len(script) == 2:
+    #             script.append(f"""def process_datetime(_datetime, pattern): \n\treturn _datetime.strftime(pattern)""")
+    #     return result
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_range.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/datetime_range.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DatetimeRange:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pd.DataFrame()
-        script.append("\n# DATETIME RANGE")
-
-        start_date: str = settings["start_date"] if "start_date" in settings else None
-        end_date: str = settings["end_date"] if "end_date" in settings else None
-        frequency: str = settings["frequency"] if "frequency" in settings else None
-
-        if not start_date:
-            msg = app_message.dataprep["nodes"]["datetime_range"]["start_date_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        if not end_date:
-            msg = app_message.dataprep["nodes"]["datetime_range"]["end_date_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        if not frequency:
-            msg = app_message.dataprep["nodes"]["datetime_range"]["frequency_is_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if start_date and end_date and frequency:
-            try:
-                df["date_range"] = pd.date_range(start=start_date, end=end_date, freq=frequency)
-                script.append(f"df['date_range'] = pd.date_range(start='{start_date}', end='{end_date}', freq='{frequency}'")
-
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
-
-            cache_handler.update_node(
-                flow_id,
-                node_key,
-                {
-                    "pout": {"Out": df},
-                    "config": json.dumps(settings, sort_keys=True),
-                    "script": script,
-                },
-            )
-            script_handler.script += script
-            return {"Out": df}
-        else:
-            msg = app_message.dataprep["nodes"]["datetime_range"]["properties_not_provided"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DatetimeRange:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pd.DataFrame()
+        script.append("\n# DATETIME RANGE")
+
+        start_date: str = settings["start_date"] if "start_date" in settings else None
+        end_date: str = settings["end_date"] if "end_date" in settings else None
+        frequency: str = settings["frequency"] if "frequency" in settings else None
+
+        if not start_date:
+            msg = app_message.dataprep["nodes"]["datetime_range"]["start_date_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not end_date:
+            msg = app_message.dataprep["nodes"]["datetime_range"]["end_date_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not frequency:
+            msg = app_message.dataprep["nodes"]["datetime_range"]["frequency_is_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if start_date and end_date and frequency:
+            try:
+                df["date_range"] = pd.date_range(start=start_date, end=end_date, freq=frequency)
+                script.append(f"df['date_range'] = pd.date_range(start='{start_date}', end='{end_date}', freq='{frequency}'")
+
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
+
+            cache_handler.update_node(
+                flow_id,
+                node_key,
+                {
+                    "pout": {"Out": df},
+                    "config": json.dumps(settings, sort_keys=True),
+                    "script": script,
+                },
+            )
+            script_handler.script += script
+            return {"Out": df}
+        else:
+            msg = app_message.dataprep["nodes"]["datetime_range"]["properties_not_provided"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/describe.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/describe.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Describe:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# DESCRIBE")
-        all_: str = "all"  # TODO: recibir desde la config
-        groupby: list = settings["groupby"] if ("groupby" in settings and settings["groupby"]) else []
-        fields: list = settings["fields"] if ("fields" in settings and settings["fields"]) else []
-        percentiles: list = settings["percentiles"] if ("percentiles" in settings and settings["percentiles"]) else []
-        custom_percentiles: list = settings["custompercentiles"] if ("custompercentiles" in settings and settings["custompercentiles"]) else []
-
-        if "pivot_data" not in settings:
-            settings["pivot_data"] = True
-        pivot_data: bool = settings["pivot_data"] if "pivot_data" in settings else True
-
-        if not fields:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        fields = list(filter(lambda x: x in df.columns, fields))
-        all_percentiles = percentiles + custom_percentiles
-
-        # Quitar percentiles repetidos
-        if type(all_percentiles) is list and len(all_percentiles) > 0:
-            all_percentiles = list(set(all_percentiles))
-
-        try:
-            if groupby:
-                df = df.groupby(by=groupby)[fields].describe(include=all_, percentiles=all_percentiles).reset_index()
-                script.append("df = df.groupby(by={})[{}].describe(include='{}', percentiles={}).reset_index()".format(groupby, fields, all_, all_percentiles))
-                if len(fields) > 1:
-                    df.columns = ["_".join(list(map(str, x))) if x[1] else x[0] for x in df.columns]
-                    script.append("df.columns = ['_'.join(list(map(str, x))) if x[1] else x[0] for x in df.columns]")
-                else:
-                    df.columns = [x[1] if x[1] else x[0] for x in df.columns]
-                    script.append("df.columns = [x[1] if x[1] else x[0] for x in df.columns]")
-
-            else:
-                df = df[fields].describe(include=all_, percentiles=all_percentiles)
-                script.append("df = df.describe(include='{}', percentiles={})".format(all_, all_percentiles))
-                if pivot_data and len(fields) == 1:
-                    df = df.T.reset_index().rename(columns={"index": "column"})
-                    script.append("# pivot data")
-                    script.append("df = df.T.reset_index().rename(columns={'index': 'column'})")
-                else:
-                    df = df.reset_index()
-                    script.append("df=df.reset_index()")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        df = df.round(2)
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Describe:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# DESCRIBE")
+        all_: str = "all"  # TODO: recibir desde la config
+        groupby: list = settings["groupby"] if ("groupby" in settings and settings["groupby"]) else []
+        fields: list = settings["fields"] if ("fields" in settings and settings["fields"]) else []
+        percentiles: list = settings["percentiles"] if ("percentiles" in settings and settings["percentiles"]) else []
+        custom_percentiles: list = settings["custompercentiles"] if ("custompercentiles" in settings and settings["custompercentiles"]) else []
+
+        if "pivot_data" not in settings:
+            settings["pivot_data"] = True
+        pivot_data: bool = settings["pivot_data"] if "pivot_data" in settings else True
+
+        if not fields:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        fields = list(filter(lambda x: x in df.columns, fields))
+        all_percentiles = percentiles + custom_percentiles
+
+        # Quitar percentiles repetidos
+        if type(all_percentiles) is list and len(all_percentiles) > 0:
+            all_percentiles = list(set(all_percentiles))
+
+        try:
+            if groupby:
+                df = df.groupby(by=groupby)[fields].describe(include=all_, percentiles=all_percentiles).reset_index()
+                script.append("df = df.groupby(by={})[{}].describe(include='{}', percentiles={}).reset_index()".format(groupby, fields, all_, all_percentiles))
+                if len(fields) > 1:
+                    df.columns = ["_".join(list(map(str, x))) if x[1] else x[0] for x in df.columns]
+                    script.append("df.columns = ['_'.join(list(map(str, x))) if x[1] else x[0] for x in df.columns]")
+                else:
+                    df.columns = [x[1] if x[1] else x[0] for x in df.columns]
+                    script.append("df.columns = [x[1] if x[1] else x[0] for x in df.columns]")
+
+            else:
+                df = df[fields].describe(include=all_, percentiles=all_percentiles)
+                script.append("df = df.describe(include='{}', percentiles={})".format(all_, all_percentiles))
+                if pivot_data and len(fields) == 1:
+                    df = df.T.reset_index().rename(columns={"index": "column"})
+                    script.append("# pivot data")
+                    script.append("df = df.T.reset_index().rename(columns={'index': 'column'})")
+                else:
+                    df = df.reset_index()
+                    script.append("df=df.reset_index()")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        df = df.round(2)
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/df_maker.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/df_maker.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import json
-
-import numpy as np
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DfMaker:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# DFMAKER")
-        data: list = settings["data"] if "data" in settings and settings["data"] else []
-        df = pd.DataFrame()
-        
-        try:
-            columns = []
-            rows = []
-            if len(data):
-                columns = [c["value"] if "value" in c else f"col_{idx+1}" for idx, c in enumerate(data[0])]
-                if len(data) > 1:
-                    rows = [[c["value"] for c in r] for r in data[1:]]
-
-            df = pd.DataFrame(np.array(rows), columns=columns)
-            script.append(f"rows = {rows}")
-            script.append(f"columns = {columns}")
-            script.append("df = pd.DataFrame(np.array(rows), columns=columns)")
-
-            for col in df.columns:
-                try:
-                    df[col] = pd.to_numeric(df[col])
-                except Exception as e:
-                    print(col, e)
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import numpy as np
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DfMaker:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# DFMAKER")
+        data: list = settings["data"] if "data" in settings and settings["data"] else []
+        df = pd.DataFrame()
+        
+        try:
+            columns = []
+            rows = []
+            if len(data):
+                columns = [c["value"] if "value" in c else f"col_{idx+1}" for idx, c in enumerate(data[0])]
+                if len(data) > 1:
+                    rows = [[c["value"] for c in r] for r in data[1:]]
+
+            df = pd.DataFrame(np.array(rows), columns=columns)
+            script.append(f"rows = {rows}")
+            script.append(f"columns = {columns}")
+            script.append("df = pd.DataFrame(np.array(rows), columns=columns)")
+
+            for col in df.columns:
+                try:
+                    df[col] = pd.to_numeric(df[col])
+                except Exception as e:
+                    print(col, e)
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/drop_duplicates.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/drop_duplicates.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class DropDuplicates:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# Drop Duplicates")
-
-        keep: str = settings["keep"] if ("keep" in settings and settings["keep"]) else "first"
-        columns: list[str] = settings["columns"] if ("columns" in settings and settings["columns"]) else []
-        only_subset: bool = settings["only_subset"] if "only_subset" in settings else False
-
-        try:
-            if len(columns) == 0:
-                df = df.drop_duplicates(keep=keep)
-                script.append(f"df = df.drop_duplicates(keep={keep})")
-            else:
-                df = df.drop_duplicates(subset=columns, keep=keep)
-                script.append(f"df = df.drop_duplicates(subset={columns}, keep={keep})")
-
-            if only_subset:
-                df = df[columns]
-                script.append(f"df = df[{columns}]")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class DropDuplicates:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# Drop Duplicates")
+
+        keep: str = settings["keep"] if ("keep" in settings and settings["keep"]) else "first"
+        columns: list[str] = settings["columns"] if ("columns" in settings and settings["columns"]) else []
+        only_subset: bool = settings["only_subset"] if "only_subset" in settings else False
+
+        try:
+            if len(columns) == 0:
+                df = df.drop_duplicates(keep=keep)
+                script.append(f"df = df.drop_duplicates(keep={keep})")
+            else:
+                df = df.drop_duplicates(subset=columns, keep=keep)
+                script.append(f"df = df.drop_duplicates(subset={columns}, keep={keep})")
+
+            if only_subset:
+                df = df[columns]
+                script.append(f"df = df[{columns}]")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/dtype.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/dtype.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.utilities import utilities
-import copy
-
-
-class Dtype:
-    def __init__(self):
-        self.script = []
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        df: pd.DataFrame = pin["In"].copy()
-        self.script.append("\n# DTYPE")
-
-        if "items" not in settings or not settings["items"]:
-            msg = app_message.dataprep["nodes"]["dtype"]["no_columns_selected"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        df, _, rename_cols = self.select_types_and_fields(flow_id, node_key, df, settings["items"])
-        
-        # Si hay alguna columna para renombrar en las seleccionadas
-        if rename_cols:
-            try:
-                df = df.rename(columns=rename_cols)
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["dtype"]["rename_columns"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            
-            self.script.append("\n# Rename columns")
-            self.script.append("df = df.rename(columns={})".format(rename_cols))
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": self.script.copy(),
-            },
-        )
-
-        script_handler.script += self.script.copy()
-        self.script = []
-        return {"Out": df}
-
-    # Retorna el df con las columnas seleccionadas y el tipo de dato
-    def select_types_and_fields(self, flow_id: str, node_key: str, df: pd.DataFrame, new_dtypes: dict):
-        # https://pbpython.com/pandas_dtypes.html
-        selected_dtypes = copy.deepcopy(new_dtypes)
-        # ? Para nodos de tipo DTYPE usar todos los campos, sin importar si estan o no en la config
-        if "dtype" in node_key.lower():  # aas
-            all_dtypes = utilities.get_dtypes_of_df(df)  # ? Todos los dtypes del Dataframe
-            selected_dtypes = copy.deepcopy(all_dtypes)
-        # ? Para nodos de tipo SELECTE obtener solo los campos seleccionados de la lista total de campos (selected==True)
-        elif "select" in node_key.lower():
-            selected_dtypes = dict(filter(lambda x: True if "selected" in x[1] and x[1]["selected"] else False, new_dtypes.items()))
-
-        # Existe la posibilidad de que ya no existan columnas que previamente fueron creadas
-        available_cols = [] # para nodo de tipo select
-        removed_cols = [] # para nodo de tipo select
-        
-        for field, x in selected_dtypes.items():
-            if field in df.columns:
-                available_cols.append(field)
-            else:
-                removed_cols.append(field)
-                msg = app_message.dataprep["nodes"]["dtype"]["column_not_in_df"](node_key, field)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
-
-        # Remover las columnas que ya no existen
-        for del_key in removed_cols:
-            del selected_dtypes[del_key]
-
-        # Mantener solamente columnas existentes y seleccionadas
-        df: pd.DataFrame = df[available_cols]
-        self.script.append("df = df[{}]".format(available_cols))
-        self.script.append("\n# DATA TYPES")
-
-        # Diccionario para el renombrado de variables
-        rename_cols = {}
-        standard_dtypes = [ "str", "object", "bool", "category", "int8", "int16", "int32", "int64", "float16", "float32", "float64"]
-        
-        for field, x in selected_dtypes.items():
-            # renombrar columnas
-            if field in new_dtypes and "rename" in new_dtypes[field] and new_dtypes[field]["rename"]:
-                rename_cols[field] = new_dtypes[field]["rename"]
-                
-            # orden de las columnas
-            if field in new_dtypes and "order" in new_dtypes[field]:
-                selected_dtypes[field]["order"] = new_dtypes[field]["order"]
-                
-            # nuevo tipo de dato desde la config (new_dtypes)
-            newtype = new_dtypes[field]["dtype"] if field in new_dtypes and "dtype" in new_dtypes[field] and new_dtypes[field]["dtype"] else x["dtype"]
-
-            # saltar cambio si el tipo sigue siendo el mismo
-            if df[field].dtype == newtype:
-                continue
-            
-            if newtype in standard_dtypes:
-                df, status = self.select_change_col_dtype(flow_id, node_key, df.copy(), field, newtype)
-                if not status:  # Si hubo un error se mantiene como texto (object)
-                    new_dtypes[field]["dtype"] = "object"
-
-            elif newtype in ["datetime64[ns]"]:
-                try:
-                    df = df.copy()
-                    df[field] = pd.to_datetime(df[field])
-
-                except Exception as e:
-                    msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, newtype)
-                    bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-                    # Si hubo un error se mantiene como texto (object)
-                    new_dtypes[field]["dtype"] = "object"
-
-            elif newtype in ["timedelta64[ns]"]:
-                try:
-                    df = df.copy()
-                    df[field] = pd.to_timedelta(df[field])
-                except Exception as e:
-                    msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, newtype)
-                    bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-                    # Si hubo un error se mantiene como texto (object)
-                    new_dtypes[field]["dtype"] = "object"
-
-            else:
-                msg = app_message.dataprep["nodes"]["dtype"]["unknow_dtype"](node_key, field, newtype)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
-                new_dtypes[field]["dtype"] = "object"
-
-        # Ordena las columnas segun el orden dado en la configuracion del nodo
-        order_cols = list(dict(sorted(selected_dtypes.items(), key=lambda item: item[1]["order"])).keys())
-        return df[order_cols], new_dtypes, rename_cols
-
-    # Cambia el tipo de dato y maneja los errores que podrían salir en el intento
-    def select_change_col_dtype(self, flow_id: str, node_key: str, df: pd.DataFrame, field: str, dtype: str):
-        try:
-            df[field] = df[field].astype(dtype)
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, dtype)
-            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            return df, False
-        else:
-            dtype_ = dtype if isinstance(dtype, str) else dtype.__name__
-            self.script.append("df['{0}'] = df['{0}'].astype('{1}')".format(field, dtype_))
-            return df, True
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.utilities import utilities
+import copy
+
+
+class Dtype:
+    def __init__(self):
+        self.script = []
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        df: pd.DataFrame = pin["In"].copy()
+        self.script.append("\n# DTYPE")
+
+        if "items" not in settings or not settings["items"]:
+            msg = app_message.dataprep["nodes"]["dtype"]["no_columns_selected"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        df, _, rename_cols = self.select_types_and_fields(flow_id, node_key, df, settings["items"])
+        
+        # Si hay alguna columna para renombrar en las seleccionadas
+        if rename_cols:
+            try:
+                df = df.rename(columns=rename_cols)
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["dtype"]["rename_columns"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            
+            self.script.append("\n# Rename columns")
+            self.script.append("df = df.rename(columns={})".format(rename_cols))
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": self.script.copy(),
+            },
+        )
+
+        script_handler.script += self.script.copy()
+        self.script = []
+        return {"Out": df}
+
+    # Retorna el df con las columnas seleccionadas y el tipo de dato
+    def select_types_and_fields(self, flow_id: str, node_key: str, df: pd.DataFrame, new_dtypes: dict):
+        # https://pbpython.com/pandas_dtypes.html
+        selected_dtypes = copy.deepcopy(new_dtypes)
+        # ? Para nodos de tipo DTYPE usar todos los campos, sin importar si estan o no en la config
+        if "dtype" in node_key.lower():  # aas
+            all_dtypes = utilities.get_dtypes_of_df(df)  # ? Todos los dtypes del Dataframe
+            selected_dtypes = copy.deepcopy(all_dtypes)
+        # ? Para nodos de tipo SELECTE obtener solo los campos seleccionados de la lista total de campos (selected==True)
+        elif "select" in node_key.lower():
+            selected_dtypes = dict(filter(lambda x: True if "selected" in x[1] and x[1]["selected"] else False, new_dtypes.items()))
+
+        # Existe la posibilidad de que ya no existan columnas que previamente fueron creadas
+        available_cols = [] # para nodo de tipo select
+        removed_cols = [] # para nodo de tipo select
+        
+        for field, x in selected_dtypes.items():
+            if field in df.columns:
+                available_cols.append(field)
+            else:
+                removed_cols.append(field)
+                msg = app_message.dataprep["nodes"]["dtype"]["column_not_in_df"](node_key, field)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning", success=True)
+
+        # Remover las columnas que ya no existen
+        for del_key in removed_cols:
+            del selected_dtypes[del_key]
+
+        # Mantener solamente columnas existentes y seleccionadas
+        df: pd.DataFrame = df[available_cols]
+        self.script.append("df = df[{}]".format(available_cols))
+        self.script.append("\n# DATA TYPES")
+
+        # Diccionario para el renombrado de variables
+        rename_cols = {}
+        standard_dtypes = [ "str", "object", "bool", "category", "int8", "int16", "int32", "int64", "float16", "float32", "float64"]
+        
+        for field, x in selected_dtypes.items():
+            # renombrar columnas
+            if field in new_dtypes and "rename" in new_dtypes[field] and new_dtypes[field]["rename"]:
+                rename_cols[field] = new_dtypes[field]["rename"]
+                
+            # orden de las columnas
+            if field in new_dtypes and "order" in new_dtypes[field]:
+                selected_dtypes[field]["order"] = new_dtypes[field]["order"]
+                
+            # nuevo tipo de dato desde la config (new_dtypes)
+            newtype = new_dtypes[field]["dtype"] if field in new_dtypes and "dtype" in new_dtypes[field] and new_dtypes[field]["dtype"] else x["dtype"]
+
+            # saltar cambio si el tipo sigue siendo el mismo
+            if df[field].dtype == newtype:
+                continue
+            
+            if newtype in standard_dtypes:
+                df, status = self.select_change_col_dtype(flow_id, node_key, df.copy(), field, newtype)
+                if not status:  # Si hubo un error se mantiene como texto (object)
+                    new_dtypes[field]["dtype"] = "object"
+
+            elif newtype in ["datetime64[ns]"]:
+                try:
+                    df = df.copy()
+                    df[field] = pd.to_datetime(df[field])
+
+                except Exception as e:
+                    msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, newtype)
+                    bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+                    # Si hubo un error se mantiene como texto (object)
+                    new_dtypes[field]["dtype"] = "object"
+
+            elif newtype in ["timedelta64[ns]"]:
+                try:
+                    df = df.copy()
+                    df[field] = pd.to_timedelta(df[field])
+                except Exception as e:
+                    msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, newtype)
+                    bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+                    # Si hubo un error se mantiene como texto (object)
+                    new_dtypes[field]["dtype"] = "object"
+
+            else:
+                msg = app_message.dataprep["nodes"]["dtype"]["unknow_dtype"](node_key, field, newtype)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
+                new_dtypes[field]["dtype"] = "object"
+
+        # Ordena las columnas segun el orden dado en la configuracion del nodo
+        order_cols = list(dict(sorted(selected_dtypes.items(), key=lambda item: item[1]["order"])).keys())
+        return df[order_cols], new_dtypes, rename_cols
+
+    # Cambia el tipo de dato y maneja los errores que podrían salir en el intento
+    def select_change_col_dtype(self, flow_id: str, node_key: str, df: pd.DataFrame, field: str, dtype: str):
+        try:
+            df[field] = df[field].astype(dtype)
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["dtype"]["change_dtype"](node_key, field, dtype)
+            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            return df, False
+        else:
+            dtype_ = dtype if isinstance(dtype, str) else dtype.__name__
+            self.script.append("df['{0}'] = df['{0}'].astype('{1}')".format(field, dtype_))
+            return df, True
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/email.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/email.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import io
-import json
-import os
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils import normpath
-from vtarget.utils.email_sender import EmailSender
-from vtarget.utils.encrypter import encrypter
-
-
-class Email:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        streams: list[dict] = []
-        files: list[str] = []
-        ports: list[str] = [p for p in dict(settings).keys() if str(p).startswith("port_")]
-
-        total_size: int = 0
-
-        # * deploy mode habilitado
-        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-
-        for port in ports:
-            port_origin: str = settings[port] if port in settings else None
-            if port_origin:
-                # * Extraer key y puerto de salida del nodo
-                sepIdx = len(port_origin) - port_origin[::-1].find("_")
-                parent_key: str = port_origin[0 : sepIdx - 1]
-                parent_port: str = port_origin[sepIdx:]
-                
-                if parent_key is not None and parent_port is not None:
-                    # ? Obtener el df del padre desde cache
-                    parent_settings = cache_handler.settings[flow_id][parent_key]
-                    parent = cache_handler.cache[flow_id][parent_key]
-                    
-                    if parent_key.lower().startswith("excel"):  # * Nodos de tipo excel
-                        # ? Obtener la ruta del archivo excel generado
-                        parent_config: dict = json.loads(parent_settings["config"]) if "config" in parent_settings else {}
-                        file_path: str = parent_config["file_path"] if "file_path" in parent_config else None
-                        
-                        if file_path is None:
-                            output_name: str = parent_config["name"] if "name" in parent_config else None
-                            output_path: str = parent_config["path"] if "path" in parent_config else None
-                            
-                            if deploy_enabled:
-                                output_path = settings["deploy_path"] if "deploy_path" in settings else None
-                                
-                            if output_name and output_path:
-                                file_path = output_path + os.path.sep + output_name + ".xlsx"
-                                file_path = normpath(file_path)
-
-                        # ? Agregar la ruta del archivo a la lista de archivos
-                        if file_path is not None:
-                            files.append(file_path)
-                            # ? sumar peso del excel al total
-                            size = os.path.getsize(file_path)
-                            total_size += size
-                            
-                    else:  # * Cualquier otro tipo de nodos
-                        # ? Convertir df del puerto de origen en un csv en memoria
-                        df_in: pd.DataFrame = parent["pout"][parent_port] if "pout" in parent and parent_port in parent["pout"] else pd.DataFrame()
-                        if len(df_in):
-                            stream = io.StringIO()
-                            df_in.to_csv(stream, index=False)
-                            # ? sumar peso del csv al total
-                            pos = stream.tell()
-                            stream.seek(0, os.SEEK_END)
-                            stream.seek(pos)
-                            total_size += pos
-                            # ? agregar el stream a la lista y asignarle un nombre por defecto
-                            streams.append({"filename": f"{port_origin}.csv", "attachment": stream})
-
-        # * Check if total size > 20Mb
-        if total_size / (1024 * 1024) > 20:
-            msg = app_message.dataprep["nodes"]["email"]["size_max"](node_key, str(validation))
-            return bug_handler.default_node_log(flow_id, node_key, msg)
-
-        script.append("\n# EMAIL")
-        SERVER: str = settings["server"] if "server" in settings and settings["server"] else None
-        PORT: str = settings["port"] if "port" in settings and settings["port"] else None
-        FROM: str = settings["from"] if "from" in settings and settings["from"] else None
-        PASS: str = settings["password"] if "password" in settings and settings["password"] else None
-
-        if deploy_enabled:
-            SERVER: str = settings["deploy_server"] if "server" in settings and settings["deploy_server"] else None
-            PORT: str = settings["deploy_port"] if "port" in settings and settings["deploy_port"] else None
-            FROM: str = settings["deploy_from"] if "from" in settings and settings["deploy_from"] else None
-            PASS: str = settings["deploy_password"] if "password" in settings and settings["deploy_password"] else None
-
-        to: list = settings["to"] if "to" in settings and settings["to"] else []
-        subject = settings["subject"] if "subject" in settings else "-"
-        message = settings["message"] if "message" in settings else ""
-        validation = list(set(["server", "port", "from", "password", "to"]) - set([k for k in settings.keys() if settings[k]]))
-
-        if len(validation) != 0:
-            msg = app_message.dataprep["nodes"]["email"]["config_required"](node_key, str(validation))
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        decryptKey = flow_id[:16]
-        DECRYPTEDPASS = encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
-
-        try:
-            emailSender = EmailSender()
-            emailSender.configure_server(SERVER, PORT, FROM, DECRYPTEDPASS)
-            emailSender.send_email(",".join(to), subject, message, streams=streams, files=files)
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["email"]["failed_send"](node_key)
-            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            return {}
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {}
+import io
+import json
+import os
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils import normpath
+from vtarget.utils.email_sender import EmailSender
+from vtarget.utils.encrypter import encrypter
+
+
+class Email:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        streams: list[dict] = []
+        files: list[str] = []
+        ports: list[str] = [p for p in dict(settings).keys() if str(p).startswith("port_")]
+
+        total_size: int = 0
+
+        # * deploy mode habilitado
+        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+
+        for port in ports:
+            port_origin: str = settings[port] if port in settings else None
+            if port_origin:
+                # * Extraer key y puerto de salida del nodo
+                sepIdx = len(port_origin) - port_origin[::-1].find("_")
+                parent_key: str = port_origin[0 : sepIdx - 1]
+                parent_port: str = port_origin[sepIdx:]
+                
+                if parent_key is not None and parent_port is not None:
+                    # ? Obtener el df del padre desde cache
+                    parent_settings = cache_handler.settings[flow_id][parent_key]
+                    parent = cache_handler.cache[flow_id][parent_key]
+                    
+                    if parent_key.lower().startswith("excel"):  # * Nodos de tipo excel
+                        # ? Obtener la ruta del archivo excel generado
+                        parent_config: dict = json.loads(parent_settings["config"]) if "config" in parent_settings else {}
+                        file_path: str = parent_config["file_path"] if "file_path" in parent_config else None
+                        
+                        if file_path is None:
+                            output_name: str = parent_config["name"] if "name" in parent_config else None
+                            output_path: str = parent_config["path"] if "path" in parent_config else None
+                            
+                            if deploy_enabled:
+                                output_path = settings["deploy_path"] if "deploy_path" in settings else None
+                                
+                            if output_name and output_path:
+                                file_path = output_path + os.path.sep + output_name + ".xlsx"
+                                file_path = normpath(file_path)
+
+                        # ? Agregar la ruta del archivo a la lista de archivos
+                        if file_path is not None:
+                            files.append(file_path)
+                            # ? sumar peso del excel al total
+                            size = os.path.getsize(file_path)
+                            total_size += size
+                            
+                    else:  # * Cualquier otro tipo de nodos
+                        # ? Convertir df del puerto de origen en un csv en memoria
+                        df_in: pd.DataFrame = parent["pout"][parent_port] if "pout" in parent and parent_port in parent["pout"] else pd.DataFrame()
+                        if len(df_in):
+                            stream = io.StringIO()
+                            df_in.to_csv(stream, index=False)
+                            # ? sumar peso del csv al total
+                            pos = stream.tell()
+                            stream.seek(0, os.SEEK_END)
+                            stream.seek(pos)
+                            total_size += pos
+                            # ? agregar el stream a la lista y asignarle un nombre por defecto
+                            streams.append({"filename": f"{port_origin}.csv", "attachment": stream})
+
+        # * Check if total size > 20Mb
+        if total_size / (1024 * 1024) > 20:
+            msg = app_message.dataprep["nodes"]["email"]["size_max"](node_key, str(validation))
+            return bug_handler.default_node_log(flow_id, node_key, msg)
+
+        script.append("\n# EMAIL")
+        SERVER: str = settings["server"] if "server" in settings and settings["server"] else None
+        PORT: str = settings["port"] if "port" in settings and settings["port"] else None
+        FROM: str = settings["from"] if "from" in settings and settings["from"] else None
+        PASS: str = settings["password"] if "password" in settings and settings["password"] else None
+
+        if deploy_enabled:
+            SERVER: str = settings["deploy_server"] if "server" in settings and settings["deploy_server"] else None
+            PORT: str = settings["deploy_port"] if "port" in settings and settings["deploy_port"] else None
+            FROM: str = settings["deploy_from"] if "from" in settings and settings["deploy_from"] else None
+            PASS: str = settings["deploy_password"] if "password" in settings and settings["deploy_password"] else None
+
+        to: list = settings["to"] if "to" in settings and settings["to"] else []
+        subject = settings["subject"] if "subject" in settings else "-"
+        message = settings["message"] if "message" in settings else ""
+        validation = list(set(["server", "port", "from", "password", "to"]) - set([k for k in settings.keys() if settings[k]]))
+
+        if len(validation) != 0:
+            msg = app_message.dataprep["nodes"]["email"]["config_required"](node_key, str(validation))
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        decryptKey = flow_id[:16]
+        DECRYPTEDPASS = encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
+
+        try:
+            emailSender = EmailSender()
+            emailSender.configure_server(SERVER, PORT, FROM, DECRYPTEDPASS)
+            emailSender.send_email(",".join(to), subject, message, streams=streams, files=files)
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["email"]["failed_send"](node_key)
+            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            return {}
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/excel.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/excel.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import json
-import math
-import os
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils import normpath
-
-
-class ExcelOutput:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# EXCEL")
-        output_name: str = settings["name"] if "name" in settings and settings["name"] != "" else "output"
-        output_path: str = settings["path"] if "path" in settings and settings["path"] != "" else ""
-        encoding: str = settings["encoding"] or "UTF-8"
-
-        # * Deploy mode habilitado
-        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-        if deploy_enabled:
-            if "deploy_path" not in settings:
-                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            output_path = settings["deploy_path"] if "deploy_path" in settings else ""
-            
-        if not output_path:
-            msg = app_message.dataprep["nodes"]["excel"]["output_path"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        df1 = pin["In"].copy() if "In" in pin else pd.DataFrame()
-        df2 = pin["In2"].copy() if "In2" in pin else pd.DataFrame()
-        df3 = pin["In3"].copy() if "In3" in pin else pd.DataFrame()
-        df4 = pin["In4"].copy() if "In4" in pin else pd.DataFrame()
-        df5 = pin["In5"].copy() if "In5" in pin else pd.DataFrame()
-
-        sheet_name_1: str = settings["sheet1"] if "sheet1" in settings and settings["sheet1"] != "" else "sheet_1"
-        sheet_name_2: str = settings["sheet2"] if "sheet2" in settings and settings["sheet2"] != "" else "sheet_2"
-        sheet_name_3: str = settings["sheet3"] if "sheet3" in settings and settings["sheet3"] != "" else "sheet_3"
-        sheet_name_4: str = settings["sheet4"] if "sheet4" in settings and settings["sheet4"] != "" else "sheet_4"
-        sheet_name_5: str = settings["sheet5"] if "sheet5" in settings and settings["sheet5"] != "" else "sheet_5"
-
-        file_path = output_path + os.path.sep + output_name + ".xlsx"
-        file_path = normpath(file_path)
-
-        settings["file_path"] = file_path
-        try:
-            # Create a excel writer object
-            with pd.ExcelWriter(file_path) as writer:
-                script.append(f"with pd.ExcelWriter({file_path}) as writer:")
-                # Use to_excel function and specify the sheet_name and index
-                # to store the dataframe in specified sheet
-                if len(df1) > 0:
-                    self.pd_to_excel(df1, writer, sheet_name_1, encoding, True)
-                    script.append(f"\tdf_In1.to_excel(writer, sheet_name='{sheet_name_1}', index=False, encoding='{encoding}')")
-                if len(df2) > 0:
-                    self.pd_to_excel(df2, writer, sheet_name_2, encoding)
-                    script.append(f"\tdf_In2.to_excel(writer, sheet_name='{sheet_name_2}', index=False, encoding='{encoding}')")
-                if len(df3) > 0:
-                    self.pd_to_excel(df3, writer, sheet_name_3, encoding)
-                    script.append(f"\tdf_In3.to_excel(writer, sheet_name='{sheet_name_3}', index=False, encoding='{encoding}')")
-                if len(df4) > 0:
-                    self.pd_to_excel(df4, writer, sheet_name_4, encoding)
-                    script.append(f"\tdf_In4.to_excel(writer, sheet_name='{sheet_name_4}', index=False, encoding='{encoding}')")
-                if len(df5) > 0:
-                    self.pd_to_excel(df5, writer, sheet_name_5, encoding)
-                    script.append(f"\tdf_In5.to_excel(writer, sheet_name='{sheet_name_5}', index=False, encoding='{encoding}')")
-                    
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["excel"]["failed_generate"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        out = []
-        sheet_names = [sheet_name_1, sheet_name_2, sheet_name_3, sheet_name_4, sheet_name_5]
-        for idx, df in enumerate([df1, df2, df3, df4, df5]):
-            if len(df):
-                out.append(
-                    {
-                        "Name": sheet_names[idx],
-                        "Columns": len(df.columns),
-                        "Rows": len(df),
-                        # "File_Path": file_path,
-                    }
-                )
-
-        df = pd.DataFrame(out)
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-        
-        script_handler.script += script
-
-        return {"Out": df}
-
-    def pd_to_excel(self, df: pd.DataFrame, writer: pd.ExcelWriter, sheet_name: str, encoding: str, index=False):
-        # https://support.microsoft.com/en-us/office/excel-specifications-and-limits-1672b34d-7043-467e-8e27-269d656771c3?ui=en-us&rs=en-us&ad=us
-        rows: int = len(df)
-        rows_per_sheet = 1048576 - 1  # max rows by worksheet = 1048576
-        if rows > rows_per_sheet:
-            steps = math.ceil(rows / rows_per_sheet)
-            start = 0
-            end = rows_per_sheet
-
-            for idx in range(steps):
-                step_df = df.copy().iloc[start:end]
-                step_df.to_excel(writer, sheet_name=f"{sheet_name}_{idx + 1}", index=False, encoding=encoding)
-                start = end
-                end += rows_per_sheet
-        else:
-            df.to_excel(writer, sheet_name=sheet_name, index=index, encoding=encoding)
+import json
+import math
+import os
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils import normpath
+
+
+class ExcelOutput:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# EXCEL")
+        output_name: str = settings["name"] if "name" in settings and settings["name"] != "" else "output"
+        output_path: str = settings["path"] if "path" in settings and settings["path"] != "" else ""
+        encoding: str = settings["encoding"] or "UTF-8"
+
+        # * Deploy mode habilitado
+        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+        if deploy_enabled:
+            if "deploy_path" not in settings:
+                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+            output_path = settings["deploy_path"] if "deploy_path" in settings else ""
+            
+        if not output_path:
+            msg = app_message.dataprep["nodes"]["excel"]["output_path"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        df1 = pin["In"].copy() if "In" in pin else pd.DataFrame()
+        df2 = pin["In2"].copy() if "In2" in pin else pd.DataFrame()
+        df3 = pin["In3"].copy() if "In3" in pin else pd.DataFrame()
+        df4 = pin["In4"].copy() if "In4" in pin else pd.DataFrame()
+        df5 = pin["In5"].copy() if "In5" in pin else pd.DataFrame()
+
+        sheet_name_1: str = settings["sheet1"] if "sheet1" in settings and settings["sheet1"] != "" else "sheet_1"
+        sheet_name_2: str = settings["sheet2"] if "sheet2" in settings and settings["sheet2"] != "" else "sheet_2"
+        sheet_name_3: str = settings["sheet3"] if "sheet3" in settings and settings["sheet3"] != "" else "sheet_3"
+        sheet_name_4: str = settings["sheet4"] if "sheet4" in settings and settings["sheet4"] != "" else "sheet_4"
+        sheet_name_5: str = settings["sheet5"] if "sheet5" in settings and settings["sheet5"] != "" else "sheet_5"
+
+        file_path = output_path + os.path.sep + output_name + ".xlsx"
+        file_path = normpath(file_path)
+
+        settings["file_path"] = file_path
+        try:
+            # Create a excel writer object
+            with pd.ExcelWriter(file_path) as writer:
+                script.append(f"with pd.ExcelWriter({file_path}) as writer:")
+                # Use to_excel function and specify the sheet_name and index
+                # to store the dataframe in specified sheet
+                if len(df1) > 0:
+                    self.pd_to_excel(df1, writer, sheet_name_1, encoding, True)
+                    script.append(f"\tdf_In1.to_excel(writer, sheet_name='{sheet_name_1}', index=False, encoding='{encoding}')")
+                if len(df2) > 0:
+                    self.pd_to_excel(df2, writer, sheet_name_2, encoding)
+                    script.append(f"\tdf_In2.to_excel(writer, sheet_name='{sheet_name_2}', index=False, encoding='{encoding}')")
+                if len(df3) > 0:
+                    self.pd_to_excel(df3, writer, sheet_name_3, encoding)
+                    script.append(f"\tdf_In3.to_excel(writer, sheet_name='{sheet_name_3}', index=False, encoding='{encoding}')")
+                if len(df4) > 0:
+                    self.pd_to_excel(df4, writer, sheet_name_4, encoding)
+                    script.append(f"\tdf_In4.to_excel(writer, sheet_name='{sheet_name_4}', index=False, encoding='{encoding}')")
+                if len(df5) > 0:
+                    self.pd_to_excel(df5, writer, sheet_name_5, encoding)
+                    script.append(f"\tdf_In5.to_excel(writer, sheet_name='{sheet_name_5}', index=False, encoding='{encoding}')")
+                    
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["excel"]["failed_generate"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        out = []
+        sheet_names = [sheet_name_1, sheet_name_2, sheet_name_3, sheet_name_4, sheet_name_5]
+        for idx, df in enumerate([df1, df2, df3, df4, df5]):
+            if len(df):
+                out.append(
+                    {
+                        "Name": sheet_names[idx],
+                        "Columns": len(df.columns),
+                        "Rows": len(df),
+                        # "File_Path": file_path,
+                    }
+                )
+
+        df = pd.DataFrame(out)
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+        
+        script_handler.script += script
+
+        return {"Out": df}
+
+    def pd_to_excel(self, df: pd.DataFrame, writer: pd.ExcelWriter, sheet_name: str, encoding: str, index=False):
+        # https://support.microsoft.com/en-us/office/excel-specifications-and-limits-1672b34d-7043-467e-8e27-269d656771c3?ui=en-us&rs=en-us&ad=us
+        rows: int = len(df)
+        rows_per_sheet = 1048576 - 1  # max rows by worksheet = 1048576
+        if rows > rows_per_sheet:
+            steps = math.ceil(rows / rows_per_sheet)
+            start = 0
+            end = rows_per_sheet
+
+            for idx in range(steps):
+                step_df = df.copy().iloc[start:end]
+                step_df.to_excel(writer, sheet_name=f"{sheet_name}_{idx + 1}", index=False, encoding=encoding)
+                start = end
+                end += rows_per_sheet
+        else:
+            df.to_excel(writer, sheet_name=sheet_name, index=index, encoding=encoding)
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/filter.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/filter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import importlib
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.utilities import utilities
-
-
-class Filter:
-    def __init__(self):
-        self.script = []
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        if "rule_type" not in settings:
-            msg = app_message.dataprep["nodes"]["filter"]["rules"](node_key)
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            return {"T": pd.DataFrame(), "F": pd.DataFrame()}
-
-        df: pd.DataFrame = pin["In"].copy()
-        df_T, df_F = pd.DataFrame(), pd.DataFrame()
-        
-        # NOTE: en versiones nuevas ya no se usa
-        if settings["rule_type"] == "preconfigured":
-            try:
-                df_T, df_F = self.filter_preconfigured(flow_id, node_key, df, settings)
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-                return {"T": pd.DataFrame(), "F": pd.DataFrame()}
-
-        elif settings["rule_type"] == "code":
-            # Agrego los modulos y alias al entorno de variables globales
-            imports_code: str = settings["imports"] if "imports" in settings and settings["imports"] else ""
-            used_modules = utilities.find_imports(imports_code)
-            for m in used_modules:
-                try:
-                    if m["alias"]:
-                        globals()[m["alias"]] = importlib.import_module(m["name"])
-                    else:
-                        globals().update(importlib.import_module(m["name"]).__dict__)
-                except ModuleNotFoundError as e:
-                    import os
-                    import subprocess
-
-                    current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
-                    python_path = os.path.join(current_path, "python", "python")
-                    
-                    if os.path.exists(python_path):
-                        subprocess.run(
-                            [
-                                python_path,
-                                "-m",
-                                "pipenv",
-                                "install",
-                                "--skip-lock",
-                                m["name"].split(".")[0],
-                            ]
-                        )
-                    else:
-                        import pip
-                        pip.main(["install", m["name"].split(".")[0]])
-                        
-                    if m["alias"]:
-                        globals()[m["alias"]] = importlib.import_module(m["name"])
-                    else:
-                        globals().update(importlib.import_module(m["name"]).__dict__)
-                        
-            df_T, df_F = self.filter_code(flow_id, node_key, df, settings["sentence"])
-        else:
-            msg = app_message.dataprep["nodes"]["filter"]["unknow_rule"](node_key, str(settings["rule_type"]))
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
-            
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"T": df_T, "F": df_F},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": self.script,
-            },
-        )
-        script_handler.script += self.script.copy()
-        self.script = []
-        return {"T": df_T, "F": df_F}
-
-    # Nodo: filter - Procesa el filtro de sentencia
-    def filter_code(self, flow_id, node_key, df, sentence):
-        self.script.append("\n# FILTER (CUSTOMIZED)")
-        str_rule = "df[{}]".format(sentence)
-        
-        try:
-            df_T = eval(str_rule)
-            self.script.append("df_T = {}".format(str_rule))
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["filter"]["failed_condition"](node_key)
-            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            return pd.DataFrame(), pd.DataFrame()
-        else:
-            # Obtengo el complemento (la parte negada de la condición)
-            df_F = df[~df.index.isin(df_T.index)]
-            self.script.append("df_F = df[~df.index.isin(df_T.index)]")
-            return df_T, df_F
-
-    # Nodo: filter - Procesa el filtro preconfigurado (Deprecated en neuvas versiones)
-    def filter_preconfigured(self, flow_id, node_key, df: pd.DataFrame, rule):
-        df_T, df_F = pd.DataFrame(), pd.DataFrame()
-        self.script.append("\n# FILTER (PRECONFIGURED)")
-        field: str = rule["field"]
-        operator: str = rule["operator"]
-        value: str = rule["value"] if "value" in rule else '""'
-        sensitive_case: bool = True if pd.api.types.is_string_dtype(df[field]) and "sensitive_case" in rule and rule["sensitive_case"] else False
-        if field not in df.columns:
-            # msg = "(filter_code) No existe la columna {} en el dataframe de entrada".format(field)
-            msg = app_message.dataprep["nodes"]["filter"]["unknow_column"](node_key, field)
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            return pd.DataFrame(), pd.DataFrame()
-
-        if pd.api.types.is_datetime64_any_dtype(df[field]):
-            value = "'{}'".format(value)
-        if operator == "=":  # Numeric, String
-            if pd.api.types.is_string_dtype(df[field]):
-                value = "'{}'".format(value)
-            str_rule = "df[(df['{}'] == {})]".format(field, value)
-            if not sensitive_case:
-                str_rule = "df[(df['{}'].str.lower() == {}.lower())]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "!=":  # Numeric, String
-            if pd.api.types.is_string_dtype(df[field]):
-                value = "'{}'".format(value)
-            str_rule = "df[(df['{}'] != {})]".format(field, value)
-            if not sensitive_case:
-                str_rule = "df[(df['{}'].str.lower() != {}.lower())]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "<":  # Numeric
-            str_rule = "df[(df['{}'] < {})]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "<=":  # Numeric
-            str_rule = "df[(df['{}'] <= {})]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == ">":  # Numeric
-            str_rule = "df[(df['{}'] > {})]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == ">=":  # Numeric
-            str_rule = "df[(df['{}'] >= {})]".format(field, value)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "is_null":  # Numeric, String
-            df_T = df[df[field].isnull()]
-            self.script.append("df_T = df[df['{}'].isnull()]".format(field))
-        elif operator == "is_not_null":  # Numeric, String
-            df_T = df[df[field].notnull()]
-            self.script.append("df_T = df[df['{}'].notnull()]".format(field))
-        elif operator == "contains":  # String
-            df_T = df[df[field].str.contains(value, case=sensitive_case)]
-            self.script.append("df_T = df[df['{}'].str.contains('{}', case={})]".format(field, value, sensitive_case))
-        elif operator == "does_not_contain":  # String
-            df_T = df[~df[field].str.contains(value, case=sensitive_case)]
-            self.script.append("df_T = df[~df['{}'].str.contains('{}', case={})]".format(field, value, sensitive_case))
-        elif operator == "is_empty":  # String
-            str_rule = "df[(df['{}'] == " ")]".format(field)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "is_not_empty":  # String
-            str_rule = "df[(df['{}'] != " ")]".format(field)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "is_true":  # True
-            str_rule = "df[(df['{}'] == True)]".format(field)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        elif operator == "is_false":  # False
-            str_rule = "df[(df['{}'] == False)]".format(field)
-            df_T = eval(str_rule)
-            self.script.append(f"df_T = {str_rule}")
-        else:
-            msg = app_message.dataprep["filter"]["unknow_operator"](node_key, rule["operator"])
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error", bug_level="error")
-        # Obtengo el complemento (la parte negada de la condición)
-        df_F = df[~df.index.isin(df_T.index)]
-        self.script.append(f"df_F = df[~df.index.isin(df_T.index)]")
-
-        return df_T, df_F
+import importlib
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.utilities import utilities
+
+
+class Filter:
+    def __init__(self):
+        self.script = []
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        if "rule_type" not in settings:
+            msg = app_message.dataprep["nodes"]["filter"]["rules"](node_key)
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            return {"T": pd.DataFrame(), "F": pd.DataFrame()}
+
+        df: pd.DataFrame = pin["In"].copy()
+        df_T, df_F = pd.DataFrame(), pd.DataFrame()
+        
+        # NOTE: en versiones nuevas ya no se usa
+        if settings["rule_type"] == "preconfigured":
+            try:
+                df_T, df_F = self.filter_preconfigured(flow_id, node_key, df, settings)
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+                return {"T": pd.DataFrame(), "F": pd.DataFrame()}
+
+        elif settings["rule_type"] == "code":
+            # Agrego los modulos y alias al entorno de variables globales
+            imports_code: str = settings["imports"] if "imports" in settings and settings["imports"] else ""
+            used_modules = utilities.find_imports(imports_code)
+            for m in used_modules:
+                try:
+                    if m["alias"]:
+                        globals()[m["alias"]] = importlib.import_module(m["name"])
+                    else:
+                        globals().update(importlib.import_module(m["name"]).__dict__)
+                except ModuleNotFoundError as e:
+                    import os
+                    import subprocess
+
+                    current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+                    python_path = os.path.join(current_path, "python", "python")
+                    
+                    if os.path.exists(python_path):
+                        subprocess.run(
+                            [
+                                python_path,
+                                "-m",
+                                "pipenv",
+                                "install",
+                                "--skip-lock",
+                                m["name"].split(".")[0],
+                            ]
+                        )
+                    else:
+                        import pip
+                        pip.main(["install", m["name"].split(".")[0]])
+                        
+                    if m["alias"]:
+                        globals()[m["alias"]] = importlib.import_module(m["name"])
+                    else:
+                        globals().update(importlib.import_module(m["name"]).__dict__)
+                        
+            df_T, df_F = self.filter_code(flow_id, node_key, df, settings["sentence"])
+        else:
+            msg = app_message.dataprep["nodes"]["filter"]["unknow_rule"](node_key, str(settings["rule_type"]))
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
+            
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"T": df_T, "F": df_F},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": self.script,
+            },
+        )
+        script_handler.script += self.script.copy()
+        self.script = []
+        return {"T": df_T, "F": df_F}
+
+    # Nodo: filter - Procesa el filtro de sentencia
+    def filter_code(self, flow_id, node_key, df, sentence):
+        self.script.append("\n# FILTER (CUSTOMIZED)")
+        str_rule = "df[{}]".format(sentence)
+        
+        try:
+            df_T = eval(str_rule)
+            self.script.append("df_T = {}".format(str_rule))
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["filter"]["failed_condition"](node_key)
+            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            return pd.DataFrame(), pd.DataFrame()
+        else:
+            # Obtengo el complemento (la parte negada de la condición)
+            df_F = df[~df.index.isin(df_T.index)]
+            self.script.append("df_F = df[~df.index.isin(df_T.index)]")
+            return df_T, df_F
+
+    # Nodo: filter - Procesa el filtro preconfigurado (Deprecated en neuvas versiones)
+    def filter_preconfigured(self, flow_id, node_key, df: pd.DataFrame, rule):
+        df_T, df_F = pd.DataFrame(), pd.DataFrame()
+        self.script.append("\n# FILTER (PRECONFIGURED)")
+        field: str = rule["field"]
+        operator: str = rule["operator"]
+        value: str = rule["value"] if "value" in rule else '""'
+        sensitive_case: bool = True if pd.api.types.is_string_dtype(df[field]) and "sensitive_case" in rule and rule["sensitive_case"] else False
+        if field not in df.columns:
+            # msg = "(filter_code) No existe la columna {} en el dataframe de entrada".format(field)
+            msg = app_message.dataprep["nodes"]["filter"]["unknow_column"](node_key, field)
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            return pd.DataFrame(), pd.DataFrame()
+
+        if pd.api.types.is_datetime64_any_dtype(df[field]):
+            value = "'{}'".format(value)
+        if operator == "=":  # Numeric, String
+            if pd.api.types.is_string_dtype(df[field]):
+                value = "'{}'".format(value)
+            str_rule = "df[(df['{}'] == {})]".format(field, value)
+            if not sensitive_case:
+                str_rule = "df[(df['{}'].str.lower() == {}.lower())]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "!=":  # Numeric, String
+            if pd.api.types.is_string_dtype(df[field]):
+                value = "'{}'".format(value)
+            str_rule = "df[(df['{}'] != {})]".format(field, value)
+            if not sensitive_case:
+                str_rule = "df[(df['{}'].str.lower() != {}.lower())]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "<":  # Numeric
+            str_rule = "df[(df['{}'] < {})]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "<=":  # Numeric
+            str_rule = "df[(df['{}'] <= {})]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == ">":  # Numeric
+            str_rule = "df[(df['{}'] > {})]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == ">=":  # Numeric
+            str_rule = "df[(df['{}'] >= {})]".format(field, value)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "is_null":  # Numeric, String
+            df_T = df[df[field].isnull()]
+            self.script.append("df_T = df[df['{}'].isnull()]".format(field))
+        elif operator == "is_not_null":  # Numeric, String
+            df_T = df[df[field].notnull()]
+            self.script.append("df_T = df[df['{}'].notnull()]".format(field))
+        elif operator == "contains":  # String
+            df_T = df[df[field].str.contains(value, case=sensitive_case)]
+            self.script.append("df_T = df[df['{}'].str.contains('{}', case={})]".format(field, value, sensitive_case))
+        elif operator == "does_not_contain":  # String
+            df_T = df[~df[field].str.contains(value, case=sensitive_case)]
+            self.script.append("df_T = df[~df['{}'].str.contains('{}', case={})]".format(field, value, sensitive_case))
+        elif operator == "is_empty":  # String
+            str_rule = "df[(df['{}'] == " ")]".format(field)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "is_not_empty":  # String
+            str_rule = "df[(df['{}'] != " ")]".format(field)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "is_true":  # True
+            str_rule = "df[(df['{}'] == True)]".format(field)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        elif operator == "is_false":  # False
+            str_rule = "df[(df['{}'] == False)]".format(field)
+            df_T = eval(str_rule)
+            self.script.append(f"df_T = {str_rule}")
+        else:
+            msg = app_message.dataprep["filter"]["unknow_operator"](node_key, rule["operator"])
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error", bug_level="error")
+        # Obtengo el complemento (la parte negada de la condición)
+        df_F = df[~df.index.isin(df_T.index)]
+        self.script.append(f"df_F = df[~df.index.isin(df_T.index)]")
+
+        return df_T, df_F
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/formula.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/formula.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import importlib
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils.utilities import utilities
-
-
-class Formula:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# FORMULA")
-
-        # Agrego los modulos y alias al entorno de variables globales
-        imports_code: str = settings["imports"] if "imports" in settings and settings["imports"] else ""
-        used_modules = utilities.find_imports(imports_code)
-        for m in used_modules:
-            try:
-                if m["alias"]:
-                    globals()[m["alias"]] = importlib.import_module(m["name"])
-                else:
-                    globals().update(importlib.import_module(m["name"]).__dict__)
-            except ModuleNotFoundError as e:
-                import os
-                import subprocess
-
-                current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
-                python_path = os.path.join(current_path, "python", "python")
-                if os.path.exists(python_path):
-                    subprocess.run(
-                        [
-                            python_path,
-                            "-m",
-                            "pipenv",
-                            "install",
-                            "--skip-lock",
-                            m["name"].split(".")[0],
-                        ]
-                    )
-                else:
-                    import pip
-
-                    pip.main(["install", m["name"].split(".")[0]])
-
-                if m["alias"]:
-                    globals()[m["alias"]] = importlib.import_module(m["name"])
-                else:
-                    globals().update(importlib.import_module(m["name"]).__dict__)
-                    
-        formulas: list = settings["items"] if "items" in settings else []
-
-        for i, item in enumerate(formulas):
-            col_name: str = ""
-            if not item["field"]:  # crea una columna nueva
-                col_name = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else f"x_{i}"
-            else:  # actualiza la misma columna seleccionada
-                col_name = item["field"]
-                
-            if "sentence" not in item:
-                continue
-
-            try:
-                df = df.copy()  # con esto evito los warning
-                df.loc[:, col_name] = eval(item["sentence"])
-                script.append("df.loc[:, '{}'] = {}".format(col_name, item["sentence"]))
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import importlib
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils.utilities import utilities
+
+
+class Formula:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# FORMULA")
+
+        # Agrego los modulos y alias al entorno de variables globales
+        imports_code: str = settings["imports"] if "imports" in settings and settings["imports"] else ""
+        used_modules = utilities.find_imports(imports_code)
+        for m in used_modules:
+            try:
+                if m["alias"]:
+                    globals()[m["alias"]] = importlib.import_module(m["name"])
+                else:
+                    globals().update(importlib.import_module(m["name"]).__dict__)
+            except ModuleNotFoundError as e:
+                import os
+                import subprocess
+
+                current_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+                python_path = os.path.join(current_path, "python", "python")
+                if os.path.exists(python_path):
+                    subprocess.run(
+                        [
+                            python_path,
+                            "-m",
+                            "pipenv",
+                            "install",
+                            "--skip-lock",
+                            m["name"].split(".")[0],
+                        ]
+                    )
+                else:
+                    import pip
+
+                    pip.main(["install", m["name"].split(".")[0]])
+
+                if m["alias"]:
+                    globals()[m["alias"]] = importlib.import_module(m["name"])
+                else:
+                    globals().update(importlib.import_module(m["name"]).__dict__)
+                    
+        formulas: list = settings["items"] if "items" in settings else []
+
+        for i, item in enumerate(formulas):
+            col_name: str = ""
+            if not item["field"]:  # crea una columna nueva
+                col_name = item["new_column_name"] if "new_column_name" in item and item["new_column_name"] else f"x_{i}"
+            else:  # actualiza la misma columna seleccionada
+                col_name = item["field"]
+                
+            if "sentence" not in item:
+                continue
+
+            try:
+                df = df.copy()  # con esto evito los warning
+                df.loc[:, col_name] = eval(item["sentence"])
+                script.append("df.loc[:, '{}'] = {}".format(col_name, item["sentence"]))
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/input_data.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/input_data.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import json
-import os
-from pathlib import Path
-from urllib.parse import urlparse
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils import normpath
-import requests
-
-
-class InputData:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# INPUT")
-
-        encoding: str = settings["encoding"] if "encoding" in settings else "ISO-8859-1"
-        dtype = str if "as_string" in settings and settings["as_string"] == True else None
-        delimiter: str = settings["delimiter"] if "delimiter" in settings and settings["delimiter"] else None
-        header: str = None if "has_header" in settings and settings["has_header"] == False else "infer"
-        file_path = settings["file_path"] if "file_path" in settings else ""
-        
-        is_external = file_path.startswith("http://") or file_path.startswith("https://")
-        if file_path and not is_external:
-            file_path = normpath(file_path)
-        
-        # !! Deploy mode habilitado
-        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-
-        if deploy_enabled:
-            if "deploy_file_path" not in settings or not settings["deploy_file_path"]:
-                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-            file_path = settings["deploy_file_path"] if "deploy_file_path" in settings else ""
-            
-            is_external = file_path.startswith("http://") or file_path.startswith("https://")
-            if file_path and not is_external:
-                file_path = normpath(file_path)
-            
-        
-        if not is_external:
-            # * check file exists
-            file_exists = os.path.exists(file_path)
-            
-            if not file_exists:
-                msg = app_message.dataprep["nodes"]["input_data"]["file_not_exist"](node_key, file_path)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-            # * get file extension
-            _, file_ext = os.path.splitext(file_path)
-            file_ext = file_ext[1:]
-            
-        else:
-            # * check if url exist
-            resp = requests.get(file_path)
-            if resp.status_code not in range(200, 300):
-                msg = app_message.dataprep["nodes"]["input_data"]["url_not_valid"](node_key, file_path)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-            # * get file extension from node config
-            file_ext = settings["extension"] if "extension" in settings else ""
-            if deploy_enabled:
-                file_ext = settings["deploy_extension"] if "deploy_extension" in settings else ""
-                
-            # * si la ext no existe en la config, intentar extraer del nombre del archivo
-            if not file_ext:
-                url_path = urlparse(file_path)
-                _, file_ext = os.path.splitext(Path(url_path.path))
-                file_ext = file_ext[1:]
-                
-            # * Error si no es posible extraer la extension dela archivo
-            if not file_ext:
-                msg = app_message.dataprep["nodes"]["input_data"]["missing_extension"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        try:
-            bug_handler.console('Leyendo fuente "{}"...'.format(file_path), "trace", flow_id)
-            if file_ext in ["csv", "txt"]:
-                df = pd.read_csv(
-                    file_path,
-                    dtype=dtype,
-                    encoding=encoding,
-                    delimiter=delimiter,
-                    header=header,
-                )
-                dtype_str = 'str' if dtype != None else None
-                header_str = f"'{header}'" if header else None
-                
-                script.append(f"df = pd.read_csv('{file_path}', dtype={dtype_str}, encoding='{encoding}', delimiter='{delimiter}', header={header_str})")
-                
-                # add prefix to df columns
-                if header is None:
-                    df.columns = [f"col_{name}" for name in df.columns]
-                    script.append('df.columns = [f"col_{name}" for name in df.columns]')
-                    
-                
-            elif file_ext == "json":
-                orient = settings["orient"] if "orient" in settings else "columns"
-                df = pd.read_json(file_path, orient=orient, encoding=encoding)
-                script.append(f"df = pd.read_json('{file_path}', orient='{orient}', encoding='{encoding}')")
-                
-            elif file_ext in ["xls", "xlsx", "xlsm", "xlsb"]:
-                sheet_name = settings["sheet_name"] if "sheet_name" in settings else 0
-                
-                df = pd.read_excel(file_path, dtype=dtype, sheet_name=sheet_name, engine=None)
-                dtype_str = 'str' if dtype != None else None
-                script.append(f"df = pd.read_excel('{file_path}', dtype={dtype_str}, sheet_name='{sheet_name}')")
-                
-            else:
-                msg = app_message.dataprep["nodes"]["input_data"]["unknow_format"](node_key, file_ext)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            df.columns = [str(c) for c in df.columns]
-
-            # revisar si algun nombre de columna tiene espacio al inicio o al final
-            if True in [c.startswith((" ", "\t")) or c.endswith((" ", "\t")) for c in df.columns]:
-                df.columns = [c.strip() for c in df.columns]
-                msg = app_message.dataprep["nodes"]["input_data"]["end_start_spaces"](node_key)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+import os
+from pathlib import Path
+from urllib.parse import urlparse
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils import normpath
+import requests
+
+
+class InputData:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# INPUT")
+
+        encoding: str = settings["encoding"] if "encoding" in settings else "ISO-8859-1"
+        dtype = str if "as_string" in settings and settings["as_string"] == True else None
+        delimiter: str = settings["delimiter"] if "delimiter" in settings and settings["delimiter"] else None
+        header: str = None if "has_header" in settings and settings["has_header"] == False else "infer"
+        file_path = settings["file_path"] if "file_path" in settings else ""
+        
+        is_external = file_path.startswith("http://") or file_path.startswith("https://")
+        if file_path and not is_external:
+            file_path = normpath(file_path)
+        
+        # !! Deploy mode habilitado
+        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+
+        if deploy_enabled:
+            if "deploy_file_path" not in settings or not settings["deploy_file_path"]:
+                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+            file_path = settings["deploy_file_path"] if "deploy_file_path" in settings else ""
+            
+            is_external = file_path.startswith("http://") or file_path.startswith("https://")
+            if file_path and not is_external:
+                file_path = normpath(file_path)
+            
+        
+        if not is_external:
+            # * check file exists
+            file_exists = os.path.exists(file_path)
+            
+            if not file_exists:
+                msg = app_message.dataprep["nodes"]["input_data"]["file_not_exist"](node_key, file_path)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+            # * get file extension
+            _, file_ext = os.path.splitext(file_path)
+            file_ext = file_ext[1:]
+            
+        else:
+            # * check if url exist
+            resp = requests.get(file_path)
+            if resp.status_code not in range(200, 300):
+                msg = app_message.dataprep["nodes"]["input_data"]["url_not_valid"](node_key, file_path)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+            # * get file extension from node config
+            file_ext = settings["extension"] if "extension" in settings else ""
+            if deploy_enabled:
+                file_ext = settings["deploy_extension"] if "deploy_extension" in settings else ""
+                
+            # * si la ext no existe en la config, intentar extraer del nombre del archivo
+            if not file_ext:
+                url_path = urlparse(file_path)
+                _, file_ext = os.path.splitext(Path(url_path.path))
+                file_ext = file_ext[1:]
+                
+            # * Error si no es posible extraer la extension dela archivo
+            if not file_ext:
+                msg = app_message.dataprep["nodes"]["input_data"]["missing_extension"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        try:
+            bug_handler.console('Leyendo fuente "{}"...'.format(file_path), "trace", flow_id)
+            if file_ext in ["csv", "txt"]:
+                df = pd.read_csv(
+                    file_path,
+                    dtype=dtype,
+                    encoding=encoding,
+                    delimiter=delimiter,
+                    header=header,
+                )
+                dtype_str = 'str' if dtype != None else None
+                header_str = f"'{header}'" if header else None
+                
+                script.append(f"df = pd.read_csv('{file_path}', dtype={dtype_str}, encoding='{encoding}', delimiter='{delimiter}', header={header_str})")
+                
+                # add prefix to df columns
+                if header is None:
+                    df.columns = [f"col_{name}" for name in df.columns]
+                    script.append('df.columns = [f"col_{name}" for name in df.columns]')
+                    
+                
+            elif file_ext == "json":
+                orient = settings["orient"] if "orient" in settings else "columns"
+                df = pd.read_json(file_path, orient=orient, encoding=encoding)
+                script.append(f"df = pd.read_json('{file_path}', orient='{orient}', encoding='{encoding}')")
+                
+            elif file_ext in ["xls", "xlsx", "xlsm", "xlsb"]:
+                sheet_name = settings["sheet_name"] if "sheet_name" in settings else 0
+                
+                df = pd.read_excel(file_path, dtype=dtype, sheet_name=sheet_name, engine=None)
+                dtype_str = 'str' if dtype != None else None
+                script.append(f"df = pd.read_excel('{file_path}', dtype={dtype_str}, sheet_name='{sheet_name}')")
+                
+            else:
+                msg = app_message.dataprep["nodes"]["input_data"]["unknow_format"](node_key, file_ext)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+            df.columns = [str(c) for c in df.columns]
+
+            # revisar si algun nombre de columna tiene espacio al inicio o al final
+            if True in [c.startswith((" ", "\t")) or c.endswith((" ", "\t")) for c in df.columns]:
+                df.columns = [c.strip() for c in df.columns]
+                msg = app_message.dataprep["nodes"]["input_data"]["end_start_spaces"](node_key)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="warn", bug_level="warning")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/inter_row.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/inter_row.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class InterRow:
-    def __init__(self):
-        self.map_timedelta = {
-            "days": "D",
-            "hours": "H",
-            "minutes": "m",
-            "seconds": "s",
-        }
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# InterRow")
-
-        # group_by, field, new_column_name, periods, fillna, fillna_value, fillna_value_timedelta
-        groupby: list = settings["group_by"] if ("group_by" in settings and settings["group_by"]) else []
-        field: str = settings["field"] if "field" in settings and settings["field"] else None
-        new_column_name: str = settings["new_column_name"] if "new_column_name" in settings and settings["new_column_name"] else "new_column"
-        periods: int = settings["periods"] if ("periods" in settings and settings["periods"]) else 0  # pyright: ignore
-        inter_row_type: str = settings["inter_row_type"] if "inter_row_type" in settings and settings["inter_row_type"] else None
-        fillna: bool = settings["fillna"] if "fillna" in settings else False
-        fillna_value: str | int = settings["fillna_value"] if "fillna_value" in settings else None
-        fillna_value_timedelta = settings["fillna_value_timedelta"] if ("fillna_value_timedelta" in settings and settings["fillna_value_timedelta"] != {}) else {}
-
-        if not field or (fillna and (not fillna_value and not fillna_value_timedelta)):
-            if not field:
-                msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            if fillna and (not fillna_value and not fillna_value_timedelta):
-                msg = app_message.dataprep["nodes"]["inter_row"]["fillna"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            query = ""
-            if groupby:
-                if fillna:
-                    if fillna_value:
-                        query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods).fillna(fillna_value)"
-                        df[new_column_name] = eval(query)
-                    else:
-                        query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods).fillna(self.timedelta_parse(fillna_value_timedelta))"
-                        df[new_column_name] = eval(query)
-                else:
-                    query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods)"
-                    df[new_column_name] = eval(query)
-            else:
-                if fillna:
-                    if fillna_value:
-                        query = f"df[[field]].{inter_row_type}(periods).fillna(fillna_value)"
-                        df[new_column_name] = eval(query)
-                    else:
-                        query = f"df[[field]].{inter_row_type}(periods).fillna(self.timedelta_parse(fillna_value_timedelta))"
-                        df[new_column_name] = eval(query)
-                else:
-                    query = f"df[field].{inter_row_type}(periods)"
-                    df[new_column_name] = eval(query)
-
-            script.append(f"df[{new_column_name}] = {query}")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
-
-    def timedelta_parse(self, timedelta_data):
-        return " ".join([str(value) + " " + key for key, value in timedelta_data.items()])
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class InterRow:
+    def __init__(self):
+        self.map_timedelta = {
+            "days": "D",
+            "hours": "H",
+            "minutes": "m",
+            "seconds": "s",
+        }
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# InterRow")
+
+        # group_by, field, new_column_name, periods, fillna, fillna_value, fillna_value_timedelta
+        groupby: list = settings["group_by"] if ("group_by" in settings and settings["group_by"]) else []
+        field: str = settings["field"] if "field" in settings and settings["field"] else None
+        new_column_name: str = settings["new_column_name"] if "new_column_name" in settings and settings["new_column_name"] else "new_column"
+        periods: int = settings["periods"] if ("periods" in settings and settings["periods"]) else 0  # pyright: ignore
+        inter_row_type: str = settings["inter_row_type"] if "inter_row_type" in settings and settings["inter_row_type"] else None
+        fillna: bool = settings["fillna"] if "fillna" in settings else False
+        fillna_value: str | int = settings["fillna_value"] if "fillna_value" in settings else None
+        fillna_value_timedelta = settings["fillna_value_timedelta"] if ("fillna_value_timedelta" in settings and settings["fillna_value_timedelta"] != {}) else {}
+
+        if not field or (fillna and (not fillna_value and not fillna_value_timedelta)):
+            if not field:
+                msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            if fillna and (not fillna_value and not fillna_value_timedelta):
+                msg = app_message.dataprep["nodes"]["inter_row"]["fillna"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            query = ""
+            if groupby:
+                if fillna:
+                    if fillna_value:
+                        query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods).fillna(fillna_value)"
+                        df[new_column_name] = eval(query)
+                    else:
+                        query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods).fillna(self.timedelta_parse(fillna_value_timedelta))"
+                        df[new_column_name] = eval(query)
+                else:
+                    query = f"df.groupby(by=groupby)[[field]].{inter_row_type}(periods)"
+                    df[new_column_name] = eval(query)
+            else:
+                if fillna:
+                    if fillna_value:
+                        query = f"df[[field]].{inter_row_type}(periods).fillna(fillna_value)"
+                        df[new_column_name] = eval(query)
+                    else:
+                        query = f"df[[field]].{inter_row_type}(periods).fillna(self.timedelta_parse(fillna_value_timedelta))"
+                        df[new_column_name] = eval(query)
+                else:
+                    query = f"df[field].{inter_row_type}(periods)"
+                    df[new_column_name] = eval(query)
+
+            script.append(f"df[{new_column_name}] = {query}")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
+
+    def timedelta_parse(self, timedelta_data):
+        return " ".join([str(value) + " " + key for key, value in timedelta_data.items()])
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/isin.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/isin.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class IsIn:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# IS_IN")
-
-        # Validar que exista df de entrada en el puerto Src
-        if "Src" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Src")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            
-        # Validar que exista df de entrada en el puerto Val
-        if "Val" not in pin:
-            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Val")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        df_S: pd.DataFrame = pin["Src"].copy() if "Src" in pin else pd.DataFrame()
-        df_V: pd.DataFrame = pin["Val"].copy() if "Val" in pin else pd.DataFrame()
-        
-        source: str = settings["source"] if "source" in settings and settings["source"] else None
-        values: str = settings["values"] if "values" in settings and settings["values"] else None
-        
-        if not source:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, 'Source')
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not values:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, 'Values')
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        try:
-            if "not_in" in settings and settings["not_in"]:
-                df = df_S[~df_S[source].isin(df_V[values])].reset_index(drop=True)
-                script.append("df = df[~df_S[{}].isin(df_V[{}])].reset_index(drop=True)".format(source, values))
-            else:
-                df = df_S[df_S[source].isin(df_V[values])].reset_index(drop=True)
-                script.append("df = df[df_S[{}].isin(df_V[{}])].reset_index(drop=True)".format(source, values))
-            
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class IsIn:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# IS_IN")
+
+        # Validar que exista df de entrada en el puerto Src
+        if "Src" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Src")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+        # Validar que exista df de entrada en el puerto Val
+        if "Val" not in pin:
+            msg = app_message.dataprep["nodes"]["missing_df"](node_key, "Val")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        df_S: pd.DataFrame = pin["Src"].copy() if "Src" in pin else pd.DataFrame()
+        df_V: pd.DataFrame = pin["Val"].copy() if "Val" in pin else pd.DataFrame()
+        
+        source: str = settings["source"] if "source" in settings and settings["source"] else None
+        values: str = settings["values"] if "values" in settings and settings["values"] else None
+        
+        if not source:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, 'Source')
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not values:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, 'Values')
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        try:
+            if "not_in" in settings and settings["not_in"]:
+                df = df_S[~df_S[source].isin(df_V[values])].reset_index(drop=True)
+                script.append("df = df[~df_S[{}].isin(df_V[{}])].reset_index(drop=True)".format(source, values))
+            else:
+                df = df_S[df_S[source].isin(df_V[values])].reset_index(drop=True)
+                script.append("df = df[df_S[{}].isin(df_V[{}])].reset_index(drop=True)".format(source, values))
+            
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/melt.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/sort.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Melt:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# MELT")
-
-        # Obtengo las configuraciones
-        id_vars: list[str] = settings["id_vars"] if "id_vars" in settings and settings["id_vars"] else []
-        value_vars: list[str] = settings["value_vars"] if "value_vars" in settings and settings["value_vars"] else []
-        
-        if not value_vars:
-            msg = app_message.dataprep["nodes"]["empty_list"](node_key, "Value Fields")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="ERROR")
-
-        # Transpone multiples columnas dejandolas en una sola columna con variables categoricas
-        try:
-            df = pd.melt(df, id_vars=id_vars, value_vars=value_vars).reset_index(drop=True)
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        script.append("df = pd.melt(df, id_vars={}, value_vars={}).reset_index(drop=True)".format(id_vars, value_vars))
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Sort:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# SORT")
+
+        sorts = settings["items"] if "items" in settings and settings["items"] else []
+
+        if sorts:
+            setting_list = list(
+                map(
+                    lambda x: (x["field"], int(x["ascending"])),
+                    [item for item in sorts if "field" in item and item["field"]],
+                )
+            )
+            if setting_list:
+                columns, order = zip(*setting_list)
+            else:
+                msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        else:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            df = df.sort_values(by=list(columns), ascending=list(order))
+            script.append("df_{} = df.sort_values(by=list({}), ascending=list({}))".format(node_key, columns, order))
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/merge.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/merge.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Merge:
-    def __init__(self):
-        self.script = []
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        edf = pd.DataFrame()
-        pout_struct = {"L": edf, "J": edf, "R": edf, "F": edf}
-
-        if "iL" not in pin or "iR" not in pin:
-            msg = app_message.dataprep["nodes"]["merge"]["input_port"](node_key)
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            return pout_struct
-
-        self.script.append("\n# MERGE")
-
-        # * Columnas de salida
-        left_columns: list[str] = settings["left_columns"] if "left_columns" in settings else []
-        right_columns: list[str] = settings["right_columns"] if "right_columns" in settings else []
-
-        # * Dataframes de entrada
-        df_iL: pd.DataFrame = pin["iL"].copy() if "iL" in pin else pd.DataFrame()
-        df_iR: pd.DataFrame = pin["iR"].copy() if "iR" in pin else pd.DataFrame()
-
-        # * Validar que array de columnas de salida exista en su respectivo DF
-        for col in left_columns:
-            if col not in df_iL.columns.tolist():
-                msg = app_message.dataprep["nodes"]["merge"]["input_port_il"](node_key, col)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-                return pout_struct
-
-        for col in right_columns:
-            if col not in df_iR.columns.tolist():
-                msg = app_message.dataprep["nodes"]["merge"]["input_port_iR"](node_key, col)
-                bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-                return pout_struct
-
-        try:
-            df_iL: pd.DataFrame = df_iL[left_columns].copy()
-            df_iR: pd.DataFrame = df_iR[right_columns].copy()
-
-            on_l: list[str] = [x["left"] for x in settings["items"] if "left" in x and x["left"]]
-            on_r: list[str] = [x["right"] for x in settings["items"] if "right" in x and x["right"]]
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            return pout_struct
-
-        if "L" in settings["outputs"]:
-            pout_struct["L"] = self.apply_join(flow_id, node_key, "left", df_iL, df_iR, on_l, on_r)
-        if "J" in settings["outputs"]:
-            pout_struct["J"] = self.apply_join(flow_id, node_key, "inner", df_iL, df_iR, on_l, on_r)
-        if "R" in settings["outputs"]:
-            pout_struct["R"] = self.apply_join(flow_id, node_key, "right", df_iL, df_iR, on_l, on_r)
-        if "F" in settings["outputs"]:
-            pout_struct["F"] = self.apply_join(flow_id, node_key, "outer", df_iL, df_iR, on_l, on_r)
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": pout_struct,
-                "config": json.dumps(settings, sort_keys=True),
-                "script": self.script,
-            },
-        )
-
-        script_handler.script += self.script
-        return pout_struct
-
-    def apply_join(self, flow_id, node_key, how, df_iL, df_iR, on_l, on_r):
-        try:
-            if how == "outer":
-                df_o = pd.merge(
-                    df_iL,
-                    df_iR,
-                    left_on=on_l,
-                    right_on=on_r,
-                    how="outer",
-                    indicator=True,
-                )
-                # Campo _merge viene como category, lo cambio a object (str)
-                df_o["merge_type"] = df_o["_merge"].astype(str)
-                del df_o["_merge"]
-                self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='outer', indicator=True)".format(on_l, on_r))
-            else:
-                df_o = pd.merge(df_iL, df_iR, left_on=on_l, right_on=on_r, how=how)
-                self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='{}', indicator=True)".format(on_l, on_r, how))
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-            return pd.DataFrame()
-        return df_o
-
-    # def full_outer_join(self, flow_id, node_key, df_iL, df_iR, on_l, on_r):
-    # 	try:
-    # 		# Outer join con indicator (que genera la columna merge) para sacar sólo las columnas de lado correspondiente
-    # 		df_o = pd.merge(df_iL, df_iR, left_on=on_l, right_on=on_r, how="outer", indicator=True)#, validate="many_to_one")
-    # 		self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='outer', indicator=True)".format(on_l, on_r))
-    # 	except Exception as e:
-    # 		msg = '(merge) Exception:' + str(e)
-    # 		bug_handler.console(msg, 'fatal', flow_id)
-    # 		bug_handler.append({'flow_id': flow_id, 'success': False, 'node_key': node_key, 'level': 'error', 'msg': msg, 'exception': str(e)})
-    # 		edf = pd.DataFrame()
-    # 		return {'L': edf, 'J': edf, 'R': edf, 'F': edf}
-
-    # 	# print('J',df_iL.shape, df_iR.shape)
-    # 	df_l = df_o[df_o['_merge'].isin(['left_only', 'both'])].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
-    # 	df_j = df_o[df_o['_merge'] == 'both'].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
-    # 	df_r = df_o[df_o['_merge'].isin(['right_only', 'both'])].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
-
-    # 	self.script.append("df_l = df_o[df_o['_merge'] == 'left_only'].drop(columns=['_merge'], axis=1)")
-    # 	self.script.append("df_j = df_o[df_o['_merge'] == 'both'].drop(columns=['_merge'], axis=1)")
-    # 	self.script.append("df_r = df_o[df_o['_merge'] == 'right_only'].drop(columns=['_merge'], axis=1)")
-
-    # 	df_o['_merge'] = df_o['_merge'].astype(str) # campo _merge viene como category, lo cambio a object (str)
-    # 	# df_o.rename(columns={'_merge': 'merge'}, inplace=True)
-    # 	# print(df_j.head())
-
-    # 	return {'L': df_l, 'J': df_j, 'R': df_r, 'F': df_o}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Merge:
+    def __init__(self):
+        self.script = []
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        edf = pd.DataFrame()
+        pout_struct = {"L": edf, "J": edf, "R": edf, "F": edf}
+
+        if "iL" not in pin or "iR" not in pin:
+            msg = app_message.dataprep["nodes"]["merge"]["input_port"](node_key)
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            return pout_struct
+
+        self.script.append("\n# MERGE")
+
+        # * Columnas de salida
+        left_columns: list[str] = settings["left_columns"] if "left_columns" in settings else []
+        right_columns: list[str] = settings["right_columns"] if "right_columns" in settings else []
+
+        # * Dataframes de entrada
+        df_iL: pd.DataFrame = pin["iL"].copy() if "iL" in pin else pd.DataFrame()
+        df_iR: pd.DataFrame = pin["iR"].copy() if "iR" in pin else pd.DataFrame()
+
+        # * Validar que array de columnas de salida exista en su respectivo DF
+        for col in left_columns:
+            if col not in df_iL.columns.tolist():
+                msg = app_message.dataprep["nodes"]["merge"]["input_port_il"](node_key, col)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+                return pout_struct
+
+        for col in right_columns:
+            if col not in df_iR.columns.tolist():
+                msg = app_message.dataprep["nodes"]["merge"]["input_port_iR"](node_key, col)
+                bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+                return pout_struct
+
+        try:
+            df_iL: pd.DataFrame = df_iL[left_columns].copy()
+            df_iR: pd.DataFrame = df_iR[right_columns].copy()
+
+            on_l: list[str] = [x["left"] for x in settings["items"] if "left" in x and x["left"]]
+            on_r: list[str] = [x["right"] for x in settings["items"] if "right" in x and x["right"]]
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            return pout_struct
+
+        if "L" in settings["outputs"]:
+            pout_struct["L"] = self.apply_join(flow_id, node_key, "left", df_iL, df_iR, on_l, on_r)
+        if "J" in settings["outputs"]:
+            pout_struct["J"] = self.apply_join(flow_id, node_key, "inner", df_iL, df_iR, on_l, on_r)
+        if "R" in settings["outputs"]:
+            pout_struct["R"] = self.apply_join(flow_id, node_key, "right", df_iL, df_iR, on_l, on_r)
+        if "F" in settings["outputs"]:
+            pout_struct["F"] = self.apply_join(flow_id, node_key, "outer", df_iL, df_iR, on_l, on_r)
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": pout_struct,
+                "config": json.dumps(settings, sort_keys=True),
+                "script": self.script,
+            },
+        )
+
+        script_handler.script += self.script
+        return pout_struct
+
+    def apply_join(self, flow_id, node_key, how, df_iL, df_iR, on_l, on_r):
+        try:
+            if how == "outer":
+                df_o = pd.merge(
+                    df_iL,
+                    df_iR,
+                    left_on=on_l,
+                    right_on=on_r,
+                    how="outer",
+                    indicator=True,
+                )
+                # Campo _merge viene como category, lo cambio a object (str)
+                df_o["merge_type"] = df_o["_merge"].astype(str)
+                del df_o["_merge"]
+                self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='outer', indicator=True)".format(on_l, on_r))
+            else:
+                df_o = pd.merge(df_iL, df_iR, left_on=on_l, right_on=on_r, how=how)
+                self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='{}', indicator=True)".format(on_l, on_r, how))
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+            return pd.DataFrame()
+        return df_o
+
+    # def full_outer_join(self, flow_id, node_key, df_iL, df_iR, on_l, on_r):
+    # 	try:
+    # 		# Outer join con indicator (que genera la columna merge) para sacar sólo las columnas de lado correspondiente
+    # 		df_o = pd.merge(df_iL, df_iR, left_on=on_l, right_on=on_r, how="outer", indicator=True)#, validate="many_to_one")
+    # 		self.script.append("df_o = pd.merge(df_iL, df_iR, left_on={}, right_on={}, how='outer', indicator=True)".format(on_l, on_r))
+    # 	except Exception as e:
+    # 		msg = '(merge) Exception:' + str(e)
+    # 		bug_handler.console(msg, 'fatal', flow_id)
+    # 		bug_handler.append({'flow_id': flow_id, 'success': False, 'node_key': node_key, 'level': 'error', 'msg': msg, 'exception': str(e)})
+    # 		edf = pd.DataFrame()
+    # 		return {'L': edf, 'J': edf, 'R': edf, 'F': edf}
+
+    # 	# print('J',df_iL.shape, df_iR.shape)
+    # 	df_l = df_o[df_o['_merge'].isin(['left_only', 'both'])].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
+    # 	df_j = df_o[df_o['_merge'] == 'both'].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
+    # 	df_r = df_o[df_o['_merge'].isin(['right_only', 'both'])].drop(columns=['_merge'], axis=1) # where 1 is the axis number (0 for rows and 1 for columns.)
+
+    # 	self.script.append("df_l = df_o[df_o['_merge'] == 'left_only'].drop(columns=['_merge'], axis=1)")
+    # 	self.script.append("df_j = df_o[df_o['_merge'] == 'both'].drop(columns=['_merge'], axis=1)")
+    # 	self.script.append("df_r = df_o[df_o['_merge'] == 'right_only'].drop(columns=['_merge'], axis=1)")
+
+    # 	df_o['_merge'] = df_o['_merge'].astype(str) # campo _merge viene como category, lo cambio a object (str)
+    # 	# df_o.rename(columns={'_merge': 'merge'}, inplace=True)
+    # 	# print(df_j.head())
+
+    # 	return {'L': df_l, 'J': df_j, 'R': df_r, 'F': df_o}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/output.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/output.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import json
-import os
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils import normpath
-
-
-class Output:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        script.append("\n# OUPUT")
-        output_format: str = settings["format"] or "csv"
-        output_name: str = settings["name"] if "name" in settings else "output"
-        output_path: str = settings["path"] if "path" in settings else ""
-        encoding: str = settings["encoding"] or "UTF-8"
-
-        # * Deploy mode habilitado
-        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
-        if deploy_enabled:
-            if "deploy_path" not in settings:
-                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            output_path = settings["deploy_path"] if "deploy_path" in settings else ""
-
-        df: pd.DataFrame = pin["In"].copy() if "In" in pin else pd.DataFrame()
-        
-        if not output_name:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Output Name")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not output_path:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Folder path")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        try:
-            if output_format == "excel":
-                file_path = output_path + os.path.sep + output_name + ".xlsx"
-                file_path = normpath(file_path)
-                df.to_excel(
-                    file_path,
-                    index=False,
-                    encoding=encoding,
-                )
-                script.append(f"df.to_excel('{file_path}', index=False, encoding='{encoding}')")
-            else:
-                file_path = output_path + os.path.sep + output_name + ".csv"
-                file_path = normpath(file_path)
-                df.to_csv(
-                    file_path,
-                    encoding=encoding,
-                    index=False,
-                )
-                script.append(f"df.to_csv('{file_path}', index=False, encoding='{encoding}')")
-
-        except Exception as e:
-            print("Error (output): ", e)
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-        
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return df
+import json
+import os
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils import normpath
+
+
+class Output:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        script.append("\n# OUPUT")
+        output_format: str = settings["format"] or "csv"
+        output_name: str = settings["name"] if "name" in settings else "output"
+        output_path: str = settings["path"] if "path" in settings else ""
+        encoding: str = settings["encoding"] or "UTF-8"
+
+        # * Deploy mode habilitado
+        deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
+        if deploy_enabled:
+            if "deploy_path" not in settings:
+                msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+            output_path = settings["deploy_path"] if "deploy_path" in settings else ""
+
+        df: pd.DataFrame = pin["In"].copy() if "In" in pin else pd.DataFrame()
+        
+        if not output_name:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Output Name")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not output_path:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Folder path")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        try:
+            if output_format == "excel":
+                file_path = output_path + os.path.sep + output_name + ".xlsx"
+                file_path = normpath(file_path)
+                df.to_excel(
+                    file_path,
+                    index=False,
+                    encoding=encoding,
+                )
+                script.append(f"df.to_excel('{file_path}', index=False, encoding='{encoding}')")
+            else:
+                file_path = output_path + os.path.sep + output_name + ".csv"
+                file_path = normpath(file_path)
+                df.to_csv(
+                    file_path,
+                    encoding=encoding,
+                    index=False,
+                )
+                script.append(f"df.to_csv('{file_path}', index=False, encoding='{encoding}')")
+
+        except Exception as e:
+            print("Error (output): ", e)
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+        
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return df
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/pivot.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/pivot.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Pivot:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# PIVOT")
-
-        # Definición de las funciones de agregación
-        def concat(x, sep):
-            return sep.join(x)
-
-        # missing = list(set(["col_group", "col_header", "col_value", "agg_method"]) - set(settings.keys()))
-
-        # if len(missing) != 0:
-        #     msg = app_message.dataprep["nodes"]["pivot"]["incompleted_fields"](node_key, missing)
-        #     return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        # Obtengo las configuraciones
-        col_group: list[str] = settings["col_group"] if "col_group" in settings and settings["col_group"] else []
-        col_header: str = settings["col_header"] if "col_header" in settings and settings["col_header"] else ""
-        col_value: str = settings["col_value"] if "col_value" in settings and settings["col_value"] else ""
-        agg_method: list[str] = settings["agg_method"] if "agg_method" in settings and settings["agg_method"] else []
-        separator: str = settings["separator"] if "separator" in settings and settings["separator"] else ","
-        remove_prefix: bool = settings["remove_prefix"] if "remove_prefix" in settings else False
-        
-        # * Validar campos obligatorios
-        if not col_group:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Group by")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not col_header:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Header")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not col_value:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Values")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        
-        if not agg_method:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Aggregation Methods")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        agg_fn = []
-        for am in agg_method:
-            if am in ["Concatenate", "Concat"]:
-
-                def lmbd(x):
-                    return concat(x, separator)
-
-                lmbd.__name__ = "concat"
-                agg_fn.append(lmbd)
-            elif am == "Count (Without Nulls)":
-                agg_fn.append(lambda x: len(x.dropna().unique()))
-            elif am == "Count (With Nulls)":
-                agg_fn.append("count")
-            elif am == "Average":
-                agg_fn.append("mean")
-            else:
-                agg_fn.append(am.lower())
-
-        # Pivotea la tabla utilizando los métodos de agregación seleccionados
-        try:
-            df = pd.pivot_table(df, index=col_group, columns=col_header, values=col_value, aggfunc=agg_fn).reset_index()
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        if remove_prefix and len(agg_method) == 1:
-            df.columns = [x[1] if str(x[1]) else str(x[0]) for x in df.columns]
-        else:
-            df.columns = ["_".join(list(map(str, x))) if str(x[1]) else str(x[0]) for x in df.columns]
-
-        script.append("df = pd.pivot_table(df, index={}, columns='{}', values='{}', aggfunc={}).reset_index()".format(col_group, col_header, col_value, agg_fn))
-        script.append('df.columns = ["_".join(list(map(str, x))) if x[1] else x[0] for x in df.columns ]')
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Pivot:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# PIVOT")
+
+        # Definición de las funciones de agregación
+        def concat(x, sep):
+            return sep.join(x)
+
+        # missing = list(set(["col_group", "col_header", "col_value", "agg_method"]) - set(settings.keys()))
+
+        # if len(missing) != 0:
+        #     msg = app_message.dataprep["nodes"]["pivot"]["incompleted_fields"](node_key, missing)
+        #     return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        # Obtengo las configuraciones
+        col_group: list[str] = settings["col_group"] if "col_group" in settings and settings["col_group"] else []
+        col_header: str = settings["col_header"] if "col_header" in settings and settings["col_header"] else ""
+        col_value: str = settings["col_value"] if "col_value" in settings and settings["col_value"] else ""
+        agg_method: list[str] = settings["agg_method"] if "agg_method" in settings and settings["agg_method"] else []
+        separator: str = settings["separator"] if "separator" in settings and settings["separator"] else ","
+        remove_prefix: bool = settings["remove_prefix"] if "remove_prefix" in settings else False
+        
+        # * Validar campos obligatorios
+        if not col_group:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Group by")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not col_header:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Header")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not col_value:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Values")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        
+        if not agg_method:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Aggregation Methods")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        agg_fn = []
+        for am in agg_method:
+            if am in ["Concatenate", "Concat"]:
+
+                def lmbd(x):
+                    return concat(x, separator)
+
+                lmbd.__name__ = "concat"
+                agg_fn.append(lmbd)
+            elif am == "Count (Without Nulls)":
+                agg_fn.append(lambda x: len(x.dropna().unique()))
+            elif am == "Count (With Nulls)":
+                agg_fn.append("count")
+            elif am == "Average":
+                agg_fn.append("mean")
+            else:
+                agg_fn.append(am.lower())
+
+        # Pivotea la tabla utilizando los métodos de agregación seleccionados
+        try:
+            df = pd.pivot_table(df, index=col_group, columns=col_header, values=col_value, aggfunc=agg_fn).reset_index()
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        if remove_prefix and len(agg_method) == 1:
+            df.columns = [x[1] if str(x[1]) else str(x[0]) for x in df.columns]
+        else:
+            df.columns = ["_".join(list(map(str, x))) if str(x[1]) else str(x[0]) for x in df.columns]
+
+        script.append("df = pd.pivot_table(df, index={}, columns='{}', values='{}', aggfunc={}).reset_index()".format(col_group, col_header, col_value, agg_fn))
+        script.append('df.columns = ["_".join(list(map(str, x))) if x[1] else x[0] for x in df.columns ]')
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/rolling.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/rolling.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Rolling:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# ROLLING")
-
-        column: str = settings["column"] if "column" in settings else None
-        window: int = settings["window"] if "window" in settings else 1
-        operation = settings["operation"] if "operation" in settings else None
-
-        if not column:
-            msg = app_message.dataprep["nodes"]["rolling"]["column_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        if not operation:
-            msg = app_message.dataprep["nodes"]["rolling"]["operation_required"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if column and operation:
-            try:
-                obj = df[column].rolling(window=window, min_periods=0, closed="right")
-                script.append(f"obj = df['{column}'].rolling(window={window}, min_periods=0, closed='right')")
-
-                if operation == "sum":
-                    df["rolling"] = obj.sum()
-                    script.append("\n# Sum")
-                    script.append(f'df["rolling"] = obj.sum()')
-                elif operation == "mean":
-                    df["rolling"] = obj.mean()
-                    script.append("\n# Mean")
-                    script.append(f'df["rolling"] = obj.mean()')
-                elif operation == "median":
-                    df["rolling"] = obj.median()
-                    script.append("\n# Median")
-                    script.append(f'df["rolling"] = obj.median()')
-                elif operation == "min":
-                    df["rolling"] = obj.min()
-                    script.append("\n# Min")
-                    script.append(f'df["rolling"] = obj.min()')
-                elif operation == "max":
-                    df["rolling"] = obj.max()
-                    script.append("\n# Max")
-                    script.append(f'df["rolling"] = obj.max()')
-
-            except Exception as e:
-                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
-
-            cache_handler.update_node(
-                flow_id,
-                node_key,
-                {
-                    "pout": {"Out": df},
-                    "config": json.dumps(settings, sort_keys=True),
-                    "script": script,
-                },
-            )
-            script_handler.script += script
-            return {"Out": df}
-        else:
-            msg = app_message.dataprep["nodes"]["rolling"]["properties_not_provided"](node_key) 
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Rolling:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# ROLLING")
+
+        column: str = settings["column"] if "column" in settings else None
+        window: int = settings["window"] if "window" in settings else 1
+        operation = settings["operation"] if "operation" in settings else None
+
+        if not column:
+            msg = app_message.dataprep["nodes"]["rolling"]["column_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not operation:
+            msg = app_message.dataprep["nodes"]["rolling"]["operation_required"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if column and operation:
+            try:
+                obj = df[column].rolling(window=window, min_periods=0, closed="right")
+                script.append(f"obj = df['{column}'].rolling(window={window}, min_periods=0, closed='right')")
+
+                if operation == "sum":
+                    df["rolling"] = obj.sum()
+                    script.append("\n# Sum")
+                    script.append(f'df["rolling"] = obj.sum()')
+                elif operation == "mean":
+                    df["rolling"] = obj.mean()
+                    script.append("\n# Mean")
+                    script.append(f'df["rolling"] = obj.mean()')
+                elif operation == "median":
+                    df["rolling"] = obj.median()
+                    script.append("\n# Median")
+                    script.append(f'df["rolling"] = obj.median()')
+                elif operation == "min":
+                    df["rolling"] = obj.min()
+                    script.append("\n# Min")
+                    script.append(f'df["rolling"] = obj.min()')
+                elif operation == "max":
+                    df["rolling"] = obj.max()
+                    script.append("\n# Max")
+                    script.append(f'df["rolling"] = obj.max()')
+
+            except Exception as e:
+                msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+                return bug_handler.default_node_log(flow_id, node_key, msg, str(e))
+
+            cache_handler.update_node(
+                flow_id,
+                node_key,
+                {
+                    "pout": {"Out": df},
+                    "config": json.dumps(settings, sort_keys=True),
+                    "script": script,
+                },
+            )
+            script_handler.script += script
+            return {"Out": df}
+        else:
+            msg = app_message.dataprep["nodes"]["rolling"]["properties_not_provided"](node_key) 
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/sample.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/sample.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-class Sample:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        df_A: pd.DataFrame = pd.DataFrame()
-        df_B: pd.DataFrame = pd.DataFrame()
-        
-        script.append("\n# SAMPLE")
-
-        random_pct: float = settings["random_pct"] if "random_pct" in settings else 0
-        first_pct: float = settings["first_pct"] if "first_pct" in settings else 0
-        last_pct: float = settings["last_pct"] if "last_pct" in settings else 0
-        random_n: float = settings["random_n"] if "random_n" in settings else 0
-        first_n: float = settings["first_n"] if "first_n" in settings else 0
-        last_n: float = settings["last_n"] if "last_n" in settings else 0        
-        
-        if (isinstance(random_pct, float) or isinstance(random_pct, int)) and random_pct > 0:
-            df_A = df.sample(int(len(df) * random_pct / 100))
-            script.append(f"df_A = df.sample(int(len(df) * {random_pct} / 100))")
-            
-        elif (isinstance(random_n, float) or isinstance(random_n, int)) and random_n > 0:
-            df_A = df.sample(int(random_n))
-            script.append(f"df_A = df.sample(int({random_n}))")
-            
-        elif (isinstance(first_pct, float) or isinstance(first_pct, int)) and first_pct > 0:
-            df_A = df[:(int(len(df) * first_pct / 100))]
-            script.append(f"df_A = df[:(int(len(df) * {first_pct} / 100))]")
-            
-        elif (isinstance(last_pct, float) or isinstance(last_pct, int)) and last_pct > 0:
-            df_A = df[-(int(len(df) * last_pct / 100)):]
-            script.append(f"df_A = df[-(int(len(df) * {last_pct} / 100)):]")
-            
-        elif (isinstance(first_n, float) or isinstance(first_n, int)) and first_n > 0:
-            df_A = df[:int(first_n)]
-            script.append(f"df_A = df[:int({first_n})]")
-            
-        elif (isinstance(last_n, float) or isinstance(last_n, int)) and last_n > 0:
-            df_A = df[-int(last_n):]
-            script.append(f"df_A = df[-int({last_n}):]")
-            
-        else:
-            msg = app_message.dataprep["nodes"]["sample"]["sample_size"](node_key)
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-            return {"A": df_A, "B": df_B}
-        
-        # Obtengo el complemento (la parte negada de la condición)
-        df_B = df[~df.index.isin(df_A.index)]
-        script.append(f"df_B = df[~df.index.isin(df_A.index)]")
-        
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"A": df_A, "B": df_B},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"A": df_A, "B": df_B}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+class Sample:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        df_A: pd.DataFrame = pd.DataFrame()
+        df_B: pd.DataFrame = pd.DataFrame()
+        
+        script.append("\n# SAMPLE")
+
+        random_pct: float = settings["random_pct"] if "random_pct" in settings else 0
+        first_pct: float = settings["first_pct"] if "first_pct" in settings else 0
+        last_pct: float = settings["last_pct"] if "last_pct" in settings else 0
+        random_n: float = settings["random_n"] if "random_n" in settings else 0
+        first_n: float = settings["first_n"] if "first_n" in settings else 0
+        last_n: float = settings["last_n"] if "last_n" in settings else 0        
+        
+        if (isinstance(random_pct, float) or isinstance(random_pct, int)) and random_pct > 0:
+            df_A = df.sample(int(len(df) * random_pct / 100))
+            script.append(f"df_A = df.sample(int(len(df) * {random_pct} / 100))")
+            
+        elif (isinstance(random_n, float) or isinstance(random_n, int)) and random_n > 0:
+            df_A = df.sample(int(random_n))
+            script.append(f"df_A = df.sample(int({random_n}))")
+            
+        elif (isinstance(first_pct, float) or isinstance(first_pct, int)) and first_pct > 0:
+            df_A = df[:(int(len(df) * first_pct / 100))]
+            script.append(f"df_A = df[:(int(len(df) * {first_pct} / 100))]")
+            
+        elif (isinstance(last_pct, float) or isinstance(last_pct, int)) and last_pct > 0:
+            df_A = df[-(int(len(df) * last_pct / 100)):]
+            script.append(f"df_A = df[-(int(len(df) * {last_pct} / 100)):]")
+            
+        elif (isinstance(first_n, float) or isinstance(first_n, int)) and first_n > 0:
+            df_A = df[:int(first_n)]
+            script.append(f"df_A = df[:int({first_n})]")
+            
+        elif (isinstance(last_n, float) or isinstance(last_n, int)) and last_n > 0:
+            df_A = df[-int(last_n):]
+            script.append(f"df_A = df[-int({last_n}):]")
+            
+        else:
+            msg = app_message.dataprep["nodes"]["sample"]["sample_size"](node_key)
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            return {"A": df_A, "B": df_B}
+        
+        # Obtengo el complemento (la parte negada de la condición)
+        df_B = df[~df.index.isin(df_A.index)]
+        script.append(f"df_B = df[~df.index.isin(df_A.index)]")
+        
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"A": df_A, "B": df_B},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"A": df_A, "B": df_B}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/shape.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/shape.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Shape:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# SHAPE")
-
-        try:
-            df = pd.DataFrame([df.shape], columns=["num_rows", "num_columns"])
-            script.append("df_shape = pd.DataFrame([df.shape], columns=['num_rows', 'num_columns'])")
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Shape:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# SHAPE")
+
+        try:
+            df = pd.DataFrame([df.shape], columns=["num_rows", "num_columns"])
+            script.append("df_shape = pd.DataFrame([df.shape], columns=['num_rows', 'num_columns'])")
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/sort.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/unique.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,43 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Sort:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# SORT")
-
-        sorts = settings["items"] if "items" in settings and settings["items"] else []
-
-        if sorts:
-            setting_list = list(
-                map(
-                    lambda x: (x["field"], int(x["ascending"])),
-                    [item for item in sorts if "field" in item and item["field"]],
-                )
-            )
-            if setting_list:
-                columns, order = zip(*setting_list)
-            else:
-                msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-        else:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            df = df.sort_values(by=list(columns), ascending=list(order))
-            script.append("df_{} = df.sort_values(by=list({}), ascending=list({}))".format(node_key, columns, order))
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Unique:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# Unique")
+
+        # field
+        field: list = settings["field"] if "field" in settings and settings["field"] else []
+
+        if not field:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            df = df.groupby(field).size().reset_index().drop(columns=[0])
+            script.append("df = df.groupby({}).size().reset_index().drop(columns=[0])".format(field))
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/split.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/split.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Split:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# SPLIT")
-
-        # field, separator, split_type
-        field: str = settings["field"] if "field" in settings and settings["field"] != "" else None
-        separator: str = settings["separator"] if "separator" in settings and settings["separator"] != "" else None
-        split_type: str = settings["split_type"] if "split_type" in settings and settings["split_type"] != "" else None
-        n_divisions: int = settings["n_divisions"] if "n_divisions" in settings and settings["n_divisions"] > 0 else None
-
-        if not field:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Field")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        if not separator or not split_type:
-            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Separator" if not separator else "Split Type")
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            if split_type == "column":
-                new_cols = df[field].str.split(separator, expand=True, n=n_divisions).fillna("NaN")
-                new_cols.columns = [f"{field}_{i}" for i in range(new_cols.shape[1])]
-                df = pd.concat([df, new_cols], axis=1)
-
-                script.append("new_cols = df['{}'].str.split('{}', expand=True, n={})".format(field, separator, n_divisions))
-                script.append("new_cols.columns = [f'" + field + "_{i}' for i in range(new_cols.shape[1])]")
-                script.append("df = pd.concat([df, new_cols], axis=1)")
-
-            elif split_type == "row":
-                df_split = df[field].str.split(separator, expand=True).stack().reset_index(level=1, drop=True).rename(f"{field}_value_split")
-                df = df.join(df_split).reset_index(drop=True)
-
-                script.append(f"df_split = df['{field}'].str.split('{separator}', expand=True).stack().reset_index(level=1, drop=True).rename('{field}_value_split')")
-                script.append("df = df.join(df_split).reset_index(drop=True)")
-            else:
-                print("Error")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Split:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# SPLIT")
+
+        # field, separator, split_type
+        field: str = settings["field"] if "field" in settings and settings["field"] != "" else None
+        separator: str = settings["separator"] if "separator" in settings and settings["separator"] != "" else None
+        split_type: str = settings["split_type"] if "split_type" in settings and settings["split_type"] != "" else None
+        n_divisions: int = settings["n_divisions"] if "n_divisions" in settings and settings["n_divisions"] > 0 else None
+
+        if not field:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Field")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        if not separator or not split_type:
+            msg = app_message.dataprep["nodes"]["required_prop"](node_key, "Separator" if not separator else "Split Type")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            if split_type == "column":
+                new_cols = df[field].str.split(separator, expand=True, n=n_divisions).fillna("NaN")
+                new_cols.columns = [f"{field}_{i}" for i in range(new_cols.shape[1])]
+                df = pd.concat([df, new_cols], axis=1)
+
+                script.append("new_cols = df['{}'].str.split('{}', expand=True, n={})".format(field, separator, n_divisions))
+                script.append("new_cols.columns = [f'" + field + "_{i}' for i in range(new_cols.shape[1])]")
+                script.append("df = pd.concat([df, new_cols], axis=1)")
+
+            elif split_type == "row":
+                df_split = df[field].str.split(separator, expand=True).stack().reset_index(level=1, drop=True).rename(f"{field}_value_split")
+                df = df.join(df_split).reset_index(drop=True)
+
+                script.append(f"df_split = df['{field}'].str.split('{separator}', expand=True).stack().reset_index(level=1, drop=True).rename('{field}_value_split')")
+                script.append("df = df.join(df_split).reset_index(drop=True)")
+            else:
+                print("Error")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/switch.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/switch.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import json
-
-import numpy as np
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Switch:
-    def __init__(self):
-        # self.functionApply = ["is null", "is not null", "in", "not in"]
-        # self.noValueRequired = ["is empty", "is not empty"]        
-        self.noValueRequired = ['is null', 'is not null', 'is empty', 'is not empty', 'True', 'False']
-
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# SWITCH")
-
-        cases: list = settings["cases"] if "cases" in settings and settings["cases"] else []
-        default_value: str = settings["default_value"] if "default_value" in settings and settings["default_value"] else None
-        default_value_field: str = settings["default_value_field"] if "default_value_field" in settings and settings["default_value_field"] else None
-        new_column: str = settings["new_column"] if "new_column" in settings and settings["new_column"] else "new_column"
-
-        if default_value == None and default_value_field == None:
-            msg = app_message.dataprep["nodes"]["switch"]["default_value"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg)
-
-        try:
-            conditions = []
-            outputs = []
-            script.append("conditions = []")
-            script.append("outputs = []")
-            for caseIdx, case in enumerate(cases):
-                output: str = case["output"] if "output" in case else None
-                output_field: str = case["output_field"] if "output_field" in case else None
-                if not output and not output_field:
-                    msg = app_message.dataprep["nodes"]["switch"]["no_return_value"](node_key, caseIdx + 1)
-                    return bug_handler.default_node_log(flow_id, node_key, msg)
-
-                query = ""
-                case_conditions: list = case["conditions"] if "conditions" in case else []
-                if not case_conditions:
-                    msg = app_message.dataprep["nodes"]["switch"]["no_conditions"](node_key, caseIdx + 1)
-                    return bug_handler.default_node_log(flow_id, node_key, msg)
-
-                for condIdx, condition in enumerate(case_conditions):
-                    rule: str = f" {condition['rule']} " if "rule" in condition else ""
-                    field: str = condition["field"] if "field" in condition and condition["field"] else None
-                    operator: str = condition["operator"] if "operator" in condition and condition["operator"] else None
-
-                    value: str = condition["value"] if "value" in condition else None
-                    value_field: str = condition["value_field"] if "value_field" in condition else None
-
-                    # Validar campos requeridos para la condicion
-                    if condIdx > 0 and not rule:
-                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Rule",  caseIdx + 1, condIdx + 1)
-                        return bug_handler.default_node_log(flow_id, node_key, msg)
-
-                    if not field:
-                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Column",  caseIdx + 1, condIdx + 1)
-                        return bug_handler.default_node_log(flow_id, node_key, msg)
-
-                    if not operator:
-                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Operator",  caseIdx + 1, condIdx + 1)
-                        return bug_handler.default_node_log(flow_id, node_key, msg)
-                    
-                    
-                    # * Operaciones que no requieren value
-                    if operator in self.noValueRequired:
-                        if operator == "is null":
-                            value = f"pd.isnull(df['{field}'])"
-                                
-                        elif operator == "is not null":
-                            value = f"pd.notnull(df['{field}'])"
-                            
-                        elif "empty" in operator:
-                            value = f'df["{field}"] == ""' if operator == "is empty" else f'df["{field}"] != ""'
-                            
-                        # TODO: Revisar casos bools
-                        elif operator == "True":
-                            value = f'df["{field}"] == True'
-                        elif operator == "False":
-                            value = f'df["{field}"] == False'
-                            
-                        query += f"{rule}{value}"
-                        
-                    # * Operaciones que REQUIEREN value o value_field
-                    else:
-                        # * Validar value y value_field para los operadores que lo requieren
-                        if (value == None or value == "") and (value_field == None or value_field == ""):
-                            msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Value",  caseIdx + 1, condIdx + 1)
-                            return bug_handler.default_node_log(flow_id, node_key, msg)
-                        
-                        # * si existe value
-                        if value != None and value != "":
-                            if operator == "in":
-                                # TODO: Hay que quitar los astype cuando se solucione el problema en el dtypes al pasar a string
-                                df[field] = df[field].astype(str)
-                                value = f"df['{field}'].str.contains('{value}')"
-                                query += f"{rule}{value}"
-                                
-                            elif operator == "not in":
-                                # TODO: Hay que quitar los astype cuando se solucione el problema en el dtypes al pasar a string
-                                df[field] = df[field].astype(str)
-                                value = f"~df['{field}'].str.contains('{value}')"
-                                query += f"{rule}{value}"
-                                
-                            else:
-                                # ? Agregar comillas si el tipo de la columna es string o datetime
-                                value = " '{}'".format(value) if pd.api.types.is_string_dtype(df[field]) or pd.api.types.is_datetime64_any_dtype(df[field]) else value
-                                query += f"{rule}df['{field}'] {operator} {value}"
-                                
-                        # * si existe value_field
-                        else:
-                            if not value_field or value_field not in df.columns:
-                                msg = app_message.dataprep["nodes"]["switch"]["no_column_in_df"](node_key, value_field)
-                                return bug_handler.default_node_log(flow_id, node_key, msg)
-
-                            query += f"{rule}df['{field}'] {operator} df['{value_field}']"
-
-                output_new = output if output else df[output_field]
-                outputs.append(output_new)
-                script.append(f"outputs.append({output_new})")
-                conditions.append(pd.eval(query))
-                script.append(f'conditions.append(pd.eval("{query}"))')
-
-            df[new_column] = np.select(conditions, outputs, default=default_value if default_value else df[default_value_field])
-
-            try:
-                df[new_column] = pd.to_numeric(df[new_column])
-            except Exception as e:
-                print(new_column, e)
-
-            default_value_new = "'" + default_value + "'" if default_value else "df['" + default_value_field + "']"
-            script.append(f'df["{new_column}"] = np.select(conditions, outputs, default={default_value_new})')
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import numpy as np
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Switch:
+    def __init__(self):
+        # self.functionApply = ["is null", "is not null", "in", "not in"]
+        # self.noValueRequired = ["is empty", "is not empty"]        
+        self.noValueRequired = ['is null', 'is not null', 'is empty', 'is not empty', 'True', 'False']
+
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# SWITCH")
+
+        cases: list = settings["cases"] if "cases" in settings and settings["cases"] else []
+        default_value: str = settings["default_value"] if "default_value" in settings and settings["default_value"] else None
+        default_value_field: str = settings["default_value_field"] if "default_value_field" in settings and settings["default_value_field"] else None
+        new_column: str = settings["new_column"] if "new_column" in settings and settings["new_column"] else "new_column"
+
+        if default_value == None and default_value_field == None:
+            msg = app_message.dataprep["nodes"]["switch"]["default_value"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg)
+
+        try:
+            conditions = []
+            outputs = []
+            script.append("conditions = []")
+            script.append("outputs = []")
+            for caseIdx, case in enumerate(cases):
+                output: str = case["output"] if "output" in case else None
+                output_field: str = case["output_field"] if "output_field" in case else None
+                if not output and not output_field:
+                    msg = app_message.dataprep["nodes"]["switch"]["no_return_value"](node_key, caseIdx + 1)
+                    return bug_handler.default_node_log(flow_id, node_key, msg)
+
+                query = ""
+                case_conditions: list = case["conditions"] if "conditions" in case else []
+                if not case_conditions:
+                    msg = app_message.dataprep["nodes"]["switch"]["no_conditions"](node_key, caseIdx + 1)
+                    return bug_handler.default_node_log(flow_id, node_key, msg)
+
+                for condIdx, condition in enumerate(case_conditions):
+                    rule: str = f" {condition['rule']} " if "rule" in condition else ""
+                    field: str = condition["field"] if "field" in condition and condition["field"] else None
+                    operator: str = condition["operator"] if "operator" in condition and condition["operator"] else None
+
+                    value: str = condition["value"] if "value" in condition else None
+                    value_field: str = condition["value_field"] if "value_field" in condition else None
+
+                    # Validar campos requeridos para la condicion
+                    if condIdx > 0 and not rule:
+                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Rule",  caseIdx + 1, condIdx + 1)
+                        return bug_handler.default_node_log(flow_id, node_key, msg)
+
+                    if not field:
+                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Column",  caseIdx + 1, condIdx + 1)
+                        return bug_handler.default_node_log(flow_id, node_key, msg)
+
+                    if not operator:
+                        msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Operator",  caseIdx + 1, condIdx + 1)
+                        return bug_handler.default_node_log(flow_id, node_key, msg)
+                    
+                    
+                    # * Operaciones que no requieren value
+                    if operator in self.noValueRequired:
+                        if operator == "is null":
+                            value = f"pd.isnull(df['{field}'])"
+                                
+                        elif operator == "is not null":
+                            value = f"pd.notnull(df['{field}'])"
+                            
+                        elif "empty" in operator:
+                            value = f'df["{field}"] == ""' if operator == "is empty" else f'df["{field}"] != ""'
+                            
+                        # TODO: Revisar casos bools
+                        elif operator == "True":
+                            value = f'df["{field}"] == True'
+                        elif operator == "False":
+                            value = f'df["{field}"] == False'
+                            
+                        query += f"{rule}{value}"
+                        
+                    # * Operaciones que REQUIEREN value o value_field
+                    else:
+                        # * Validar value y value_field para los operadores que lo requieren
+                        if (value == None or value == "") and (value_field == None or value_field == ""):
+                            msg = app_message.dataprep["nodes"]["switch"]["missing_condition_prop"](node_key, "Value",  caseIdx + 1, condIdx + 1)
+                            return bug_handler.default_node_log(flow_id, node_key, msg)
+                        
+                        # * si existe value
+                        if value != None and value != "":
+                            if operator == "in":
+                                # TODO: Hay que quitar los astype cuando se solucione el problema en el dtypes al pasar a string
+                                df[field] = df[field].astype(str)
+                                value = f"df['{field}'].str.contains('{value}')"
+                                query += f"{rule}{value}"
+                                
+                            elif operator == "not in":
+                                # TODO: Hay que quitar los astype cuando se solucione el problema en el dtypes al pasar a string
+                                df[field] = df[field].astype(str)
+                                value = f"~df['{field}'].str.contains('{value}')"
+                                query += f"{rule}{value}"
+                                
+                            else:
+                                # ? Agregar comillas si el tipo de la columna es string o datetime
+                                value = " '{}'".format(value) if pd.api.types.is_string_dtype(df[field]) or pd.api.types.is_datetime64_any_dtype(df[field]) else value
+                                query += f"{rule}df['{field}'] {operator} {value}"
+                                
+                        # * si existe value_field
+                        else:
+                            if not value_field or value_field not in df.columns:
+                                msg = app_message.dataprep["nodes"]["switch"]["no_column_in_df"](node_key, value_field)
+                                return bug_handler.default_node_log(flow_id, node_key, msg)
+
+                            query += f"{rule}df['{field}'] {operator} df['{value_field}']"
+
+                output_new = output if output else df[output_field]
+                outputs.append(output_new)
+                script.append(f"outputs.append({output_new})")
+                conditions.append(pd.eval(query))
+                script.append(f'conditions.append(pd.eval("{query}"))')
+
+            df[new_column] = np.select(conditions, outputs, default=default_value if default_value else df[default_value_field])
+
+            try:
+                df[new_column] = pd.to_numeric(df[new_column])
+            except Exception as e:
+                print(new_column, e)
+
+            default_value_new = "'" + default_value + "'" if default_value else "df['" + default_value_field + "']"
+            script.append(f'df["{new_column}"] = np.select(conditions, outputs, default={default_value_new})')
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/unique.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/melt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class Unique:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# Unique")
-
-        # field
-        field: list = settings["field"] if "field" in settings and settings["field"] else []
-
-        if not field:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            df = df.groupby(field).size().reset_index().drop(columns=[0])
-            script.append("df = df.groupby({}).size().reset_index().drop(columns=[0])".format(field))
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class Melt:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# MELT")
+
+        # Obtengo las configuraciones
+        id_vars: list[str] = settings["id_vars"] if "id_vars" in settings and settings["id_vars"] else []
+        value_vars: list[str] = settings["value_vars"] if "value_vars" in settings and settings["value_vars"] else []
+        
+        if not value_vars:
+            msg = app_message.dataprep["nodes"]["empty_list"](node_key, "Value Fields")
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="ERROR")
+
+        # Transpone multiples columnas dejandolas en una sola columna con variables categoricas
+        try:
+            df = pd.melt(df, id_vars=id_vars, value_vars=value_vars).reset_index(drop=True)
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        script.append("df = pd.melt(df, id_vars={}, value_vars={}).reset_index(drop=True)".format(id_vars, value_vars))
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/nodes/value_counts.py` & `vtarget-0.8.7/vtarget/dataprep/nodes/value_counts.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import json
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.handlers.script_handler import script_handler
-from vtarget.language.app_message import app_message
-
-
-class ValueCounts:
-    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
-        script = []
-        df: pd.DataFrame = pin["In"].copy()
-        script.append("\n# VALUE_COUNTS")
-
-        field: str = settings["field"] if "field" in settings else None
-        ascending: bool = settings["ascending"] if "ascending" in settings else True
-        drop_na: bool = settings["drop_na"] if "drop_na" in settings else False
-        
-        if not field:
-            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-        try:
-            df_pct = df.value_counts(subset=field, normalize=True, ascending=ascending, dropna=drop_na)
-            df_pct = df_pct.reset_index(name="value_pct")
-
-            df_count = df.value_counts(subset=field, normalize=False, ascending=ascending, dropna=drop_na)
-            df_count = df_count.reset_index(name="value_count")
-
-            df = pd.merge(df_count, df_pct)
-
-            script.append("\n# pct data")
-            script.append("df_pct = df.value_counts(subset=[{}], normalize=True, ascending={}, dropna={})".format(field, ascending, drop_na))
-            script.append("df_pct = df_pct.reset_index(name='value_pct')")
-
-            script.append("\n# count data")
-            script.append("df_count = df.value_counts(subset=[{}], normalize=False, ascending={}, dropna={})".format(field, ascending, drop_na))
-            script.append("df_count = df_count.reset_index(name='value_count')")
-
-            script.append("\n# merge data")
-            script.append("df = pd.merge(df_count, df_pct)")
-
-        except Exception as e:
-            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
-            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
-
-        cache_handler.update_node(
-            flow_id,
-            node_key,
-            {
-                "pout": {"Out": df},
-                "config": json.dumps(settings, sort_keys=True),
-                "script": script,
-            },
-        )
-
-        script_handler.script += script
-        return {"Out": df}
+import json
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.handlers.script_handler import script_handler
+from vtarget.language.app_message import app_message
+
+
+class ValueCounts:
+    def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
+        script = []
+        df: pd.DataFrame = pin["In"].copy()
+        script.append("\n# VALUE_COUNTS")
+
+        field: str = settings["field"] if "field" in settings else None
+        ascending: bool = settings["ascending"] if "ascending" in settings else True
+        drop_na: bool = settings["drop_na"] if "drop_na" in settings else False
+        
+        if not field:
+            msg = app_message.dataprep["nodes"]["missing_column"](node_key)
+            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+
+        try:
+            df_pct = df.value_counts(subset=field, normalize=True, ascending=ascending, dropna=drop_na)
+            df_pct = df_pct.reset_index(name="value_pct")
+
+            df_count = df.value_counts(subset=field, normalize=False, ascending=ascending, dropna=drop_na)
+            df_count = df_count.reset_index(name="value_count")
+
+            df = pd.merge(df_count, df_pct)
+
+            script.append("\n# pct data")
+            script.append("df_pct = df.value_counts(subset=[{}], normalize=True, ascending={}, dropna={})".format(field, ascending, drop_na))
+            script.append("df_pct = df_pct.reset_index(name='value_pct')")
+
+            script.append("\n# count data")
+            script.append("df_count = df.value_counts(subset=[{}], normalize=False, ascending={}, dropna={})".format(field, ascending, drop_na))
+            script.append("df_count = df_count.reset_index(name='value_count')")
+
+            script.append("\n# merge data")
+            script.append("df = pd.merge(df_count, df_pct)")
+
+        except Exception as e:
+            msg = app_message.dataprep["nodes"]["exception"](node_key, str(e))
+            return bug_handler.default_node_log(flow_id, node_key, msg, f"{e.__class__.__name__}({', '.join(e.args)})")
+
+        cache_handler.update_node(
+            flow_id,
+            node_key,
+            {
+                "pout": {"Out": df},
+                "config": json.dumps(settings, sort_keys=True),
+                "script": script,
+            },
+        )
+
+        script_handler.script += script
+        return {"Out": df}
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/pipeline.py` & `vtarget-0.8.7/vtarget/dataprep/pipeline.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-class Pipeline:
-    def __init__(self):
-        from vtarget.dataprep.nodes.api_rest import ApiRest
-        from vtarget.dataprep.nodes.code import Code
-        from vtarget.dataprep.nodes.column import Column
-        from vtarget.dataprep.nodes.concat import Concat
-        from vtarget.dataprep.nodes.cross_join import CrossJoin
-        from vtarget.dataprep.nodes.cumsum import Cumsum
-        from vtarget.dataprep.nodes.cut import Cut
-        from vtarget.dataprep.nodes.data_cleansing import DataCleansing
-        from vtarget.dataprep.nodes.database import Database
-        from vtarget.dataprep.nodes.database_write import DatabaseWrite
-        from vtarget.dataprep.nodes.datetime_extract import DatetimeExtract
-        from vtarget.dataprep.nodes.datetime_fill import DatetimeFill
-        from vtarget.dataprep.nodes.datetime_formatter import DatetimeFormatter
-        from vtarget.dataprep.nodes.datetime_range import DatetimeRange
-        from vtarget.dataprep.nodes.describe import Describe
-        from vtarget.dataprep.nodes.df_maker import DfMaker
-        from vtarget.dataprep.nodes.drop_duplicates import DropDuplicates
-        from vtarget.dataprep.nodes.dtype import Dtype
-        from vtarget.dataprep.nodes.email import Email
-        from vtarget.dataprep.nodes.excel import ExcelOutput
-        from vtarget.dataprep.nodes.filter import Filter
-        from vtarget.dataprep.nodes.formula import Formula
-        from vtarget.dataprep.nodes.groupby import Groupby
-        from vtarget.dataprep.nodes.input_data import InputData
-        from vtarget.dataprep.nodes.inter_row import InterRow
-        from vtarget.dataprep.nodes.isin import IsIn
-        from vtarget.dataprep.nodes.melt import Melt
-        from vtarget.dataprep.nodes.merge import Merge
-        from vtarget.dataprep.nodes.output import Output
-        from vtarget.dataprep.nodes.pivot import Pivot
-        from vtarget.dataprep.nodes.rolling import Rolling
-        from vtarget.dataprep.nodes.sample import Sample
-        from vtarget.dataprep.nodes.shape import Shape
-        from vtarget.dataprep.nodes.sort import Sort
-        from vtarget.dataprep.nodes.split import Split
-        from vtarget.dataprep.nodes.switch import Switch
-        from vtarget.dataprep.nodes.unique import Unique
-        from vtarget.dataprep.nodes.v_output import VOutput
-        from vtarget.dataprep.nodes.value_counts import ValueCounts
-
-        self.decimal_round = False
-        self.nodes_instances = {
-            "API_Rest": ApiRest(),
-            "Input_Data": InputData(),
-            "Database": Database(),
-            "Database_Write": DatabaseWrite(),
-            "Sort": Sort(),
-            "Filter": Filter(),
-            "Formula": Formula(),
-            "Merge": Merge(),
-            "Group_By": Groupby(),
-            "Cross_Join": CrossJoin(),
-            "Concat": Concat(),
-            "Pivot": Pivot(),
-            "Shape": Shape(),
-            "Melt": Melt(),
-            "Output_Data": Output(),
-            "Code": Code(),
-            "Value_Counts": ValueCounts(),
-            "Describe": Describe(),
-            "Isin": IsIn(),
-            "Cumsum": Cumsum(),
-            "V_Output": VOutput(),
-            "Inter_Row": InterRow(),
-            "Unique": Unique(),
-            "Drop_Duplicates": DropDuplicates(),
-            "Data_Cleansing": DataCleansing(),
-            "Datetime_Formatter": DatetimeFormatter(),
-            "Datetime_Extract": DatetimeExtract(),
-            "Switch": Switch(),
-            "Select": Dtype(),
-            "Dtype": Dtype(),
-            "Column": Column(),
-            "Excel": ExcelOutput(),
-            "Email": Email(),
-            "DF_Maker": DfMaker(),
-            "Source": Code(),
-            "Datetime_Range": DatetimeRange(),
-            "Rolling": Rolling(),
-            "Datetime_Fill": DatetimeFill(),
-            "Sample": Sample(),
-            "Split": Split(),
-            "Cut": Cut(),
-        }
-
-    def exec(self, flow_id: str, node: dict, input_port: dict):
-        import gc
-        import json
-        from typing import Dict
-
-        import pandas as pd
-
-        from vtarget.dataprep.types import NodeType
-        from vtarget.handlers.bug_handler import bug_handler
-        from vtarget.handlers.cache_handler import cache_handler
-        from vtarget.language.app_message import app_message
-        from vtarget.utils.utilities import utilities
-
-        settings = node["meta"]["config"] if "config" in node["meta"] else dict()
-        max_rows: int = settings["max_rows"] if "max_rows" in settings else 0
-        
-        dict_pout: Dict[pd.DataFrame] = self.nodes_instances[node["type"]].exec(
-            flow_id,
-            node["key"],
-            input_port,
-            settings,
-        )
-
-        if max_rows > 0:
-            for pout in dict_pout:
-                if isinstance(dict_pout[pout], pd.DataFrame) and dict_pout[pout].shape[0] > max_rows:
-                    msg = app_message.dataprep["builder"]["max_rows"](node["key"], max_rows)
-                    bug_handler.default_node_log(flow_id, node["key"], msg, console_level="warn", bug_level="warning")
-                    dict_pout[pout] = dict_pout[pout].head(max_rows)
-
-        if "STDOUT" in dict_pout:
-            node["meta"]["STDOUT"] = dict_pout["STDOUT"]
-
-        node["meta"]["script"] = (
-            cache_handler.settings[flow_id][node["key"]]["script"]
-            if node["key"] in cache_handler.settings[flow_id] and "script" in cache_handler.settings[flow_id][node["key"]]
-            else []
-        )
-
-        # agregar ports_config a caché
-        if "ports_config" in node["meta"]:
-            cache_handler.update_node(
-                flow_id,
-                node["key"],
-                {"ports_config": json.dumps(node["meta"]["ports_config"], sort_keys=True)},
-            )
-
-        for port_name in node["meta"]["ports_map"]["pout"].keys():
-            port_config: dict = utilities.get_table_config(node["meta"], port_name)
-            port_df: pd.DataFrame = dict_pout[port_name]
-            node["meta"]["ports_map"]["pout"][port_name]["head"] = utilities.get_head_of_df_as_list(port_df, port_config, flow_id, node["key"], port_name)
-            # TODO: revisar si la referencia de dict_pout se actualiza al modificar cache por el sort_by del puerto
-            node["meta"]["ports_map"]["pout"][port_name]["rows"] = port_df.shape[0]
-            node["meta"]["ports_map"]["pout"][port_name]["cols"] = port_df.shape[1]
-            prev_dtypes: dict = (
-                node["meta"]["ports_map"]["pout"][port_name]["dtypes"]
-                if port_name in node["meta"]["ports_map"]["pout"] and "dtypes" in node["meta"]["ports_map"]["pout"][port_name]
-                else {}
-            )
-            new_dtypes: dict = utilities.get_dtypes_of_df(port_df)
-
-            # * Merge dtypes previo con los nuevos, para conservar config de la tabla
-            if prev_dtypes and new_dtypes:
-                for k in new_dtypes:
-                    if k in prev_dtypes:
-                        if "visible" in prev_dtypes[k]:
-                            new_dtypes[k]["visible"] = prev_dtypes[k]["visible"]
-                        if "numberFormat" in prev_dtypes[k]:
-                            new_dtypes[k]["numberFormat"] = prev_dtypes[k]["numberFormat"]
-                        # TODO: Mejorar la forma en que se asigna el orden cuando hay nuevas columnas
-                        # # * mantener orden seteado desde las opciones de la tabla (excepto para nodos Column, Dtypes y Select)
-                        # if (
-                        #     node["type"]
-                        #     not in [
-                        #         NodeType.COLUMN.value,
-                        #         NodeType.DTYPE.value,
-                        #         NodeType.SELECT.value,
-                        #         NodeType.GROUPBY.value,
-                        #         # NodeType.CUMSUM.value, # puede incluir groupby que ordena las columnas a agrupar
-                        #         # NodeType.DESCRIBE.value, # puede incluir groupby que ordena las columnas a agrupar
-                        #         # NodeType.INTERROW.value, # puede incluir groupby que ordena las columnas a agrupar
-                        #         # NodeType.PIVOT.value, # puede incluir groupby que ordena las columnas a agrupar
-                        #     ]
-                        #     and "order" in prev_dtypes[k]
-                        # ):
-                        #     new_dtypes[k]["order"] = prev_dtypes[k]["order"]
-
-            node["meta"]["ports_map"]["pout"][port_name]["dtypes"] = new_dtypes
-            node["meta"]["ports_map"]["pout"][port_name]["summary"] = {}
-            node["meta"]["ports_map"]["pout"][port_name]["describe"] = {}
-            node["meta"]["readed_from_cache"] = False
-
-        del dict_pout
-        gc.collect()
-        return node
+class Pipeline:
+    def __init__(self):
+        from vtarget.dataprep.nodes.api_rest import ApiRest
+        from vtarget.dataprep.nodes.code import Code
+        from vtarget.dataprep.nodes.column import Column
+        from vtarget.dataprep.nodes.concat import Concat
+        from vtarget.dataprep.nodes.cross_join import CrossJoin
+        from vtarget.dataprep.nodes.cumsum import Cumsum
+        from vtarget.dataprep.nodes.cut import Cut
+        from vtarget.dataprep.nodes.data_cleansing import DataCleansing
+        from vtarget.dataprep.nodes.database import Database
+        from vtarget.dataprep.nodes.database_write import DatabaseWrite
+        from vtarget.dataprep.nodes.datetime_extract import DatetimeExtract
+        from vtarget.dataprep.nodes.datetime_fill import DatetimeFill
+        from vtarget.dataprep.nodes.datetime_formatter import DatetimeFormatter
+        from vtarget.dataprep.nodes.datetime_range import DatetimeRange
+        from vtarget.dataprep.nodes.describe import Describe
+        from vtarget.dataprep.nodes.df_maker import DfMaker
+        from vtarget.dataprep.nodes.drop_duplicates import DropDuplicates
+        from vtarget.dataprep.nodes.dtype import Dtype
+        from vtarget.dataprep.nodes.email import Email
+        from vtarget.dataprep.nodes.excel import ExcelOutput
+        from vtarget.dataprep.nodes.filter import Filter
+        from vtarget.dataprep.nodes.formula import Formula
+        from vtarget.dataprep.nodes.groupby import Groupby
+        from vtarget.dataprep.nodes.input_data import InputData
+        from vtarget.dataprep.nodes.inter_row import InterRow
+        from vtarget.dataprep.nodes.isin import IsIn
+        from vtarget.dataprep.nodes.melt import Melt
+        from vtarget.dataprep.nodes.merge import Merge
+        from vtarget.dataprep.nodes.output import Output
+        from vtarget.dataprep.nodes.pivot import Pivot
+        from vtarget.dataprep.nodes.rolling import Rolling
+        from vtarget.dataprep.nodes.sample import Sample
+        from vtarget.dataprep.nodes.shape import Shape
+        from vtarget.dataprep.nodes.sort import Sort
+        from vtarget.dataprep.nodes.split import Split
+        from vtarget.dataprep.nodes.switch import Switch
+        from vtarget.dataprep.nodes.unique import Unique
+        from vtarget.dataprep.nodes.v_output import VOutput
+        from vtarget.dataprep.nodes.value_counts import ValueCounts
+
+        self.decimal_round = False
+        self.nodes_instances = {
+            "API_Rest": ApiRest(),
+            "Input_Data": InputData(),
+            "Database": Database(),
+            "Database_Write": DatabaseWrite(),
+            "Sort": Sort(),
+            "Filter": Filter(),
+            "Formula": Formula(),
+            "Merge": Merge(),
+            "Group_By": Groupby(),
+            "Cross_Join": CrossJoin(),
+            "Concat": Concat(),
+            "Pivot": Pivot(),
+            "Shape": Shape(),
+            "Melt": Melt(),
+            "Output_Data": Output(),
+            "Code": Code(),
+            "Value_Counts": ValueCounts(),
+            "Describe": Describe(),
+            "Isin": IsIn(),
+            "Cumsum": Cumsum(),
+            "V_Output": VOutput(),
+            "Inter_Row": InterRow(),
+            "Unique": Unique(),
+            "Drop_Duplicates": DropDuplicates(),
+            "Data_Cleansing": DataCleansing(),
+            "Datetime_Formatter": DatetimeFormatter(),
+            "Datetime_Extract": DatetimeExtract(),
+            "Switch": Switch(),
+            "Select": Dtype(),
+            "Dtype": Dtype(),
+            "Column": Column(),
+            "Excel": ExcelOutput(),
+            "Email": Email(),
+            "DF_Maker": DfMaker(),
+            "Source": Code(),
+            "Datetime_Range": DatetimeRange(),
+            "Rolling": Rolling(),
+            "Datetime_Fill": DatetimeFill(),
+            "Sample": Sample(),
+            "Split": Split(),
+            "Cut": Cut(),
+        }
+
+    def exec(self, flow_id: str, node: dict, input_port: dict):
+        import gc
+        import json
+        from typing import Dict
+
+        import pandas as pd
+
+        from vtarget.dataprep.types import NodeType
+        from vtarget.handlers.bug_handler import bug_handler
+        from vtarget.handlers.cache_handler import cache_handler
+        from vtarget.language.app_message import app_message
+        from vtarget.utils.utilities import utilities
+
+        settings = node["meta"]["config"] if "config" in node["meta"] else dict()
+        max_rows: int = settings["max_rows"] if "max_rows" in settings else 0
+        
+        dict_pout: Dict[pd.DataFrame] = self.nodes_instances[node["type"]].exec(
+            flow_id,
+            node["key"],
+            input_port,
+            settings,
+        )
+
+        if max_rows > 0:
+            for pout in dict_pout:
+                if isinstance(dict_pout[pout], pd.DataFrame) and dict_pout[pout].shape[0] > max_rows:
+                    msg = app_message.dataprep["builder"]["max_rows"](node["key"], max_rows)
+                    bug_handler.default_node_log(flow_id, node["key"], msg, console_level="warn", bug_level="warning")
+                    dict_pout[pout] = dict_pout[pout].head(max_rows)
+
+        if "STDOUT" in dict_pout:
+            node["meta"]["STDOUT"] = dict_pout["STDOUT"]
+
+        node["meta"]["script"] = (
+            cache_handler.settings[flow_id][node["key"]]["script"]
+            if node["key"] in cache_handler.settings[flow_id] and "script" in cache_handler.settings[flow_id][node["key"]]
+            else []
+        )
+
+        # agregar ports_config a caché
+        if "ports_config" in node["meta"]:
+            cache_handler.update_node(
+                flow_id,
+                node["key"],
+                {"ports_config": json.dumps(node["meta"]["ports_config"], sort_keys=True)},
+            )
+
+        for port_name in node["meta"]["ports_map"]["pout"].keys():
+            port_config: dict = utilities.get_table_config(node["meta"], port_name)
+            port_df: pd.DataFrame = dict_pout[port_name]
+            node["meta"]["ports_map"]["pout"][port_name]["head"] = utilities.get_head_of_df_as_list(port_df, port_config, flow_id, node["key"], port_name)
+            # TODO: revisar si la referencia de dict_pout se actualiza al modificar cache por el sort_by del puerto
+            node["meta"]["ports_map"]["pout"][port_name]["rows"] = port_df.shape[0]
+            node["meta"]["ports_map"]["pout"][port_name]["cols"] = port_df.shape[1]
+            prev_dtypes: dict = (
+                node["meta"]["ports_map"]["pout"][port_name]["dtypes"]
+                if port_name in node["meta"]["ports_map"]["pout"] and "dtypes" in node["meta"]["ports_map"]["pout"][port_name]
+                else {}
+            )
+            new_dtypes: dict = utilities.get_dtypes_of_df(port_df)
+
+            # * Merge dtypes previo con los nuevos, para conservar config de la tabla
+            if prev_dtypes and new_dtypes:
+                for k in new_dtypes:
+                    if k in prev_dtypes:
+                        if "visible" in prev_dtypes[k]:
+                            new_dtypes[k]["visible"] = prev_dtypes[k]["visible"]
+                        if "numberFormat" in prev_dtypes[k]:
+                            new_dtypes[k]["numberFormat"] = prev_dtypes[k]["numberFormat"]
+                        # TODO: Mejorar la forma en que se asigna el orden cuando hay nuevas columnas
+                        # # * mantener orden seteado desde las opciones de la tabla (excepto para nodos Column, Dtypes y Select)
+                        # if (
+                        #     node["type"]
+                        #     not in [
+                        #         NodeType.COLUMN.value,
+                        #         NodeType.DTYPE.value,
+                        #         NodeType.SELECT.value,
+                        #         NodeType.GROUPBY.value,
+                        #         # NodeType.CUMSUM.value, # puede incluir groupby que ordena las columnas a agrupar
+                        #         # NodeType.DESCRIBE.value, # puede incluir groupby que ordena las columnas a agrupar
+                        #         # NodeType.INTERROW.value, # puede incluir groupby que ordena las columnas a agrupar
+                        #         # NodeType.PIVOT.value, # puede incluir groupby que ordena las columnas a agrupar
+                        #     ]
+                        #     and "order" in prev_dtypes[k]
+                        # ):
+                        #     new_dtypes[k]["order"] = prev_dtypes[k]["order"]
+
+            node["meta"]["ports_map"]["pout"][port_name]["dtypes"] = new_dtypes
+            node["meta"]["ports_map"]["pout"][port_name]["summary"] = {}
+            node["meta"]["ports_map"]["pout"][port_name]["describe"] = {}
+            node["meta"]["readed_from_cache"] = False
+
+        del dict_pout
+        gc.collect()
+        return node
```

### Comparing `vtarget-0.8.6/vtarget/dataprep/types.py` & `vtarget-0.8.7/vtarget/dataprep/types.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from enum import Enum
-
-
-# NOTE: Debe estar actualizado con el NodeType de vtarget-client
-class NodeType(Enum):
-    BARCHART = 'Bar_Chart'
-    CODE = 'Code'
-    COLUMN = 'Column'
-    COMMENT = 'Comment'
-    CONCAT = 'Concat'
-    CROSSJOIN = 'Cross_Join'
-    CUMSUM = 'Cumsum'
-    DATABASE = 'Database'
-    DATABASEWRITE = 'Database_Write'
-    DATACLEANSING = 'Data_Cleansing'
-    DATETIMEEXTRACT = 'Datetime_Extract'
-    DATETIMEFILL = 'Datetime_Fill',
-    DATETIMEFORMATTER = 'Datetime_Formatter'
-    DATETIMERANGE = 'Datetime_Range'
-    DESCRIBE = 'Describe'
-    DFMAKER = 'DF_Maker'
-    DROPDUPLICATES = 'Drop_Duplicates'
-    DTYPE = 'Dtype'
-    FILTER = 'Filter'
-    FORMULA = 'Formula'
-    GROUPBY = 'Group_By'
-    INPUTDATA = 'Input_Data'
-    INTERROW = 'Inter_Row'
-    ISIN = 'Isin'
-    JOINMULTI = 'Join_Multi'
-    LINECHART = 'Line_Chart'
-    BARLINECHART = 'BarLine_Chart'
-    MELT = 'Melt'
-    MERGE = 'Merge'
-    OUTPUTDATA = 'Output_Data'
-    PIECHART = 'Pie_Chart'
-    PIVOT = 'Pivot'
-    RADARCHART = 'Radar_Chart'
-    ROLLING = 'Rolling'
-    SAMPLE = 'Sample'
-    SCATTERCHART = 'Scatter_Chart'
-    SELECT = 'Select'
-    SHAPE = 'Shape'
-    SORT = 'Sort'
-    SWITCH = 'Switch'
-    UNIQUE = 'Unique'
-    VALUECOUNTS = 'Value_Counts'
-    VOUTPUT = 'V_Output'
-    EXCEL = 'Excel'
-    EMAIL = 'Email'
-    IF = 'If'
-    WAIT = 'Wait'
-    SOURCE = 'Source'
-    BINARYMODEL = 'Binary_Model'
-    REGRESSIONMODEL = 'Regression_Model'
-    MULTICLASSMODEL = 'Multiclass_Model'
-    SPLIT = 'Split'
-    CUT = 'Cut'
-    APIREST = 'API_Rest'
+from enum import Enum
+
+
+# NOTE: Debe estar actualizado con el NodeType de vtarget-client
+class NodeType(Enum):
+    BARCHART = 'Bar_Chart'
+    CODE = 'Code'
+    COLUMN = 'Column'
+    COMMENT = 'Comment'
+    CONCAT = 'Concat'
+    CROSSJOIN = 'Cross_Join'
+    CUMSUM = 'Cumsum'
+    DATABASE = 'Database'
+    DATABASEWRITE = 'Database_Write'
+    DATACLEANSING = 'Data_Cleansing'
+    DATETIMEEXTRACT = 'Datetime_Extract'
+    DATETIMEFILL = 'Datetime_Fill',
+    DATETIMEFORMATTER = 'Datetime_Formatter'
+    DATETIMERANGE = 'Datetime_Range'
+    DESCRIBE = 'Describe'
+    DFMAKER = 'DF_Maker'
+    DROPDUPLICATES = 'Drop_Duplicates'
+    DTYPE = 'Dtype'
+    FILTER = 'Filter'
+    FORMULA = 'Formula'
+    GROUPBY = 'Group_By'
+    INPUTDATA = 'Input_Data'
+    INTERROW = 'Inter_Row'
+    ISIN = 'Isin'
+    JOINMULTI = 'Join_Multi'
+    LINECHART = 'Line_Chart'
+    BARLINECHART = 'BarLine_Chart'
+    MELT = 'Melt'
+    MERGE = 'Merge'
+    OUTPUTDATA = 'Output_Data'
+    PIECHART = 'Pie_Chart'
+    PIVOT = 'Pivot'
+    RADARCHART = 'Radar_Chart'
+    ROLLING = 'Rolling'
+    SAMPLE = 'Sample'
+    SCATTERCHART = 'Scatter_Chart'
+    SELECT = 'Select'
+    SHAPE = 'Shape'
+    SORT = 'Sort'
+    SWITCH = 'Switch'
+    UNIQUE = 'Unique'
+    VALUECOUNTS = 'Value_Counts'
+    VOUTPUT = 'V_Output'
+    EXCEL = 'Excel'
+    EMAIL = 'Email'
+    IF = 'If'
+    WAIT = 'Wait'
+    SOURCE = 'Source'
+    BINARYMODEL = 'Binary_Model'
+    REGRESSIONMODEL = 'Regression_Model'
+    MULTICLASSMODEL = 'Multiclass_Model'
+    SPLIT = 'Split'
+    CUT = 'Cut'
+    APIREST = 'API_Rest'
```

### Comparing `vtarget-0.8.6/vtarget/handlers/bug_handler.py` & `vtarget-0.8.7/vtarget/handlers/bug_handler.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import pandas as pd
-from termcolor import colored
-
-from vtarget.handlers.log_handler import log_handler
-
-
-class Bug_Handler:
-    def __init__(self):
-        self.bug = []
-        self.__append_handler = None
-
-    def on_append(self, handler):
-        self.__append_handler = handler
-
-    def append_handler(self, bug):
-        if self.__append_handler is not None:
-            self.__append_handler(bug)
-
-    def append(self, bug, use_handler=True):
-        self.bug.append(bug)
-        if use_handler:
-            self.append_handler(bug)
-
-    def console(self, msg, level, flow_id, emit=True):
-        level = level.upper()
-        if level == "DEBUG":
-            color = "green"
-        elif level == "INFO":
-            color = "cyan"
-        elif level == "WARN":
-            color = "yellow"
-        elif level == "ERROR":
-            color = "red"
-        elif level == "FATAL":
-            color = "white"
-            print(colored(f"[{level}] {msg}", color, "on_red"))
-            return
-        elif level == "TRACE":
-            color = "magenta"
-        else:
-            color = "white"
-        print(colored(f"[{level}] {msg}", color))
-        log_handler.append({"flow_id": flow_id, "level": level, "msg": msg, "color": color}, emit)
-
-    def default_node_log(
-        self,
-        flow_id: str,
-        node_key: str,
-        msg: str,
-        exception="",
-        console_level="fatal",
-        bug_level="error",
-        success=False,
-    ):
-        self.console(msg, console_level, flow_id)
-        self.append(
-            {
-                "flow_id": flow_id,
-                "success": success,
-                "node_key": node_key,
-                "level": bug_level,
-                "msg": msg,
-                "exception": exception,
-            }
-        )
-        return {"Out": pd.DataFrame()}
-
-
-bug_handler = Bug_Handler()
+import pandas as pd
+from termcolor import colored
+
+from vtarget.handlers.log_handler import log_handler
+
+
+class Bug_Handler:
+    def __init__(self):
+        self.bug = []
+        self.__append_handler = None
+
+    def on_append(self, handler):
+        self.__append_handler = handler
+
+    def append_handler(self, bug):
+        if self.__append_handler is not None:
+            self.__append_handler(bug)
+
+    def append(self, bug, use_handler=True):
+        self.bug.append(bug)
+        if use_handler:
+            self.append_handler(bug)
+
+    def console(self, msg, level, flow_id, emit=True):
+        level = level.upper()
+        if level == "DEBUG":
+            color = "green"
+        elif level == "INFO":
+            color = "cyan"
+        elif level == "WARN":
+            color = "yellow"
+        elif level == "ERROR":
+            color = "red"
+        elif level == "FATAL":
+            color = "white"
+            print(colored(f"[{level}] {msg}", color, "on_red"))
+            return
+        elif level == "TRACE":
+            color = "magenta"
+        else:
+            color = "white"
+        print(colored(f"[{level}] {msg}", color))
+        log_handler.append({"flow_id": flow_id, "level": level, "msg": msg, "color": color}, emit)
+
+    def default_node_log(
+        self,
+        flow_id: str,
+        node_key: str,
+        msg: str,
+        exception="",
+        console_level="fatal",
+        bug_level="error",
+        success=False,
+    ):
+        self.console(msg, console_level, flow_id)
+        self.append(
+            {
+                "flow_id": flow_id,
+                "success": success,
+                "node_key": node_key,
+                "level": bug_level,
+                "msg": msg,
+                "exception": exception,
+            }
+        )
+        return {"Out": pd.DataFrame()}
+
+
+bug_handler = Bug_Handler()
```

### Comparing `vtarget-0.8.6/vtarget/handlers/cache_handler.py` & `vtarget-0.8.7/vtarget/handlers/cache_handler.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-import gc
-import os
-import pickle
-import sys
-import traceback
-from random import randint
-from typing import Any, Dict
-
-import pandas as pd
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.language.app_message import app_message
-from vtarget.utils import TEMP_DIR
-
-
-def get_size(obj):
-    size = sys.getsizeof(obj)
-    if isinstance(obj, dict):
-        size += sum([get_size(v) for v in obj.values()])
-    elif hasattr(obj, "__iter__") and not isinstance(obj, (str, bytes, bytearray)):
-        size += sum([get_size(i) for i in obj])
-    return size
-
-
-class __Cache_Handler:
-    cache: Dict[str, Dict[str, Dict[str, Dict[str, pd.DataFrame]]]]
-    settings: Dict[str, Dict[str, Dict[str, Any]]]
-    dump_enabled: bool
-
-    def __init__(self):
-        super().__init__()
-        self.cache = dict()
-        self.settings = dict()
-        self.dump_enabled = False
-        self.wtf = randint(0, 256)
-    #     self.daemon = True
-    #     self.start()
-
-    # def run(self):
-    #     import json
-    #     import time
-
-    #     import matplotlib.pyplot as plt
-    #     import networkx as nx
-
-    #     from vtarget import utils
-
-    #     n_nodes = 0
-    #     while True:
-    #         try:
-    #             G = nx.DiGraph()
-    #             for flow_id in self.settings:
-    #                 for node_key in self.settings[flow_id]:
-    #                     G.add_node(node_key)
-
-    #             for flow_id in self.settings:
-    #                 for node_key in self.settings[flow_id]:
-    #                     config: Dict[str, Any] = json.loads(self.settings[flow_id][node_key]["config"])
-    #                     for port_name in config:
-    #                         if port_name.startswith("port_"):
-    #                             G.add_edge(config[port_name], node_key)
-
-    #             if n_nodes != G.number_of_nodes():
-    #                 n_nodes = G.number_of_nodes()
-    #                 if n_nodes > 0:
-    #                     plt.clf()  # limpiar el gráfico para la próxima iteración
-    #                     nx.draw_networkx(G, with_labels=True, arrows=True)
-    #                     plt.draw()
-    #             plt.pause(1)  # pausa de 1 segundo
-    #         except Exception:
-    #             e, tb = utils.trace_error()
-    #             print(e)
-    #             for t in tb:
-    #                 print(t)
-    #             time.sleep(1)
-
-    def write(self, flow_id: str, node_key: str) -> None:
-        if flow_id not in self.cache or node_key not in self.cache[flow_id] or "pout" not in self.cache[flow_id][node_key]:
-            return
-        try:
-            if not os.path.exists(f"{TEMP_DIR}/cache"):
-                os.mkdir(f"{TEMP_DIR}/cache")
-            if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
-                os.mkdir(f"{TEMP_DIR}/cache/{flow_id}")
-            for port_name in self.cache[flow_id][node_key]["pout"]:
-                if os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}"):
-                    os.remove(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}")
-                with open(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}.tmp", "wb") as file:
-                    pickle.dump(self.cache[flow_id][node_key]["pout"][port_name], file)
-                os.rename(
-                    f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}.tmp",
-                    f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}",
-                )
-            msg = app_message.handlers["cache_handler"]["node_cache_saved"](node_key)
-            bug_handler.console(msg, "info", flow_id)
-            if self.dump_enabled:
-                del self.cache[flow_id][node_key]
-                gc.collect()
-        except:
-            traceback.print_exception(*sys.exc_info())
-
-    def reset(self, flow_id: str):
-        if flow_id in self.cache:
-            self.cache[flow_id].clear()
-            del self.cache[flow_id]
-        if flow_id in self.settings:
-            self.settings[flow_id].clear()
-            del self.settings[flow_id]
-        gc.collect()
-        if not os.path.exists(f"{TEMP_DIR}/cache"):
-            return
-        if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
-            return
-        for root, dirs, files in os.walk(f"{TEMP_DIR}/cache/{flow_id}", topdown=False):
-            for name in files:
-                os.remove(os.path.join(root, name))
-            for name in dirs:
-                os.rmdir(os.path.join(root, name))
-
-    def update_node(self, flow_id: str, node_key: str, new_props: Dict[str, Any] = {}):
-        if node_key not in cache_handler.settings[flow_id]:
-            cache_handler.settings[flow_id][node_key] = dict()
-        if "pout" in new_props:
-            pout: Dict[str, pd.DataFrame] = new_props.pop("pout")
-            for port_name in pout:
-                if flow_id not in self.cache:
-                    self.cache[flow_id] = dict()
-                if node_key not in self.cache[flow_id]:
-                    self.cache[flow_id][node_key] = dict()
-                if "pout" not in self.cache[flow_id][node_key]:
-                    self.cache[flow_id][node_key]["pout"] = dict()
-                self.cache[flow_id][node_key]["pout"][port_name] = pout[port_name]
-            self.settings[flow_id][node_key]["pout"] = list(pout.keys())
-        self.settings[flow_id][node_key].update(new_props)
-        if not self.dump_enabled:
-            if node_key.startswith("v_output"):
-                self.write(flow_id, node_key)
-            else:
-                msg = app_message.handlers["cache_handler"]["node_ram_saved"](node_key)
-                bug_handler.console(msg, "info", flow_id)
-
-    def delete_node(self, flow_id: str, node_key: str) -> bool:
-        cache_deleted = False
-        if flow_id in self.cache:
-            if node_key in self.cache[flow_id]:
-                del self.cache[flow_id][node_key]
-                gc.collect()
-                cache_deleted = True
-        settings_deleted = False
-        if flow_id in self.settings:
-            if node_key in self.settings[flow_id]:
-                del self.settings[flow_id][node_key]
-                gc.collect()
-                settings_deleted = True
-        return cache_deleted and settings_deleted
-
-    def dump(self, flow_id: str, node_key: str) -> None:
-        if self.dump_enabled:
-            self.write(flow_id, node_key)
-
-    def load(self, flow_id: str, node_key: str, port_name: str) -> None:
-        loaded = True
-        if flow_id not in self.cache:
-            self.cache[flow_id] = dict()
-        if node_key not in self.cache[flow_id]:
-            self.cache[flow_id][node_key] = dict()
-        if "pout" not in self.cache[flow_id][node_key]:
-            self.cache[flow_id][node_key]["pout"] = dict()
-        # NOTE: se comentó para tener siempre la data actualizada desde el archivo en disco del voutput
-        # if port_name not in self.cache[flow_id][node_key]["pout"]:
-        if os.path.exists(f"{TEMP_DIR}/cache") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}"):
-            try:
-                with open(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}", "rb") as file:
-                    self.cache[flow_id][node_key]["pout"][port_name] = pickle.load(file)
-            except:
-                traceback.print_exception(*sys.exc_info())
-                loaded = False
-        return loaded
-
-    def load_settings(self, flow_id: str) -> None:
-        if flow_id not in self.settings:
-            self.settings[flow_id] = dict()
-        if os.path.exists(f"{TEMP_DIR}/cache") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/settings"):
-            try:
-                with open(f"{TEMP_DIR}/cache/{flow_id}/settings", "rb") as file:
-                    self.settings[flow_id] = pickle.load(file)
-            except:
-                traceback.print_exception(*sys.exc_info())
-
-    def dump_settings(self, flow_id: str) -> None:
-        if flow_id not in self.settings:
-            return
-        try:
-            if not os.path.exists(f"{TEMP_DIR}/cache"):
-                os.mkdir(f"{TEMP_DIR}/cache")
-            if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
-                os.mkdir(f"{TEMP_DIR}/cache/{flow_id}")
-            if os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/settings"):
-                os.remove(f"{TEMP_DIR}/cache/{flow_id}/settings")
-            with open(f"{TEMP_DIR}/cache/{flow_id}/settings.tmp", "wb") as file:
-                pickle.dump(self.settings[flow_id], file)
-            os.rename(
-                f"{TEMP_DIR}/cache/{flow_id}/settings.tmp",
-                f"{TEMP_DIR}/cache/{flow_id}/settings",
-            )
-            if self.dump_enabled:
-                self.settings[flow_id].clear()
-                del self.settings[flow_id]
-                gc.collect()
-        except:
-            traceback.print_exception(*sys.exc_info())
-
-    def log(self, *args, **kwargs):
-        print("[cache-handler]", *args, **kwargs)
-
-
-cache_handler = __Cache_Handler()
+import gc
+import os
+import pickle
+import sys
+import traceback
+from random import randint
+from typing import Any, Dict
+
+import pandas as pd
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.language.app_message import app_message
+from vtarget.utils import TEMP_DIR
+
+
+def get_size(obj):
+    size = sys.getsizeof(obj)
+    if isinstance(obj, dict):
+        size += sum([get_size(v) for v in obj.values()])
+    elif hasattr(obj, "__iter__") and not isinstance(obj, (str, bytes, bytearray)):
+        size += sum([get_size(i) for i in obj])
+    return size
+
+
+class __Cache_Handler:
+    cache: Dict[str, Dict[str, Dict[str, Dict[str, pd.DataFrame]]]]
+    settings: Dict[str, Dict[str, Dict[str, Any]]]
+    dump_enabled: bool
+
+    def __init__(self):
+        super().__init__()
+        self.cache = dict()
+        self.settings = dict()
+        self.dump_enabled = False
+        self.wtf = randint(0, 256)
+    #     self.daemon = True
+    #     self.start()
+
+    # def run(self):
+    #     import json
+    #     import time
+
+    #     import matplotlib.pyplot as plt
+    #     import networkx as nx
+
+    #     from vtarget import utils
+
+    #     n_nodes = 0
+    #     while True:
+    #         try:
+    #             G = nx.DiGraph()
+    #             for flow_id in self.settings:
+    #                 for node_key in self.settings[flow_id]:
+    #                     G.add_node(node_key)
+
+    #             for flow_id in self.settings:
+    #                 for node_key in self.settings[flow_id]:
+    #                     config: Dict[str, Any] = json.loads(self.settings[flow_id][node_key]["config"])
+    #                     for port_name in config:
+    #                         if port_name.startswith("port_"):
+    #                             G.add_edge(config[port_name], node_key)
+
+    #             if n_nodes != G.number_of_nodes():
+    #                 n_nodes = G.number_of_nodes()
+    #                 if n_nodes > 0:
+    #                     plt.clf()  # limpiar el gráfico para la próxima iteración
+    #                     nx.draw_networkx(G, with_labels=True, arrows=True)
+    #                     plt.draw()
+    #             plt.pause(1)  # pausa de 1 segundo
+    #         except Exception:
+    #             e, tb = utils.trace_error()
+    #             print(e)
+    #             for t in tb:
+    #                 print(t)
+    #             time.sleep(1)
+
+    def write(self, flow_id: str, node_key: str) -> None:
+        if flow_id not in self.cache or node_key not in self.cache[flow_id] or "pout" not in self.cache[flow_id][node_key]:
+            return
+        try:
+            if not os.path.exists(f"{TEMP_DIR}/cache"):
+                os.mkdir(f"{TEMP_DIR}/cache")
+            if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
+                os.mkdir(f"{TEMP_DIR}/cache/{flow_id}")
+            for port_name in self.cache[flow_id][node_key]["pout"]:
+                if os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}"):
+                    os.remove(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}")
+                with open(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}.tmp", "wb") as file:
+                    pickle.dump(self.cache[flow_id][node_key]["pout"][port_name], file)
+                os.rename(
+                    f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}.tmp",
+                    f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}",
+                )
+            msg = app_message.handlers["cache_handler"]["node_cache_saved"](node_key)
+            bug_handler.console(msg, "info", flow_id)
+            if self.dump_enabled:
+                del self.cache[flow_id][node_key]
+                gc.collect()
+        except:
+            traceback.print_exception(*sys.exc_info())
+
+    def reset(self, flow_id: str):
+        if flow_id in self.cache:
+            self.cache[flow_id].clear()
+            del self.cache[flow_id]
+        if flow_id in self.settings:
+            self.settings[flow_id].clear()
+            del self.settings[flow_id]
+        gc.collect()
+        if not os.path.exists(f"{TEMP_DIR}/cache"):
+            return
+        if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
+            return
+        for root, dirs, files in os.walk(f"{TEMP_DIR}/cache/{flow_id}", topdown=False):
+            for name in files:
+                os.remove(os.path.join(root, name))
+            for name in dirs:
+                os.rmdir(os.path.join(root, name))
+
+    def update_node(self, flow_id: str, node_key: str, new_props: Dict[str, Any] = {}):
+        if node_key not in cache_handler.settings[flow_id]:
+            cache_handler.settings[flow_id][node_key] = dict()
+        if "pout" in new_props:
+            pout: Dict[str, pd.DataFrame] = new_props.pop("pout")
+            for port_name in pout:
+                if flow_id not in self.cache:
+                    self.cache[flow_id] = dict()
+                if node_key not in self.cache[flow_id]:
+                    self.cache[flow_id][node_key] = dict()
+                if "pout" not in self.cache[flow_id][node_key]:
+                    self.cache[flow_id][node_key]["pout"] = dict()
+                self.cache[flow_id][node_key]["pout"][port_name] = pout[port_name]
+            self.settings[flow_id][node_key]["pout"] = list(pout.keys())
+        self.settings[flow_id][node_key].update(new_props)
+        if not self.dump_enabled:
+            if node_key.startswith("v_output"):
+                self.write(flow_id, node_key)
+            else:
+                msg = app_message.handlers["cache_handler"]["node_ram_saved"](node_key)
+                bug_handler.console(msg, "info", flow_id)
+
+    def delete_node(self, flow_id: str, node_key: str) -> bool:
+        cache_deleted = False
+        if flow_id in self.cache:
+            if node_key in self.cache[flow_id]:
+                del self.cache[flow_id][node_key]
+                gc.collect()
+                cache_deleted = True
+        settings_deleted = False
+        if flow_id in self.settings:
+            if node_key in self.settings[flow_id]:
+                del self.settings[flow_id][node_key]
+                gc.collect()
+                settings_deleted = True
+        return cache_deleted and settings_deleted
+
+    def dump(self, flow_id: str, node_key: str) -> None:
+        if self.dump_enabled:
+            self.write(flow_id, node_key)
+
+    def load(self, flow_id: str, node_key: str, port_name: str) -> None:
+        loaded = True
+        if flow_id not in self.cache:
+            self.cache[flow_id] = dict()
+        if node_key not in self.cache[flow_id]:
+            self.cache[flow_id][node_key] = dict()
+        if "pout" not in self.cache[flow_id][node_key]:
+            self.cache[flow_id][node_key]["pout"] = dict()
+        # NOTE: se comentó para tener siempre la data actualizada desde el archivo en disco del voutput
+        # if port_name not in self.cache[flow_id][node_key]["pout"]:
+        if os.path.exists(f"{TEMP_DIR}/cache") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}"):
+            try:
+                with open(f"{TEMP_DIR}/cache/{flow_id}/{node_key}_{port_name}", "rb") as file:
+                    self.cache[flow_id][node_key]["pout"][port_name] = pickle.load(file)
+            except:
+                traceback.print_exception(*sys.exc_info())
+                loaded = False
+        return loaded
+
+    def load_settings(self, flow_id: str) -> None:
+        if flow_id not in self.settings:
+            self.settings[flow_id] = dict()
+        if os.path.exists(f"{TEMP_DIR}/cache") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}") and os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/settings"):
+            try:
+                with open(f"{TEMP_DIR}/cache/{flow_id}/settings", "rb") as file:
+                    self.settings[flow_id] = pickle.load(file)
+            except:
+                traceback.print_exception(*sys.exc_info())
+
+    def dump_settings(self, flow_id: str) -> None:
+        if flow_id not in self.settings:
+            return
+        try:
+            if not os.path.exists(f"{TEMP_DIR}/cache"):
+                os.mkdir(f"{TEMP_DIR}/cache")
+            if not os.path.exists(f"{TEMP_DIR}/cache/{flow_id}"):
+                os.mkdir(f"{TEMP_DIR}/cache/{flow_id}")
+            if os.path.exists(f"{TEMP_DIR}/cache/{flow_id}/settings"):
+                os.remove(f"{TEMP_DIR}/cache/{flow_id}/settings")
+            with open(f"{TEMP_DIR}/cache/{flow_id}/settings.tmp", "wb") as file:
+                pickle.dump(self.settings[flow_id], file)
+            os.rename(
+                f"{TEMP_DIR}/cache/{flow_id}/settings.tmp",
+                f"{TEMP_DIR}/cache/{flow_id}/settings",
+            )
+            if self.dump_enabled:
+                self.settings[flow_id].clear()
+                del self.settings[flow_id]
+                gc.collect()
+        except:
+            traceback.print_exception(*sys.exc_info())
+
+    def log(self, *args, **kwargs):
+        print("[cache-handler]", *args, **kwargs)
+
+
+cache_handler = __Cache_Handler()
```

### Comparing `vtarget-0.8.6/vtarget/handlers/event_handler.py` & `vtarget-0.8.7/vtarget/handlers/event_handler.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import json
-import queue
-import sys
-import threading
-import traceback
-
-
-class EventHandler(threading.Thread):
-    def __init__(self):
-        super().__init__()
-        self.emit_queue = queue.Queue()
-        self.__event_callback = None
-        self.daemon = True
-        self.start()
-
-    def on_event(self, callback):
-        self.__event_callback = callback
-
-    def event_callback(self, payload):
-        if self.__event_callback is not None:
-            self.__event_callback(payload)
-
-    def log(self, *args, **kwargs):
-        print("[event-handler]", *args, **kwargs)
-
-    def run(self):
-        self.log("iniciando hilo envio de eventos")
-        self.running = True
-        while self.running:
-            try:
-                payload = self.emit_queue.get(timeout=1)
-                # self.log(payload["name"], len(json.dumps(payload)), "bytes") # NOTE: Descomentar para depurar
-                self.event_callback(payload)
-            except:
-                c, e, t = sys.exc_info()
-                if c is not queue.Empty:
-                    error = f"{c.__name__}: {e}"
-                    tb = [f"{s.filename}:{s.lineno}" for s in traceback.extract_tb(t)]
-                    self.log(error)
-                    for line in tb:
-                        self.log(line)
-
-    def stop(self):
-        self.log("stopping...")
-        self.running = False
-        self.join()
-        self.log("stopped")
-
-
-event_handler = EventHandler()
+import json
+import queue
+import sys
+import threading
+import traceback
+
+
+class EventHandler(threading.Thread):
+    def __init__(self):
+        super().__init__()
+        self.emit_queue = queue.Queue()
+        self.__event_callback = None
+        self.daemon = True
+        self.start()
+
+    def on_event(self, callback):
+        self.__event_callback = callback
+
+    def event_callback(self, payload):
+        if self.__event_callback is not None:
+            self.__event_callback(payload)
+
+    def log(self, *args, **kwargs):
+        print("[event-handler]", *args, **kwargs)
+
+    def run(self):
+        self.log("iniciando hilo envio de eventos")
+        self.running = True
+        while self.running:
+            try:
+                payload = self.emit_queue.get(timeout=1)
+                # self.log(payload["name"], len(json.dumps(payload)), "bytes") # NOTE: Descomentar para depurar
+                self.event_callback(payload)
+            except:
+                c, e, t = sys.exc_info()
+                if c is not queue.Empty:
+                    error = f"{c.__name__}: {e}"
+                    tb = [f"{s.filename}:{s.lineno}" for s in traceback.extract_tb(t)]
+                    self.log(error)
+                    for line in tb:
+                        self.log(line)
+
+    def stop(self):
+        self.log("stopping...")
+        self.running = False
+        self.join()
+        self.log("stopped")
+
+
+event_handler = EventHandler()
```

### Comparing `vtarget-0.8.6/vtarget/language/app_message.py` & `vtarget-0.8.7/vtarget/language/app_message.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,584 +1,584 @@
-# TODO: Importar el language acá
-
-
-class __AppMessage:
-    def __init__(self, languaje):
-        if languaje == "es":
-            self.dataprep = self.dataprep_spanish()
-            self.dataviz = self.dataviz_spanish()
-            self.autots = self.autots_spanish()
-            self.automl = self.automl_spanish()
-            self.handlers = self.handlers_spanish()
-            self.utils = self.utils_spanish()
-            self.worker = self.worker_spanish()
-            self.service = self.service_spanish()
-        else:
-            self.dataprep = self.dataprep_english()
-            self.dataviz = self.dataviz_english()
-            self.autots = self.autots_english()
-            self.automl = self.automl_english()
-            self.handlers = self.handlers_english()
-            self.utils = self.utils_english()
-            self.worker = self.worker_english()
-            self.service = self.service_english()
-
-    # ===================================
-    # Spanish
-    # ===================================
-    def dataprep_spanish(self):
-        return {
-            "nodes": {
-                "api_rest": {
-                    "no_method": lambda node_key: f"({node_key}): Debes seleccionar un método de envío",
-                    "no_url": lambda node_key: f"({node_key}): Debes seleccionar una URL",
-                },
-                "code": {
-                    "no_vtg_codeout": lambda node_key: f"({node_key}): Debes llamar a la función vtg_codeout(Df) con tu DataFrame de salida",
-                },
-                "column": {
-                    "no_columns_selected": lambda node_key: f"({node_key}): No hay columnas seleccionadas",
-                    "rename_columns": lambda node_key: f"({node_key}): No fue posible renombrar las columnas",
-                    "column_not_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
-                },
-                "dtype": {
-                    "no_columns_selected": lambda node_key: f"({node_key}): No hay columnas seleccionadas",
-                    "rename_columns": lambda node_key: f"({node_key}): No fue posible renombrar las columnas",
-                    "column_not_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
-                    "change_dtype": lambda node_key, column, dtype: f"({node_key}): No fue posible transformar el tipo de dato de la columna '{column}' a '{dtype}'",
-                    "unknow_dtype": lambda node_key, column, dtype: f"({node_key}): Tipo de dato '{dtype}' desconocido. Columna '{column}' se mantiene como string",
-                },
-                "datetime_fill": {
-                    "time_column_required": lambda node_key: f"({node_key}): La columna 'Tiempo' es obligatoria",
-                    "key_column_required": lambda node_key: f"({node_key}): Se requiere la lista de columnas clave",
-                    "frequency_column_required": lambda node_key: f"({node_key}): Se requiere 'Frecuencia'",
-                    "properties_not_provided": lambda node_key: f"({node_key}): Debes proporcionar todas las propiedades",
-                },
-                "datetime_range": {
-                    "start_date_required": lambda node_key: f"({node_key}): Se requiere el campo 'Fecha Inicio'",
-                    "end_date_required": lambda node_key: f"({node_key}): Se requiere 'Fecha Fin'",
-                    "frequency_is_required": lambda node_key: f"({node_key}): Se requiere 'Frecuencia'",
-                    "properties_not_provided": lambda node_key: f"({node_key}): Debes proporcionar todas las propiedades",
-                },
-                "concat": {
-                    "column_required": lambda node_key, port: f"({node_key}): Debes mantener al menos un campo en la entrada '{port}'",
-                },
-                "corss_join": {
-                    "column_required": lambda node_key, port: f"({node_key}): Debes mantener al menos un campo en la entrada '{port}'",
-                },
-                "cumsum": {
-                    "aggregation_required": lambda node_key: f"({node_key}): Debes seleccionar al menos un método de agregación",
-                },
-                "cut": {
-                    "no_cutting_parameter": lambda node_key: f"({node_key}): No hay parámetro de corte",
-                    "no_type_cut": lambda node_key: f"({node_key}): El tipo de corte no existe",
-                },
-                "database_write": {
-                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
-                    "no_column_in_table": lambda node_key, column, table: f'({node_key}): La columna "{column}" no existe en la tabla "{table}"',
-                },
-                "database": {
-                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
-                },
-                "datetime_extract": {},
-                "datetime_formatter": {
-                    "pattern_quotes": lambda node_key: f"({node_key}): Usa comillas en el patrón personalizado",
-                    "pattern_required": lambda node_key: f"({node_key}): Debes seleccionar al menos un formato",
-                },
-                "describe": {},
-                "df_maker": {},
-                "email": {
-                    "config_required": lambda node_key, fields: f"({node_key}): Todos los campos deben ser completados. Campos faltantes {fields}",
-                    "failed_send": lambda node_key: f"({node_key}): No fue posible realizar el envío de email",
-                    "size_max": lambda node_key: f"({node_key}): No es posible enviar el correo ya que el tamaño de los archivos adjuntos supera el límite máximo",
-                },
-                "excel": {
-                    "failed_generate": lambda node_key: f"({node_key}): No fue posible generar el archivo excel",
-                    "output_path": lambda node_key: f"({node_key}): Seleccione directorio de salida",
-                },
-                "filter": {
-                    "rules": lambda node_key: f"({node_key}): Debes crear una regla",
-                    "unknow_rule": lambda node_key, rule: f"({node_key}): No se reconoce la regla '{rule}'",
-                    "failed_condition": lambda node_key: f"({node_key}): No fue posible procesar la condición",
-                    "unknow_column": lambda node_key, field: f"({node_key}): No existe la columna '{field}' en el Dataframe de entrada",
-                    "unknow_operator": lambda node_key, operator: f"({node_key}): Operador '{operator}' no reconocido ",
-                },
-                "group_by": {"missing_props": lambda node_key: f"({node_key}): Alguna de las propiedades para el método de agregación no ha sido proporcionada"},
-                "input_data": {
-                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' no existe o no es válida",
-                    "missing_extension": lambda node_key: f"({node_key}): No existe extensión del archivo",
-                    "file_not_exist": lambda node_key, path: f"({node_key}): Archivo '{path}' no existe en disco",
-                    "unknow_format": lambda node_key, format: f"({node_key}): Formato '{format}' no reconocido",
-                    "end_start_spaces": lambda node_key: f"({node_key}): Archivo fuente contiene espacios al inicio o final del nombre de una o más columnas. Se ha corregido para la lectura",
-                },
-                "inter_row": {
-                    "fillna": lambda node_key: f"({node_key}): La función 'fillna', debes especificar el valor para los nulos",
-                },
-                "merge": {
-                    "input_port": lambda node_key: f"({node_key}): Puerto entrada iL o iR no conectado",
-                    "input_port_il": lambda node_key, col: f"({node_key}): La columna '{col}' no está en las columnas del Dataframe iL",
-                    "input_port_iR": lambda node_key, col: f"({node_key}): La columna '{col}' no está en las columnas del Dataframe iR",
-                },
-                "pivot": {
-                    "incompleted_fields": lambda node_key, missing: f"({node_key}): Faltan campos de la configuración. Campos faltantes: {missing}",
-                },
-                "rolling": {
-                    "column_required": lambda node_key: f"({node_key}): Column is required",
-                    "operation_required": lambda node_key: f"({node_key}): Operation is required",
-                    "properties_not_provided": lambda node_key: f"({node_key}): Algunas de las propiedades no han sido proporcionadas",
-                },
-                "sample": {"sample_size": lambda node_key: f"({node_key}) Debes ingresar un tamaño de muestra válida mayor a 0"},
-                "split": {
-                    "default_value": lambda node_key: f"({node_key}): No existe Valor o Columna por defecto",
-                },
-                "switch": {
-                    "default_value": lambda node_key: f"({node_key}): Default Value no existe o es vacío",
-                    "no_column_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
-                    "no_conditions": lambda node_key, caseIdx: f"({node_key}): No existe condiciones para el caso {caseIdx}",
-                    "no_return_value": lambda node_key, caseIdx: f"({node_key}): No existe valor de salida para el caso {caseIdx}",
-                    "no_value_or_field": lambda node_key, caseIdx, conditionIdx: f"({node_key}): No existe valor para la condición {conditionIdx} del caso {caseIdx}",
-                    "missing_condition_prop": lambda node_key, prop, caseIdx, conditionIdx: f"({node_key}): No existe {prop} para la condición {conditionIdx} del caso {caseIdx}",
-                },
-                "database_utilities": {
-                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
-                    "check_missing_source": lambda node_key: f"({node_key}): El recurso de conexión no se encuentra",
-                    "check_fields_to_connection": lambda node_key, field: f"({node_key}): Falta la columna '{field}' para establecer la conexión",
-                    "check_empty_fields": lambda node_key, field: f"({node_key}): La columna '{field}' se encuentra vacía",
-                    "check_optional_fields": lambda node_key: f"({node_key}): Faltan campos para establecer conexión",
-                },
-                "deploy_enabled": lambda node_key: f"({node_key}): El deploy_mode está habilitado, pero deploy_path no existe en la configuración del nodo",
-                "exception": lambda node_key, error: f"({node_key}) Error: " + error,
-                "missing_column": lambda node_key: f"({node_key}): Debes seleccionar al menos una columna",
-                "empty_list": lambda node_key, name: f"({node_key}): Debes seleccionar al menos una opción de la lista de '{name}'",
-                "missing_specific_column": lambda node_key, column: f"({node_key}): Debes seleccionar la columna '{column}'",
-                "empty_df": lambda node_key, name: f"({node_key}): Dataframe de entrada {name} está vacío",
-                "missing_df": lambda node_key, name: f"({node_key}): No existe dataframe de entrada {name}",
-                "required_prop": lambda node_key, prop: f"({node_key}): El campo '{prop}' es obligatorio",
-            },
-            "builder": {
-                "reset_cache": lambda flow_name: f"Caché reseteada en flujo '{flow_name}'",
-                "nodes_in_cache": lambda q_nodes: f"'{q_nodes}' Nodos en caché",
-                "not_send": lambda node_key: f"Se omite envío para nodo '{node_key}'",
-                "skip_writing": lambda node_key: f"Se omite escritura de archivo para nodo '{node_key}'",
-                "parent_without_entry": lambda node_key: f"Se omite nodo '{node_key}' sin entrada padre",
-                "save_cache": lambda q_nodes: f"Se almacenaron '{q_nodes}' nodos en caché",
-                "processed_flow": lambda seconds: f"Flujo procesado en '{seconds}' segundos",
-                "stopped_flow": f"La ejecución del flujo ha sido interrumpida",
-                "exec_flow": "El flujo aún no se ha ejecutado",
-                "max_rows": lambda node_key, max_rows: f"({node_key}): Se ha exedido el máximo de filas permitido ({f'{max_rows:_}'.replace('_','.')})",
-            },
-        }
-
-    def dataviz_spanish(self):
-        return {
-            "data_source_reader": {
-                "not_memory_flow": lambda node_key, flow_name: f"La fuente de datos del nodo '{node_key}' en el flujo '{flow_name}' No está en memoria. Por favor ejecuta el flujo en el módulo Dataprep",
-                "no_such_file": lambda file_path: f"No se encuentró el archivo '{file_path}'",
-                "unspecified_extension": f"El archivo debe tener alguna extensión",
-                "invalid_extension": lambda extensions: f"Las extensiones permitidas son: '{extensions}'",
-            },
-            "data_frame_operator": {
-                "specified_operation": "Operación no especificada. Por favor selecciona alguna operación para la métrica.",
-                "invalid_operation": lambda operation, operation_dict: f"La operación '{operation}' es inválida'. Operaciones permitidas: '{operation_dict}'",
-                "field_numeric": lambda operation, field_name: f"La operación '{operation}' requiere que el campo '{field_name}' sea númerico",
-            },
-            "items": {
-                "scatter": {
-                    "non_numeric_xaxis": "La variable del eje x debe ser numérica",
-                    "non_numeric_yaxis": "La variable del eje y debe ser numérica",
-                }
-            }
-        }
-
-    def autots_spanish(self):
-        return {
-            "autots": {
-                "not_train": "Aún no se ha realizado el entrenamiento",
-                "not_path": lambda pickle: f"{pickle}: Ruta no existe",
-            },
-            "train": {},
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def automl_spanish(self):
-        return {
-            "automl": {
-                "not_train": "Aún no se ha realizado el entrenamiento",
-                "not_path": lambda pickle: f"{pickle}: Ruta no existe",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def handlers_spanish(self):
-        return {
-            "cache_handler": {
-                "node_cache_saved": lambda node_key: f"({node_key}) Almacenado en cache",
-                "node_ram_saved": lambda node_key: f"({node_key}) Almacenado en RAM",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def utils_spanish(self):
-        return {
-            "utilities": {
-                "sort_column_not_in_df": "Algunas columnas de orden no existen en la tabla de resultados",
-                "var_not_in_df": lambda prop: f"La columna '{prop}' no existe en el Dataframe",
-                "duplicated_columns": lambda columns: f"Se han corregido las siguientes columnas duplicadas: {columns}. Revise la configuración del nodo",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def worker_spanish(self):
-        return {
-            "listener": {
-                "automl": {
-                    "get_interaction": {
-                        "missing_property": lambda prop: f"Falta la propiedad '{prop}'",
-                    },
-                    "load_source": {
-                        "not_path": f"Falta la ruta del archivo",
-                    },
-                    "load_voutput": {
-                        "not_flow_cache": f"Flujo no cargado en caché",
-                    },
-                    "set_cache": {
-                        "not_flow_cache": f"Flujo no cargado en caché",
-                        "not_source": f"No existe fuente de datos",
-                    },
-                    "start_training": {
-                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
-                    },
-                },
-                "autots": {
-                    "get_interaction": {
-                        "missing_property": lambda prop: f"Falta la propiedad '{prop}'",
-                    },
-                    "load_source": {
-                        "not_path": f"Falta la ruta del archivo",
-                    },
-                    "load_voutput": {
-                        "not_flow_cache": f"Flujo no cargado en caché",
-                    },
-                    "set_cache": {
-                        "not_flow_cache": f"Flujo no cargado en caché",
-                        "not_source": f"No existe fuente de datos",
-                        "processing_error": lambda error: f"Error al intentar procesar: " + error,
-                    },
-                    "start_training": {
-                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
-                    },
-                },
-                "dataprep": {
-                    "node_output": {
-                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
-                    },
-                },
-            },
-            "exception": lambda error: f"Error: " + error,
-            "unexpected_error": "Ha ocurrido un error inesperado",
-        }
-
-    def service_spanish(self):
-        return {
-            "socket_listeners": {
-                "dataprep": {
-                    "database_connections": {
-                        "get_databases": {
-                            "get_database_error": lambda db, error: f"Error al obtener las Bases de Datos desde '{db}'\nError: {error}",
-                        },
-                        "get_projects": {
-                            "get_project_error": lambda db, error: f"Error al obtener los Proyectos desde '{db}'\nError: {error}",
-                        },
-                        "get_tables": {
-                            "get_table_error": lambda db, error: f"Error al obtener las Tablas desde '{db}'\nError: {error}",
-                        },
-                        "get_warehouses": {
-                            "get_warehouse_error": lambda db, error: f"Error al obtener los Almacenes desde '{db}'\nError: {error}",
-                        },
-                        "unknow_source": "El recurso no coincide con ninguno de la lista",
-                    }
-                }
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    # ===================================
-    # English
-    # ===================================
-    def dataprep_english(self):
-        return {
-            "nodes": {
-                "api_rest": {
-                    "no_method": lambda node_key: f"({node_key}): You must select a sending method",
-                    "no_url": lambda node_key: f"({node_key}): You must select a URL",
-                },
-                "code": {
-                    "no_vtg_codeout": lambda node_key: f"({node_key}): You must invoke the vtg_codeout(Df) function with your output DataFrame",
-                },
-                "column": {
-                    "no_columns_selected": lambda node_key: f"({node_key}): No columns selected",
-                    "rename_columns": lambda node_key: f"({node_key}): Could not rename columns",
-                    "column_not_in_df": lambda node_key, column: f"({node_key}): Column '{column}' does not exist in the Dataframe",
-                },
-                "dtype": {
-                    "no_columns_selected": lambda node_key: f"({node_key}): No columns selected",
-                    "rename_columns": lambda node_key: f"({node_key}): Could not rename columns",
-                    "column_not_in_df": lambda node_key, column: f"({node_key}): Column '{column}' does not exist in Dataframe",
-                    "change_dtype": lambda node_key, column, dtype: f"({node_key}): It was not possible to transform the column '{column}' data type to '{dtype}'",
-                    "unknow_dtype": lambda node_key, column, dtype: f"({node_key}): Unknown data type '{dtype}' in '{column}', it will be maintained as string",
-                },
-                "datetime_fill": {
-                    "time_column_required": lambda node_key: f"({node_key}): 'Time' column is required",
-                    "key_column_required": lambda node_key: f"({node_key}): Key columns list is required",
-                    "frequency_column_required": lambda node_key: f"({node_key}): 'Frequency' column is required",
-                    "properties_not_provided": lambda node_key: f"({node_key}): You must provide all properties",
-                },
-                "datetime_range": {
-                    "start_date_required": lambda node_key: f"({node_key}): Start Date field is required",
-                    "end_date_required": lambda node_key: f"({node_key}): End Date field is required",
-                    "frequency_is_required": lambda node_key: f"({node_key}): Frequency field is required",
-                    "properties_not_provided": lambda node_key: f"({node_key}): You must provide all properties",
-                },
-                "concat": {
-                    "column_required": lambda node_key, port: f"({node_key}): You must keep at least one field in the entry '{port}'",
-                },
-                "corss_join": {
-                    "column_required": lambda node_key, port: f"({node_key}): You must keep at least one field in the entry '{port}'",
-                },
-                "cumsum": {
-                    "aggregation_required": lambda node_key: f"({node_key}): You must select at least one aggregation method",
-                },
-                "cut": {
-                    "no_cutting_parameter": lambda node_key: f"({node_key}): There is no cutting parameter",
-                    "no_type_cut": lambda node_key: f"({node_key}): The type of cut does not exist",
-                },
-                "database_write": {
-                    "source_required": lambda node_key: f"({node_key}): You must select a connection resource",
-                    "no_column_in_table": lambda node_key, column, table: f'({node_key}): Column "{column}" does not exist in table "{table}"',
-                },
-                "database": {
-                    "source_required": lambda node_key: f"({node_key}): You must select a connection resource",
-                },
-                "datetime_extract": {},
-                "datetime_formatter": {
-                    "pattern_quotes": lambda node_key: f"({node_key}): Use quotes in custom pattern",
-                    "pattern_required": lambda node_key: f"({node_key}): You must select at least one format",
-                },
-                "describe": {},
-                "df_maker": {},
-                "email": {
-                    "config_required": lambda node_key, fields: f"({node_key}): All fields must be completed. Missing fields {fields}",
-                    "failed_send": lambda node_key: f"({node_key}): Email was not sent",
-                    "size_max": lambda node_key: f"({node_key}): Unable to send the email, the size of the attachments exceeds the maximum limit",
-                },
-                "excel": {
-                    "failed_generate": lambda node_key: f"({node_key}): It was not possible to generate the excel file",
-                    "output_path": lambda node_key: f"({node_key}): Select output directory",
-                },
-                "filter": {
-                    "rules": lambda node_key: f"({node_key}): You must create a Rule",
-                    "unknow_rule": lambda node_key, rule: f"({node_key}): The rule is not recognized '{rule}'",
-                    "failed_condition": lambda node_key: f"({node_key}): Condition could not be processed",
-                    "unknow_column": lambda node_key, field: f"({node_key}): Column '{field}' does not exist in the input Dataframe",
-                    "unknow_operator": lambda node_key, operator: f"({node_key}): Operator '{operator}' not recognized",
-                },
-                "group_by": {"missing_props": lambda node_key: f"({node_key}): Some of the properties of aggregate method have not been provided"},
-                "input_data": {
-                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' does not exist or does not valid",
-                    "missing_extension": lambda node_key: f"({node_key}): Does not exist extension",
-                    "file_not_exist": lambda node_key, path: f"({node_key}): File '{path}' does not exist on disk",
-                    "unknow_format": lambda node_key, format: f"({node_key}): Format '{format}' not recognized",
-                    "end_start_spaces": lambda node_key: f"({node_key}): Source file contains spaces at the beginning or end of the name of one or more columns. It has been corrected for reading",
-                },
-                "inter_row": {
-                    "fillna": lambda node_key: f"({node_key}): 'fillna' function, must specify the value for nulls",
-                },
-                "merge": {
-                    "input_port": lambda node_key: f"({node_key}): iL or iR input port not connected",
-                    "input_port_il": lambda node_key, col: f"({node_key}): Column '{col}' not contained in 'iL' Dataframe columns",
-                    "input_port_iR": lambda node_key, col: f"({node_key}): Column '{col}' not contained in 'iR' Dataframe columns",
-                },
-                "pivot": {
-                    "incompleted_fields": lambda node_key, missing: f"({node_key}): Empty fields in setting: '{missing}'",
-                },
-                "rolling": {
-                    "column_required": lambda node_key: f"({node_key}): Column is required",
-                    "operation_required": lambda node_key: f"({node_key}): Operation is required",
-                    "properties_not_provided": lambda node_key: f"({node_key}): Empty properties",
-                },
-                "sample": {"sample_size": lambda node_key: f"({node_key}) You must enter a valid sample size greater than 0"},
-                "split": {
-                    "default_value": lambda node_key: f"({node_key}): Default value does not exist",
-                },
-                "switch": {
-                    "default_value": lambda node_key: f"({node_key}): Default Value does not exist or is empty",
-                    "no_column_in_df": lambda node_key, column: f"({node_key}): The column '{column}' does not exist in the Dataframe",
-                    "no_return_value": lambda node_key, caseIdx: f"({node_key}): Return value does not exist for case {caseIdx}",
-                    "no_conditions": lambda node_key, caseIdx: f"({node_key}): Condition list does not exist for case {caseIdx}",
-                    "no_value_or_field": lambda node_key, caseIdx, conditionIdx: f"({node_key}): Value does not exist for condition {conditionIdx} of case {caseIdx}",
-                    "missing_condition_prop": lambda node_key, prop, caseIdx, conditionIdx: f"({node_key}): {prop} does not exist for condition {conditionIdx} of case {caseIdx}",
-                },
-                "database_utilities": {
-                    "source_required": lambda node_key: f"({node_key}): Select a connection resource",
-                    "check_missing_source": lambda node_key: f"({node_key}): Connection resource not found",
-                    "check_fields_to_connection": lambda node_key, field: f"({node_key}): Empty Column: '{field}'",
-                    "check_empty_fields": lambda node_key, field: f"({node_key}): Empty Column: '{field}'",
-                    "check_optional_fields": lambda node_key: f"({node_key}): Empty fields to establish connection",
-                },
-                "deploy_enabled": lambda node_key: f"({node_key}): 'deploy_mode' is enabled, but 'deploy_path' does not exist in the node configuration",
-                "exception": lambda node_key, error: f"({node_key}) Error: " + error,
-                "missing_column": lambda node_key: f"({node_key}): At least one column must be selected",
-                "empty_list": lambda node_key, name: f"({node_key}): Must select at least one option from the '{name}' list",
-                "missing_specific_column": lambda node_key, column: f"({node_key}): Must select the column '{column}'",
-                "empty_df": lambda node_key, name: f"({node_key}): Input dataframe {name} is empty",
-                "missing_df": lambda node_key, name: f"({node_key}): Input dataframe {name} does not exist",
-                "required_prop": lambda node_key, prop: f"({node_key}): The '{prop}' field is required",
-            },
-            "builder": {
-                "reset_cache": lambda flow_name: f"Reset cache in flow '{flow_name}'",
-                "nodes_in_cache": lambda q_nodes: f"'{q_nodes}' Cached nodes",
-                "not_send": lambda node_key: f"Sending is skipped for node '{node_key}'",
-                "skip_writing": lambda node_key: f"File write skipped for node '{node_key}'",
-                "parent_without_entry": lambda node_key: f"Node '{node_key}' is omitted without parent entry",
-                "save_cache": lambda q_nodes: f"'{q_nodes}' nodes were cached",
-                "processed_flow": lambda seconds: f"Stream processed in '{seconds}' seconds",
-                "stopped_flow": f"Flow execution has been stopped",
-                "exec_flow": "Flow has not run yet",
-                "max_rows": lambda node_key, max_rows: f"({node_key}): Maximum number of rows allowed has been exceeded ({f'{max_rows:_}'.replace('_','.')})",
-            },
-        }
-
-    def dataviz_english(self):
-        return {
-            "data_source_reader": {
-                "not_memory_flow": lambda node_key, flow_name: f"The data source of node '{node_key}' in flow '{flow_name}' is not in memory. Please Run the flow in the Dataprep module",
-                "no_such_file": lambda file_path: f"File '{file_path}' cannot be found",
-                "unspecified_extension": f"The file must have some extension",
-                "invalid_extension": lambda extensions: f"The allowed extensions are: '{extensions}'",
-            },
-            "data_frame_operator": {
-                "specified_operation": "Unspecified operation. Please select some operation for the metric.",
-                "invalid_operation": lambda operation, operation_dict: f"The operation '{operation}' is invalid'. Allowed operations: '{operation_dict}'",
-                "field_numeric": lambda operation, field_name: f"Operation '{operation}' requires field '{field_name}' to be numeric",
-            },
-            "items": {
-                "scatter": {
-                    "non_numeric_xaxis": "The x-axis variable must be numeric",
-                    "non_numeric_yaxis": "The y-axis variable must be numeric",
-                }
-            }
-        }
-
-    def autots_english(self):
-        return {
-            "autots": {
-                "not_train": "Training has not been done yet",
-                "not_path": lambda pickle: f"{pickle}: Route does not exist",
-            },
-            "train": {},
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def automl_english(self):
-        return {
-            "automl": {
-                "not_train": "Training has not been done yet",
-                "not_path": lambda pickle: f"{pickle}: Route does not exist",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def handlers_english(self):
-        return {
-            "cache_handler": {
-                "node_cache_saved": lambda node_key: f"({node_key}) Stored in cache",
-                "node_ram_saved": lambda node_key: f"({node_key}) Stored in RAM",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def utils_english(self):
-        return {
-            "utilities": {
-                "sort_column_not_in_df": "Some order columns do not exist in results table",
-                "var_not_in_df": lambda prop: f"Column '{prop}' is not in the Dataframe",
-                "duplicated_columns": lambda columns: f"Fixed the following duplicate columns: {columns}. Check node configuration",
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-    def worker_english(self):
-        return {
-            "listener": {
-                "automl": {
-                    "get_interaction": {
-                        "missing_property": lambda prop: f"Property '{prop}' is missing",
-                    },
-                    "load_source": {
-                        "not_path": f"File path is missing",
-                    },
-                    "load_voutput": {
-                        "not_flow_cache": f"Flow not loaded in cache",
-                    },
-                    "set_cache": {
-                        "not_flow_cache": f"Flow not loaded in cache",
-                        "not_source": f"There is no data source",
-                    },
-                    "start_training": {
-                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
-                    },
-                },
-                "autots": {
-                    "get_interaction": {
-                        "missing_property": lambda prop: f"Property '{prop}' is missing",
-                    },
-                    "load_source": {
-                        "not_path": f"File path is missing",
-                    },
-                    "load_voutput": {
-                        "not_flow_cache": f"Flow not loaded in cache",
-                    },
-                    "set_cache": {
-                        "not_flow_cache": f"Flow not loaded in cache",
-                        "not_source": f"There is no data source",
-                        "processing_error": lambda error: f"Error trying to process: " + error,
-                    },
-                    "start_training": {
-                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
-                    },
-                },
-                "dataprep": {
-                    "node_output": {
-                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
-                    },
-                },
-            },
-            "exception": lambda error: f"Error: " + error,
-            "unexpected_error": "An unexpected error has occurred",
-        }
-
-    def service_english(self):
-        return {
-            "socket_listeners": {
-                "dataprep": {
-                    "database_connections": {
-                        "get_databases": {
-                            "get_database_error": lambda db, error: f"Error obtaining Databases from '{db}'\nError: {error}",
-                        },
-                        "get_projects": {
-                            "get_project_error": lambda db, error: f"Error getting Projects from '{db}'\nError: {error}",
-                        },
-                        "get_tables": {
-                            "get_table_error": lambda db, error: f"Error getting Tables from '{db}'\nError: {error}",
-                        },
-                        "get_warehouses": {
-                            "get_warehouse_error": lambda db, error: f"Error getting Stores from '{db}'\nError: {error}",
-                        },
-                        "unknow_source": "The resource does not match any in the list",
-                    }
-                }
-            },
-            "exception": lambda error: f"Error: " + error,
-        }
-
-
-app_message = __AppMessage("es")
+# TODO: Importar el language acá
+
+
+class __AppMessage:
+    def __init__(self, languaje):
+        if languaje == "es":
+            self.dataprep = self.dataprep_spanish()
+            self.dataviz = self.dataviz_spanish()
+            self.autots = self.autots_spanish()
+            self.automl = self.automl_spanish()
+            self.handlers = self.handlers_spanish()
+            self.utils = self.utils_spanish()
+            self.worker = self.worker_spanish()
+            self.service = self.service_spanish()
+        else:
+            self.dataprep = self.dataprep_english()
+            self.dataviz = self.dataviz_english()
+            self.autots = self.autots_english()
+            self.automl = self.automl_english()
+            self.handlers = self.handlers_english()
+            self.utils = self.utils_english()
+            self.worker = self.worker_english()
+            self.service = self.service_english()
+
+    # ===================================
+    # Spanish
+    # ===================================
+    def dataprep_spanish(self):
+        return {
+            "nodes": {
+                "api_rest": {
+                    "no_method": lambda node_key: f"({node_key}): Debes seleccionar un método de envío",
+                    "no_url": lambda node_key: f"({node_key}): Debes seleccionar una URL",
+                },
+                "code": {
+                    "no_vtg_codeout": lambda node_key: f"({node_key}): Debes llamar a la función vtg_codeout(Df) con tu DataFrame de salida",
+                },
+                "column": {
+                    "no_columns_selected": lambda node_key: f"({node_key}): No hay columnas seleccionadas",
+                    "rename_columns": lambda node_key: f"({node_key}): No fue posible renombrar las columnas",
+                    "column_not_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
+                },
+                "dtype": {
+                    "no_columns_selected": lambda node_key: f"({node_key}): No hay columnas seleccionadas",
+                    "rename_columns": lambda node_key: f"({node_key}): No fue posible renombrar las columnas",
+                    "column_not_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
+                    "change_dtype": lambda node_key, column, dtype: f"({node_key}): No fue posible transformar el tipo de dato de la columna '{column}' a '{dtype}'",
+                    "unknow_dtype": lambda node_key, column, dtype: f"({node_key}): Tipo de dato '{dtype}' desconocido. Columna '{column}' se mantiene como string",
+                },
+                "datetime_fill": {
+                    "time_column_required": lambda node_key: f"({node_key}): La columna 'Tiempo' es obligatoria",
+                    "key_column_required": lambda node_key: f"({node_key}): Se requiere la lista de columnas clave",
+                    "frequency_column_required": lambda node_key: f"({node_key}): Se requiere 'Frecuencia'",
+                    "properties_not_provided": lambda node_key: f"({node_key}): Debes proporcionar todas las propiedades",
+                },
+                "datetime_range": {
+                    "start_date_required": lambda node_key: f"({node_key}): Se requiere el campo 'Fecha Inicio'",
+                    "end_date_required": lambda node_key: f"({node_key}): Se requiere 'Fecha Fin'",
+                    "frequency_is_required": lambda node_key: f"({node_key}): Se requiere 'Frecuencia'",
+                    "properties_not_provided": lambda node_key: f"({node_key}): Debes proporcionar todas las propiedades",
+                },
+                "concat": {
+                    "column_required": lambda node_key, port: f"({node_key}): Debes mantener al menos un campo en la entrada '{port}'",
+                },
+                "corss_join": {
+                    "column_required": lambda node_key, port: f"({node_key}): Debes mantener al menos un campo en la entrada '{port}'",
+                },
+                "cumsum": {
+                    "aggregation_required": lambda node_key: f"({node_key}): Debes seleccionar al menos un método de agregación",
+                },
+                "cut": {
+                    "no_cutting_parameter": lambda node_key: f"({node_key}): No hay parámetro de corte",
+                    "no_type_cut": lambda node_key: f"({node_key}): El tipo de corte no existe",
+                },
+                "database_write": {
+                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
+                    "no_column_in_table": lambda node_key, column, table: f'({node_key}): La columna "{column}" no existe en la tabla "{table}"',
+                },
+                "database": {
+                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
+                },
+                "datetime_extract": {},
+                "datetime_formatter": {
+                    "pattern_quotes": lambda node_key: f"({node_key}): Usa comillas en el patrón personalizado",
+                    "pattern_required": lambda node_key: f"({node_key}): Debes seleccionar al menos un formato",
+                },
+                "describe": {},
+                "df_maker": {},
+                "email": {
+                    "config_required": lambda node_key, fields: f"({node_key}): Todos los campos deben ser completados. Campos faltantes {fields}",
+                    "failed_send": lambda node_key: f"({node_key}): No fue posible realizar el envío de email",
+                    "size_max": lambda node_key: f"({node_key}): No es posible enviar el correo ya que el tamaño de los archivos adjuntos supera el límite máximo",
+                },
+                "excel": {
+                    "failed_generate": lambda node_key: f"({node_key}): No fue posible generar el archivo excel",
+                    "output_path": lambda node_key: f"({node_key}): Seleccione directorio de salida",
+                },
+                "filter": {
+                    "rules": lambda node_key: f"({node_key}): Debes crear una regla",
+                    "unknow_rule": lambda node_key, rule: f"({node_key}): No se reconoce la regla '{rule}'",
+                    "failed_condition": lambda node_key: f"({node_key}): No fue posible procesar la condición",
+                    "unknow_column": lambda node_key, field: f"({node_key}): No existe la columna '{field}' en el Dataframe de entrada",
+                    "unknow_operator": lambda node_key, operator: f"({node_key}): Operador '{operator}' no reconocido ",
+                },
+                "group_by": {"missing_props": lambda node_key: f"({node_key}): Alguna de las propiedades para el método de agregación no ha sido proporcionada"},
+                "input_data": {
+                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' no existe o no es válida",
+                    "missing_extension": lambda node_key: f"({node_key}): No existe extensión del archivo",
+                    "file_not_exist": lambda node_key, path: f"({node_key}): Archivo '{path}' no existe en disco",
+                    "unknow_format": lambda node_key, format: f"({node_key}): Formato '{format}' no reconocido",
+                    "end_start_spaces": lambda node_key: f"({node_key}): Archivo fuente contiene espacios al inicio o final del nombre de una o más columnas. Se ha corregido para la lectura",
+                },
+                "inter_row": {
+                    "fillna": lambda node_key: f"({node_key}): La función 'fillna', debes especificar el valor para los nulos",
+                },
+                "merge": {
+                    "input_port": lambda node_key: f"({node_key}): Puerto entrada iL o iR no conectado",
+                    "input_port_il": lambda node_key, col: f"({node_key}): La columna '{col}' no está en las columnas del Dataframe iL",
+                    "input_port_iR": lambda node_key, col: f"({node_key}): La columna '{col}' no está en las columnas del Dataframe iR",
+                },
+                "pivot": {
+                    "incompleted_fields": lambda node_key, missing: f"({node_key}): Faltan campos de la configuración. Campos faltantes: {missing}",
+                },
+                "rolling": {
+                    "column_required": lambda node_key: f"({node_key}): Column is required",
+                    "operation_required": lambda node_key: f"({node_key}): Operation is required",
+                    "properties_not_provided": lambda node_key: f"({node_key}): Algunas de las propiedades no han sido proporcionadas",
+                },
+                "sample": {"sample_size": lambda node_key: f"({node_key}) Debes ingresar un tamaño de muestra válida mayor a 0"},
+                "split": {
+                    "default_value": lambda node_key: f"({node_key}): No existe Valor o Columna por defecto",
+                },
+                "switch": {
+                    "default_value": lambda node_key: f"({node_key}): Default Value no existe o es vacío",
+                    "no_column_in_df": lambda node_key, column: f"({node_key}): La columna '{column}' no existe en el Dataframe",
+                    "no_conditions": lambda node_key, caseIdx: f"({node_key}): No existe condiciones para el caso {caseIdx}",
+                    "no_return_value": lambda node_key, caseIdx: f"({node_key}): No existe valor de salida para el caso {caseIdx}",
+                    "no_value_or_field": lambda node_key, caseIdx, conditionIdx: f"({node_key}): No existe valor para la condición {conditionIdx} del caso {caseIdx}",
+                    "missing_condition_prop": lambda node_key, prop, caseIdx, conditionIdx: f"({node_key}): No existe {prop} para la condición {conditionIdx} del caso {caseIdx}",
+                },
+                "database_utilities": {
+                    "source_required": lambda node_key: f"({node_key}): Debes seleccionar un recurso de conexión",
+                    "check_missing_source": lambda node_key: f"({node_key}): El recurso de conexión no se encuentra",
+                    "check_fields_to_connection": lambda node_key, field: f"({node_key}): Falta la columna '{field}' para establecer la conexión",
+                    "check_empty_fields": lambda node_key, field: f"({node_key}): La columna '{field}' se encuentra vacía",
+                    "check_optional_fields": lambda node_key: f"({node_key}): Faltan campos para establecer conexión",
+                },
+                "deploy_enabled": lambda node_key: f"({node_key}): El deploy_mode está habilitado, pero deploy_path no existe en la configuración del nodo",
+                "exception": lambda node_key, error: f"({node_key}) Error: " + error,
+                "missing_column": lambda node_key: f"({node_key}): Debes seleccionar al menos una columna",
+                "empty_list": lambda node_key, name: f"({node_key}): Debes seleccionar al menos una opción de la lista de '{name}'",
+                "missing_specific_column": lambda node_key, column: f"({node_key}): Debes seleccionar la columna '{column}'",
+                "empty_df": lambda node_key, name: f"({node_key}): Dataframe de entrada {name} está vacío",
+                "missing_df": lambda node_key, name: f"({node_key}): No existe dataframe de entrada {name}",
+                "required_prop": lambda node_key, prop: f"({node_key}): El campo '{prop}' es obligatorio",
+            },
+            "builder": {
+                "reset_cache": lambda flow_name: f"Caché reseteada en flujo '{flow_name}'",
+                "nodes_in_cache": lambda q_nodes: f"'{q_nodes}' Nodos en caché",
+                "not_send": lambda node_key: f"Se omite envío para nodo '{node_key}'",
+                "skip_writing": lambda node_key: f"Se omite escritura de archivo para nodo '{node_key}'",
+                "parent_without_entry": lambda node_key: f"Se omite nodo '{node_key}' sin entrada padre",
+                "save_cache": lambda q_nodes: f"Se almacenaron '{q_nodes}' nodos en caché",
+                "processed_flow": lambda seconds: f"Flujo procesado en '{seconds}' segundos",
+                "stopped_flow": f"La ejecución del flujo ha sido interrumpida",
+                "exec_flow": "El flujo aún no se ha ejecutado",
+                "max_rows": lambda node_key, max_rows: f"({node_key}): Se ha exedido el máximo de filas permitido ({f'{max_rows:_}'.replace('_','.')})",
+            },
+        }
+
+    def dataviz_spanish(self):
+        return {
+            "data_source_reader": {
+                "not_memory_flow": lambda node_key, flow_name: f"La fuente de datos del nodo '{node_key}' en el flujo '{flow_name}' No está en memoria. Por favor ejecuta el flujo en el módulo Dataprep",
+                "no_such_file": lambda file_path: f"No se encuentró el archivo '{file_path}'",
+                "unspecified_extension": f"El archivo debe tener alguna extensión",
+                "invalid_extension": lambda extensions: f"Las extensiones permitidas son: '{extensions}'",
+            },
+            "data_frame_operator": {
+                "specified_operation": "Operación no especificada. Por favor selecciona alguna operación para la métrica.",
+                "invalid_operation": lambda operation, operation_dict: f"La operación '{operation}' es inválida'. Operaciones permitidas: '{operation_dict}'",
+                "field_numeric": lambda operation, field_name: f"La operación '{operation}' requiere que el campo '{field_name}' sea númerico",
+            },
+            "items": {
+                "scatter": {
+                    "non_numeric_xaxis": "La variable del eje x debe ser numérica",
+                    "non_numeric_yaxis": "La variable del eje y debe ser numérica",
+                }
+            }
+        }
+
+    def autots_spanish(self):
+        return {
+            "autots": {
+                "not_train": "Aún no se ha realizado el entrenamiento",
+                "not_path": lambda pickle: f"{pickle}: Ruta no existe",
+            },
+            "train": {},
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def automl_spanish(self):
+        return {
+            "automl": {
+                "not_train": "Aún no se ha realizado el entrenamiento",
+                "not_path": lambda pickle: f"{pickle}: Ruta no existe",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def handlers_spanish(self):
+        return {
+            "cache_handler": {
+                "node_cache_saved": lambda node_key: f"({node_key}) Almacenado en cache",
+                "node_ram_saved": lambda node_key: f"({node_key}) Almacenado en RAM",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def utils_spanish(self):
+        return {
+            "utilities": {
+                "sort_column_not_in_df": "Algunas columnas de orden no existen en la tabla de resultados",
+                "var_not_in_df": lambda prop: f"La columna '{prop}' no existe en el Dataframe",
+                "duplicated_columns": lambda columns: f"Se han corregido las siguientes columnas duplicadas: {columns}. Revise la configuración del nodo",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def worker_spanish(self):
+        return {
+            "listener": {
+                "automl": {
+                    "get_interaction": {
+                        "missing_property": lambda prop: f"Falta la propiedad '{prop}'",
+                    },
+                    "load_source": {
+                        "not_path": f"Falta la ruta del archivo",
+                    },
+                    "load_voutput": {
+                        "not_flow_cache": f"Flujo no cargado en caché",
+                    },
+                    "set_cache": {
+                        "not_flow_cache": f"Flujo no cargado en caché",
+                        "not_source": f"No existe fuente de datos",
+                    },
+                    "start_training": {
+                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
+                    },
+                },
+                "autots": {
+                    "get_interaction": {
+                        "missing_property": lambda prop: f"Falta la propiedad '{prop}'",
+                    },
+                    "load_source": {
+                        "not_path": f"Falta la ruta del archivo",
+                    },
+                    "load_voutput": {
+                        "not_flow_cache": f"Flujo no cargado en caché",
+                    },
+                    "set_cache": {
+                        "not_flow_cache": f"Flujo no cargado en caché",
+                        "not_source": f"No existe fuente de datos",
+                        "processing_error": lambda error: f"Error al intentar procesar: " + error,
+                    },
+                    "start_training": {
+                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
+                    },
+                },
+                "dataprep": {
+                    "node_output": {
+                        "var_not_in_data": lambda prop: f"La variable '{prop}' no está en la data",
+                    },
+                },
+            },
+            "exception": lambda error: f"Error: " + error,
+            "unexpected_error": "Ha ocurrido un error inesperado",
+        }
+
+    def service_spanish(self):
+        return {
+            "socket_listeners": {
+                "dataprep": {
+                    "database_connections": {
+                        "get_databases": {
+                            "get_database_error": lambda db, error: f"Error al obtener las Bases de Datos desde '{db}'\nError: {error}",
+                        },
+                        "get_projects": {
+                            "get_project_error": lambda db, error: f"Error al obtener los Proyectos desde '{db}'\nError: {error}",
+                        },
+                        "get_tables": {
+                            "get_table_error": lambda db, error: f"Error al obtener las Tablas desde '{db}'\nError: {error}",
+                        },
+                        "get_warehouses": {
+                            "get_warehouse_error": lambda db, error: f"Error al obtener los Almacenes desde '{db}'\nError: {error}",
+                        },
+                        "unknow_source": "El recurso no coincide con ninguno de la lista",
+                    }
+                }
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    # ===================================
+    # English
+    # ===================================
+    def dataprep_english(self):
+        return {
+            "nodes": {
+                "api_rest": {
+                    "no_method": lambda node_key: f"({node_key}): You must select a sending method",
+                    "no_url": lambda node_key: f"({node_key}): You must select a URL",
+                },
+                "code": {
+                    "no_vtg_codeout": lambda node_key: f"({node_key}): You must invoke the vtg_codeout(Df) function with your output DataFrame",
+                },
+                "column": {
+                    "no_columns_selected": lambda node_key: f"({node_key}): No columns selected",
+                    "rename_columns": lambda node_key: f"({node_key}): Could not rename columns",
+                    "column_not_in_df": lambda node_key, column: f"({node_key}): Column '{column}' does not exist in the Dataframe",
+                },
+                "dtype": {
+                    "no_columns_selected": lambda node_key: f"({node_key}): No columns selected",
+                    "rename_columns": lambda node_key: f"({node_key}): Could not rename columns",
+                    "column_not_in_df": lambda node_key, column: f"({node_key}): Column '{column}' does not exist in Dataframe",
+                    "change_dtype": lambda node_key, column, dtype: f"({node_key}): It was not possible to transform the column '{column}' data type to '{dtype}'",
+                    "unknow_dtype": lambda node_key, column, dtype: f"({node_key}): Unknown data type '{dtype}' in '{column}', it will be maintained as string",
+                },
+                "datetime_fill": {
+                    "time_column_required": lambda node_key: f"({node_key}): 'Time' column is required",
+                    "key_column_required": lambda node_key: f"({node_key}): Key columns list is required",
+                    "frequency_column_required": lambda node_key: f"({node_key}): 'Frequency' column is required",
+                    "properties_not_provided": lambda node_key: f"({node_key}): You must provide all properties",
+                },
+                "datetime_range": {
+                    "start_date_required": lambda node_key: f"({node_key}): Start Date field is required",
+                    "end_date_required": lambda node_key: f"({node_key}): End Date field is required",
+                    "frequency_is_required": lambda node_key: f"({node_key}): Frequency field is required",
+                    "properties_not_provided": lambda node_key: f"({node_key}): You must provide all properties",
+                },
+                "concat": {
+                    "column_required": lambda node_key, port: f"({node_key}): You must keep at least one field in the entry '{port}'",
+                },
+                "corss_join": {
+                    "column_required": lambda node_key, port: f"({node_key}): You must keep at least one field in the entry '{port}'",
+                },
+                "cumsum": {
+                    "aggregation_required": lambda node_key: f"({node_key}): You must select at least one aggregation method",
+                },
+                "cut": {
+                    "no_cutting_parameter": lambda node_key: f"({node_key}): There is no cutting parameter",
+                    "no_type_cut": lambda node_key: f"({node_key}): The type of cut does not exist",
+                },
+                "database_write": {
+                    "source_required": lambda node_key: f"({node_key}): You must select a connection resource",
+                    "no_column_in_table": lambda node_key, column, table: f'({node_key}): Column "{column}" does not exist in table "{table}"',
+                },
+                "database": {
+                    "source_required": lambda node_key: f"({node_key}): You must select a connection resource",
+                },
+                "datetime_extract": {},
+                "datetime_formatter": {
+                    "pattern_quotes": lambda node_key: f"({node_key}): Use quotes in custom pattern",
+                    "pattern_required": lambda node_key: f"({node_key}): You must select at least one format",
+                },
+                "describe": {},
+                "df_maker": {},
+                "email": {
+                    "config_required": lambda node_key, fields: f"({node_key}): All fields must be completed. Missing fields {fields}",
+                    "failed_send": lambda node_key: f"({node_key}): Email was not sent",
+                    "size_max": lambda node_key: f"({node_key}): Unable to send the email, the size of the attachments exceeds the maximum limit",
+                },
+                "excel": {
+                    "failed_generate": lambda node_key: f"({node_key}): It was not possible to generate the excel file",
+                    "output_path": lambda node_key: f"({node_key}): Select output directory",
+                },
+                "filter": {
+                    "rules": lambda node_key: f"({node_key}): You must create a Rule",
+                    "unknow_rule": lambda node_key, rule: f"({node_key}): The rule is not recognized '{rule}'",
+                    "failed_condition": lambda node_key: f"({node_key}): Condition could not be processed",
+                    "unknow_column": lambda node_key, field: f"({node_key}): Column '{field}' does not exist in the input Dataframe",
+                    "unknow_operator": lambda node_key, operator: f"({node_key}): Operator '{operator}' not recognized",
+                },
+                "group_by": {"missing_props": lambda node_key: f"({node_key}): Some of the properties of aggregate method have not been provided"},
+                "input_data": {
+                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' does not exist or does not valid",
+                    "missing_extension": lambda node_key: f"({node_key}): Does not exist extension",
+                    "file_not_exist": lambda node_key, path: f"({node_key}): File '{path}' does not exist on disk",
+                    "unknow_format": lambda node_key, format: f"({node_key}): Format '{format}' not recognized",
+                    "end_start_spaces": lambda node_key: f"({node_key}): Source file contains spaces at the beginning or end of the name of one or more columns. It has been corrected for reading",
+                },
+                "inter_row": {
+                    "fillna": lambda node_key: f"({node_key}): 'fillna' function, must specify the value for nulls",
+                },
+                "merge": {
+                    "input_port": lambda node_key: f"({node_key}): iL or iR input port not connected",
+                    "input_port_il": lambda node_key, col: f"({node_key}): Column '{col}' not contained in 'iL' Dataframe columns",
+                    "input_port_iR": lambda node_key, col: f"({node_key}): Column '{col}' not contained in 'iR' Dataframe columns",
+                },
+                "pivot": {
+                    "incompleted_fields": lambda node_key, missing: f"({node_key}): Empty fields in setting: '{missing}'",
+                },
+                "rolling": {
+                    "column_required": lambda node_key: f"({node_key}): Column is required",
+                    "operation_required": lambda node_key: f"({node_key}): Operation is required",
+                    "properties_not_provided": lambda node_key: f"({node_key}): Empty properties",
+                },
+                "sample": {"sample_size": lambda node_key: f"({node_key}) You must enter a valid sample size greater than 0"},
+                "split": {
+                    "default_value": lambda node_key: f"({node_key}): Default value does not exist",
+                },
+                "switch": {
+                    "default_value": lambda node_key: f"({node_key}): Default Value does not exist or is empty",
+                    "no_column_in_df": lambda node_key, column: f"({node_key}): The column '{column}' does not exist in the Dataframe",
+                    "no_return_value": lambda node_key, caseIdx: f"({node_key}): Return value does not exist for case {caseIdx}",
+                    "no_conditions": lambda node_key, caseIdx: f"({node_key}): Condition list does not exist for case {caseIdx}",
+                    "no_value_or_field": lambda node_key, caseIdx, conditionIdx: f"({node_key}): Value does not exist for condition {conditionIdx} of case {caseIdx}",
+                    "missing_condition_prop": lambda node_key, prop, caseIdx, conditionIdx: f"({node_key}): {prop} does not exist for condition {conditionIdx} of case {caseIdx}",
+                },
+                "database_utilities": {
+                    "source_required": lambda node_key: f"({node_key}): Select a connection resource",
+                    "check_missing_source": lambda node_key: f"({node_key}): Connection resource not found",
+                    "check_fields_to_connection": lambda node_key, field: f"({node_key}): Empty Column: '{field}'",
+                    "check_empty_fields": lambda node_key, field: f"({node_key}): Empty Column: '{field}'",
+                    "check_optional_fields": lambda node_key: f"({node_key}): Empty fields to establish connection",
+                },
+                "deploy_enabled": lambda node_key: f"({node_key}): 'deploy_mode' is enabled, but 'deploy_path' does not exist in the node configuration",
+                "exception": lambda node_key, error: f"({node_key}) Error: " + error,
+                "missing_column": lambda node_key: f"({node_key}): At least one column must be selected",
+                "empty_list": lambda node_key, name: f"({node_key}): Must select at least one option from the '{name}' list",
+                "missing_specific_column": lambda node_key, column: f"({node_key}): Must select the column '{column}'",
+                "empty_df": lambda node_key, name: f"({node_key}): Input dataframe {name} is empty",
+                "missing_df": lambda node_key, name: f"({node_key}): Input dataframe {name} does not exist",
+                "required_prop": lambda node_key, prop: f"({node_key}): The '{prop}' field is required",
+            },
+            "builder": {
+                "reset_cache": lambda flow_name: f"Reset cache in flow '{flow_name}'",
+                "nodes_in_cache": lambda q_nodes: f"'{q_nodes}' Cached nodes",
+                "not_send": lambda node_key: f"Sending is skipped for node '{node_key}'",
+                "skip_writing": lambda node_key: f"File write skipped for node '{node_key}'",
+                "parent_without_entry": lambda node_key: f"Node '{node_key}' is omitted without parent entry",
+                "save_cache": lambda q_nodes: f"'{q_nodes}' nodes were cached",
+                "processed_flow": lambda seconds: f"Stream processed in '{seconds}' seconds",
+                "stopped_flow": f"Flow execution has been stopped",
+                "exec_flow": "Flow has not run yet",
+                "max_rows": lambda node_key, max_rows: f"({node_key}): Maximum number of rows allowed has been exceeded ({f'{max_rows:_}'.replace('_','.')})",
+            },
+        }
+
+    def dataviz_english(self):
+        return {
+            "data_source_reader": {
+                "not_memory_flow": lambda node_key, flow_name: f"The data source of node '{node_key}' in flow '{flow_name}' is not in memory. Please Run the flow in the Dataprep module",
+                "no_such_file": lambda file_path: f"File '{file_path}' cannot be found",
+                "unspecified_extension": f"The file must have some extension",
+                "invalid_extension": lambda extensions: f"The allowed extensions are: '{extensions}'",
+            },
+            "data_frame_operator": {
+                "specified_operation": "Unspecified operation. Please select some operation for the metric.",
+                "invalid_operation": lambda operation, operation_dict: f"The operation '{operation}' is invalid'. Allowed operations: '{operation_dict}'",
+                "field_numeric": lambda operation, field_name: f"Operation '{operation}' requires field '{field_name}' to be numeric",
+            },
+            "items": {
+                "scatter": {
+                    "non_numeric_xaxis": "The x-axis variable must be numeric",
+                    "non_numeric_yaxis": "The y-axis variable must be numeric",
+                }
+            }
+        }
+
+    def autots_english(self):
+        return {
+            "autots": {
+                "not_train": "Training has not been done yet",
+                "not_path": lambda pickle: f"{pickle}: Route does not exist",
+            },
+            "train": {},
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def automl_english(self):
+        return {
+            "automl": {
+                "not_train": "Training has not been done yet",
+                "not_path": lambda pickle: f"{pickle}: Route does not exist",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def handlers_english(self):
+        return {
+            "cache_handler": {
+                "node_cache_saved": lambda node_key: f"({node_key}) Stored in cache",
+                "node_ram_saved": lambda node_key: f"({node_key}) Stored in RAM",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def utils_english(self):
+        return {
+            "utilities": {
+                "sort_column_not_in_df": "Some order columns do not exist in results table",
+                "var_not_in_df": lambda prop: f"Column '{prop}' is not in the Dataframe",
+                "duplicated_columns": lambda columns: f"Fixed the following duplicate columns: {columns}. Check node configuration",
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+    def worker_english(self):
+        return {
+            "listener": {
+                "automl": {
+                    "get_interaction": {
+                        "missing_property": lambda prop: f"Property '{prop}' is missing",
+                    },
+                    "load_source": {
+                        "not_path": f"File path is missing",
+                    },
+                    "load_voutput": {
+                        "not_flow_cache": f"Flow not loaded in cache",
+                    },
+                    "set_cache": {
+                        "not_flow_cache": f"Flow not loaded in cache",
+                        "not_source": f"There is no data source",
+                    },
+                    "start_training": {
+                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
+                    },
+                },
+                "autots": {
+                    "get_interaction": {
+                        "missing_property": lambda prop: f"Property '{prop}' is missing",
+                    },
+                    "load_source": {
+                        "not_path": f"File path is missing",
+                    },
+                    "load_voutput": {
+                        "not_flow_cache": f"Flow not loaded in cache",
+                    },
+                    "set_cache": {
+                        "not_flow_cache": f"Flow not loaded in cache",
+                        "not_source": f"There is no data source",
+                        "processing_error": lambda error: f"Error trying to process: " + error,
+                    },
+                    "start_training": {
+                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
+                    },
+                },
+                "dataprep": {
+                    "node_output": {
+                        "var_not_in_data": lambda prop: f"The variable '{prop}' is not in the data",
+                    },
+                },
+            },
+            "exception": lambda error: f"Error: " + error,
+            "unexpected_error": "An unexpected error has occurred",
+        }
+
+    def service_english(self):
+        return {
+            "socket_listeners": {
+                "dataprep": {
+                    "database_connections": {
+                        "get_databases": {
+                            "get_database_error": lambda db, error: f"Error obtaining Databases from '{db}'\nError: {error}",
+                        },
+                        "get_projects": {
+                            "get_project_error": lambda db, error: f"Error getting Projects from '{db}'\nError: {error}",
+                        },
+                        "get_tables": {
+                            "get_table_error": lambda db, error: f"Error getting Tables from '{db}'\nError: {error}",
+                        },
+                        "get_warehouses": {
+                            "get_warehouse_error": lambda db, error: f"Error getting Stores from '{db}'\nError: {error}",
+                        },
+                        "unknow_source": "The resource does not match any in the list",
+                    }
+                }
+            },
+            "exception": lambda error: f"Error: " + error,
+        }
+
+
+app_message = __AppMessage("es")
```

### Comparing `vtarget-0.8.6/vtarget/utils/__init__.py` & `vtarget-0.8.7/vtarget/utils/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import os as __os
-from typing import Union
-
-TEMP_DIR = __os.environ.get("TMPDIR")
-if TEMP_DIR is None:
-    TEMP_DIR = __os.environ.get("TEMP")
-if TEMP_DIR is None:
-    TEMP_DIR = __os.environ.get("TMP")
-if TEMP_DIR is None:
-    TEMP_DIR = "."
-
-
-def dprint(*args, **kwargs):
-    import traceback
-
-    """
-    Pre-pends the filename and linenumber to the print statement
-    """
-    try:
-        stack = traceback.extract_stack()[:-1]
-        last = stack[-1]
-
-        # Handle different versions of the traceback module
-        if hasattr(last, "filename"):
-            _filename = last.filename.split("lib")
-            filename = "lib".join(_filename[1:])[1:] if len(_filename) >= 2 else last.filename
-            out_str = f"\t\033[90m{filename}:{last.lineno}\033[0m"
-        else:
-            _filename = last[0].split("lib")
-            filename = "lib".join(_filename[1:])[1:] if len(_filename) >= 2 else last[0]
-            out_str = f"\t\033[90m{filename}:{last[1]}\033[0m"
-
-        # Prepend the filename and linenumber
-        __builtins__["oldprint"](*args, out_str, **kwargs)
-    except:
-        __builtins__["oldprint"](*args, **kwargs)
-
-
-def override():
-    if "oldprint" not in __builtins__:
-        __builtins__["oldprint"] = __builtins__["print"]
-
-    __builtins__["print"] = dprint
-
-
-def regpid(target: str = None):
-    import os
-
-    id = 0
-
-    if target is None or len(target) == 0:
-        vtarget_pids_path = os.path.join(TEMP_DIR, "vtarget-pids")
-
-    else:
-        vtarget_pids_path = os.path.join(TEMP_DIR, f"vtarget-{target}-pids")
-
-    print(vtarget_pids_path)
-
-    with open(vtarget_pids_path, "a+") as f:
-        id = os.getpid()
-        f.write(f"{id}\n")
-    return id
-
-
-def syspath():
-    import sys
-
-    if getattr(sys, "frozen", False):
-        import os
-
-        current_path = os.path.dirname(sys.executable)
-        sys.path.insert(0, os.path.join(current_path, "python"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib", "site-packages"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3", "site-packages"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.10", "site-packages"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.11", "site-packages"))
-        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.12", "site-packages"))
-        sys.path.insert(0, os.path.join(current_path, "python", "DLLs"))
-
-
-def get_serial_number() -> Union[bytes, None]:
-    import platform
-    import subprocess
-    import uuid
-
-    os_type = platform.system()
-    try:
-        if os_type == "Windows":
-            result = subprocess.check_output("wmic bios get serialnumber", shell=True)
-            result = result.decode("utf-8").strip().split("\n")[1]
-            return result
-        elif os_type == "Linux":
-            result = subprocess.check_output("dmidecode -s system-serial-number", shell=True)
-            result = result.decode("utf-8").strip()
-            return result
-        elif os_type == "Darwin":
-            result = subprocess.check_output("system_profiler SPHardwareDataType", shell=True)
-            result = result.decode("utf-8").strip()
-            lines = result.split("\n")
-            serial_number_line = [line for line in lines if "Serial Number" in line][0]
-            serial_number = serial_number_line.split(":")[-1].strip()
-            return serial_number
-        else:
-            raise Exception(os_type)
-    except:
-        mac_address = hex(uuid.getnode()).replace("0x", "").upper()
-        mac_address = ":".join(mac_address[i : i + 2] for i in range(0, 11, 2))
-        return f"Dirección MAC en uso: {mac_address}"
-
-
-def normpath(path: str) -> str:
-    import os
-
-    parts = path.split(r"[\\\/]")
-
-    return os.path.join(*parts)
-
-
-def trace_error():
-    import sys
-    import traceback
-
-    c, e, t = sys.exc_info()
-    error = f"{c.__name__}: {e}"
-    tb = [f"{s.filename}:{s.lineno}" for s in traceback.extract_tb(t)]
-    return error, tb
+import os as __os
+from typing import Union
+
+TEMP_DIR = __os.environ.get("TMPDIR")
+if TEMP_DIR is None:
+    TEMP_DIR = __os.environ.get("TEMP")
+if TEMP_DIR is None:
+    TEMP_DIR = __os.environ.get("TMP")
+if TEMP_DIR is None:
+    TEMP_DIR = "."
+
+
+def dprint(*args, **kwargs):
+    import traceback
+
+    """
+    Pre-pends the filename and linenumber to the print statement
+    """
+    try:
+        stack = traceback.extract_stack()[:-1]
+        last = stack[-1]
+
+        # Handle different versions of the traceback module
+        if hasattr(last, "filename"):
+            _filename = last.filename.split("lib")
+            filename = "lib".join(_filename[1:])[1:] if len(_filename) >= 2 else last.filename
+            out_str = f"\t\033[90m{filename}:{last.lineno}\033[0m"
+        else:
+            _filename = last[0].split("lib")
+            filename = "lib".join(_filename[1:])[1:] if len(_filename) >= 2 else last[0]
+            out_str = f"\t\033[90m{filename}:{last[1]}\033[0m"
+
+        # Prepend the filename and linenumber
+        __builtins__["oldprint"](*args, out_str, **kwargs)
+    except:
+        __builtins__["oldprint"](*args, **kwargs)
+
+
+def override():
+    if "oldprint" not in __builtins__:
+        __builtins__["oldprint"] = __builtins__["print"]
+
+    __builtins__["print"] = dprint
+
+
+def regpid(target: str = None):
+    import os
+
+    id = 0
+
+    if target is None or len(target) == 0:
+        vtarget_pids_path = os.path.join(TEMP_DIR, "vtarget-pids")
+
+    else:
+        vtarget_pids_path = os.path.join(TEMP_DIR, f"vtarget-{target}-pids")
+
+    print(vtarget_pids_path)
+
+    with open(vtarget_pids_path, "a+") as f:
+        id = os.getpid()
+        f.write(f"{id}\n")
+    return id
+
+
+def syspath():
+    import sys
+
+    if getattr(sys, "frozen", False):
+        import os
+
+        current_path = os.path.dirname(sys.executable)
+        sys.path.insert(0, os.path.join(current_path, "python"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib", "site-packages"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3", "site-packages"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.10", "site-packages"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.11", "site-packages"))
+        sys.path.insert(0, os.path.join(current_path, "python", "lib", "python3.12", "site-packages"))
+        sys.path.insert(0, os.path.join(current_path, "python", "DLLs"))
+
+
+def get_serial_number() -> Union[bytes, None]:
+    import platform
+    import subprocess
+    import uuid
+
+    os_type = platform.system()
+    try:
+        if os_type == "Windows":
+            result = subprocess.check_output("wmic bios get serialnumber", shell=True)
+            result = result.decode("utf-8").strip().split("\n")[1]
+            return result
+        elif os_type == "Linux":
+            result = subprocess.check_output("dmidecode -s system-serial-number", shell=True)
+            result = result.decode("utf-8").strip()
+            return result
+        elif os_type == "Darwin":
+            result = subprocess.check_output("system_profiler SPHardwareDataType", shell=True)
+            result = result.decode("utf-8").strip()
+            lines = result.split("\n")
+            serial_number_line = [line for line in lines if "Serial Number" in line][0]
+            serial_number = serial_number_line.split(":")[-1].strip()
+            return serial_number
+        else:
+            raise Exception(os_type)
+    except:
+        mac_address = hex(uuid.getnode()).replace("0x", "").upper()
+        mac_address = ":".join(mac_address[i : i + 2] for i in range(0, 11, 2))
+        return f"Dirección MAC en uso: {mac_address}"
+
+
+def normpath(path: str) -> str:
+    import os
+
+    parts = path.split(r"[\\\/]")
+
+    return os.path.join(*parts)
+
+
+def trace_error():
+    import sys
+    import traceback
+
+    c, e, t = sys.exc_info()
+    error = f"{c.__name__}: {e}"
+    tb = [f"{s.filename}:{s.lineno}" for s in traceback.extract_tb(t)]
+    return error, tb
```

### Comparing `vtarget-0.8.6/vtarget/utils/calc_metrics.py` & `vtarget-0.8.7/vtarget/utils/calc_metrics.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import math
-
-import numpy as np
-from sklearn import metrics as skmetrics
-
-
-class CalcMetrics:
-    def __init__(self):
-        pass
-
-    def MASE(self, training_series, testing_series, prediction_series):
-        """
-        Computes the MEAN-ABSOLUTE SCALED ERROR forcast error for univariate time series prediction.
-
-        See "Another look at measures of forecast accuracy", Rob J Hyndman
-
-        parameters:
-                training_series: the series used to train the model, 1d numpy array
-                testing_series: the test series to predict, 1d numpy array or float
-                prediction_series: the prediction of testing_series, 1d numpy array (same size as testing_series) or float
-                absolute: "squares" to use sum of squares and root the result, "absolute" to use absolute values.
-
-        """
-        # print "Needs to be tested."
-        n = training_series.shape[0]
-        d = np.abs(np.diff(training_series)).sum() / (n - 1)
-
-        errors = np.abs(testing_series - prediction_series)
-        return errors.mean() / d
-
-    def main_ts_metrics(self, real, pred, train):
-        R2 = skmetrics.r2_score(real, pred)
-        MAPE = skmetrics.mean_absolute_percentage_error(real, pred)
-        MAE = skmetrics.mean_absolute_error(real, pred)
-        MSE = skmetrics.mean_squared_error(real, pred)
-
-        return {
-            "R2": R2,
-            "MAPE": MAPE,
-            "MAE": MAE,
-            "MSE": MSE,
-            "RMSE": math.sqrt(MSE),
-            "MASE": self.MASE(train, real, pred) if len(train) else None,
-        }
+import math
+
+import numpy as np
+from sklearn import metrics as skmetrics
+
+
+class CalcMetrics:
+    def __init__(self):
+        pass
+
+    def MASE(self, training_series, testing_series, prediction_series):
+        """
+        Computes the MEAN-ABSOLUTE SCALED ERROR forcast error for univariate time series prediction.
+
+        See "Another look at measures of forecast accuracy", Rob J Hyndman
+
+        parameters:
+                training_series: the series used to train the model, 1d numpy array
+                testing_series: the test series to predict, 1d numpy array or float
+                prediction_series: the prediction of testing_series, 1d numpy array (same size as testing_series) or float
+                absolute: "squares" to use sum of squares and root the result, "absolute" to use absolute values.
+
+        """
+        # print "Needs to be tested."
+        n = training_series.shape[0]
+        d = np.abs(np.diff(training_series)).sum() / (n - 1)
+
+        errors = np.abs(testing_series - prediction_series)
+        return errors.mean() / d
+
+    def main_ts_metrics(self, real, pred, train):
+        R2 = skmetrics.r2_score(real, pred)
+        MAPE = skmetrics.mean_absolute_percentage_error(real, pred)
+        MAE = skmetrics.mean_absolute_error(real, pred)
+        MSE = skmetrics.mean_squared_error(real, pred)
+
+        return {
+            "R2": R2,
+            "MAPE": MAPE,
+            "MAE": MAE,
+            "MSE": MSE,
+            "RMSE": math.sqrt(MSE),
+            "MASE": self.MASE(train, real, pred) if len(train) else None,
+        }
```

### Comparing `vtarget-0.8.6/vtarget/utils/database_connection/field_validation.py` & `vtarget-0.8.7/vtarget/utils/database_connection/field_validation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# TIER 1
-FIELD_VALIDATION_DATABASE = {
-    "oracle": {
-        "database": {
-            "required": ["host", "user", "service_name"],
-        },
-        "table": {"required": ["host", "user", "service_name", "database"]},
-        "data": {
-            "required": ["host", "user", "service_name", "database"],
-            "optional": [["table", "query"]],
-        },
-        "write_data": {"required": ["host", "user", "service_name", "database", "table", "save_type"]},
-    },
-    "sqlserver_2000": {
-        "database": {
-            "required": ["host", "user"],
-        },
-        "table": {"required": ["host", "user", "database"]},
-        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
-        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
-    },
-    "postgresql": {
-        "database": {
-            "required": ["host", "user"],
-        },
-        "table": {"required": ["host", "user", "database"]},
-        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
-        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
-    },
-    "mysql": {
-        "database": {"required": ["host", "user"]},
-        "table": {"required": ["host", "user", "database"]},
-        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
-        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
-    },
-    "mariadb": {
-        "database": {"required": ["host", "user"]},
-        "table": {"required": ["host", "user", "database"]},
-        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
-        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
-    },
-    "sqlite": {
-        "database": {"required": ["path"]},
-        "table": {"required": ["path"]},
-        "data": {"required": ["path"], "optional": [["table", "query"]]},
-        "write_data": {"required": ["path", "table", "save_type"]},
-    },
-    "mongodb": {
-        "database": {"required": ["mongo_client"]},
-        "table": {"required": ["mongo_client", "database"]},
-        "data": {"required": ["mongo_client", "database", "table"]},
-        "write_data": {"required": ["mongo_client", "database", "table", "save_type"]},
-    },
-    "bigquery": {
-        "project": {"required": ["service_account_host"]},
-        "database": {"required": ["service_account_host", "project"]},
-        "table": {"required": ["service_account_host", "project", "database"]},
-        "data": {"required": ["service_account_host", "project", "database", "table"]},
-        "write_data": {"required": ["service_account_host", "project", "database", "table", "save_type"]},
-    },
-    "snowflake": {
-        "project": {"required": ["account", "user", "password"]},
-        "database": {"required": ["account", "user", "password", "project"]},
-        "table": {"required": ["account", "user", "password", "project", "database"]},
-        "data": {
-            "required": ["account", "user", "password", "project", "database"],
-            "optional": [["table", "query"]],
-        },
-        "write_data": {"required": ["account", "user", "password", "project", "database", "table", "save_type"]},
-    },
-}
+# TIER 1
+FIELD_VALIDATION_DATABASE = {
+    "oracle": {
+        "database": {
+            "required": ["host", "user", "service_name"],
+        },
+        "table": {"required": ["host", "user", "service_name", "database"]},
+        "data": {
+            "required": ["host", "user", "service_name", "database"],
+            "optional": [["table", "query"]],
+        },
+        "write_data": {"required": ["host", "user", "service_name", "database", "table", "save_type"]},
+    },
+    "sqlserver_2000": {
+        "database": {
+            "required": ["host", "user"],
+        },
+        "table": {"required": ["host", "user", "database"]},
+        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
+        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
+    },
+    "postgresql": {
+        "database": {
+            "required": ["host", "user"],
+        },
+        "table": {"required": ["host", "user", "database"]},
+        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
+        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
+    },
+    "mysql": {
+        "database": {"required": ["host", "user"]},
+        "table": {"required": ["host", "user", "database"]},
+        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
+        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
+    },
+    "mariadb": {
+        "database": {"required": ["host", "user"]},
+        "table": {"required": ["host", "user", "database"]},
+        "data": {"required": ["host", "user", "database"], "optional": [["table", "query"]]},
+        "write_data": {"required": ["host", "user", "database", "table", "save_type"]},
+    },
+    "sqlite": {
+        "database": {"required": ["path"]},
+        "table": {"required": ["path"]},
+        "data": {"required": ["path"], "optional": [["table", "query"]]},
+        "write_data": {"required": ["path", "table", "save_type"]},
+    },
+    "mongodb": {
+        "database": {"required": ["mongo_client"]},
+        "table": {"required": ["mongo_client", "database"]},
+        "data": {"required": ["mongo_client", "database", "table"]},
+        "write_data": {"required": ["mongo_client", "database", "table", "save_type"]},
+    },
+    "bigquery": {
+        "project": {"required": ["service_account_host"]},
+        "database": {"required": ["service_account_host", "project"]},
+        "table": {"required": ["service_account_host", "project", "database"]},
+        "data": {"required": ["service_account_host", "project", "database", "table"]},
+        "write_data": {"required": ["service_account_host", "project", "database", "table", "save_type"]},
+    },
+    "snowflake": {
+        "project": {"required": ["account", "user", "password"]},
+        "database": {"required": ["account", "user", "password", "project"]},
+        "table": {"required": ["account", "user", "password", "project", "database"]},
+        "data": {
+            "required": ["account", "user", "password", "project", "database"],
+            "optional": [["table", "query"]],
+        },
+        "write_data": {"required": ["account", "user", "password", "project", "database", "table", "save_type"]},
+    },
+}
```

### Comparing `vtarget-0.8.6/vtarget/utils/database_connection/utilities.py` & `vtarget-0.8.7/vtarget/utils/database_connection/utilities.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from vtarget.language.app_message import app_message
-from vtarget.utils.database_connection.field_validation import FIELD_VALIDATION_DATABASE
-from vtarget.utils.encrypter import encrypter
-
-
-class Utilities:
-    def __init__(self):
-        pass
-
-    def check_fields(self, data: dict = dict(), tier: str = str(), node_key: str = str()) -> tuple:
-        """
-        Método que retorna si los datos entregados en conjunto con el nivel son válidos
-        """
-        
-        prefix: str = "" # Se usa para obtener claves y valores en modo deploy
-        if "deploy_enabled" in data and data["deploy_enabled"]:
-            prefix = "deploy_"
-
-        source: str = data[f"{prefix}source"] if (f"{prefix}source" in data and data[f"{prefix}source"] is not None) else None
-        # Valida que venga el recurso de conexión
-        if not source:
-            return False, app_message.dataprep["nodes"]["database_utilities"]["source_required"](node_key)
-
-        # Valida que el recurso de conexión exista en el arreglo
-        if not (source in FIELD_VALIDATION_DATABASE and tier in FIELD_VALIDATION_DATABASE[source]):
-            return False, app_message.dataprep["nodes"]["database_utilities"]["check_missing_source"](node_key)
-
-        fields: list = FIELD_VALIDATION_DATABASE[source][tier]["required"]
-
-        # Valida que cada campo tenga valor
-        for field in fields:
-            field = prefix + field
-            if not field in data:
-                return False, app_message.dataprep["nodes"]["database_utilities"]["check_fields_to_connection"](node_key, field)
-
-            value: any = data[field]
-            if not value:
-                return False, app_message.dataprep["nodes"]["database_utilities"]["check_empty_fields"](node_key, field)
-
-        if "optional" in FIELD_VALIDATION_DATABASE[source][tier]:
-            # Se recorren los arreglos de claves
-            for _list in FIELD_VALIDATION_DATABASE[source][tier]["optional"]:
-                flag: bool = False
-
-                # Se recorren las claves
-                for field in _list:
-                    field = prefix + field
-                    # Valida que el campo exista en la data y que tenga un valor
-                    if field in data and data[field]:
-                        flag = True
-                        break
-
-                # En caso que no exista ninguna clave con valor, da error
-                if not flag:
-                    # return False, "(check_fields) Falló la validación de variables opcionales"
-                    return False, app_message.dataprep["nodes"]["database_utilities"]["check_optional_fields"](node_key)
-
-        return True, ""
-
-    def get_url_connection(self, flow_id: str, data: dict, with_database: bool = False) -> str:
-        """
-        Método que retorna el string de conexión para cada base de datos
-        """
-        
-        prefix: str = "" # Se usa para obtener claves y valores en modo deploy
-        if "deploy_enabled" in data and data["deploy_enabled"]:
-            prefix = "deploy_"
-
-        if data[f"{prefix}source"] == "sqlite":
-            return f"sqlite:///{data[f'{prefix}path']}"
-
-        if data[f"{prefix}source"] == "postgresql":
-            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
-            database: str = "/" + data[f"{prefix}database"] if with_database else ""
-            
-            decryptKey = flow_id[:16]
-            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
-
-            return f"postgresql://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}" + database
-
-        if data[f"{prefix}source"] == "sqlserver_2000":
-            # ['SQL Server', 'SQL Server Native Client 11.0', 'ODBC Driver 17 for SQL Server']
-            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            database: str = f'Database={data[f"{prefix}database"]};' if with_database else ""
-            
-            decryptKey = flow_id[:16]
-            DECRYPTEDPASS = (encrypter.decrypt(PASS, decryptKey)) if PASS is not None and decryptKey is not None else ""
-
-            return "DRIVER={SQL Server};" + f'USER={data[f"{prefix}user"]};PASSWORD={DECRYPTEDPASS};' + database + f'SERVER={data[f"{prefix}host"]};PORT={data[f"{prefix}port"]};'
-
-        if data[f"{prefix}source"] == "sqlserver_2000_v2":
-            # ['SQL Server', 'SQL Server Native Client 11.0', 'ODBC Driver 17 for SQL Server']
-            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            database: str = f'Database={data[f"{prefix}database"]};' if with_database else ""
-            
-            decryptKey = flow_id[:16]
-            DECRYPTEDPASS = (encrypter.decrypt(PASS, decryptKey)) if PASS is not None and decryptKey is not None else ""
-
-            return "DRIVER={SQL Server};" + f'UID={data[f"{prefix}user"]};PWD={DECRYPTEDPASS};' + database + f'SERVER={data[f"{prefix}host"]};PORT={data[f"{prefix}port"]};'
-
-        if data[f"{prefix}source"] == "mysql" or data[f"{prefix}source"] == "mariadb":
-            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
-            database: str = "/" + data[f"{prefix}database"] if with_database else ""
-            
-            decryptKey = flow_id[:16]
-            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
-
-            return f"mysql+pymysql://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}" + database
-
-        if data[f"{prefix}source"] == "oracle":
-            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
-            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
-            database: str = "/" + data[f"{prefix}database"] if with_database else ""
-            service_name: str = "?service_name=" + data[f"{prefix}service_name"] if data[f"{prefix}service_name"] is not None or len(data[f"{prefix}service_name"]) > 0 else ""
-            
-            decryptKey = flow_id[:16]
-            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""            
-            
-            return f"oracle+cx_oracle://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}{service_name}"
-
-database_utilities = Utilities()
+from vtarget.language.app_message import app_message
+from vtarget.utils.database_connection.field_validation import FIELD_VALIDATION_DATABASE
+from vtarget.utils.encrypter import encrypter
+
+
+class Utilities:
+    def __init__(self):
+        pass
+
+    def check_fields(self, data: dict = dict(), tier: str = str(), node_key: str = str()) -> tuple:
+        """
+        Método que retorna si los datos entregados en conjunto con el nivel son válidos
+        """
+        
+        prefix: str = "" # Se usa para obtener claves y valores en modo deploy
+        if "deploy_enabled" in data and data["deploy_enabled"]:
+            prefix = "deploy_"
+
+        source: str = data[f"{prefix}source"] if (f"{prefix}source" in data and data[f"{prefix}source"] is not None) else None
+        # Valida que venga el recurso de conexión
+        if not source:
+            return False, app_message.dataprep["nodes"]["database_utilities"]["source_required"](node_key)
+
+        # Valida que el recurso de conexión exista en el arreglo
+        if not (source in FIELD_VALIDATION_DATABASE and tier in FIELD_VALIDATION_DATABASE[source]):
+            return False, app_message.dataprep["nodes"]["database_utilities"]["check_missing_source"](node_key)
+
+        fields: list = FIELD_VALIDATION_DATABASE[source][tier]["required"]
+
+        # Valida que cada campo tenga valor
+        for field in fields:
+            field = prefix + field
+            if not field in data:
+                return False, app_message.dataprep["nodes"]["database_utilities"]["check_fields_to_connection"](node_key, field)
+
+            value: any = data[field]
+            if not value:
+                return False, app_message.dataprep["nodes"]["database_utilities"]["check_empty_fields"](node_key, field)
+
+        if "optional" in FIELD_VALIDATION_DATABASE[source][tier]:
+            # Se recorren los arreglos de claves
+            for _list in FIELD_VALIDATION_DATABASE[source][tier]["optional"]:
+                flag: bool = False
+
+                # Se recorren las claves
+                for field in _list:
+                    field = prefix + field
+                    # Valida que el campo exista en la data y que tenga un valor
+                    if field in data and data[field]:
+                        flag = True
+                        break
+
+                # En caso que no exista ninguna clave con valor, da error
+                if not flag:
+                    # return False, "(check_fields) Falló la validación de variables opcionales"
+                    return False, app_message.dataprep["nodes"]["database_utilities"]["check_optional_fields"](node_key)
+
+        return True, ""
+
+    def get_url_connection(self, flow_id: str, data: dict, with_database: bool = False) -> str:
+        """
+        Método que retorna el string de conexión para cada base de datos
+        """
+        
+        prefix: str = "" # Se usa para obtener claves y valores en modo deploy
+        if "deploy_enabled" in data and data["deploy_enabled"]:
+            prefix = "deploy_"
+
+        if data[f"{prefix}source"] == "sqlite":
+            return f"sqlite:///{data[f'{prefix}path']}"
+
+        if data[f"{prefix}source"] == "postgresql":
+            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
+            database: str = "/" + data[f"{prefix}database"] if with_database else ""
+            
+            decryptKey = flow_id[:16]
+            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
+
+            return f"postgresql://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}" + database
+
+        if data[f"{prefix}source"] == "sqlserver_2000":
+            # ['SQL Server', 'SQL Server Native Client 11.0', 'ODBC Driver 17 for SQL Server']
+            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            database: str = f'Database={data[f"{prefix}database"]};' if with_database else ""
+            
+            decryptKey = flow_id[:16]
+            DECRYPTEDPASS = (encrypter.decrypt(PASS, decryptKey)) if PASS is not None and decryptKey is not None else ""
+
+            return "DRIVER={SQL Server};" + f'USER={data[f"{prefix}user"]};PASSWORD={DECRYPTEDPASS};' + database + f'SERVER={data[f"{prefix}host"]};PORT={data[f"{prefix}port"]};'
+
+        if data[f"{prefix}source"] == "sqlserver_2000_v2":
+            # ['SQL Server', 'SQL Server Native Client 11.0', 'ODBC Driver 17 for SQL Server']
+            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            database: str = f'Database={data[f"{prefix}database"]};' if with_database else ""
+            
+            decryptKey = flow_id[:16]
+            DECRYPTEDPASS = (encrypter.decrypt(PASS, decryptKey)) if PASS is not None and decryptKey is not None else ""
+
+            return "DRIVER={SQL Server};" + f'UID={data[f"{prefix}user"]};PWD={DECRYPTEDPASS};' + database + f'SERVER={data[f"{prefix}host"]};PORT={data[f"{prefix}port"]};'
+
+        if data[f"{prefix}source"] == "mysql" or data[f"{prefix}source"] == "mariadb":
+            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
+            database: str = "/" + data[f"{prefix}database"] if with_database else ""
+            
+            decryptKey = flow_id[:16]
+            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""
+
+            return f"mysql+pymysql://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}" + database
+
+        if data[f"{prefix}source"] == "oracle":
+            PASS: str = data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            # password: str = ":" + data[f"{prefix}password"] if (f"{prefix}password" in data and data[f"{prefix}password"] is not None) else ""
+            port: str = ":" + str(data[f"{prefix}port"]) if (f"{prefix}port" in data and data[f"{prefix}port"] is not None) else ""
+            database: str = "/" + data[f"{prefix}database"] if with_database else ""
+            service_name: str = "?service_name=" + data[f"{prefix}service_name"] if data[f"{prefix}service_name"] is not None or len(data[f"{prefix}service_name"]) > 0 else ""
+            
+            decryptKey = flow_id[:16]
+            DECRYPTEDPASS = ":"+ encrypter.decrypt(PASS, decryptKey) if PASS is not None and decryptKey is not None else ""            
+            
+            return f"oracle+cx_oracle://{data[f'{prefix}user']}{DECRYPTEDPASS}@{data[f'{prefix}host']}{port}{service_name}"
+
+database_utilities = Utilities()
```

### Comparing `vtarget-0.8.6/vtarget/utils/email_sender.py` & `vtarget-0.8.7/vtarget/utils/email_sender.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# # -*- coding: utf-8 -*-
-import io
-import os
-import smtplib
-from email import encoders
-from email.header import Header
-from email.mime.base import MIMEBase
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from typing import Dict, List
-
-
-class EmailSender(object):
-    """
-    Envia un correo automático utilizando un App Password ded Google
-    https://towardsdatascience.com/automate-sending-emails-with-gmail-in-python-449cc0c3c317
-    """
-
-    def __init__(self):
-        self.SERVER: str = None
-        self.PORT: int = None
-        self.FROM: str = None
-        self.PASS: str = None
-        self.TO: str = None
-        self.SUBJECT: str = None
-        self.HTML: str = None
-        self.FILES: list[str] = []
-        self.FOOTER: str = None
-        self.prepare_footer()
-
-    def configure_server(self, SERVER: str, PORT: int, FROM: str, PASS: str):
-        self.FROM = FROM
-        self.PASS = PASS
-        self.SERVER = SERVER
-        self.PORT = PORT
-
-    def send_email(self, to: str, subject: str, message: str, files: List = None, streams: List[Dict] = None):
-        msg = MIMEMultipart()
-        if to is not None:
-            self.TO = to
-        if subject is not None:
-            self.SUBJECT = subject
-        msg["From"] = self.FROM
-        msg["To"] = self.TO
-        msg["Subject"] = Header(self.SUBJECT)
-
-        self.HTML = message
-
-        if self.HTML:
-            msg.attach(MIMEText(self.HTML, "html"))
-
-        msg.attach(MIMEText(self.FOOTER, "html"))
-
-        if files is not None and len(files):
-            self.prepare_files(files)
-
-        for f in self.FILES:
-            part = MIMEBase("application", "octet-stream")
-            part.set_payload(open(f, "rb").read())
-            encoders.encode_base64(part)
-            part.add_header(
-                "Content-Disposition",
-                'attachment; filename="{0}"'.format(os.path.basename(f)),
-            )
-            msg.attach(part)
-
-        if streams is not None and len(streams):
-            for f in streams:
-                attach: io.StringIO = f["attachment"]
-                if type(attach) is io.StringIO:
-                    attachment = MIMEText(attach.getvalue())
-                    attachment.add_header("Content-Disposition", "attachment", filename=f["filename"] or "out")
-                    msg.attach(attachment)
-
-        # image_path = f"{os.getcwd()}\\lib\\utils\\logo.png"
-
-        # fp = open(image_path, 'rb')
-        # msgImage = MIMEImage(fp.read())
-        # fp.close()
-
-        # # Define the image's ID as referenced above
-        # msgImage.add_header('Content-ID', '<image1>')
-        # msg.attach(msgImage)
-
-        s = smtplib.SMTP(self.SERVER, self.PORT)
-        s.ehlo()  # Hostname to send for this command defaults to the fully qualified domain name of the local host.
-        s.starttls()  # Puts connection to SMTP server in TLS mode
-        s.login(self.FROM, self.PASS)
-        s.sendmail(self.FROM, self.TO.split(","), msg.as_string())
-        s.quit()
-
-    def prepare_footer(self):
-        self.FOOTER = (
-            "<br/><br/>"
-            + "<p>This email was sent automatically</p>"
-            +
-            # "<img src=\"cid:image1\" alt=\"Logo\" style=\"height:70px;\"><br/>"
-            '<p><a href="https://ai/">VTarget</a></p>'
-        )
-
-    def prepare_files(self, files=[]):
-        self.FILES = list(filter(lambda x: os.path.exists(x), files))
-
-
-# if __name__ == "__main__":
-#     se = EmailSender()
-#     se.send_email()
+# # -*- coding: utf-8 -*-
+import io
+import os
+import smtplib
+from email import encoders
+from email.header import Header
+from email.mime.base import MIMEBase
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from typing import Dict, List
+
+
+class EmailSender(object):
+    """
+    Envia un correo automático utilizando un App Password ded Google
+    https://towardsdatascience.com/automate-sending-emails-with-gmail-in-python-449cc0c3c317
+    """
+
+    def __init__(self):
+        self.SERVER: str = None
+        self.PORT: int = None
+        self.FROM: str = None
+        self.PASS: str = None
+        self.TO: str = None
+        self.SUBJECT: str = None
+        self.HTML: str = None
+        self.FILES: list[str] = []
+        self.FOOTER: str = None
+        self.prepare_footer()
+
+    def configure_server(self, SERVER: str, PORT: int, FROM: str, PASS: str):
+        self.FROM = FROM
+        self.PASS = PASS
+        self.SERVER = SERVER
+        self.PORT = PORT
+
+    def send_email(self, to: str, subject: str, message: str, files: List = None, streams: List[Dict] = None):
+        msg = MIMEMultipart()
+        if to is not None:
+            self.TO = to
+        if subject is not None:
+            self.SUBJECT = subject
+        msg["From"] = self.FROM
+        msg["To"] = self.TO
+        msg["Subject"] = Header(self.SUBJECT)
+
+        self.HTML = message
+
+        if self.HTML:
+            msg.attach(MIMEText(self.HTML, "html"))
+
+        msg.attach(MIMEText(self.FOOTER, "html"))
+
+        if files is not None and len(files):
+            self.prepare_files(files)
+
+        for f in self.FILES:
+            part = MIMEBase("application", "octet-stream")
+            part.set_payload(open(f, "rb").read())
+            encoders.encode_base64(part)
+            part.add_header(
+                "Content-Disposition",
+                'attachment; filename="{0}"'.format(os.path.basename(f)),
+            )
+            msg.attach(part)
+
+        if streams is not None and len(streams):
+            for f in streams:
+                attach: io.StringIO = f["attachment"]
+                if type(attach) is io.StringIO:
+                    attachment = MIMEText(attach.getvalue())
+                    attachment.add_header("Content-Disposition", "attachment", filename=f["filename"] or "out")
+                    msg.attach(attachment)
+
+        # image_path = f"{os.getcwd()}\\lib\\utils\\logo.png"
+
+        # fp = open(image_path, 'rb')
+        # msgImage = MIMEImage(fp.read())
+        # fp.close()
+
+        # # Define the image's ID as referenced above
+        # msgImage.add_header('Content-ID', '<image1>')
+        # msg.attach(msgImage)
+
+        s = smtplib.SMTP(self.SERVER, self.PORT)
+        s.ehlo()  # Hostname to send for this command defaults to the fully qualified domain name of the local host.
+        s.starttls()  # Puts connection to SMTP server in TLS mode
+        s.login(self.FROM, self.PASS)
+        s.sendmail(self.FROM, self.TO.split(","), msg.as_string())
+        s.quit()
+
+    def prepare_footer(self):
+        self.FOOTER = (
+            "<br/><br/>"
+            + "<p>This email was sent automatically</p>"
+            +
+            # "<img src=\"cid:image1\" alt=\"Logo\" style=\"height:70px;\"><br/>"
+            '<p><a href="https://ai/">VTarget</a></p>'
+        )
+
+    def prepare_files(self, files=[]):
+        self.FILES = list(filter(lambda x: os.path.exists(x), files))
+
+
+# if __name__ == "__main__":
+#     se = EmailSender()
+#     se.send_email()
```

### Comparing `vtarget-0.8.6/vtarget/utils/encrypter.py` & `vtarget-0.8.7/vtarget/utils/encrypter.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import base64
-
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import pad, unpad
-
-
-# https://medium.com/@sachadehe/encrypt-decrypt-data-between-python-3-and-javascript-true-aes-algorithm-7c4e2fa3a9ff
-class Encrypter:
-    def encrypt(self, data: str, key: str, iv: str = "VTVTVTVTVTVTVTVT"):
-        iv = iv.encode("utf-8")  # 16 char for AES128
-        data = pad(data.encode(), 16)
-        cipher = AES.new(key.encode("utf-8"), AES.MODE_CBC, iv)
-        return base64.b64encode(cipher.encrypt(data))
-
-    def decrypt(self, enc: str, key: str, iv: str = "VTVTVTVTVTVTVTVT"):
-        iv = iv.encode("utf-8")  # 16 char for AES128
-        enc = base64.b64decode(enc)
-        cipher = AES.new(key.encode("utf-8"), AES.MODE_CBC, iv)
-        b = unpad(cipher.decrypt(enc), 16)
-        return b.decode("utf-8")
-
-
-encrypter = Encrypter()
+import base64
+
+from Crypto.Cipher import AES
+from Crypto.Util.Padding import pad, unpad
+
+
+# https://medium.com/@sachadehe/encrypt-decrypt-data-between-python-3-and-javascript-true-aes-algorithm-7c4e2fa3a9ff
+class Encrypter:
+    def encrypt(self, data: str, key: str, iv: str = "VTVTVTVTVTVTVTVT"):
+        iv = iv.encode("utf-8")  # 16 char for AES128
+        data = pad(data.encode(), 16)
+        cipher = AES.new(key.encode("utf-8"), AES.MODE_CBC, iv)
+        return base64.b64encode(cipher.encrypt(data))
+
+    def decrypt(self, enc: str, key: str, iv: str = "VTVTVTVTVTVTVTVT"):
+        iv = iv.encode("utf-8")  # 16 char for AES128
+        enc = base64.b64decode(enc)
+        cipher = AES.new(key.encode("utf-8"), AES.MODE_CBC, iv)
+        b = unpad(cipher.decrypt(enc), 16)
+        return b.decode("utf-8")
+
+
+encrypter = Encrypter()
```

### Comparing `vtarget-0.8.6/vtarget/utils/modeling.py` & `vtarget-0.8.7/vtarget/utils/modeling.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,441 +1,441 @@
-class AutoMLSearch:
-    """Automated Pipeline search.
-
-    Args:
-        X_train (pd.DataFrame): The input training data of shape [n_samples, n_features]. Required.
-
-        y_train (pd.Series): The target training data of length [n_samples]. Required for supervised learning tasks.
-
-        X_holdout (pd.DataFrame): The input holdout data of shape [n_samples, n_features].
-
-        y_holdout (pd.Series): The target holdout data of length [n_samples].
-
-        problem_type (str or ProblemTypes): Type of supervised learning problem.
-
-        objective (str, ObjectiveBase): The objective to optimize for. Used to propose and rank pipelines, but not for optimizing each pipeline during fit-time.
-            When set to 'auto', chooses:
-            - LogLossBinary for binary classification problems,
-            - LogLossMulticlass for multiclass classification problems, and
-            - R2 for regression problems.
-
-        max_iterations (int): Maximum number of iterations to search. If max_iterations and
-            max_time is not set, then max_iterations will default to max_iterations of 5.
-
-        max_time (int, str): Maximum time to search for pipelines.
-            This will not start a new pipeline search after the duration
-            has elapsed. If it is an integer, then the time will be in seconds.
-            For strings, time can be specified as seconds, minutes, or hours.
-
-        patience (int): Number of iterations without improvement to stop search early. Must be positive.
-            If None, early stopping is disabled. Defaults to None.
-
-        tolerance (float): Minimum percentage difference to qualify as score improvement for early stopping.
-            Only applicable if patience is not None. Defaults to None.
-
-        allowed_component_graphs (dict): A dictionary of lists or ComponentGraphs indicating the component graphs allowed in the search.
-            The format should follow { "Name_0": [list_of_components], "Name_1": ComponentGraph(...) }
-
-            The default of None indicates all pipeline component graphs for this problem type are allowed. Setting this field will cause
-            allowed_model_families to be ignored.
-
-            e.g. allowed_component_graphs = { "My_Graph": ["Imputer", "One Hot Encoder", "Random Forest Classifier"] }
-
-        allowed_model_families (list(str, ModelFamily)): The model families to search. The default of None searches over all
-            model families. Change `binary` to `multiclass` or `regression` depending on the problem type. Note that if allowed_pipelines
-            is provided, this parameter will be ignored.
-
-        features (list)[FeatureBase]: List of features to run DFS on AutoML pipelines. Defaults to None.
-            Features will only be computed if the columns used by the feature exist in the search input
-            and if the feature itself is not in search input. If features is an empty list, the DFS Transformer will not be included in pipelines.
-
-        data_splitter (sklearn.model_selection.BaseCrossValidator): Data splitting method to use. Defaults to StratifiedKFold.
-
-        tuner_class: The tuner class to use. Defaults to SKOptTuner.
-
-        optimize_thresholds (bool): Whether or not to optimize the binary pipeline threshold. Defaults to True.
-
-        start_iteration_callback (callable): Function called before each pipeline training iteration.
-            Callback function takes three positional parameters: The pipeline instance and the AutoMLSearch object.
-
-        add_result_callback (callable): Function called after each pipeline training iteration.
-            Callback function takes three positional parameters: A dictionary containing the training results for the new pipeline, an
-            untrained_pipeline containing the parameters used during training, and the AutoMLSearch object.
-
-        error_callback (callable): Function called when `search()` errors and raises an Exception.
-            Callback function takes three positional parameters: the Exception raised, the traceback, and the AutoMLSearch object.
-            Must also accepts kwargs, so AutoMLSearch is able to pass along other appropriate parameters by default.
-            Defaults to None, which will call `log_error_callback`.
-
-        additional_objectives (list): Custom set of objectives to score on.
-            Will override default objectives for problem type if not empty.
-
-        alternate_thresholding_objective (str): The objective to use for thresholding binary classification pipelines if the main objective provided isn't tuneable.
-            Defaults to F1.
-
-        random_seed (int): Seed for the random number generator. Defaults to 0.
-
-        n_jobs (int or None): Non-negative integer describing level of parallelism used for pipelines.
-            None and 1 are equivalent. If set to -1, all CPUs are used. For n_jobs below -1, (n_cpus + 1 + n_jobs) are used.
-
-        ensembling (boolean): If True, runs ensembling in a separate batch after every allowed pipeline class has been iterated over.
-            If the number of unique pipelines to search over per batch is one, ensembling will not run. Defaults to False.
-
-        max_batches (int): The maximum number of batches of pipelines to search. Parameters max_time, and
-            max_iterations have precedence over stopping the search.
-
-        problem_configuration (dict, None): Additional parameters needed to configure the search. For example,
-            in time series problems, values should be passed in for the time_index, gap, forecast_horizon, and max_delay variables.
-
-        train_best_pipeline (boolean): Whether or not to train the best pipeline before returning it. Defaults to True.
-
-        search_parameters (dict): A dict of the hyperparameter ranges or pipeline parameters used to iterate over during search.
-            Keys should consist of the component names and values should specify a singular value/list for pipeline parameters, or skopt.Space for hyperparameter ranges.
-            In the example below, the Imputer parameters would be passed to the hyperparameter ranges, and the Label Encoder parameters would be used as the component parameter.
-
-            e.g. search_parameters = { 'Imputer' : { 'numeric_impute_strategy': Categorical(['most_frequent', 'median']) },
-                                       'Label Encoder': {'positive_label': True} }
-
-        sampler_method (str): The data sampling component to use in the pipelines if the problem type is classification and the target balance is smaller than the sampler_balanced_ratio.
-            Either 'auto', which will use our preferred sampler for the data, 'Undersampler', 'Oversampler', or None. Defaults to 'auto'.
-
-        sampler_balanced_ratio (float): The minority:majority class ratio that we consider balanced, so a 1:4 ratio would be equal to 0.25. If the class balance is larger than this provided value,
-            then we will not add a sampler since the data is then considered balanced. Overrides the `sampler_ratio` of the samplers. Defaults to 0.25.
-
-        allow_long_running_models (bool): Whether or not to allow longer-running models for large multiclass problems. If False and no pipelines, component graphs, or model families are provided,
-            AutoMLSearch will not use Elastic Net or XGBoost when there are more than 75 multiclass targets and will not use CatBoost when there are more than 150 multiclass targets. Defaults to False.
-
-        _ensembling_split_size (float): The amount of the training data we'll set aside for training ensemble metalearners. Only used when ensembling is True.
-            Must be between 0 and 1, exclusive. Defaults to 0.2
-
-        _pipelines_per_batch (int): The number of pipelines to train for every batch after the first one.
-            The first batch will train a baseline pipline + one of each pipeline family allowed in the search.
-
-        automl_algorithm (str): The automl algorithm to use. Currently the two choices are 'iterative' and 'default'. Defaults to `default`.
-
-        engine (EngineBase or str): The engine instance used to evaluate pipelines. Dask or concurrent.futures engines can also
-            be chosen by providing a string from the list ["sequential", "cf_threaded", "cf_process", "dask_threaded", "dask_process"].
-            If a parallel engine is selected this way, the maximum amount of parallelism, as determined by the engine, will be used. Defaults to "sequential".
-
-        verbose (boolean): Whether or not to display semi-real-time updates to stdout while search is running. Defaults to False.
-
-        timing (boolean): Whether or not to write pipeline search times to the logger. Defaults to False.
-        exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by search.
-            Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
-
-        holdout_set_size (float): The size of the holdout set that AutoML search will take for datasets larger than 500 rows. If set to 0, holdout set will not be taken regardless of number of rows. Must be between 0 and 1, exclusive. Defaults to 0.1.
-    """
-
-    def __init__(
-        self,
-        X_train=None,
-        y_train=None,
-        X_holdout=None,
-        y_holdout=None,
-        problem_type=None,
-        objective="auto",
-        max_iterations=None,
-        max_time=None,
-        patience=None,
-        tolerance=None,
-        data_splitter=None,
-        allowed_component_graphs=None,
-        allowed_model_families=None,
-        features=None,
-        start_iteration_callback=None,
-        add_result_callback=None,
-        error_callback=None,
-        additional_objectives=None,
-        alternate_thresholding_objective="F1",
-        random_seed=0,
-        n_jobs=-1,
-        tuner_class=None,
-        optimize_thresholds=True,
-        ensembling=False,
-        max_batches=None,
-        problem_configuration=None,
-        train_best_pipeline=True,
-        search_parameters=None,
-        sampler_method="auto",
-        sampler_balanced_ratio=0.25,
-        allow_long_running_models=False,
-        _pipelines_per_batch=5,
-        automl_algorithm="default",
-        engine="sequential",
-        verbose=False,
-        timing=False,
-        exclude_featurizers=None,
-        holdout_set_size=0,
-        empty=False,
-    ):
-        from evalml.automl.automl_search import AutoMLSearch
-
-        if not empty:
-            self.__ = AutoMLSearch(
-                X_train,
-                y_train,
-                X_holdout,
-                y_holdout,
-                problem_type,
-                objective,
-                max_iterations,
-                max_time,
-                patience,
-                tolerance,
-                data_splitter,
-                allowed_component_graphs,
-                allowed_model_families,
-                features,
-                start_iteration_callback,
-                add_result_callback,
-                error_callback,
-                additional_objectives,
-                alternate_thresholding_objective,
-                random_seed,
-                n_jobs,
-                tuner_class,
-                optimize_thresholds,
-                ensembling,
-                max_batches,
-                problem_configuration,
-                train_best_pipeline,
-                search_parameters,
-                sampler_method,
-                sampler_balanced_ratio,
-                allow_long_running_models,
-                _pipelines_per_batch,
-                automl_algorithm,
-                engine,
-                verbose,
-                timing,
-                exclude_featurizers,
-                holdout_set_size,
-            )
-
-    def __str__(self):
-        """Returns string representation of the AutoMLSearch object."""
-        from evalml.objectives import get_objective
-        from evalml.problem_types.utils import handle_problem_types
-
-        def _print_list(obj_list):
-            lines = sorted(["\t{}".format(o.name) for o in obj_list])
-            return "\n".join(lines)
-
-        def _get_funct_name(function):
-            if callable(function):
-                return function.__name__
-            else:
-                return None
-
-        search_desc = (
-            f"{handle_problem_types(self.problem_type).name} Search\n\n"
-            f"Parameters: \n{'='*20}\n"
-            f"Objective: {get_objective(self.objective).name}\n"
-            f"Max Time: {self.max_time}\n"
-            f"Max Iterations: {self.max_iterations}\n"
-            f"Max Batches: {self.max_batches}\n"
-            f"Allowed Pipelines: \n{_print_list(self.allowed_pipelines or [])}\n"
-            f"Patience: {self.patience}\n"
-            f"Tolerance: {self.tolerance}\n"
-            f"Data Splitting: {self.data_splitter}\n"
-            f"Tuner: {self.tuner_class.__name__}\n"
-            f"Start Iteration Callback: {_get_funct_name(self.start_iteration_callback)}\n"
-            f"Add Result Callback: {_get_funct_name(self.add_result_callback)}\n"
-            f"Additional Objectives: {_print_list(self.additional_objectives or [])}\n"
-            f"Random Seed: {self.random_seed}\n"
-            f"n_jobs: {self.n_jobs}\n"
-            f"Optimize Thresholds: {self.optimize_thresholds}\n"
-        )
-
-        rankings_desc = ""
-        if not self.rankings.empty:
-            rankings_str = self.rankings.drop(
-                ["parameters"],
-                axis="columns",
-            ).to_string()
-            rankings_desc = f"\nSearch Results: \n{'='*20}\n{rankings_str}"
-
-        return search_desc + rankings_desc
-
-    def close_engine(self):
-        """Function to explicitly close the engine, client, parallel resources."""
-        return self.__.close_engine()
-
-    def search(self, interactive_plot=True):
-        """Find the best pipeline for the data set.
-
-        Args:
-            interactive_plot (boolean, True): Shows an iteration vs. score plot in Jupyter notebook.
-                Disabled by default in non-Jupyter enviroments.
-
-        Raises:
-            AutoMLSearchException: If all pipelines in the current AutoML batch produced a score of np.nan on the primary objective.
-
-        Returns:
-            Dict[int, Dict[str, Timestamp]]: Dictionary keyed by batch number that maps to the timings for pipelines run in that batch,
-            as well as the total time for each batch. Pipelines within a batch are labeled by pipeline name.
-        """
-        return self.__.search(interactive_plot)
-
-    def get_pipeline(self, pipeline_id):
-        """Given the ID of a pipeline training result, returns an untrained instance of the specified pipeline initialized with the parameters used to train that pipeline during automl search.
-
-        Args:
-            pipeline_id (int): Pipeline to retrieve.
-
-        Returns:
-            PipelineBase: Untrained pipeline instance associated with the provided ID.
-
-        Raises:
-            PipelineNotFoundError: if pipeline_id is not a valid ID.
-        """
-        return self.__.get_pipeline(pipeline_id)
-
-    def describe_pipeline(self, pipeline_id, return_dict=False):
-        """Describe a pipeline.
-
-        Args:
-            pipeline_id (int): pipeline to describe
-            return_dict (bool): If True, return dictionary of information
-                about pipeline. Defaults to False.
-
-        Returns:
-            Description of specified pipeline. Includes information such as
-            type of pipeline components, problem, training time, cross validation, etc.
-
-        Raises:
-            PipelineNotFoundError: If pipeline_id is not a valid ID.
-        """
-        return self.__.describe_pipeline(pipeline_id, return_dict)
-
-    def add_to_rankings(self, pipeline):
-        """Fits and evaluates a given pipeline then adds the results to the automl rankings with the requirement that automl search has been run.
-
-        Args:
-            pipeline (PipelineBase): pipeline to train and evaluate.
-        """
-        return self.__.add_to_rankings(pipeline)
-
-    @property
-    def results(self):
-        """Class that allows access to a copy of the results from `automl_search`.
-
-        Returns:
-            dict: Dictionary containing `pipeline_results`, a dict with results from each pipeline,
-                 and `search_order`, a list describing the order the pipelines were searched.
-        """
-        return self.__.results
-
-    @property
-    def rankings(self):
-        """Returns a pandas.DataFrame with scoring results from the highest-scoring set of parameters used with each pipeline."""
-        return self.__.rankings
-
-    @property
-    def full_rankings(self):
-        """Returns a pandas.DataFrame with scoring results from all pipelines searched."""
-        return self.__.full_rankings
-
-    @property
-    def best_pipeline(self):
-        """Returns a trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
-
-        Returns:
-            PipelineBase: A trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
-
-        Raises:
-            PipelineNotFoundError: If this is called before .search() is called.
-        """
-        return self.__.best_pipeline
-
-    import cloudpickle
-
-    def save(
-        self,
-        file_path,
-        pickle_type="cloudpickle",
-        pickle_protocol=cloudpickle.DEFAULT_PROTOCOL,
-    ):
-        """Saves AutoML object at file path.
-
-        Args:
-            file_path (str): Location to save file.
-            pickle_type ({"pickle", "cloudpickle"}): The pickling library to use.
-            pickle_protocol (int): The pickle data stream format.
-
-        Raises:
-            ValueError: If pickle_type is not "pickle" or "cloudpickle".
-        """
-        return self.__.save(file_path, pickle_type, pickle_protocol)
-
-    @staticmethod
-    def load(
-        file_path,
-        pickle_type="cloudpickle",
-    ):
-        """Loads AutoML object at file path.
-
-        Args:
-            file_path (str): Location to find file to load
-            pickle_type ({"pickle", "cloudpickle"}): The pickling library to use. Currently not used since the standard pickle library can handle cloudpickles.
-
-        Returns:
-            AutoSearchBase object
-        """
-        import pickle
-
-        self = AutoMLSearch(empty=True)
-
-        with open(file_path, "rb") as f:
-            self.__ = pickle.load(f)
-
-        return self
-
-    def train_pipelines(self, pipelines):
-        """Train a list of pipelines on the training data.
-
-        This can be helpful for training pipelines once the search is complete.
-
-        Args:
-            pipelines (list[PipelineBase]): List of pipelines to train.
-
-        Returns:
-            Dict[str, PipelineBase]: Dictionary keyed by pipeline name that maps to the fitted pipeline.
-            Note that the any pipelines that error out during training will not be included in the dictionary
-            but the exception and stacktrace will be displayed in the log.
-        """
-        return self.__.train_pipelines(pipelines)
-
-    def score_pipelines(self, pipelines, X_holdout, y_holdout, objectives):
-        """Score a list of pipelines on the given holdout data.
-
-        Args:
-            pipelines (list[PipelineBase]): List of pipelines to train.
-            X_holdout (pd.DataFrame): Holdout features.
-            y_holdout (pd.Series): Holdout targets for scoring.
-            objectives (list[str], list[ObjectiveBase]): Objectives used for scoring.
-
-        Returns:
-            dict[str, Dict[str, float]]: Dictionary keyed by pipeline name that maps to a dictionary of scores.
-            Note that the any pipelines that error out during scoring will not be included in the dictionary
-            but the exception and stacktrace will be displayed in the log.
-        """
-        return self.__.score_pipelines(pipelines, X_holdout, y_holdout, objectives)
-
-    @property
-    def plot(self):
-        """Return an instance of the plot with the latest scores."""
-        return self.__.plot
-
-    def get_ensembler_input_pipelines(self, ensemble_pipeline_id):
-        """Returns a list of input pipeline IDs given an ensembler pipeline ID.
-
-        Args:
-            ensemble_pipeline_id (id): Ensemble pipeline ID to get input pipeline IDs from.
-
-        Returns:
-            list[int]: A list of ensemble input pipeline IDs.
-
-        Raises:
-            ValueError: If `ensemble_pipeline_id` does not correspond to a valid ensemble pipeline ID.
-        """
-        return self.__.get_ensembler_input_pipelines(ensemble_pipeline_id)
+class AutoMLSearch:
+    """Automated Pipeline search.
+
+    Args:
+        X_train (pd.DataFrame): The input training data of shape [n_samples, n_features]. Required.
+
+        y_train (pd.Series): The target training data of length [n_samples]. Required for supervised learning tasks.
+
+        X_holdout (pd.DataFrame): The input holdout data of shape [n_samples, n_features].
+
+        y_holdout (pd.Series): The target holdout data of length [n_samples].
+
+        problem_type (str or ProblemTypes): Type of supervised learning problem.
+
+        objective (str, ObjectiveBase): The objective to optimize for. Used to propose and rank pipelines, but not for optimizing each pipeline during fit-time.
+            When set to 'auto', chooses:
+            - LogLossBinary for binary classification problems,
+            - LogLossMulticlass for multiclass classification problems, and
+            - R2 for regression problems.
+
+        max_iterations (int): Maximum number of iterations to search. If max_iterations and
+            max_time is not set, then max_iterations will default to max_iterations of 5.
+
+        max_time (int, str): Maximum time to search for pipelines.
+            This will not start a new pipeline search after the duration
+            has elapsed. If it is an integer, then the time will be in seconds.
+            For strings, time can be specified as seconds, minutes, or hours.
+
+        patience (int): Number of iterations without improvement to stop search early. Must be positive.
+            If None, early stopping is disabled. Defaults to None.
+
+        tolerance (float): Minimum percentage difference to qualify as score improvement for early stopping.
+            Only applicable if patience is not None. Defaults to None.
+
+        allowed_component_graphs (dict): A dictionary of lists or ComponentGraphs indicating the component graphs allowed in the search.
+            The format should follow { "Name_0": [list_of_components], "Name_1": ComponentGraph(...) }
+
+            The default of None indicates all pipeline component graphs for this problem type are allowed. Setting this field will cause
+            allowed_model_families to be ignored.
+
+            e.g. allowed_component_graphs = { "My_Graph": ["Imputer", "One Hot Encoder", "Random Forest Classifier"] }
+
+        allowed_model_families (list(str, ModelFamily)): The model families to search. The default of None searches over all
+            model families. Change `binary` to `multiclass` or `regression` depending on the problem type. Note that if allowed_pipelines
+            is provided, this parameter will be ignored.
+
+        features (list)[FeatureBase]: List of features to run DFS on AutoML pipelines. Defaults to None.
+            Features will only be computed if the columns used by the feature exist in the search input
+            and if the feature itself is not in search input. If features is an empty list, the DFS Transformer will not be included in pipelines.
+
+        data_splitter (sklearn.model_selection.BaseCrossValidator): Data splitting method to use. Defaults to StratifiedKFold.
+
+        tuner_class: The tuner class to use. Defaults to SKOptTuner.
+
+        optimize_thresholds (bool): Whether or not to optimize the binary pipeline threshold. Defaults to True.
+
+        start_iteration_callback (callable): Function called before each pipeline training iteration.
+            Callback function takes three positional parameters: The pipeline instance and the AutoMLSearch object.
+
+        add_result_callback (callable): Function called after each pipeline training iteration.
+            Callback function takes three positional parameters: A dictionary containing the training results for the new pipeline, an
+            untrained_pipeline containing the parameters used during training, and the AutoMLSearch object.
+
+        error_callback (callable): Function called when `search()` errors and raises an Exception.
+            Callback function takes three positional parameters: the Exception raised, the traceback, and the AutoMLSearch object.
+            Must also accepts kwargs, so AutoMLSearch is able to pass along other appropriate parameters by default.
+            Defaults to None, which will call `log_error_callback`.
+
+        additional_objectives (list): Custom set of objectives to score on.
+            Will override default objectives for problem type if not empty.
+
+        alternate_thresholding_objective (str): The objective to use for thresholding binary classification pipelines if the main objective provided isn't tuneable.
+            Defaults to F1.
+
+        random_seed (int): Seed for the random number generator. Defaults to 0.
+
+        n_jobs (int or None): Non-negative integer describing level of parallelism used for pipelines.
+            None and 1 are equivalent. If set to -1, all CPUs are used. For n_jobs below -1, (n_cpus + 1 + n_jobs) are used.
+
+        ensembling (boolean): If True, runs ensembling in a separate batch after every allowed pipeline class has been iterated over.
+            If the number of unique pipelines to search over per batch is one, ensembling will not run. Defaults to False.
+
+        max_batches (int): The maximum number of batches of pipelines to search. Parameters max_time, and
+            max_iterations have precedence over stopping the search.
+
+        problem_configuration (dict, None): Additional parameters needed to configure the search. For example,
+            in time series problems, values should be passed in for the time_index, gap, forecast_horizon, and max_delay variables.
+
+        train_best_pipeline (boolean): Whether or not to train the best pipeline before returning it. Defaults to True.
+
+        search_parameters (dict): A dict of the hyperparameter ranges or pipeline parameters used to iterate over during search.
+            Keys should consist of the component names and values should specify a singular value/list for pipeline parameters, or skopt.Space for hyperparameter ranges.
+            In the example below, the Imputer parameters would be passed to the hyperparameter ranges, and the Label Encoder parameters would be used as the component parameter.
+
+            e.g. search_parameters = { 'Imputer' : { 'numeric_impute_strategy': Categorical(['most_frequent', 'median']) },
+                                       'Label Encoder': {'positive_label': True} }
+
+        sampler_method (str): The data sampling component to use in the pipelines if the problem type is classification and the target balance is smaller than the sampler_balanced_ratio.
+            Either 'auto', which will use our preferred sampler for the data, 'Undersampler', 'Oversampler', or None. Defaults to 'auto'.
+
+        sampler_balanced_ratio (float): The minority:majority class ratio that we consider balanced, so a 1:4 ratio would be equal to 0.25. If the class balance is larger than this provided value,
+            then we will not add a sampler since the data is then considered balanced. Overrides the `sampler_ratio` of the samplers. Defaults to 0.25.
+
+        allow_long_running_models (bool): Whether or not to allow longer-running models for large multiclass problems. If False and no pipelines, component graphs, or model families are provided,
+            AutoMLSearch will not use Elastic Net or XGBoost when there are more than 75 multiclass targets and will not use CatBoost when there are more than 150 multiclass targets. Defaults to False.
+
+        _ensembling_split_size (float): The amount of the training data we'll set aside for training ensemble metalearners. Only used when ensembling is True.
+            Must be between 0 and 1, exclusive. Defaults to 0.2
+
+        _pipelines_per_batch (int): The number of pipelines to train for every batch after the first one.
+            The first batch will train a baseline pipline + one of each pipeline family allowed in the search.
+
+        automl_algorithm (str): The automl algorithm to use. Currently the two choices are 'iterative' and 'default'. Defaults to `default`.
+
+        engine (EngineBase or str): The engine instance used to evaluate pipelines. Dask or concurrent.futures engines can also
+            be chosen by providing a string from the list ["sequential", "cf_threaded", "cf_process", "dask_threaded", "dask_process"].
+            If a parallel engine is selected this way, the maximum amount of parallelism, as determined by the engine, will be used. Defaults to "sequential".
+
+        verbose (boolean): Whether or not to display semi-real-time updates to stdout while search is running. Defaults to False.
+
+        timing (boolean): Whether or not to write pipeline search times to the logger. Defaults to False.
+        exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by search.
+            Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
+
+        holdout_set_size (float): The size of the holdout set that AutoML search will take for datasets larger than 500 rows. If set to 0, holdout set will not be taken regardless of number of rows. Must be between 0 and 1, exclusive. Defaults to 0.1.
+    """
+
+    def __init__(
+        self,
+        X_train=None,
+        y_train=None,
+        X_holdout=None,
+        y_holdout=None,
+        problem_type=None,
+        objective="auto",
+        max_iterations=None,
+        max_time=None,
+        patience=None,
+        tolerance=None,
+        data_splitter=None,
+        allowed_component_graphs=None,
+        allowed_model_families=None,
+        features=None,
+        start_iteration_callback=None,
+        add_result_callback=None,
+        error_callback=None,
+        additional_objectives=None,
+        alternate_thresholding_objective="F1",
+        random_seed=0,
+        n_jobs=-1,
+        tuner_class=None,
+        optimize_thresholds=True,
+        ensembling=False,
+        max_batches=None,
+        problem_configuration=None,
+        train_best_pipeline=True,
+        search_parameters=None,
+        sampler_method="auto",
+        sampler_balanced_ratio=0.25,
+        allow_long_running_models=False,
+        _pipelines_per_batch=5,
+        automl_algorithm="default",
+        engine="sequential",
+        verbose=False,
+        timing=False,
+        exclude_featurizers=None,
+        holdout_set_size=0,
+        empty=False,
+    ):
+        from evalml.automl.automl_search import AutoMLSearch
+
+        if not empty:
+            self.__ = AutoMLSearch(
+                X_train,
+                y_train,
+                X_holdout,
+                y_holdout,
+                problem_type,
+                objective,
+                max_iterations,
+                max_time,
+                patience,
+                tolerance,
+                data_splitter,
+                allowed_component_graphs,
+                allowed_model_families,
+                features,
+                start_iteration_callback,
+                add_result_callback,
+                error_callback,
+                additional_objectives,
+                alternate_thresholding_objective,
+                random_seed,
+                n_jobs,
+                tuner_class,
+                optimize_thresholds,
+                ensembling,
+                max_batches,
+                problem_configuration,
+                train_best_pipeline,
+                search_parameters,
+                sampler_method,
+                sampler_balanced_ratio,
+                allow_long_running_models,
+                _pipelines_per_batch,
+                automl_algorithm,
+                engine,
+                verbose,
+                timing,
+                exclude_featurizers,
+                holdout_set_size,
+            )
+
+    def __str__(self):
+        """Returns string representation of the AutoMLSearch object."""
+        from evalml.objectives import get_objective
+        from evalml.problem_types.utils import handle_problem_types
+
+        def _print_list(obj_list):
+            lines = sorted(["\t{}".format(o.name) for o in obj_list])
+            return "\n".join(lines)
+
+        def _get_funct_name(function):
+            if callable(function):
+                return function.__name__
+            else:
+                return None
+
+        search_desc = (
+            f"{handle_problem_types(self.problem_type).name} Search\n\n"
+            f"Parameters: \n{'='*20}\n"
+            f"Objective: {get_objective(self.objective).name}\n"
+            f"Max Time: {self.max_time}\n"
+            f"Max Iterations: {self.max_iterations}\n"
+            f"Max Batches: {self.max_batches}\n"
+            f"Allowed Pipelines: \n{_print_list(self.allowed_pipelines or [])}\n"
+            f"Patience: {self.patience}\n"
+            f"Tolerance: {self.tolerance}\n"
+            f"Data Splitting: {self.data_splitter}\n"
+            f"Tuner: {self.tuner_class.__name__}\n"
+            f"Start Iteration Callback: {_get_funct_name(self.start_iteration_callback)}\n"
+            f"Add Result Callback: {_get_funct_name(self.add_result_callback)}\n"
+            f"Additional Objectives: {_print_list(self.additional_objectives or [])}\n"
+            f"Random Seed: {self.random_seed}\n"
+            f"n_jobs: {self.n_jobs}\n"
+            f"Optimize Thresholds: {self.optimize_thresholds}\n"
+        )
+
+        rankings_desc = ""
+        if not self.rankings.empty:
+            rankings_str = self.rankings.drop(
+                ["parameters"],
+                axis="columns",
+            ).to_string()
+            rankings_desc = f"\nSearch Results: \n{'='*20}\n{rankings_str}"
+
+        return search_desc + rankings_desc
+
+    def close_engine(self):
+        """Function to explicitly close the engine, client, parallel resources."""
+        return self.__.close_engine()
+
+    def search(self, interactive_plot=True):
+        """Find the best pipeline for the data set.
+
+        Args:
+            interactive_plot (boolean, True): Shows an iteration vs. score plot in Jupyter notebook.
+                Disabled by default in non-Jupyter enviroments.
+
+        Raises:
+            AutoMLSearchException: If all pipelines in the current AutoML batch produced a score of np.nan on the primary objective.
+
+        Returns:
+            Dict[int, Dict[str, Timestamp]]: Dictionary keyed by batch number that maps to the timings for pipelines run in that batch,
+            as well as the total time for each batch. Pipelines within a batch are labeled by pipeline name.
+        """
+        return self.__.search(interactive_plot)
+
+    def get_pipeline(self, pipeline_id):
+        """Given the ID of a pipeline training result, returns an untrained instance of the specified pipeline initialized with the parameters used to train that pipeline during automl search.
+
+        Args:
+            pipeline_id (int): Pipeline to retrieve.
+
+        Returns:
+            PipelineBase: Untrained pipeline instance associated with the provided ID.
+
+        Raises:
+            PipelineNotFoundError: if pipeline_id is not a valid ID.
+        """
+        return self.__.get_pipeline(pipeline_id)
+
+    def describe_pipeline(self, pipeline_id, return_dict=False):
+        """Describe a pipeline.
+
+        Args:
+            pipeline_id (int): pipeline to describe
+            return_dict (bool): If True, return dictionary of information
+                about pipeline. Defaults to False.
+
+        Returns:
+            Description of specified pipeline. Includes information such as
+            type of pipeline components, problem, training time, cross validation, etc.
+
+        Raises:
+            PipelineNotFoundError: If pipeline_id is not a valid ID.
+        """
+        return self.__.describe_pipeline(pipeline_id, return_dict)
+
+    def add_to_rankings(self, pipeline):
+        """Fits and evaluates a given pipeline then adds the results to the automl rankings with the requirement that automl search has been run.
+
+        Args:
+            pipeline (PipelineBase): pipeline to train and evaluate.
+        """
+        return self.__.add_to_rankings(pipeline)
+
+    @property
+    def results(self):
+        """Class that allows access to a copy of the results from `automl_search`.
+
+        Returns:
+            dict: Dictionary containing `pipeline_results`, a dict with results from each pipeline,
+                 and `search_order`, a list describing the order the pipelines were searched.
+        """
+        return self.__.results
+
+    @property
+    def rankings(self):
+        """Returns a pandas.DataFrame with scoring results from the highest-scoring set of parameters used with each pipeline."""
+        return self.__.rankings
+
+    @property
+    def full_rankings(self):
+        """Returns a pandas.DataFrame with scoring results from all pipelines searched."""
+        return self.__.full_rankings
+
+    @property
+    def best_pipeline(self):
+        """Returns a trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
+
+        Returns:
+            PipelineBase: A trained instance of the best pipeline and parameters found during automl search. If `train_best_pipeline` is set to False, returns an untrained pipeline instance.
+
+        Raises:
+            PipelineNotFoundError: If this is called before .search() is called.
+        """
+        return self.__.best_pipeline
+
+    import cloudpickle
+
+    def save(
+        self,
+        file_path,
+        pickle_type="cloudpickle",
+        pickle_protocol=cloudpickle.DEFAULT_PROTOCOL,
+    ):
+        """Saves AutoML object at file path.
+
+        Args:
+            file_path (str): Location to save file.
+            pickle_type ({"pickle", "cloudpickle"}): The pickling library to use.
+            pickle_protocol (int): The pickle data stream format.
+
+        Raises:
+            ValueError: If pickle_type is not "pickle" or "cloudpickle".
+        """
+        return self.__.save(file_path, pickle_type, pickle_protocol)
+
+    @staticmethod
+    def load(
+        file_path,
+        pickle_type="cloudpickle",
+    ):
+        """Loads AutoML object at file path.
+
+        Args:
+            file_path (str): Location to find file to load
+            pickle_type ({"pickle", "cloudpickle"}): The pickling library to use. Currently not used since the standard pickle library can handle cloudpickles.
+
+        Returns:
+            AutoSearchBase object
+        """
+        import pickle
+
+        self = AutoMLSearch(empty=True)
+
+        with open(file_path, "rb") as f:
+            self.__ = pickle.load(f)
+
+        return self
+
+    def train_pipelines(self, pipelines):
+        """Train a list of pipelines on the training data.
+
+        This can be helpful for training pipelines once the search is complete.
+
+        Args:
+            pipelines (list[PipelineBase]): List of pipelines to train.
+
+        Returns:
+            Dict[str, PipelineBase]: Dictionary keyed by pipeline name that maps to the fitted pipeline.
+            Note that the any pipelines that error out during training will not be included in the dictionary
+            but the exception and stacktrace will be displayed in the log.
+        """
+        return self.__.train_pipelines(pipelines)
+
+    def score_pipelines(self, pipelines, X_holdout, y_holdout, objectives):
+        """Score a list of pipelines on the given holdout data.
+
+        Args:
+            pipelines (list[PipelineBase]): List of pipelines to train.
+            X_holdout (pd.DataFrame): Holdout features.
+            y_holdout (pd.Series): Holdout targets for scoring.
+            objectives (list[str], list[ObjectiveBase]): Objectives used for scoring.
+
+        Returns:
+            dict[str, Dict[str, float]]: Dictionary keyed by pipeline name that maps to a dictionary of scores.
+            Note that the any pipelines that error out during scoring will not be included in the dictionary
+            but the exception and stacktrace will be displayed in the log.
+        """
+        return self.__.score_pipelines(pipelines, X_holdout, y_holdout, objectives)
+
+    @property
+    def plot(self):
+        """Return an instance of the plot with the latest scores."""
+        return self.__.plot
+
+    def get_ensembler_input_pipelines(self, ensemble_pipeline_id):
+        """Returns a list of input pipeline IDs given an ensembler pipeline ID.
+
+        Args:
+            ensemble_pipeline_id (id): Ensemble pipeline ID to get input pipeline IDs from.
+
+        Returns:
+            list[int]: A list of ensemble input pipeline IDs.
+
+        Raises:
+            ValueError: If `ensemble_pipeline_id` does not correspond to a valid ensemble pipeline ID.
+        """
+        return self.__.get_ensembler_input_pipelines(ensemble_pipeline_id)
```

### Comparing `vtarget-0.8.6/vtarget/utils/utilities.py` & `vtarget-0.8.7/vtarget/utils/utilities.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,305 @@
-import ast
-import json
-import re
-
-import numpy as np
-import pandas as pd
-from pandas.api.types import is_numeric_dtype
-from scipy import stats
-
-from vtarget.handlers.bug_handler import bug_handler
-from vtarget.handlers.cache_handler import cache_handler
-from vtarget.language.app_message import app_message
-
-
-class Utilities:
-    # Retorna la metadata del dtypes de un df
-    def get_dtypes_of_df(self, df: pd.DataFrame):
-        dict_dtypes = {}
-        res = df.dtypes.to_frame("dtypes")
-        res = res["dtypes"].astype(str).reset_index()
-        res["selected"] = True
-        res["order"] = pd.RangeIndex(stop=res.shape[0])
-        for _, x in res.iterrows():
-            dict_dtypes[x["index"]] = {
-                "dtype": x["dtypes"],
-                "selected": x["selected"],
-                "order": x["order"],
-            }
-
-        return dict_dtypes
-
-    def get_table_config(self, meta: dict, port_name: str):
-        # ? Sacar config desde meta.ports_config con el puerto
-        ports_config: dict = meta["ports_config"][port_name] if "ports_config" in meta and port_name in meta["ports_config"] else {}
-        return {
-            "page": ports_config["page"] if "page" in ports_config else 1,
-            "rows": ports_config["rows"] if "rows" in ports_config and ports_config["rows"] is not None else 50,
-            "decimals": ports_config["decimals"] if "decimals" in ports_config and ports_config["decimals"] is not None else -1,
-            "source": ports_config["source"] if "source" in ports_config and ports_config["source"] else "head",
-            "sort_by": ports_config["sort_by"] if "sort_by" in ports_config and ports_config["sort_by"] else [],
-        }
-
-    def sort_df(self, full_df: pd.DataFrame, sorts: list[dict], flow_id, node_key):
-        if sorts:
-            setting_list = list(
-                map(
-                    lambda x: (x["field"], int(x["ascending"])),
-                    [item for item in sorts if "field" in item and item["field"]],
-                )
-            )
-            if setting_list:
-                columns, order = zip(*setting_list)
-                if columns and order:
-                    is_subset = set(columns).issubset(set(full_df.columns.tolist()))
-                    if is_subset:
-                        full_df = full_df.sort_values(by=list(columns), ascending=list(order))
-                    else:
-                        msg = app_message.utils["utilities"]["sort_column_not_in_df"]
-                        bug_handler.default_node_log(flow_id, node_key, msg, console_level="WARN", bug_level="warning")
-
-        return full_df
-
-    def get_head_of_df_as_list(
-        self,
-        port_df: pd.DataFrame,
-        config: dict,
-        flow_id: str = None,
-        node_key: str = None,
-        port_name: str = None,
-    ):
-        # * Check if exists duplicated columns
-        if any(port_df.columns.duplicated()):
-            duplicated : pd.DataFrame = port_df.loc[:, port_df.columns.duplicated()]
-            msg = app_message.utils["utilities"]["duplicated_columns"](" ,".join(duplicated.columns.to_list()))
-            bug_handler.default_node_log(flow_id, node_key, msg, console_level="WARN", bug_level="warning")
-            # * Remove dupicated columns from Dataframe
-            port_df = port_df.loc[:, ~port_df.columns.duplicated()]
-
-        df: pd.DataFrame = port_df.head(50).copy()
-        page_num = config["page"] if "page" in config else 1
-        page_size = len(port_df) if "rows" in config and config["rows"] > len(port_df) else config["rows"]
-        
-        # sort
-        if df is not None and len(df) and "sort_by" in config and len(config["sort_by"]) > 0:
-            port_df = self.sort_df(port_df, config["sort_by"], flow_id, node_key)
-            cached_node = cache_handler.cache[flow_id][node_key] if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id] else dict()
-            # Actualizar cache del nodo con el nuevo order
-            if flow_id and node_key and port_name:
-                # Actualizar cache del nodo con el nuevo order
-                if cached_node["pout"]:
-                    cached_node["pout"][port_name] = port_df
-                    cache_handler.update_node(flow_id, node_key, {"pout": cached_node["pout"]})
-
-        if config["source"] == "head":
-            start = page_size * (page_num - 1)
-            df = port_df[start : start + page_size].copy()
-        elif config["source"] == "tail":
-            start = page_size * (page_num)
-            if start == page_size:
-                df = port_df[-start:].copy()
-            else:
-                df = port_df[-start : -start + page_size].copy()
-        elif config["source"] == "sample":
-            df = port_df.sample(page_size).copy()
-            if len(df) and "sort_by" in config and len(config["sort_by"]) > 0:
-                df = self.sort_df(df, config["sort_by"], flow_id, node_key)
-        else:
-            df = port_df.head(50).copy()
-            print("Source {} no reconocido opciones válidas [head|sample|tail]. Se utilizará head(50)".format(config["source"]))
-
-        # decimals
-        if config["decimals"] != -1:
-            df = df.round(config["decimals"])
-
-            # float_columns = df.select_dtypes(include=['float16', 'float32', 'float64']).columns
-            # for c in float_columns:
-            #     df[c] = df[c].apply(lambda x: f'{{:.{config["decimals"]}f}}'.format(x))
-
-        # Esto para efectos de la visualización al transformar a json
-        # special_cols = df.select_dtypes(include=['bool', 'datetime64', 'category']).columns.values.tolist()
-        special_cols = df.select_dtypes(
-            exclude=[
-                # "object",  # NOTE: Timestamp parece ser de tipo 'object'. TypeError: Object of type Timestamp is not JSON serializable
-                "int8",
-                "int16",
-                "int32",
-                "int64",
-                "float16",
-                "float32",
-                "float64",
-                # "Int8", # tipo de dato Bigquery
-                # "Int16", # tipo de dato Bigquery
-                # "Int32", # tipo de dato Bigquery
-                # "Int64", # tipo de dato Bigquery
-                # "Float16", # tipo de dato Bigquery
-                # "Float32", # tipo de dato Bigquery
-                # "Float64", # tipo de dato Bigquery
-            ]
-        ).columns.values.tolist()
-
-        if len(special_cols):
-            df[special_cols] = df[special_cols].astype(str)
-
-        try:
-            df = df.fillna("NaN")
-        except Exception as e:
-            df.replace([None, ''], np.nan, inplace=True)
-
-        try:
-            df.replace(["nan", "None", None, ''], "NaN", inplace=True)
-        except Exception as e:
-            df.replace(["nan", "None", None, ''], np.nan, inplace=True)
-
-
-        df_head = df.to_dict("records")
-        return df_head
-
-    def format_setting(self, settings, ignore_keys=["ports_map", "readed_from_cache"]):
-        setting_copy = {key: value for key, value in settings.items() if key not in ignore_keys}
-        return json.dumps(setting_copy, sort_keys=True)
-
-    def viz_summary(self, df):
-        cat_col = df.select_dtypes(include=["object", "category", "bool", "datetime64", "timedelta"]).columns.tolist()
-        num_col = df.select_dtypes(include=["int16", "int32", "int64", "float16", "float32", "float64"]).columns.tolist()
-        # date_col = df.select_dtypes(include=['datetime64', 'timedelta']).columns.tolist()
-        out = {}
-        for c in num_col:
-            count, bin_ = np.histogram(df[c][np.isfinite(df[c])])
-            out[c] = {
-                "viz_type": "histogram",
-                "y": count.tolist(),
-                "x": np.around(bin_, decimals=2).tolist(),
-            }
-
-        max_cat = 3
-        for c in cat_col:
-            cat_viz = "pie"
-            vc = df[c].value_counts().iloc[:max_cat]
-            vc.index = vc.index.astype("str")
-            cat_counts = vc.to_dict()
-            if df[c].nunique() > max_cat:
-                others = df[~df[c].isin(vc.index)][c].value_counts()
-                cat_counts[f"Other ({len(others)})"] = others.sum().item()
-                cat_viz = "list"
-            out[c] = {"viz_type": cat_viz, "values": cat_counts}
-        return out
-
-    def get_central_tendency_measures(self, df: pd.DataFrame):
-        if df.empty:
-            return {}
-        info = df.describe(percentiles=[0.1, 0.25, 0.5, 0.75, 0.9], include="all", datetime_is_numeric=True).T.reset_index()
-        # info = info.astype(str)
-        # print(info.dtypes)
-        jsonlist = json.loads(info.to_json(orient="records"))
-        return dict([(x["index"], x) for x in jsonlist])
-
-    def find_imports(self, code_snippet: str):
-        code_snippet = "\n".join([l for l in code_snippet.split("\n") if len(l) > 0 and l[0] != "#"])
-        # Busco los modulos que tienen la forma ['import * as *']
-        matchs = re.findall("import (.*?) as (.*?)$", code_snippet, flags=re.MULTILINE)
-        # print(matchs)
-        out = [{"name": m[0].strip(), "alias": m[1].strip(), "objects": []} for m in matchs]
-        # print(out)
-        # Busco los ['from * import *', 'import *']
-        # modules = []
-        for node in ast.iter_child_nodes(ast.parse(code_snippet)):
-            if isinstance(node, ast.ImportFrom):
-                objects = [node.names[i].name for i in range(len(node.names))]
-                if not node.names[0].asname:  # excluding the 'as' part of import
-                    # modules.append(node.module)
-                    out.append({"name": node.module, "alias": None, "objects": objects})
-            elif isinstance(node, ast.Import):  # excluding the 'as' part of import
-                if not node.names[0].asname:
-                    out.append({"name": node.names[0].name, "alias": None, "objects": []})
-                    # modules.append(node.names[0].name)
-        return out
-
-    def iqr_outliers(self, col: pd.Series):
-        q1 = col.quantile(0.25)
-        q3 = col.quantile(0.75)
-        IQR = q3 - q1
-        ll = q1 - (1.5 * IQR)
-        ul = q3 + (1.5 * IQR)
-        upper_outliers = col[col > ul].index.tolist()
-        lower_outliers = col[col < ll].index.tolist()
-        return list(set(upper_outliers + lower_outliers))
-
-    def zscore_outliers(self, col: pd.Series, limit: int):
-        return col[np.abs(stats.zscore(col)) >= limit]
-
-    def get_nulls(self, df: pd.DataFrame):
-        nulls = {}
-        for col_name in df.columns:
-            col = df[col_name]
-            nulls[col_name] = len(col[col.isnull()])
-        return nulls
-
-    def get_zero_excess(self, col: pd.Series):
-        r = col.rolling(int(round(len(col) * 0.05)))
-        return col[r.min().eq(0) & r.max().eq(0)]
-
-    def get_interaction_data(self, df: pd.DataFrame, x_col: str, y_col: str, max_cats: int = 5):
-        if x_col not in df.columns:
-            msg = app_message.utils["utilities"]["var_not_in_df"](str(x_col))
-            return {"success": False, "error": msg}
-        if y_col not in df.columns:
-            msg = app_message.utils["utilities"]["var_not_in_df"](str(y_col))
-            return {"success": False, "error": msg}
-
-        x_isNumeric = is_numeric_dtype(df[x_col])
-        y_isNumeric = is_numeric_dtype(df[y_col])
-
-        if x_isNumeric and y_isNumeric:  # ambos numericos
-            return {
-                "type": "scatter",
-                "data": [
-                    {
-                        "x": df[x_col].values.tolist(),
-                        "y": df[y_col].values.tolist(),
-                        "mode": "markers",
-                        "type": "scatter",
-                    }
-                ],
-            }
-        else:
-            x_cats = df[x_col].value_counts(dropna=False)[:max_cats].keys()
-            y_cats = df[y_col].value_counts(dropna=False)[:max_cats].keys()
-
-            x_cats = [str(x) for x in x_cats]
-            y_cats = [str(x) for x in y_cats]
-
-            df["x_"] = df[x_col].apply(lambda l: str(l) if str(l) in x_cats else "Other")
-            df["y_"] = df[y_col].apply(lambda l: str(l) if str(l) in y_cats else "Other")
-
-            # agregar contador de others
-            other_x = df[df["x_"] == "Other"][x_col].nunique(dropna=False)
-            df["x_"] = df["x_"].apply(lambda x: f"{x}({other_x})" if x == "Other" else x)
-
-            other_y = df[df["y_"] == "Other"][y_col].nunique(dropna=False)
-            df["y_"] = df["y_"].apply(lambda x: f"{x}({other_y})" if x == "Other" else x)
-
-            if not x_isNumeric and not y_isNumeric:  # ambos categoricos
-                df_out = df[["x_", "y_"]].value_counts().reset_index(name="count")
-                df_out["x_"] = df_out["x_"].astype(str)
-                df_out["y_"] = df_out["y_"].astype(str)
-
-                return {
-                    "type": "table",
-                    "data": df_out.rename(columns={"x_": "x", "y_": "y"}).to_dict("records"),
-                }
-            else:  # categorico y numerico
-                cat_key = "x_" if y_isNumeric else "y_"
-                val_key = "x_" if x_isNumeric else "y_"
-                val_col = x_col if x_isNumeric else y_col
-
-                df_out = df.groupby(cat_key)[val_col].apply(list).reset_index(name=val_key.replace("_", ""))
-                df_out[cat_key] = df_out[cat_key].astype(str)
-                df_out["type"] = "box"
-                return {
-                    "type": "box",
-                    "data": df_out.rename(columns={cat_key: "name"}).to_dict("records"),
-                }
-
-
-utilities = Utilities()
+import ast
+import json
+import re
+
+import numpy as np
+import pandas as pd
+from pandas.api.types import is_numeric_dtype
+from scipy import stats
+
+from vtarget.handlers.bug_handler import bug_handler
+from vtarget.handlers.cache_handler import cache_handler
+from vtarget.language.app_message import app_message
+
+
+class Utilities:
+    # Retorna la metadata del dtypes de un df
+    def get_dtypes_of_df(self, df: pd.DataFrame):
+        dict_dtypes = {}
+        res = df.dtypes.to_frame("dtypes")
+        res = res["dtypes"].astype(str).reset_index()
+        res["selected"] = True
+        res["order"] = pd.RangeIndex(stop=res.shape[0])
+        for _, x in res.iterrows():
+            dict_dtypes[x["index"]] = {
+                "dtype": x["dtypes"],
+                "selected": x["selected"],
+                "order": x["order"],
+            }
+
+        return dict_dtypes
+
+    def get_table_config(self, meta: dict, port_name: str):
+        # ? Sacar config desde meta.ports_config con el puerto
+        ports_config: dict = meta["ports_config"][port_name] if "ports_config" in meta and port_name in meta["ports_config"] else {}
+        return {
+            "page": ports_config["page"] if "page" in ports_config else 1,
+            "rows": ports_config["rows"] if "rows" in ports_config and ports_config["rows"] is not None else 50,
+            "decimals": ports_config["decimals"] if "decimals" in ports_config and ports_config["decimals"] is not None else -1,
+            "source": ports_config["source"] if "source" in ports_config and ports_config["source"] else "head",
+            "sort_by": ports_config["sort_by"] if "sort_by" in ports_config and ports_config["sort_by"] else [],
+        }
+
+    def sort_df(self, full_df: pd.DataFrame, sorts: list[dict], flow_id, node_key):
+        if sorts:
+            setting_list = list(
+                map(
+                    lambda x: (x["field"], int(x["ascending"])),
+                    [item for item in sorts if "field" in item and item["field"]],
+                )
+            )
+            if setting_list:
+                columns, order = zip(*setting_list)
+                if columns and order:
+                    is_subset = set(columns).issubset(set(full_df.columns.tolist()))
+                    if is_subset:
+                        full_df = full_df.sort_values(by=list(columns), ascending=list(order))
+                    else:
+                        msg = app_message.utils["utilities"]["sort_column_not_in_df"]
+                        bug_handler.default_node_log(flow_id, node_key, msg, console_level="WARN", bug_level="warning")
+
+        return full_df
+
+    def get_head_of_df_as_list(
+        self,
+        port_df: pd.DataFrame,
+        config: dict,
+        flow_id: str = None,
+        node_key: str = None,
+        port_name: str = None,
+    ):
+        # * Check if exists duplicated columns
+        if any(port_df.columns.duplicated()):
+            duplicated : pd.DataFrame = port_df.loc[:, port_df.columns.duplicated()]
+            msg = app_message.utils["utilities"]["duplicated_columns"](" ,".join(duplicated.columns.to_list()))
+            bug_handler.default_node_log(flow_id, node_key, msg, console_level="WARN", bug_level="warning")
+            # * Remove dupicated columns from Dataframe
+            port_df = port_df.loc[:, ~port_df.columns.duplicated()]
+
+        df: pd.DataFrame = port_df.head(50).copy()
+        page_num = config["page"] if "page" in config else 1
+        page_size = len(port_df) if "rows" in config and config["rows"] > len(port_df) else config["rows"]
+        
+        # sort
+        if df is not None and len(df) and "sort_by" in config and len(config["sort_by"]) > 0:
+            port_df = self.sort_df(port_df, config["sort_by"], flow_id, node_key)
+            cached_node = cache_handler.cache[flow_id][node_key] if flow_id in cache_handler.cache and node_key in cache_handler.cache[flow_id] else dict()
+            # Actualizar cache del nodo con el nuevo order
+            if flow_id and node_key and port_name:
+                # Actualizar cache del nodo con el nuevo order
+                if cached_node["pout"]:
+                    cached_node["pout"][port_name] = port_df
+                    cache_handler.update_node(flow_id, node_key, {"pout": cached_node["pout"]})
+
+        if config["source"] == "head":
+            start = page_size * (page_num - 1)
+            df = port_df[start : start + page_size].copy()
+        elif config["source"] == "tail":
+            start = page_size * (page_num)
+            if start == page_size:
+                df = port_df[-start:].copy()
+            else:
+                df = port_df[-start : -start + page_size].copy()
+        elif config["source"] == "sample":
+            df = port_df.sample(page_size).copy()
+            if len(df) and "sort_by" in config and len(config["sort_by"]) > 0:
+                df = self.sort_df(df, config["sort_by"], flow_id, node_key)
+        else:
+            df = port_df.head(50).copy()
+            print("Source {} no reconocido opciones válidas [head|sample|tail]. Se utilizará head(50)".format(config["source"]))
+
+        # decimals
+        if config["decimals"] != -1:
+            df = df.round(config["decimals"])
+
+            # float_columns = df.select_dtypes(include=['float16', 'float32', 'float64']).columns
+            # for c in float_columns:
+            #     df[c] = df[c].apply(lambda x: f'{{:.{config["decimals"]}f}}'.format(x))
+
+        # Esto para efectos de la visualización al transformar a json
+        # special_cols = df.select_dtypes(include=['bool', 'datetime64', 'category']).columns.values.tolist()
+        special_cols = df.select_dtypes(
+            exclude=[
+                # "object",  # NOTE: Timestamp parece ser de tipo 'object'. TypeError: Object of type Timestamp is not JSON serializable
+                "int8",
+                "int16",
+                "int32",
+                "int64",
+                "float16",
+                "float32",
+                "float64",
+                # "Int8", # tipo de dato Bigquery
+                # "Int16", # tipo de dato Bigquery
+                # "Int32", # tipo de dato Bigquery
+                # "Int64", # tipo de dato Bigquery
+                # "Float16", # tipo de dato Bigquery
+                # "Float32", # tipo de dato Bigquery
+                # "Float64", # tipo de dato Bigquery
+            ]
+        ).columns.values.tolist()
+
+        if len(special_cols):
+            df[special_cols] = df[special_cols].astype(str)
+
+        try:
+            df = df.fillna("NaN")
+        except Exception as e:
+            df.replace([None, ''], np.nan, inplace=True)
+
+        try:
+            df.replace(["nan", "None", None, ''], "NaN", inplace=True)
+        except Exception as e:
+            df.replace(["nan", "None", None, ''], np.nan, inplace=True)
+
+
+        df_head = df.to_dict("records")
+        return df_head
+
+    def format_setting(self, settings, ignore_keys=["ports_map", "readed_from_cache"]):
+        setting_copy = {key: value for key, value in settings.items() if key not in ignore_keys}
+        return json.dumps(setting_copy, sort_keys=True)
+
+    def viz_summary(self, df):
+        cat_col = df.select_dtypes(include=["object", "category", "bool", "datetime64", "timedelta"]).columns.tolist()
+        num_col = df.select_dtypes(include=["int16", "int32", "int64", "float16", "float32", "float64"]).columns.tolist()
+        # date_col = df.select_dtypes(include=['datetime64', 'timedelta']).columns.tolist()
+        out = {}
+        for c in num_col:
+            count, bin_ = np.histogram(df[c][np.isfinite(df[c])])
+            out[c] = {
+                "viz_type": "histogram",
+                "y": count.tolist(),
+                "x": np.around(bin_, decimals=2).tolist(),
+            }
+
+        max_cat = 3
+        for c in cat_col:
+            cat_viz = "pie"
+            vc = df[c].value_counts().iloc[:max_cat]
+            vc.index = vc.index.astype("str")
+            cat_counts = vc.to_dict()
+            if df[c].nunique() > max_cat:
+                others = df[~df[c].isin(vc.index)][c].value_counts()
+                cat_counts[f"Other ({len(others)})"] = others.sum().item()
+                cat_viz = "list"
+            out[c] = {"viz_type": cat_viz, "values": cat_counts}
+        return out
+
+    def get_central_tendency_measures(self, df: pd.DataFrame):
+        if df.empty:
+            return {}
+        info = df.describe(percentiles=[0.1, 0.25, 0.5, 0.75, 0.9], include="all", datetime_is_numeric=True).T.reset_index()
+        # info = info.astype(str)
+        # print(info.dtypes)
+        jsonlist = json.loads(info.to_json(orient="records"))
+        return dict([(x["index"], x) for x in jsonlist])
+
+    def find_imports(self, code_snippet: str):
+        code_snippet = "\n".join([l for l in code_snippet.split("\n") if len(l) > 0 and l[0] != "#"])
+        # Busco los modulos que tienen la forma ['import * as *']
+        matchs = re.findall("import (.*?) as (.*?)$", code_snippet, flags=re.MULTILINE)
+        # print(matchs)
+        out = [{"name": m[0].strip(), "alias": m[1].strip(), "objects": []} for m in matchs]
+        # print(out)
+        # Busco los ['from * import *', 'import *']
+        # modules = []
+        for node in ast.iter_child_nodes(ast.parse(code_snippet)):
+            if isinstance(node, ast.ImportFrom):
+                objects = [node.names[i].name for i in range(len(node.names))]
+                if not node.names[0].asname:  # excluding the 'as' part of import
+                    # modules.append(node.module)
+                    out.append({"name": node.module, "alias": None, "objects": objects})
+            elif isinstance(node, ast.Import):  # excluding the 'as' part of import
+                if not node.names[0].asname:
+                    out.append({"name": node.names[0].name, "alias": None, "objects": []})
+                    # modules.append(node.names[0].name)
+        return out
+
+    def iqr_outliers(self, col: pd.Series):
+        q1 = col.quantile(0.25)
+        q3 = col.quantile(0.75)
+        IQR = q3 - q1
+        ll = q1 - (1.5 * IQR)
+        ul = q3 + (1.5 * IQR)
+        upper_outliers = col[col > ul].index.tolist()
+        lower_outliers = col[col < ll].index.tolist()
+        return list(set(upper_outliers + lower_outliers))
+
+    def zscore_outliers(self, col: pd.Series, limit: int):
+        return col[np.abs(stats.zscore(col)) >= limit]
+
+    def get_nulls(self, df: pd.DataFrame):
+        nulls = {}
+        for col_name in df.columns:
+            col = df[col_name]
+            nulls[col_name] = len(col[col.isnull()])
+        return nulls
+
+    def get_zero_excess(self, col: pd.Series):
+        r = col.rolling(int(round(len(col) * 0.05)))
+        return col[r.min().eq(0) & r.max().eq(0)]
+
+    def get_interaction_data(self, df: pd.DataFrame, x_col: str, y_col: str, max_cats: int = 5):
+        if x_col not in df.columns:
+            msg = app_message.utils["utilities"]["var_not_in_df"](str(x_col))
+            return {"success": False, "error": msg}
+        if y_col not in df.columns:
+            msg = app_message.utils["utilities"]["var_not_in_df"](str(y_col))
+            return {"success": False, "error": msg}
+
+        x_isNumeric = is_numeric_dtype(df[x_col])
+        y_isNumeric = is_numeric_dtype(df[y_col])
+
+        if x_isNumeric and y_isNumeric:  # ambos numericos
+            return {
+                "type": "scatter",
+                "data": [
+                    {
+                        "x": df[x_col].values.tolist(),
+                        "y": df[y_col].values.tolist(),
+                        "mode": "markers",
+                        "type": "scatter",
+                    }
+                ],
+            }
+        else:
+            x_cats = df[x_col].value_counts(dropna=False)[:max_cats].keys()
+            y_cats = df[y_col].value_counts(dropna=False)[:max_cats].keys()
+
+            x_cats = [str(x) for x in x_cats]
+            y_cats = [str(x) for x in y_cats]
+
+            df["x_"] = df[x_col].apply(lambda l: str(l) if str(l) in x_cats else "Other")
+            df["y_"] = df[y_col].apply(lambda l: str(l) if str(l) in y_cats else "Other")
+
+            # agregar contador de others
+            other_x = df[df["x_"] == "Other"][x_col].nunique(dropna=False)
+            df["x_"] = df["x_"].apply(lambda x: f"{x}({other_x})" if x == "Other" else x)
+
+            other_y = df[df["y_"] == "Other"][y_col].nunique(dropna=False)
+            df["y_"] = df["y_"].apply(lambda x: f"{x}({other_y})" if x == "Other" else x)
+
+            if not x_isNumeric and not y_isNumeric:  # ambos categoricos
+                df_out = df[["x_", "y_"]].value_counts().reset_index(name="count")
+                df_out["x_"] = df_out["x_"].astype(str)
+                df_out["y_"] = df_out["y_"].astype(str)
+
+                return {
+                    "type": "table",
+                    "data": df_out.rename(columns={"x_": "x", "y_": "y"}).to_dict("records"),
+                }
+            else:  # categorico y numerico
+                cat_key = "x_" if y_isNumeric else "y_"
+                val_key = "x_" if x_isNumeric else "y_"
+                val_col = x_col if x_isNumeric else y_col
+
+                df_out = df.groupby(cat_key)[val_col].apply(list).reset_index(name=val_key.replace("_", ""))
+                df_out[cat_key] = df_out[cat_key].astype(str)
+                df_out["type"] = "box"
+                return {
+                    "type": "box",
+                    "data": df_out.rename(columns={cat_key: "name"}).to_dict("records"),
+                }
+
+
+utilities = Utilities()
```

### Comparing `vtarget-0.8.6/vtarget.egg-info/PKG-INFO` & `vtarget-0.8.7/vtarget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtarget
-Version: 0.8.6
+Version: 0.8.7
 Summary: vtarget lib
 Author: vTarget Team
 Author-email: contact@vtarget.ai
 License: BSD
 Keywords: vtarget,dataprep
 Requires-Python: >=3.9.0,<3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `vtarget-0.8.6/vtarget.egg-info/SOURCES.txt` & `vtarget-0.8.7/vtarget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

