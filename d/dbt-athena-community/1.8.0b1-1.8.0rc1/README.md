# Comparing `tmp/dbt_athena_community-1.8.0b1.tar.gz` & `tmp/dbt_athena_community-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_athena_community-1.8.0b1.tar", last modified: Mon Apr 15 19:25:07 2024, max compression
+gzip compressed data, was "dbt_athena_community-1.8.0rc1.tar", last modified: Tue May  7 07:24:18 2024, max compression
```

## Comparing `dbt_athena_community-1.8.0b1.tar` & `dbt_athena_community-1.8.0rc1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.925308 dbt_athena_community-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-04-15 19:25:07.925308 dbt_athena_community-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32051 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.913308 dbt_athena_community-1.8.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.913308 dbt_athena_community-1.8.0b1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.913308 dbt_athena_community-1.8.0b1/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57359 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/lakeformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.909308 dbt_athena_community-1.8.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.909308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/python_submissions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.909308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.917308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.921308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.921308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.921308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.921308 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:25:07.925308 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33195 2024-04-15 19:25:07.000000 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-15 19:25:07.000000 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:25:07.000000 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 19:25:07.000000 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:25:07.000000 dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:25:07.925308 dbt_athena_community-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 19:25:02.000000 dbt_athena_community-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33196 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32051 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57310 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/lakeformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/python_submissions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.737608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.733608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.741608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33196 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 07:24:18.000000 dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:24:18.745608 dbt_athena_community-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-07 07:24:14.000000 dbt_athena_community-1.8.0rc1/setup.py
```

### Comparing `dbt_athena_community-1.8.0b1/LICENSE.txt` & `dbt_athena_community-1.8.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/PKG-INFO` & `dbt_athena_community-1.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.0b1
+Version: 1.8.0rc1
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0rc1 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `dbt_athena_community-1.8.0b1/README.md` & `dbt_athena_community-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/column.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/config.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/config.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/connections.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,14 @@
             "work_group",
             "region_name",
             "database",
             "schema",
             "poll_interval",
             "aws_profile_name",
             "aws_access_key_id",
-            "aws_secret_access_key",
-            "aws_session_token",
             "endpoint_url",
             "s3_data_dir",
             "s3_data_naming",
             "s3_tmp_table_dir",
             "debug_query_state",
             "seed_s3_upload_args",
             "lf_tags_database",
```

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/constants.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/impl.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -690,56 +690,55 @@
         client = conn.handle
         with boto3_client_lock:
             glue_client = client.session.client(
                 "glue",
                 region_name=client.region_name,
                 config=get_boto3_config(num_retries=creds.effective_num_retries),
             )
-        paginator = glue_client.get_paginator("get_tables")
 
         kwargs = {
             "DatabaseName": schema_relation.schema,
         }
-        # If the catalog is `awsdatacatalog` we don't need to pass CatalogId as boto3 infers it from the account Id.
         if catalog_id := get_catalog_id(data_catalog):
             kwargs["CatalogId"] = catalog_id
-        page_iterator = paginator.paginate(**kwargs)
-
-        relations = []
-        quote_policy = {"database": True, "schema": True, "identifier": True}
-
+        paginator = glue_client.get_paginator("get_tables")
         try:
-            for page in page_iterator:
-                tables = page["TableList"]
-                for table in tables:
-                    if "TableType" not in table:
-                        LOGGER.debug(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
-                        continue
-                    _type = table["TableType"]
-                    _detailed_table_type = table.get("Parameters", {}).get("table_type", "")
-                    if _type == "VIRTUAL_VIEW":
-                        _type = self.Relation.View
-                    else:
-                        _type = self.Relation.Table
-
-                    relations.append(
-                        self.Relation.create(
-                            schema=schema_relation.schema,
-                            database=schema_relation.database,
-                            identifier=table["Name"],
-                            quote_policy=quote_policy,
-                            type=_type,
-                            detailed_table_type=_detailed_table_type,
-                        )
-                    )
+            tables = paginator.paginate(**kwargs).build_full_result().get("TableList")
         except ClientError as e:
             # don't error out when schema doesn't exist
             # this allows dbt to create and manage schemas/databases
-            LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
+            if e.response["Error"]["Code"] == "EntityNotFoundException":
+                LOGGER.debug(f"Schema '{schema_relation.schema}' does not exist - Ignoring: {e}")
+                return []
+            else:
+                raise e
+
+        relations: list[BaseRelation] = []
+        quote_policy = {"database": True, "schema": True, "identifier": True}
+        for table in tables:
+            if "TableType" not in table:
+                LOGGER.info(f"Table '{table['Name']}' has no TableType attribute - Ignoring")
+                continue
+            _type = table["TableType"]
+            _detailed_table_type = table.get("Parameters", {}).get("table_type", "")
+            if _type == "VIRTUAL_VIEW":
+                _type = self.Relation.View
+            else:
+                _type = self.Relation.Table
 
+            relations.append(
+                self.Relation.create(
+                    schema=schema_relation.schema,
+                    database=schema_relation.database,
+                    identifier=table["Name"],
+                    quote_policy=quote_policy,
+                    type=_type,
+                    detailed_table_type=_detailed_table_type,
+                )
+            )
         return relations
 
     def _get_one_catalog_by_relations(
         self,
         information_schema: InformationSchema,
         relations: List[AthenaRelation],
         used_schemas: FrozenSet[Tuple[str, str]],
@@ -1078,18 +1077,23 @@
         with boto3_client_lock:
             glue_client = client.session.client(
                 "glue",
                 region_name=client.region_name,
                 config=get_boto3_config(num_retries=creds.effective_num_retries),
             )
 
+        get_table_kwargs = dict(
+            DatabaseName=relation.schema,
+            Name=relation.identifier,
+        )
+        if catalog_id:
+            get_table_kwargs["CatalogId"] = catalog_id
+
         try:
-            table = glue_client.get_table(CatalogId=catalog_id, DatabaseName=relation.schema, Name=relation.identifier)[
-                "Table"
-            ]
+            table = glue_client.get_table(**get_table_kwargs)["Table"]
         except ClientError as e:
             if e.response["Error"]["Code"] == "EntityNotFoundException":
                 LOGGER.debug("table not exist, catching the error")
                 return []
             else:
                 LOGGER.error(e)
                 raise e
```

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/lakeformation.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/lakeformation.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/python_submissions.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/query_headers.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/relation.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/session.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/session.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/adapters/athena/utils.py` & `dbt_athena_community-1.8.0rc1/dbt/adapters/athena/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/columns.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/metadata.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/python_submissions.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/python_submissions.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/adapters/relation.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/hooks.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/get_partition_batches.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/helpers/process_bucket_column.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/merge.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/table/table.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/table/table.sql`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,14 @@
         {%- do rename_relation(tmp_relation, target_relation) -%}
       {%- else -%}
         -- delete old tmp iceberg table if it exists
         {%- if old_tmp_relation is not none -%}
           {%- do drop_relation(old_tmp_relation) -%}
         {%- endif -%}
 
-        {%- set old_relation_bkp = make_temp_relation(old_relation, '__bkp') -%}
         -- If we have this, it means that at least the first renaming occurred but there was an issue
         -- afterwards, therefore we are in weird state. The easiest and cleanest should be to remove
         -- the backup relation. It won't have an impact because since we are in the else condition,
         -- that means that old relation exists therefore no downtime yet.
         {%- if old_bkp_relation is not none -%}
           {%- do drop_relation(old_bkp_relation) -%}
         {%- endif -%}
@@ -128,18 +127,30 @@
         {% set query_result = safe_create_table_as(False, tmp_relation, compiled_code, language, force_batch) %}
         -- Execute python code that is available in query result object
         {%- if language == 'python' -%}
           {% call statement('create_table', language=language) %}
             {{ query_result }}
           {% endcall %}
         {%- endif -%}
-        {{ rename_relation(old_relation, old_relation_bkp) }}
+
+        {%- set old_relation_table_type = adapter.get_glue_table_type(old_relation) -%}
+
+        {%- if old_relation_table_type == 'iceberg' -%}
+          {{ rename_relation(old_relation, old_bkp_relation) }}
+        {%- else  -%}
+          {%- do drop_relation_glue(old_relation) -%}
+        {%- endif -%}
+
         {{ rename_relation(tmp_relation, target_relation) }}
 
-        {{ drop_relation(old_relation_bkp) }}
+        -- old_bkp_relation might not exists in case we have a switch from hive to iceberg
+        -- we prevent to drop something that doesn't exist even if drop_relation is able to deal with not existing tables
+        {%- if old_bkp_relation is not none -%}
+          {%- do drop_relation(old_bkp_relation) -%}
+        {%- endif -%}
       {%- endif -%}
     {%- endif -%}
 
   {%- endif -%}
 
   {% call statement("main", language=language) %}
     {%- if language=='sql' -%}
```

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/models/view/view.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/datediff.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/ddl_dml_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/macros/utils/timestamps.sql` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt/include/athena/profile_template.yml` & `dbt_athena_community-1.8.0rc1/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/PKG-INFO` & `dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.8.0b1
+Version: 1.8.0rc1
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.8.0rc1 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena License: Apache License 2.0 Platform: any Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `dbt_athena_community-1.8.0b1/dbt_athena_community.egg-info/SOURCES.txt` & `dbt_athena_community-1.8.0rc1/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/pyproject.toml` & `dbt_athena_community-1.8.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_athena_community-1.8.0b1/setup.py` & `dbt_athena_community-1.8.0rc1/setup.py`

 * *Files identical despite different names*

