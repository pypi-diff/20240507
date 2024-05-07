# Comparing `tmp/dbt_snowflake-1.8.0b3.tar.gz` & `tmp/dbt_snowflake-1.8.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snowflake-1.8.0b3.tar", last modified: Wed Apr 17 16:37:08 2024, max compression
+gzip compressed data, was "dbt_snowflake-1.8.0b4.tar", last modified: Mon May  6 23:46:16 2024, max compression
```

## Comparing `dbt_snowflake-1.8.0b3.tar` & `dbt_snowflake-1.8.0b4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.978399 dbt_snowflake-1.8.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.978399 dbt_snowflake-1.8.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.982399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/dynamic_table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/metadata.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/drop.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.986400 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:08.990399 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 16:37:08.000000 dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:37:08.994400 dbt_snowflake-1.8.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-17 16:36:57.000000 dbt_snowflake-1.8.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.167313 dbt_snowflake-1.8.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 23:46:16.167313 dbt_snowflake-1.8.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.155313 dbt_snowflake-1.8.0b4/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.155313 dbt_snowflake-1.8.0b4/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.159313 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.159313 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.155313 dbt_snowflake-1.8.0b4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.159313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.159313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.163313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/dynamic_table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/metadata.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.163313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/drop.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.163313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.163313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.163313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.167313 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:46:16.167313 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 23:46:16.000000 dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:46:16.167313 dbt_snowflake-1.8.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-06 23:46:05.000000 dbt_snowflake-1.8.0b4/setup.py
```

### Comparing `dbt_snowflake-1.8.0b3/LICENSE.md` & `dbt_snowflake-1.8.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/PKG-INFO` & `dbt_snowflake-1.8.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b3
+Version: 1.8.0b4
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
-Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
+Requires-Dist: dbt-adapters<2.0,>=1.1.0rc1
 Requires-Dist: snowflake-connector-python[secure-local-storage]~=3.0
 Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b3 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b4 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: dbt-
-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-Dist:
+common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=1.1.0rc1 Requires-Dist:
 snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: dbt-
 core>=1.8.0a1 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
```

### Comparing `dbt_snowflake-1.8.0b3/README.md` & `dbt_snowflake-1.8.0b4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/__init__.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/column.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/connections.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/impl.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class SnowflakeRelation(BaseRelation):
     type: Optional[SnowflakeRelationType] = None  # type: ignore
     quote_policy: SnowflakeQuotePolicy = field(default_factory=lambda: SnowflakeQuotePolicy())
-
+    require_alias: bool = False
     renameable_relations: FrozenSet[SnowflakeRelationType] = field(
         default_factory=lambda: frozenset(
             {
                 SnowflakeRelationType.Table,
                 SnowflakeRelationType.View,
             }
         )
```

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/base.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/dynamic_table.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/adapters/snowflake/relation_configs/policies.py` & `dbt_snowflake-1.8.0b4/dbt/adapters/snowflake/relation_configs/policies.py`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/adapters.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/catalog.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/dynamic_table.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/dynamic_table.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/materializations/table.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/metadata.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/table/create.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/relations/view/create.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt/include/snowflake/profile_template.yml` & `dbt_snowflake-1.8.0b4/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/PKG-INFO` & `dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b3
+Version: 1.8.0b4
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
-Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
+Requires-Dist: dbt-adapters<2.0,>=1.1.0rc1
 Requires-Dist: snowflake-connector-python[secure-local-storage]~=3.0
 Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b3 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b4 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: dbt-
-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-Dist:
+common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=1.1.0rc1 Requires-Dist:
 snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: dbt-
 core>=1.8.0a1 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
```

### Comparing `dbt_snowflake-1.8.0b3/dbt_snowflake.egg-info/SOURCES.txt` & `dbt_snowflake-1.8.0b4/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_snowflake-1.8.0b3/setup.py` & `dbt_snowflake-1.8.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 package_name = "dbt-snowflake"
-package_version = "1.8.0b3"
+package_version = "1.8.0b4"
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
@@ -56,15 +56,15 @@
     author="dbt Labs",
     author_email="info@dbtlabs.com",
     url="https://github.com/dbt-labs/dbt-snowflake",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=0.1.0a1,<2.0",
-        "dbt-adapters>=0.1.0a1,<2.0",
+        "dbt-adapters>=1.1.0rc1,<2.0",
         "snowflake-connector-python[secure-local-storage]~=3.0",
         # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
         "dbt-core>=1.8.0a1",
         # installed via dbt-core but referenced directly; don't pin to avoid version conflicts with dbt-core
         "agate",
     ],
     zip_safe=False,
```
