# Comparing `tmp/pydiverse_pipedag-0.9.1.tar.gz` & `tmp/pydiverse_pipedag-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.9.1.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.9.2.tar", max compression
```

## Comparing `pydiverse_pipedag-0.9.1.tar` & `pydiverse_pipedag-0.9.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1517 2024-04-26 13:54:34.519514 pydiverse_pipedag-0.9.1/LICENSE
--rw-r--r--   0        0        0     5623 2024-04-26 13:54:34.519514 pydiverse_pipedag-0.9.1/docs/package/README.md
--rw-r--r--   0        0        0     3912 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       13 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      629 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2024-04-26 13:54:34.523514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     6613 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6102 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13646 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    30931 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3455 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     7777 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6757 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      103 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    41933 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      230 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     4411 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0    10717 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0    12826 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     5490 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0     3777 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/snowflake.py
--rw-r--r--   0        0        0    30134 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4617 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    62658 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     9164 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0    12059 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    27776 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      408 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    26497 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    51959 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     7891 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/group_node.py
--rw-r--r--   0        0        0     4552 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     8529 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8768 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      135 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/debug/__init__.py
--rw-r--r--   0        0        0      493 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3123 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1981 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1191 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2795 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      258 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     2735 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    24375 2024-04-26 13:54:34.527514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    38201 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     4453 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/debug.py
--rw-r--r--   0        0        0     3837 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/details.py
--rw-r--r--   0        0        0     2074 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    21432 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     9273 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/computation_tracing.py
--rw-r--r--   0        0        0     2061 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1848 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3816 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     5375 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2024-04-26 13:54:34.531514 pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-07 16:08:18.160457 pydiverse_pipedag-0.9.2/LICENSE
+-rw-r--r--   0        0        0     5623 2024-05-07 16:08:18.160457 pydiverse_pipedag-0.9.2/docs/package/README.md
+-rw-r--r--   0        0        0     3912 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      683 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     6613 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6178 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13784 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    31271 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3455 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     7777 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6841 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      103 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    41933 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      230 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     4411 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0    10851 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0    12826 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     5490 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0     3777 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/snowflake.py
+-rw-r--r--   0        0        0    30134 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     5033 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    62730 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     9164 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0    19202 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    28491 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      408 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    20913 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    51959 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     7891 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/group_node.py
+-rw-r--r--   0        0        0     4552 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     9577 2024-05-07 16:08:18.168457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     9104 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      135 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/debug/__init__.py
+-rw-r--r--   0        0        0      493 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3123 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1981 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1191 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2795 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      308 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     2735 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    24551 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    62458 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     4453 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/debug.py
+-rw-r--r--   0        0        0     3837 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/details.py
+-rw-r--r--   0        0        0     2074 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    21874 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     9273 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/computation_tracing.py
+-rw-r--r--   0        0        0     2061 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1848 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3816 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     5681 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2024-05-07 16:08:18.172457 pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.9.2/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.9.1/LICENSE` & `pydiverse_pipedag-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/docs/package/README.md` & `pydiverse_pipedag-0.9.2/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/pyproject.toml` & `pydiverse_pipedag-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.9.1"
+version = "0.9.2"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/__init__.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 )
 from .materialize import (
     Blob,
     ExternalTableReference,
     RawSql,
     Schema,
     Table,
+    input_stage_versions,
     materialize,
 )
 from .materialize.core import AUTO_VERSION
 
 __all__ = [
     "Flow",
     "Stage",
     "materialize",
+    "input_stage_versions",
     "AUTO_VERSION",
     "Table",
     "RawSql",
     "Blob",
     "GroupNode",
     "VisualizationStyle",
     "Schema",
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from enum import Enum
 from typing import Callable, Union
 
 import structlog
 
-from pydiverse.pipedag.core import Stage
 from pydiverse.pipedag.errors import LockError
 from pydiverse.pipedag.util import Disposable
 
 
 class LockState(Enum):
     """Lock State
 
@@ -41,28 +40,32 @@
 
     UNLOCKED = 0
     LOCKED = 1
     UNCERTAIN = 2
     INVALID = 3
 
 
-Lockable = Union[Stage, str]  # noqa: UP007
+Lockable = Union[str]  # noqa: UP007
 LockStateListener = Callable[[Lockable, LockState, LockState], None]
 
 
 class BaseLockManager(Disposable, ABC):
     """Lock Manager base class
 
     A lock manager is responsible for acquiring and releasing locks on
     stage. This is necessary to prevent two flows from accessing the
     same stage at the same time (which would lead to corrupted data).
     """
 
-    def __init__(self):
-        self.logger = structlog.get_logger(logger_name=type(self).__name__)
+    def __init__(self, logger_kwargs=None):
+        if logger_kwargs is None:
+            logger_kwargs = {}
+        self.logger = structlog.get_logger(
+            logger_name=type(self).__name__, **logger_kwargs
+        )
 
         self.state_listeners = set()
         self.lock_states = {}
         self.__lock_state_lock = threading.Lock()
 
     @contextmanager
     def __call__(self, lock: Lockable):
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,19 @@
     def __init__(
         self,
         engine: sa.Engine,
         instance_id: str,
         lock_schema: Schema | None = None,
         create_lock_schema: bool = True,
     ):
-        super().__init__()
+        super().__init__(
+            logger_kwargs=dict(
+                engine_url=engine.url, instance_id=instance_id, schema=lock_schema
+            )
+        )
 
         self.engine = engine
         self.instance_id = instance_id
         self.lock_schema = lock_schema
         self.create_lock_schema = create_lock_schema
 
         # Stage level locking
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,17 +536,23 @@
 
         If the table doesn't exist in the transaction stage, fail silently.
         """
 
     def retrieve_table_obj(
         self,
         table: Table,
-        as_type: type[T],
+        as_type: type[T] | None,
         for_auto_versioning: bool = False,
     ) -> T:
+        if as_type is None:
+            # Simply return enough information that a user could dematerialize the table
+            # or perform it with some other library.
+            # hint: `schema = table_store.get_schema(table.stage.current_name).get()`
+            return table.name, table.stage.current_name
+
         if for_auto_versioning:
             return super().retrieve_table_obj(table, as_type, for_auto_versioning)
 
         if self.local_table_cache:
             obj = self.local_table_cache.retrieve_table_obj(table, as_type)
             if obj is not None:
                 return obj
@@ -659,15 +665,15 @@
         to produce those objects) when executing RawSQL.
 
         :param stage: the stage
         :return: list of object names in the stage at the current point in time.
         """
 
     @abstractmethod
-    def get_table_objects_in_stage(self, stage: Stage) -> list[str]:
+    def get_table_objects_in_stage(self, stage: Stage, include_views=True) -> list[str]:
         """
         List all table-like objects that are in the current stage.
 
         :param stage: the stage
         :return: list of table-like object names in the stage at
             the current point in time.
         """
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,16 @@
             return self.lazy_table_metadata[stage.name][cache_key]
         except (TypeError, KeyError):
             raise CacheError("Couldn't find metadata for lazy table") from None
 
     def get_objects_in_stage(self, stage):
         return list(self.store[stage.transaction_name].keys())
 
-    def get_table_objects_in_stage(self, stage: Stage) -> list[str]:
+    def get_table_objects_in_stage(self, stage: Stage, include_views=True) -> list[str]:
+        _ = include_views  # not supported for dict table store
         return list(self.store[stage.transaction_name].keys())
 
 
 @DictTableStore.register_table(pd)
 class PandasTableHook(TableHook[DictTableStore]):
     @classmethod
     def can_materialize(cls, type_) -> bool:
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections.abc import Iterable
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
-import sqlalchemy.exc
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateTableWithSuffix,
     LockSourceTable,
     LockTable,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import PandasTableHook
@@ -236,14 +235,17 @@
         if isinstance(compression, str):
             compression = [compression]
         elif compression is None:
             compression = []
         compression_suffix = " ".join(compression)
         return " ".join((table_space_suffix, compression_suffix))
 
+    def _get_all_objects_in_schema(self, schema: Schema) -> dict[str, Any]:
+        return PipedagDB2Reflection.get_all_objects(self.engine, schema.get())
+
 
 @IBMDB2TableStore.register_table(pd)
 class PandasTableHook(PandasTableHook):
     @classmethod
     def _get_dialect_dtypes(cls, dtypes: dict[str, DType], table: Table[pd.DataFrame]):
         # Default string target is CLOB which can't be used for indexing.
         # -> Convert indexed string columns to VARCHAR(256)
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/dialects/snowflake.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,26 @@
         """
         with engine.connect() as conn:
             aliases = conn.exec_driver_sql(query).scalars().all()
         aliases = [engine.dialect.normalize_name(name) for name in aliases]
         return list(aliases)
 
     @staticmethod
+    def get_all_objects(engine: sa.Engine, schema: str):
+        schema = engine.dialect.denormalize_name(schema)
+        query = f"""
+        SELECT TABNAME, TYPE
+        FROM SYSCAT.TABLES
+        WHERE TABSCHEMA = '{schema}'
+        """
+        with engine.connect() as conn:
+            result = conn.exec_driver_sql(query).all()
+        return {name: type_.strip() for name, type_ in result}
+
+    @staticmethod
     def resolve_alias(engine: sa.Engine, name: str, schema: str) -> tuple[str, str]:
         """Recursively resolves an alias
 
         :returns: A tuple (table_name, schema)
         """
 
         _schema = engine.dialect.denormalize_name(schema)
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1540,22 +1540,24 @@
             self.get_schema(stage_name).get()
             if table.external_schema is None
             else table.external_schema
         )
         return table.name, schema
 
     def get_objects_in_stage(self, stage: Stage):
-        schema = self.get_schema(stage.transaction_name)
+        schema = self.get_schema(stage.current_name)
         return list(self._get_all_objects_in_schema(schema).keys())
 
-    def get_table_objects_in_stage(self, stage: Stage):
+    def get_table_objects_in_stage(self, stage: Stage, include_views=True):
         schema = self.get_schema(stage.current_name).get()
         inspector = sa.inspect(self.engine)
 
         tables = inspector.get_table_names(schema)
+        if not include_views:
+            return tables
         views = inspector.get_view_names(schema)
         return [*tables, *views]
 
     def get_stage_hash(self, stage: Stage) -> str:
         """Compute hash that represents entire stage's output metadata."""
         # We only need to look in tasks_table since the output_json column is updated
         # after evaluating lazy output objects for cache validity. This is the same
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/context/context.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
+import copy
+import threading
 from collections.abc import Mapping
 from contextvars import ContextVar, Token
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from threading import Lock
-from typing import TYPE_CHECKING, ClassVar
+from typing import TYPE_CHECKING, Any, ClassVar
 
 import structlog
 from attrs import define, evolve, field, frozen
 from box import Box
 
 from pydiverse.pipedag.util import deep_merge
 from pydiverse.pipedag.util.import_ import import_object, load_object
@@ -23,37 +25,43 @@
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
     from pydiverse.pipedag.engine.base import OrchestrationEngine
     from pydiverse.pipedag.materialize import Table
 
 
 class BaseContext:
     _context_var: ClassVar[ContextVar]
-    _token: Token = None
-    _enter_counter: int = 0
     _lock: Lock = Lock()
+    _thread_state: dict[int, list[Token]] = {}
+    _instance_state: dict[int, int] = {}
 
     def __enter__(self):
         with self._lock:
-            object.__setattr__(self, "_enter_counter", self._enter_counter + 1)
-
-            if self._token is not None:
-                return self
-
+            _id = id(self) + (threading.get_ident() << 64)
+            if _id not in self._thread_state:
+                self._thread_state[_id] = []
+            _tokens = self._thread_state[_id]
             token = self._context_var.set(self)
-            object.__setattr__(self, "_token", token)
+            _tokens.append(token)
+            if id(self) not in self._instance_state:
+                self._instance_state[id(self)] = 0
+            # count threads that entered this context object
+            self._instance_state[id(self)] += 1
         return self
 
     def __exit__(self, *_):
         with self._lock:
-            object.__setattr__(self, "_enter_counter", self._enter_counter - 1)
-            if self._enter_counter == 0:
-                if not self._token:
-                    raise RuntimeError
-                self._context_var.reset(self._token)
-                object.__setattr__(self, "_token", None)
+            _id = id(self) + (threading.get_ident() << 64)
+            _tokens = self._thread_state[_id]
+            self._context_var.reset(_tokens.pop())
+            if len(_tokens) == 0:
+                del self._thread_state[_id]
+            self._instance_state[id(self)] -= 1
+            if self._instance_state[id(self)] == 0:
+                # in case of multi-threading, only close objects once
+                del self._instance_state[id(self)]
                 self._close()
 
     def _close(self):
         """Function that gets called at __exit__"""
 
     @classmethod
     def get(cls: type[T]) -> T:
@@ -61,16 +69,14 @@
 
         :raises LookupError: If no such context has been entered yet.
         """
         return cls._context_var.get()
 
     def __getstate__(self):
         state = self.__dict__.copy()
-        del state["_token"]
-        del state["_enter_counter"]
         return state
 
 
 @frozen(slots=False)
 class BaseAttrsContext(BaseContext):
     pass
 
@@ -188,14 +194,15 @@
         Values from the :ref:`config-attrs` config section, stored in a |Box|_ object.
         Useful for passing any custom, use case specific config options to your flow.
 
         .. |Box| replace:: ``Box``
         .. _Box: https://github.com/cdgriffith/Box/wiki
     """
 
+    # the actual configuration values
     _config_dict: dict
 
     # names
     pipedag_name: str
     flow_name: str | None
     instance_name: str
 
@@ -212,14 +219,15 @@
     attrs: Box
 
     table_hook_args: Box
 
     # INTERNAL FLAGS - ONLY FOR PIPEDAG USE
     # When set to True, exceptions raised in a flow don't get logged
     _swallow_exceptions: bool = False
+    _is_evolved: bool = False  # if True, _config_dict might be out of date
 
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
         return tuple(map(import_object, self._config_dict.get("auto_table", ())))
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
@@ -274,27 +282,29 @@
         .. _attrs.evolve(): https://www.attrs.org/en/stable/api.html#attrs.evolve
         """
         dicts = {}
         for name, value in changes.items():
             if isinstance(value, Mapping):
                 dicts[name] = deep_merge(getattr(self, name), value)
         changes.update(dicts)
+        changes.update(dict(is_evolved=True))
         evolved = evolve(self, **changes)
 
         # Transfer cached properties
         cached_properties = ["auto_table", "auto_blob", "store"]
         for name in cached_properties:
             if name in self.__dict__:
                 evolved.__dict__[name] = self.__dict__[name]
                 evolved.__dict__[f"__{name}_inherited"] = True
 
         return evolved
 
     def create_lock_manager(self) -> BaseLockManager:
-        return load_object(self._config_dict["lock_manager"])
+        with self:  # ensure that DatabaseLockManager uses correct engine
+            return load_object(self._config_dict["lock_manager"])
 
     def create_orchestration_engine(self) -> OrchestrationEngine:
         return load_object(self._config_dict["orchestration"])
 
     def _close(self):
         # If the store has been initialized (and thus cached in the __dict__),
         # dispose of it, and remove it from the cache.
@@ -308,14 +318,171 @@
         # store is not serializable, but @cached_property will reload
         # it from config_dict
         state.pop("store", None)
         state.pop("auto_table", None)
         state.pop("auto_blob", None)
         return state
 
+    @staticmethod
+    def new(config: dict[str, Any], pipedag_name: str, flow: str, instance: str):
+        """
+        Create a new ConfigContext instance from dictionary and a few names.
+
+        :param config:
+            dictionary with config values
+        :param pipedag_name:
+            name of pipedag config
+        :param flow:
+            name of flow
+        :param instance:
+            name of instance
+        :return:
+            ConfigContext instance
+        """
+
+        # check enums
+        # Alternative: could be a feature of __get_merged_config_dict
+        # in case default value is set to Enum
+        for parent_cfg, enum_name, enum_type in [
+            (config, "stage_commit_technique", StageCommitTechnique),
+            (config["cache_validation"], "mode", CacheValidationMode),
+        ]:
+            parent_cfg[enum_name] = parent_cfg[enum_name].strip().upper()
+            if not hasattr(enum_type, parent_cfg[enum_name]):
+                raise ValueError(
+                    f"Found unknown setting {enum_name}: '{parent_cfg[enum_name]}';"
+                    f" Expected one of: {', '.join([v.name for v in enum_type])}"
+                )
+        stage_commit_technique = getattr(
+            StageCommitTechnique, config["stage_commit_technique"]
+        )
+        cache_validation = copy.deepcopy(config["cache_validation"])
+        cache_validation["mode"] = getattr(
+            CacheValidationMode, config["cache_validation"]["mode"]
+        )
+        # parsing visualization dictionaries into objects (this could be generalized
+        # and possible an open source solution exists)
+        from pydiverse.pipedag import VisualizationStyle
+
+        if not isinstance(config.get("visualization", {}), dict):
+            raise ValueError(
+                "Config section 'visualization' must be a dictionary, "
+                f"found {type(config['visualization'])}"
+            )
+        visualization = {}
+        for key, value in config.get("visualization", {}).items():
+            ConfigContext.parse_in_object(
+                key, value, VisualizationConfig, "visualization", inout=visualization
+            )
+            for _field, structure, class_type in [
+                ("styles", visualization[key].styles, VisualizationStyle),
+                ("group_nodes", visualization[key].group_nodes, GroupNodeConfig),
+            ]:
+                if structure:
+                    for key2, value2 in structure.items():
+                        ConfigContext.parse_in_object(
+                            key2,
+                            value2,
+                            class_type,
+                            f"visualization.{key}.{_field}",
+                            inout=structure,
+                        )
+        if (
+            cache_validation["mode"] == CacheValidationMode.NORMAL
+            and cache_validation["disable_cache_function"]
+        ):
+            raise ValueError(
+                "cache_validation.disable_cache_function=True is not allowed in "
+                "combination with cache_validation.mode=NORMAL"
+            )
+        # Construct final ConfigContext
+        config_context = ConfigContext(
+            config_dict=config,
+            pipedag_name=pipedag_name,
+            flow_name=flow,
+            instance_name=instance,
+            fail_fast=config["fail_fast"],
+            strict_result_get_locking=config["strict_result_get_locking"],
+            instance_id=config["instance_id"],
+            stage_commit_technique=stage_commit_technique,
+            cache_validation=Box(cache_validation, frozen_box=True),
+            visualization=visualization,
+            network_interface=config["network_interface"],
+            disable_kroki=config.get("disable_kroki"),
+            kroki_url=config.get("kroki_url"),
+            attrs=Box(config["attrs"], frozen_box=True),
+            table_hook_args=Box(
+                config["table_store"].get("hook_args", {}), frozen_box=True
+            ),
+        )
+        return config_context
+
+    @staticmethod
+    def parse_in_object(
+        key: str,
+        value: dict[str, Any],
+        class_type: Any,
+        within: str,
+        *,
+        inout: dict[str, Any],
+    ):
+        """
+        Parse a dictionary into a dataclass instance.
+
+        :param key:
+            key of inout dictionary to be modified
+        :param value:
+            dictionary to be parsed into a dataclass instance and stored in inout[key]
+        :param class_type:
+            dataclass type for what should be written to inout[key]
+        :param within:
+            context for error messages
+        :param inout:
+            dictionary to be modified by this function call
+        :return:
+            None
+        """
+        structure = inout
+        if not isinstance(value, dict):
+            raise ValueError(
+                f"Config section '{key}' within '{within}' must be a dictionary, "
+                f"found {type(value)}"
+            )
+        members = set(class_type.__dataclass_fields__.keys())
+        if unexpected := set(value.keys()) - members:
+            raise ValueError(
+                f"Unexpected keys in section '{key}' within '{within}': "
+                f"{unexpected}; expected: '{', '.join(members)}'"
+            )
+        structure[key] = class_type(
+            **{m: copy.copy(value[m]) for m in members if m in value}
+        )
+        for m in value:
+            annotation = class_type.__annotations__[m]
+            if annotation.startswith("dict[") and not isinstance(value[m], dict):
+                raise ValueError(
+                    f"Expected dictionary for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("bool") and not isinstance(value[m], bool):
+                raise ValueError(
+                    f"Expected boolean for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("str") and not isinstance(value[m], str):
+                raise ValueError(
+                    f"Expected string for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+            if annotation.startswith("int") and not isinstance(value[m], int):
+                raise ValueError(
+                    f"Expected integer for '{m}' within '{within}.{key}', "
+                    f"found {type(value[m])}"
+                )
+
     _context_var = ContextVar("config_context")
 
 
 class StageLockContext(BaseContext):
     """
     Context manager used to keep stages locked until after :py:meth:`Flow.run()`.
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/context/run_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,41 +114,51 @@
         self.stage_state_lock = Lock()
         self.names_lock = Lock()
         self.task_memo_lock = Lock()
         self.deferred_ops_lock = RLock()
         self.local_table_cache_lock = Lock()
 
         # LOCKING
-        self.lock_manager = config_ctx.create_lock_manager()
-        self.lock_handler = StageLockStateHandler(self.lock_manager)
-
         try:
             # If we are inside a StageLockContext, then we shouldn't release any
             # stage locks, instead they get released when StageLockContext.__exit__
             # gets called.
             stage_lock_context = StageLockContext.get()
-            stage_lock_context.lock_state_handlers.append(self.lock_handler)
+            if stage_lock_context.lock_state_handlers:
+                # reuse existing lock manager and handler
+                self.lock_handler = stage_lock_context.lock_state_handlers[0]
+                self.lock_manager = self.lock_handler.lock_manager
+            else:
+                self.lock_manager = config_ctx.create_lock_manager()
+                self.lock_handler = StageLockStateHandler(self.lock_manager)
+                stage_lock_context.lock_state_handlers.append(self.lock_handler)
             self.keep_stages_locked = True
         except LookupError:
             self.keep_stages_locked = False
+            self.lock_manager = config_ctx.create_lock_manager()
+            self.lock_handler = StageLockStateHandler(self.lock_manager)
 
     def __enter__(self):
         super().__enter__()
+        from pydiverse.pipedag.backend import LockState
 
         # INITIALIZE EVERYTHING
         with self.lock_manager("_pipedag_setup_"):
             self.config_ctx.store.table_store.setup()
 
             # Acquire a lock on all stages
             # We must lock all stages from the start to prevent two flows from
             # deadlocking each other (lock order inversion). To lock the stage
             # only when it's needed (may result in deadlocks), the lock should
             # get acquired in the `PipeDAGStore.init_stage` function instead.
             for stage in self.stages:
-                self.lock_manager.acquire(stage)
+                # only lock stage if it is not already locked within current
+                # StageLockContext
+                if self.lock_manager.get_lock_state(stage.name) != LockState.LOCKED:
+                    self.lock_manager.acquire(stage.name)
 
         # INITIALIZE REFERENCE COUNTERS
         for stage in self.stages:
             for task in stage.all_tasks():
                 for s in task.upstream_stages:
                     self.ref_count[s.id] += 1
 
@@ -306,20 +316,20 @@
             else:
                 raise RuntimeError
 
     # LOCKING
 
     def acquire_stage_lock(self, stage_id: int):
         stage = self.stages[stage_id]
-        self.lock_manager.acquire(stage)
+        self.lock_manager.acquire(stage.name)
 
     def release_stage_lock(self, stage_id: int):
         if not self.keep_stages_locked:
             stage = self.stages[stage_id]
-            self.lock_manager.release(stage)
+            self.lock_manager.release(stage.name)
 
     def validate_stage_lock(self, stage_id: int):
         stage = self.stages[stage_id]
         self.lock_handler.validate_stage_lock(stage)
 
     # DEFERRED TABLE STORE OPERATIONS
     # Allows deferring operations that should be run on the table store object
@@ -406,15 +416,15 @@
                         "Reference counter is negative.",
                         reference_count=rc,
                         stage=stage,
                     )
 
         if not self.keep_stages_locked:
             for stage in stages_to_release:
-                self.lock_manager.release(stage)
+                self.lock_manager.release(stage.name)
 
     def get_task_states(self) -> list[int]:
         return [state.value for state in self.task_state]
 
     def enter_task_memo(self, task_id: int, cache_key: str) -> tuple[bool, Any]:
         task = self.tasks[task_id]
         memo_key = (task.stage.id, cache_key)
@@ -733,15 +743,15 @@
             self.logger.error(f"Lock for stage '{stage.name}' has become INVALID.")
 
     def validate_stage_lock(self, stage):
         from pydiverse.pipedag.backend.lock import LockState
 
         did_log = False
         while True:
-            state = self.lock_manager.get_lock_state(stage)
+            state = self.lock_manager.get_lock_state(stage.name)
 
             if state == LockState.LOCKED:
                 return
             elif state == LockState.UNLOCKED:
                 raise LockError(f"Lock for stage '{stage.name}' is unlocked.")
             elif state == LockState.INVALID:
                 raise LockError(f"Lock for stage '{stage.name}' is invalid.")
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,15 @@
 from collections.abc import Iterable
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy as sa
 import structlog
 import yaml
-from box import Box
 
-from pydiverse.pipedag.context.context import (
-    CacheValidationMode,
-    GroupNodeConfig,
-    VisualizationConfig,
-)
 from pydiverse.pipedag.util.deep_merge import deep_merge
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.context import ConfigContext
 
 
 # noinspection PyPep8Naming
@@ -159,74 +153,14 @@
                 "stage_commit_technique": "SCHEMA_SWAP",
                 "auto_table": [],
                 "auto_blob": [],
                 "attrs": {},
             },
         ).copy()
 
-        # check enums
-        # Alternative: could be a feature of __get_merged_config_dict
-        # in case default value is set to Enum
-        from pydiverse.pipedag.context.context import StageCommitTechnique
-
-        for parent_cfg, enum_name, enum_type in [
-            (config, "stage_commit_technique", StageCommitTechnique),
-            (config["cache_validation"], "mode", CacheValidationMode),
-        ]:
-            parent_cfg[enum_name] = parent_cfg[enum_name].strip().upper()
-            if not hasattr(enum_type, parent_cfg[enum_name]):
-                raise ValueError(
-                    f"Found unknown setting {enum_name}: '{parent_cfg[enum_name]}';"
-                    f" Expected one of: {', '.join([v.name for v in enum_type])}"
-                )
-        stage_commit_technique = getattr(
-            StageCommitTechnique, config["stage_commit_technique"]
-        )
-        cache_validation = copy.deepcopy(config["cache_validation"])
-        cache_validation["mode"] = getattr(
-            CacheValidationMode, config["cache_validation"]["mode"]
-        )
-
-        # parsing visualization dictionaries into objects (this could be generalized
-        # and possible an open source solution exists)
-        from pydiverse.pipedag import VisualizationStyle
-
-        if not isinstance(config.get("visualization", {}), dict):
-            raise ValueError(
-                "Config section 'visualization' must be a dictionary, "
-                f"found {type(config['visualization'])}"
-            )
-        visualization = {}
-        for key, value in config.get("visualization", {}).items():
-            self.parse_in_object(
-                key, value, VisualizationConfig, "visualization", inout=visualization
-            )
-            for field, structure, class_type in [
-                ("styles", visualization[key].styles, VisualizationStyle),
-                ("group_nodes", visualization[key].group_nodes, GroupNodeConfig),
-            ]:
-                if structure:
-                    for key2, value2 in structure.items():
-                        self.parse_in_object(
-                            key2,
-                            value2,
-                            class_type,
-                            f"visualization.{key}.{field}",
-                            inout=structure,
-                        )
-
-        if (
-            cache_validation["mode"] == CacheValidationMode.NORMAL
-            and cache_validation["disable_cache_function"]
-        ):
-            raise ValueError(
-                "cache_validation.disable_cache_function=True is not allowed in "
-                "combination with cache_validation.mode=NORMAL"
-            )
-
         # TODO: Delegate selecting where variables can be expanded to the
         #  corresponding classes.
         #    eg. SQLTableStore._expand_env_vars = ["url", "url_attrs_file"]
         #    eg. SQLTableStore._expand_vars = ["url", "schema_prefix", "schema_suffix"]
 
         # First expand all environment variables
         self.__expand_environment_variables(inout_config=config)
@@ -253,34 +187,15 @@
             url = _get(config, "table_store", "args", "url")
             url = expand_variables(url, url_attrs, skip_missing=True)
             _set(config, url, "table_store", "args", "url")
 
         # Finally, expand all normal variables
         config = self.__expand_variables(config)
 
-        # Construct final ConfigContext
-        config_context = ConfigContext(
-            config_dict=config,
-            pipedag_name=self.name,
-            flow_name=flow,
-            instance_name=instance,
-            fail_fast=config["fail_fast"],
-            strict_result_get_locking=config["strict_result_get_locking"],
-            instance_id=config["instance_id"],
-            stage_commit_technique=stage_commit_technique,
-            cache_validation=Box(cache_validation, frozen_box=True),
-            visualization=visualization,
-            network_interface=config["network_interface"],
-            disable_kroki=config.get("disable_kroki"),
-            kroki_url=config.get("kroki_url"),
-            attrs=Box(config["attrs"], frozen_box=True),
-            table_hook_args=Box(
-                config["table_store"].get("hook_args", {}), frozen_box=True
-            ),
-        )
+        config_context = ConfigContext.new(config, self.name, flow, instance)
 
         if "PYDIVERSE_PIPEDAG_PYTEST" not in os.environ:
             # If we're running test cases, this can be skipped to improve performance
             try:
                 # Make sure @cached_property store is set up and loaded
                 # and throw config errors early.
                 with config_context:
@@ -294,61 +209,14 @@
                 raise RuntimeError(
                     "Error while creating backend objects from pipedag config "
                     f"(instance={instance}, flow={flow}): {self.path}"
                 ) from e
 
         return config_context
 
-    @staticmethod
-    def parse_in_object(
-        key: str,
-        value: dict[str, Any],
-        class_type: Any,
-        within: str,
-        *,
-        inout: dict[str, Any],
-    ):
-        structure = inout
-        if not isinstance(value, dict):
-            raise ValueError(
-                f"Config section '{key}' within '{within}' must be a dictionary, "
-                f"found {type(value)}"
-            )
-        members = set(class_type.__dataclass_fields__.keys())
-        if unexpected := set(value.keys()) - members:
-            raise ValueError(
-                f"Unexpected keys in section '{key}' within '{within}': "
-                f"{unexpected}; expected: '{', '.join(members)}'"
-            )
-        structure[key] = class_type(
-            **{m: copy.copy(value[m]) for m in members if m in value}
-        )
-        for m in value:
-            annotation = class_type.__annotations__[m]
-            if annotation.startswith("dict[") and not isinstance(value[m], dict):
-                raise ValueError(
-                    f"Expected dictionary for '{m}' within '{within}.{key}', "
-                    f"found {type(value[m])}"
-                )
-            if annotation.startswith("bool") and not isinstance(value[m], bool):
-                raise ValueError(
-                    f"Expected boolean for '{m}' within '{within}.{key}', "
-                    f"found {type(value[m])}"
-                )
-            if annotation.startswith("str") and not isinstance(value[m], str):
-                raise ValueError(
-                    f"Expected string for '{m}' within '{within}.{key}', "
-                    f"found {type(value[m])}"
-                )
-            if annotation.startswith("int") and not isinstance(value[m], int):
-                raise ValueError(
-                    f"Expected integer for '{m}' within '{within}.{key}', "
-                    f"found {type(value[m])}"
-                )
-
     def __get_merged_config_dict(self, instance, flow, default=None):
         search_paths = [
             ("instances", "__any__"),
             ("instances", instance),
             ("flows", "__any__"),
             ("flows", "__any__", "instances", instance),
             ("flows", flow),
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/group_node.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/group_node.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     """
 
     def __init__(
         self,
         name: str,
         materialization_details: str | None = None,
         group_node_tag: str | None = None,
+        force_committed=False,
     ):
         self._name = normalize_name(name)
         self._transaction_name = f"{self._name}__tmp"
 
         self.tasks: list[Task] = []
         self.commit_task: CommitStageTask = None  # type: ignore
         self.barrier_tasks: list[Task] = []
@@ -57,16 +58,37 @@
 
         self.logger = structlog.get_logger(logger_name=type(self).__name__, stage=self)
         self.id: int = None  # type: ignore
 
         self.materialization_details = materialization_details
         self.group_node_tag = group_node_tag
 
+        self.force_committed = force_committed
         self._did_enter = False
 
+    def __lt__(self, other: Stage):
+        # Essentially stage name is all that matters and should be unique per flow.
+        # In case of comparing stages among different flows or pipeline instances,
+        # the caller needs to check whether those are different. The stage links to
+        # tasks which are somewhat bound to a flow, but it is unclear what behavior the
+        # caller wants from the comparison operators.
+        return self.name < other.name
+
+    def __eq__(self, other: Stage):
+        # Essentially stage name is all that matters and should be unique per flow.
+        # See __lt__ for more details.
+        if not isinstance(other, Stage):
+            return False
+        return self.name == other.name
+
+    def __hash__(self):
+        # Essentially stage name is all that matters and should be unique per flow.
+        # See __lt__ for more details.
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         """The name of the stage."""
         return self._name
 
     @property
     def transaction_name(self) -> str:
@@ -89,14 +111,17 @@
         if self.did_commit:
             return self.name
         else:
             return self.transaction_name
 
     @property
     def did_commit(self) -> bool:
+        if self.force_committed:
+            return True
+
         from pydiverse.pipedag.context.run_context import RunContext, StageState
 
         return RunContext.get().get_stage_state(self) == StageState.COMMITTED
 
     def __repr__(self):
         return f"<Stage: {self.name}>"
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/core/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,29 @@
     def __init__(
         self,
         fn: Callable,
         *,
         name: str | None = None,
         nout: int | None = None,
         group_node_tag: str | None = None,
+        call_context: Callable[[], Any] | None = None,
     ):
         if not callable(fn):
             raise TypeError("`fn` must be callable")
         if nout is not None and (nout <= 0 or not isinstance(nout, int)):
             raise ValueError("`nout` must be a positive integer")
 
         if name is None:
             name = getattr(fn, "__name__", type(self).__name__)
 
         self.fn = fn
         self.name = name
         self.nout = nout
         self.group_node_tag = group_node_tag
+        self.call_context = call_context
 
         self._bound_task_type = Task
         self._signature = inspect.signature(fn)
 
     def __repr__(self):
         return f"<UnboundTask 'name' {hex(id(self))}>"
 
@@ -93,14 +95,15 @@
         flow: Flow,
         stage: Stage,
     ):
         self.fn = unbound_task.fn
         self.name = unbound_task.name
         self.nout = unbound_task.nout
         self.group_node_tag = unbound_task.group_node_tag
+        self.call_context = unbound_task.call_context
 
         self.logger = structlog.get_logger(logger_name=f"Task '{self.name}'", task=self)
 
         self._bound_args = bound_args
         self.flow = flow
         self.stage = stage
         self.group_node = None  # will be set by UnboundTask.__call__
@@ -203,15 +206,19 @@
                 return x.resolve_value(inputs[x.task.id])
             return x
 
         args = deep_map(args, task_result_mapper)
         kwargs = deep_map(kwargs, task_result_mapper)
 
         with TaskContext(task=self) as task_context:
-            result = self.fn(*args, **kwargs)
+            if hasattr(self, "call_context") and self.call_context:
+                with self.call_context():
+                    result = self.fn(*args, **kwargs)
+            else:
+                result = self.fn(*args, **kwargs)
 
         return result, task_context
 
     def __compute_position_hash(self) -> str:
         """
         The position hash encodes the position & wiring of a task within a flow.
         If two tasks have the same position hash, this means that their inputs are
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,21 @@
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
         self._name = normalize_name(value)
 
+    def copy_without_obj(self) -> Blob:
+        obj = self.obj
+        self.obj = None
+        self_copy = copy.deepcopy(self)
+        self.obj = obj
+        return self_copy
+
 
 class ExternalTableReference:
     """Reference to a user-created table.
 
     By returning a `ExternalTableReference` wrapped in a :py:class:`~.Table` from,
     a task you can tell pipedag about a table, a view or DB2 nickname in an external
     `schema`. The schema may be a multi-part identifier like "[db_name].[schema_name]"
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 from __future__ import annotations
 
 import copy
 import functools
 import inspect
 import uuid
 from collections.abc import Callable, Iterable
+from contextlib import contextmanager
 from functools import partial
 from typing import TYPE_CHECKING, Any, overload
 
 import sqlalchemy as sa
 
 from pydiverse.pipedag._typing import CallableT
 from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
-from pydiverse.pipedag.context.context import CacheValidationMode
+from pydiverse.pipedag.context.context import (
+    CacheValidationMode,
+)
 from pydiverse.pipedag.core.task import Task, TaskGetItem, UnboundTask
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.cache import TaskCacheInfo, task_cache_key
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
 from pydiverse.pipedag.util import deep_map
 from pydiverse.pipedag.util.computation_tracing import (
     ComputationTraceRef,
     ComputationTracerProxy,
 )
 from pydiverse.pipedag.util.hashing import stable_hash
+from pydiverse.pipedag.util.json import PipedagJSONEncoder
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Flow, Stage
     from pydiverse.pipedag.backend.table.base import TableHook
     from pydiverse.pipedag.materialize.store import PipeDAGStore
 
 
 @overload
 def materialize(
     *,
     name: str | None = None,
-    input_type: type | tuple | dict[str, Any] | None = None,
+    input_type: type | None = None,
     version: str | None = None,
-    cache: Callable[[Any], Any] | None = None,
+    cache: Callable[..., Any] | None = None,
     lazy: bool = False,
     nout: int = 1,
+    add_input_source: bool = False,
+    ordering_barrier: bool | dict[str, Any] = False,
+    call_context: Callable[[], Any] | None = None,
 ) -> Callable[[CallableT], CallableT | UnboundMaterializingTask]:
     ...
 
 
 @overload
 def materialize(fn: CallableT, /) -> CallableT | UnboundMaterializingTask:
     ...
 
 
 def materialize(
     fn: CallableT | None = None,
     *,
     name: str | None = None,
-    input_type: type | tuple | dict[str, Any] | None = None,
+    input_type: type | None = None,
     version: str | None = None,
-    cache: Callable[[Any], Any] | None = None,
+    cache: Callable[..., Any] | None = None,
     lazy: bool = False,
     group_node_tag: str | None = None,
     nout: int = 1,
+    add_input_source: bool = False,
+    ordering_barrier: bool | dict[str, Any] = False,
+    call_context: Callable[[], Any] | None = None,
 ):
     """Decorator to create a task whose outputs get materialized.
 
     This decorator takes a class and turns it into a :py:class:`MaterializingTask`.
     This means, that this function can only be used as part of a flow.
     Any outputs it produces get written to their appropriate storage backends
     (either the table or blob store). Additionally, any :py:class:`Table`
@@ -118,15 +128,26 @@
         the `version` of a lazy task. This only works because for lazy tables
         generating the query is very cheap compared to executing it.
     :param group_node_tag:
         Set a tag that may add this task to a configuration based group node.
     :param nout:
         The number of objects returned by the task.
         If set, this allows unpacking and iterating over the results from the task.
-
+    :param add_input_source:
+        If true, Table and Blob objects are provided as tuple together with the
+        dematerialized object. ``task(a=tbl)`` will result in
+        ``a=(dematerialized_tbl, tbl)`` in the task.
+    :param ordering_barrier:
+        If true, the task will be surrounded by a GroupNode(ordering_barrier=True).
+        If a dictionary is provided, it is surrounded by a
+        GroupNode(**ordering_barrier). This allows passing style, style_tag, and label
+        arguments.
+    :param call_context:
+        An optional context manager function that is opened before the task or its
+        optional cache function is called and closed afterward.
     Example
     -------
 
     ::
 
         @materialize(version="1.0", input_type=pd.DataFrame)
         def task(df: pd.DataFrame) -> pd.DataFrame:
@@ -189,25 +210,31 @@
             name=name,
             input_type=input_type,
             version=version,
             cache=cache,
             lazy=lazy,
             group_node_tag=group_node_tag,
             nout=nout,
+            add_input_source=add_input_source,
+            ordering_barrier=ordering_barrier,
+            call_context=call_context,
         )
 
     return UnboundMaterializingTask(
         fn,
         name=name,
         input_type=input_type,
         version=version,
         cache=cache,
         lazy=lazy,
         group_node_tag=group_node_tag,
         nout=nout,
+        add_input_source=add_input_source,
+        ordering_barrier=ordering_barrier,
+        call_context=call_context,
     )
 
 
 class UnboundMaterializingTask(UnboundTask):
     """A materializing task without any bound arguments.
 
     Instances of this class get initialized using the
@@ -256,18 +283,21 @@
     def __init__(
         self,
         fn: Callable,
         *,
         name: str | None = None,
         input_type: type | None = None,
         version: str | None = None,
-        cache: Callable[[Any], Any] | None = None,
+        cache: Callable[..., Any] | None = None,
         lazy: bool = False,
         group_node_tag: str | None = None,
         nout: int = 1,
+        add_input_source: bool = False,
+        ordering_barrier: bool | dict[str, Any] = False,
+        call_context: Callable[[], Any] | None = None,
     ):
         super().__init__(
             MaterializationWrapper(fn),
             name=name,
             nout=nout,
         )
 
@@ -275,31 +305,60 @@
         self._original_fn = fn
 
         self.input_type = input_type
         self.version = version
         self.cache = cache
         self.lazy = lazy
         self.group_node_tag = group_node_tag
+        self.add_input_source = add_input_source
+        self.call_context = call_context
+
+        if isinstance(ordering_barrier, bool):
+            group_node_args = {"ordering_barrier": ordering_barrier}
+        elif isinstance(ordering_barrier, dict):
+            group_node_args = ordering_barrier.copy()
+            if "ordering_barrier" not in group_node_args:
+                group_node_args["ordering_barrier"] = True
+
+            group_node_keys = {"ordering_barrier", "label", "style", "style_tag"}
+            unexpected_keys = set(ordering_barrier.keys()) - group_node_keys
+            if unexpected_keys:
+                raise ValueError(
+                    "If ordering_barrier is a dictionary, it must only contain keys "
+                    "that are valid parameters of class GroupNode constructor."
+                    f"{unexpected_keys} are unexpected."
+                )
+        else:
+            raise ValueError(
+                "The ordering_barrier parameter must be a boolean or a dictionary."
+            )
+        self.group_node_args = group_node_args
 
         if version is AUTO_VERSION:
             if input_type is None:
                 # The input_type is used to determine which type of auto versioning
                 # to use (either not supported, lazy or tracing)
                 raise ValueError("Auto-versioning task must specify an input type")
             if lazy:
                 raise ValueError(
                     "Task can't be lazy and auto-versioning at the same time"
                 )
 
     def __call__(self, *args, **kwargs) -> MaterializingTask:
+        if self.group_node_args["ordering_barrier"]:
+            from pydiverse.pipedag import GroupNode
+
+            with GroupNode(**self.group_node_args):
+                return super().__call__(*args, **kwargs)  # type: ignore
         return super().__call__(*args, **kwargs)  # type: ignore
 
     def _call_original_function(self, *args, **kwargs):
         try:
             task_context = TaskContext.get()  # this may raise Lookup Error
+
             # this is a subtask call. Thus we demand identical input_types
             sub_task: MaterializingTask = task_context.task  # type: ignore
             if (
                 sub_task.input_type is not None
                 and self.input_type is not None
                 and sub_task.input_type != self.input_type
             ):
@@ -342,14 +401,15 @@
         bound_args: inspect.BoundArguments,
         flow: Flow,
         stage: Stage,
     ):
         super().__init__(unbound_task, bound_args, flow, stage)
 
         self.input_type = unbound_task.input_type
+        self.add_input_source = unbound_task.add_input_source
         self._version = unbound_task.version
         self.cache = unbound_task.cache
         self.lazy = unbound_task.lazy
 
     @property
     def version(self):
         try:
@@ -926,14 +986,526 @@
 
         if len(blobs) != 0:
             raise ValueError(f"Task with version={AUTO_VERSION} can't return Blobs.")
 
         return output, tables
 
 
+@overload
+def input_stage_versions(
+    *,
+    name: str | None = None,
+    input_type: type | None = None,
+    version: str | None = None,
+    cache: Callable[..., Any] | None = None,
+    lazy: bool = False,
+    group_node_tag: str | None = None,
+    nout: int = 1,
+    add_input_source: bool = False,
+    ordering_barrier: bool | dict[str, Any] = True,
+    call_context: Callable[[], Any] | None = None,
+    include_views=True,
+    lock_source_stages=True,
+    pass_args: Iterable[str] = tuple(),
+) -> Callable[[CallableT], CallableT | UnboundMaterializingTask]:
+    ...
+
+
+@overload
+def input_stage_versions(fn: CallableT, /) -> CallableT | UnboundMaterializingTask:
+    ...
+
+
+def input_stage_versions(
+    fn: CallableT | None = None,
+    *,
+    name: str | None = None,
+    input_type: type | None = None,
+    version: str | None = None,
+    cache: Callable[..., Any] | None = None,
+    lazy: bool = False,
+    group_node_tag: str | None = None,
+    nout: int = 1,
+    add_input_source: bool = False,
+    ordering_barrier: bool | dict[str, Any] = True,
+    call_context: Callable[[], Any] | None = None,
+    include_views=True,
+    lock_source_stages=True,
+    pass_args: Iterable[str] = tuple(),
+):
+    """
+    A decorator that marks a function as a task that receives tables from two versions
+    of the same stage. This can either be the currently active schema of this stage
+    before schema swapping, or it can be an active schema of another pipeline instance.
+
+    The arguments to the resulting task are significantly different from a task created
+    with `@materialize` decorator. An arbitrary expression with lists, tuples, dicts,
+    and Table/Blob/RawSQL references can be provided. This decorator will only collect
+    tables referenced and will pass them as one dictionary per version to the task. It
+    maps table names to some reference for the respective stage version in the form
+    specified by input_type parameter.
+
+    When a ConfigContext object is passed as toplevel parameter or named parameter in
+    the wiring call of decorated task, it is used for referencing the second stage
+    version. The idea is that the other configuration is just another pipeline instance
+    accessible with the same SQLAlchemy engine of the table store. It may work also if
+    this is not the case, but it may be harder for the task to process the dictionaries
+    it receives. Currently, it is not allowed to pass more than one ConfigContext
+    object.
+
+    When no parameters (except for an optional ConfigContext) is passed, all currently
+    existing tables of both stage versions (or their respective schema) are passed in
+    the dictionaries to the task.
+
+    With pass_blobs=True, two additional dictionaries are passed to the task at the end.
+    In addition to the arguments mentioned above, pass_args can be used to feed defined
+    keyword arguments through to the decorated task.
+
+    :param fn:
+        The function that gets executed by this task.
+    :param name:
+        The name of this task.
+        If no `name` is provided, the name of `fn` is used instead.
+    :param input_type:
+        The data type as which to retrieve table objects from the store.
+        All tables passed to this task get loaded from the table store and converted
+        to this type. See :doc:`Table Backends </table_backends>` for
+        more information.
+    :param version:
+        The version of this task.
+        Unless the task is lazy, you always need to manually change this
+        version number when you change the implementation to ensure that the
+        task gets executed and the cache flushed.
+
+        If the `version` is ``None`` and the task isn't lazy, then the task always
+        gets executed, and all downstream tasks get invalidated.
+    :param cache:
+        An explicit cache function used to determine cache validity of the task inputs.
+
+        This function gets called every time before the task gets executed.
+        It gets called with the same arguments as the task.
+
+        An explicit function for validating cache validity. If the output
+        of this function changes while the source parameters are the same (e.g.
+        the source is a filepath and `cache` loads data from this file), then the
+        cache will be deemed invalid and is not used.
+    :param lazy:
+        Whether this task is lazy or not.
+
+        Unlike a normal task, lazy tasks always get executed. However, if a lazy
+        task produces a lazy table (e.g. a SQL query), the table store checks if
+        the same query has been executed before. If this is the case, then the
+        query doesn't get executed, and instead, the table gets copied from the cache.
+
+        This behaviour is very useful, because you don't need to manually bump
+        the `version` of a lazy task. This only works because for lazy tables
+        generating the query is very cheap compared to executing it.
+    :param group_node_tag:
+        Set a tag that may add this task to a configuration based group node.
+    :param nout:
+        The number of objects returned by the task.
+        If set, this allows unpacking and iterating over the results from the task.
+    :param add_input_source:
+        If true, Table and Blob objects are provided as tuple together with the
+        dematerialized object. ``task(a=tbl)`` will result in
+        ``a=(dematerialized_tbl, tbl)`` in the task.
+    :param ordering_barrier:
+        If true, the task will be surrounded by a GroupNode(ordering_barrier=True).
+        If a dictionary is provided, it is surrounded by a
+        GroupNode(**ordering_barrier). This allows passing style, style_tag, and label
+        arguments.
+        Attention: In contrast to @materialize, the default value is True.
+    :param call_context:
+        An optional context manager function that is opened before the task or its
+        optional cache function is called and closed afterward.
+    :param include_views:
+        In case no explicit table references are given, if true, include views when
+        collecting all tables of both stage versions.
+    :param lock_source_stages:
+        If true, lock the other stage version when a ConfigContext object is passed to
+        this task.
+    :param pass_args
+        A list of named arguments that whould be passed from the call to the task
+        function. By default, no arguments are passed, and just tables are extracted.
+    Example
+    -------
+
+    ::
+
+        @input_stage_versions(lazy=True, input_type=sa.Table)
+        def validate_stage(
+            transaction: dict[str, sa.Alias],
+            other: dict[str, sa.Alias],
+        ):
+            compare_tables(transaction, other)
+
+        def get_flow():
+            with Flow() as f:
+                a = produce_a_table()
+                validate_stage()  # implicitly receives all tables written before
+    """
+    from pydiverse.pipedag import Stage
+
+    forward_args = dict(
+        name=name,
+        input_type=input_type,
+        version=version,
+        cache=cache,
+        lazy=lazy,
+        group_node_tag=group_node_tag,
+        nout=nout,
+        add_input_source=add_input_source,
+        ordering_barrier=ordering_barrier,
+        call_context=call_context,
+        include_views=include_views,
+        lock_source_stages=lock_source_stages,
+        pass_args=pass_args,
+    )
+
+    if fn is None:
+        return partial(input_stage_versions, **forward_args)
+
+    class OtherStageLockManager:
+        def __init__(self):
+            self.stages = None
+            self.lock_manager = None
+
+        @contextmanager
+        def __call__(self):
+            yield
+            self.release_all()
+
+        def release_all(self):
+            # clear locks after either cache_fn or cache_fn and task function were
+            # called
+            if self.lock_manager is not None:
+                for stage in sorted(self.stages, reverse=True):
+                    self.lock_manager.release(stage.name)
+                self.lock_manager.dispose()
+                self.lock_manager = None
+
+        def memorize(self, stages, lock_manager):
+            self.release_all()
+            self.stages = stages
+            self.lock_manager = lock_manager
+
+    other_stage_lock_manager = OtherStageLockManager()
+
+    def cache_fn(*args, **kwargs):
+        user_cache_fn = cache
+        if user_cache_fn is None:
+            # we don't care about the cache function, but we still need to cache the
+            # arguments that are also used to call the task itself
+            def user_cache_fn(*args, **kwargs):
+                return None
+
+        ret, cfg2, stages, lock_manager = _call_fn(
+            user_cache_fn,
+            args,
+            kwargs,
+            input_type=None,
+            is_dematerialized=False,
+            lock_source_stages=lock_source_stages,
+        )
+        other_stage_lock_manager.memorize(stages, lock_manager)
+        if cfg2 is None:
+            return uuid.uuid4().hex  # return random hash to ensure invalidation
+        # get a hash of all task outputs of all relevant stage from other pipeline
+        # instance
+        ret = stable_hash(ret)
+        for stage in stages:
+            try:
+                ret = ret + cfg2.store.table_store.get_stage_hash(stage)
+            except sa.exc.ProgrammingError:
+                # this happens for example if the other instance did not run, yet
+                return uuid.uuid4().hex  # return random hash to ensure invalidation
+        return ret
+
+    # extract @materialize arguments from forward_args via __code__.co_varnames:
+    n_args = materialize.__code__.co_argcount + materialize.__code__.co_kwonlyargcount
+    arg_names = materialize.__code__.co_varnames[0:n_args]
+    materialize_args = {k: v for k, v in forward_args.items() if k in arg_names}
+    materialize_args["add_input_source"] = True  # we need the names
+    materialize_args["cache"] = cache_fn
+    if materialize_args.get("name") is None:
+        materialize_args["name"] = getattr(fn, "__name__", "input_stage_versions-task")
+    materialize_args["call_context"] = other_stage_lock_manager
+
+    # For every input_state_versions-Task, we create a materialize-Task and give it the
+    # same name as the input_state_versions-Task should get. The @materialize decorator
+    # will dematerialize any Table/Blob/RawSQL objects passed to the
+    # input_state_versions-Task. We pass add_input_source=True, so we still receive the
+    # Table/Blob/RawSQL reference objects, so we can use them to dematerialize the
+    # second stage version. Both are arranged in dictionaries indexable by table name or
+    # blob name and handed over to the function annotated with @input_stage_versions.
+    @materialize(**materialize_args)
+    def task(*args, **kwargs):
+        # the locks are already acquired by cache_fn if it is called
+        lock_stages = (
+            False
+            if other_stage_lock_manager.lock_manager is not None
+            else lock_source_stages
+        )
+        ret, _, _, _ = _call_fn(
+            fn,
+            args,
+            kwargs,
+            input_type=input_type,
+            is_dematerialized=True,
+            lock_source_stages=lock_stages,
+        )
+        return ret
+
+    def _call_fn(
+        _fn: Callable[..., Any],
+        args: tuple,
+        kwargs: dict[str, Any],
+        *,
+        input_type,
+        is_dematerialized,
+        lock_source_stages,
+    ):
+        _task = TaskContext.get().task
+        stage = _task.stage
+        pass_kwargs = {k: v for k, v in kwargs.items() if k in set(pass_args)}
+
+        (
+            stages,
+            table_dict,
+            blob_dict,
+            raw_sqls,
+            other_cfg,
+            any_data_arguments_collected,
+        ) = _collect_arguments(args, kwargs, is_dematerialized)
+        stages.add(stage)
+
+        # The connection to the other stage version configuration can either be the same
+        # (in this case, we provide the active stage cache before swapping) or another
+        # pipeline instance (in this case, we also take the active stage cache schema
+        # of the same stage in the other instance)
+        cfg1 = ConfigContext.get()
+        cfg2 = other_cfg
+        if cfg2 is None:
+            cfg2 = cfg1
+        stage2 = Stage(
+            stage.name,
+            stage.materialization_details,
+            stage.group_node_tag,
+            force_committed=True,
+        )
+        stage2.id = stage.id
+        if lock_source_stages and other_cfg is not None:
+            lock_manager = cfg2.create_lock_manager()
+        else:
+            lock_manager = None
+            lock_source_stages = False
+
+        transaction_table_dict, other_table_dict = {}, {}
+        transaction_blob_dict, other_blob_dict = {}, {}
+        try:
+            # lock the source stages if they are read from another instance
+            if lock_source_stages:
+                for stage in sorted(stages):
+                    lock_manager.acquire(stage.name)
+            # cnt[0] counts the number of arguments in args and kwargs. pass_args within
+            # kwargs are neglected.
+            # cnt[0] is at least 2 due to deep_map calls on args and kwargs. If a
+            # ConfigContext object is passed as argument, cfg_cnt=1 and cnt=3.
+            if not any_data_arguments_collected:
+                # dematerialize all tables and optionally views of both stage versions
+
+                def _dematerialize_all(cfg, stage):
+                    table_dict = {}
+                    if include_views:
+                        # also include table aliases
+                        tbls1 = cfg.store.table_store.get_objects_in_stage(stage)
+                    else:
+                        # won't detect aliases
+                        tbls1 = cfg.store.table_store.get_table_objects_in_stage(
+                            stage, include_views=include_views
+                        )
+                    for name in tbls1:
+                        tbl = Table(name=name)
+                        tbl.stage = stage
+                        if include_views:
+                            (
+                                tbl.name,
+                                tbl.external_schema,
+                            ) = cfg.store.table_store.resolve_alias(
+                                tbl, stage.current_name
+                            )
+                            if not cfg.store.table_store.has_table_or_view(
+                                tbl.name, tbl.external_schema
+                            ):
+                                continue  # skip because it is neither view nor alias
+                        table_dict[tbl.name] = cfg.store.dematerialize_item(
+                            tbl, input_type
+                        )
+                    return table_dict
+
+                transaction_table_dict = _dematerialize_all(cfg1, stage)
+                other_table_dict = _dematerialize_all(cfg2, stage2)
+            else:
+
+                def _dematerialize_versions(
+                    ref: Table | Blob,
+                    obj,
+                    transaction_dict: dict[str, Any],
+                    other_dict: dict[str, Any],
+                    cfg2: ConfigContext,
+                    stage: Stage,
+                ):
+                    key = (
+                        ref.name
+                        if ref.stage == stage
+                        else f"{ref.stage.name}.{ref.name}"
+                    )
+                    transaction_dict[key] = obj
+                    # load committed version of stage (either same pipeline instace or
+                    # other)
+                    tbl2 = ref.copy_without_obj()
+                    tbl2.stage = Stage(
+                        ref.stage.name,
+                        ref.stage.materialization_details,
+                        ref.stage.group_node_tag,
+                        force_committed=True,
+                    )
+                    tbl2.stage.id = ref.stage.id
+                    try:
+                        store2 = cfg2.store.table_store
+                        # Only try to dematerialize if an object with the correct name
+                        # exists. Otherwise, we might run into retry loops.
+                        if not isinstance(tbl2, Table) or tbl2.name.lower() in {
+                            s.lower() for s in store2.get_objects_in_stage(tbl2.stage)
+                        }:
+                            other_dict[key] = cfg2.store.dematerialize_item(
+                                tbl2, input_type
+                            )
+                        else:
+                            other_dict[key] = (
+                                "Table not found in other stage version: "
+                                f"{PipedagJSONEncoder().encode(tbl2)}"
+                            )
+                    except Exception as e:
+                        _task.logger.error(
+                            "Failed to dematerialize table from other stage version",
+                            table=ref,
+                            stage=tbl2.stage,
+                            instance=cfg2.instance_name,
+                            instance_id=cfg2.instance_id,
+                            cause=str(e),
+                        )
+                        other_dict[key] = e
+
+                for tbl, obj in table_dict.items():
+                    _dematerialize_versions(
+                        tbl, obj, transaction_table_dict, other_table_dict, cfg2, stage
+                    )
+                for blob, obj in blob_dict.items():
+                    _dematerialize_versions(
+                        blob, obj, transaction_blob_dict, other_blob_dict, cfg2, stage
+                    )
+                for raw_sql in raw_sqls:
+                    for tbl, obj in raw_sql.loaded_tables:
+                        _dematerialize_versions(
+                            tbl,
+                            obj,
+                            transaction_table_dict,
+                            other_table_dict,
+                            cfg2,
+                            stage,
+                        )
+
+            optional_cfg = [] if other_cfg is None else [other_cfg]
+
+            # restructure arbitrary arguments referencing Tables/Blobs/RawSQL into 2 or
+            # 4 dictionaries providing references only to tables and optionally blobs
+            if len(transaction_blob_dict) > 0:
+                ret = _fn(
+                    transaction_table_dict,
+                    other_table_dict,
+                    transaction_blob_dict,
+                    other_blob_dict,
+                    *optional_cfg,
+                    **pass_kwargs,
+                )
+            else:
+                ret = _fn(
+                    transaction_table_dict,
+                    other_table_dict,
+                    *optional_cfg,
+                    **pass_kwargs,
+                )
+        except Exception as e:
+            if lock_source_stages:
+                for stage in sorted(stages, reverse=True):
+                    lock_manager.release(stage.name)
+            raise e
+        return ret, cfg2, stages, lock_manager
+
+    def _collect_arguments(args, kwargs, is_dematerialized):
+        remaining_kwargs = {k: v for k, v in kwargs.items() if k not in set(pass_args)}
+        table_dict, blob_dict, raw_sqls = {}, {}, []
+        stages = set()
+        other_cfg = [None]  # list to allow modification in visitor
+        cnt = [0]
+        cfg_cnt = [0]
+        str_dict_keys = [0]
+
+        def visitor(x):
+            if isinstance(x, dict):
+                str_dict_keys[0] += sum(isinstance(k, str) for k in x.keys())
+            if not isinstance(x, (list, tuple, dict)):
+                cnt[0] += 1  # count non-collection arguments
+            if isinstance(x, ConfigContext):
+                if cfg_cnt[0] > 0:
+                    raise ValueError(
+                        "Only one ConfigContext object is allowed when calling a task "
+                        "decorated with @input_stage_versions."
+                    )
+                other_cfg[0] = x
+                cfg_cnt[0] += 1
+            if is_dematerialized:
+                if isinstance(x, tuple) and len(x) == 2:
+                    # with the add_input_source parameter of @materialize, we receive
+                    # tuples of the reference object (Table/Blob/RawSQL) together with
+                    # the dematerialized object
+                    obj, ref = x
+                else:
+                    return x
+            else:
+                obj, ref = x, x
+            if isinstance(ref, (Table, Blob, RawSql)):
+                stages.add(ref.stage)
+            if isinstance(ref, Table):
+                table_dict[ref] = obj
+            elif isinstance(ref, Blob):
+                blob_dict[ref] = obj
+            elif isinstance(ref, RawSql):
+                # ref and obj are identical for RawSql
+                raw_sqls.append(ref)
+            return x
+
+        deep_map(args, visitor)
+        deep_map(remaining_kwargs, visitor)
+        # dictionary keys don't count since we like to be f(config=cfg) to be considered
+        # as not any_data_arguements_collected
+        any_data_arguements_collected = cnt[0] > cfg_cnt[0] + str_dict_keys[0]
+        return (
+            stages,
+            table_dict,
+            blob_dict,
+            raw_sqls,
+            other_cfg[0],
+            any_data_arguements_collected,
+        )
+
+    return task
+
+
 def _get_output_from_store(
     task: MaterializingTask | MaterializingTaskGetItem, as_type: type
 ) -> Any:
     """Helper to retrieve task output from store"""
     from pydiverse.pipedag.context.run_context import DematerializeRunContext
     from pydiverse.pipedag.materialize.store import dematerialize_output_from_store
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/debug.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/debug.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/details.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/details.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/materialize/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             self.blob_store.commit_stage(stage)
 
     # ### Materialization ### #
 
     def dematerialize_item(
         self,
         item: Table | RawSql | Blob | Any,
-        as_type: type[T],
+        as_type: type[T] | None,
         ctx: RunContext | None = None,
         for_auto_versioning: bool = False,
     ):
         if ctx is None:
             ctx = RunContext.get()
 
         if isinstance(item, Table):
@@ -166,20 +166,23 @@
             for use with auto versioning.
         :return: A tuple with the dematerialized args and kwargs
         """
 
         ctx = RunContext.get()
 
         def dematerialize_mapper(x):
-            return self.dematerialize_item(
+            ret = self.dematerialize_item(
                 x,
                 as_type=task.input_type,
                 ctx=ctx,
                 for_auto_versioning=for_auto_versioning,
             )
+            if task.add_input_source and isinstance(x, (Table, Blob, RawSql)):
+                return ret, x
+            return ret
 
         d_args = deep_map(args, dematerialize_mapper)
         d_kwargs = deep_map(kwargs, dematerialize_mapper)
 
         return d_args, d_kwargs
 
     def materialize_task(
@@ -294,14 +297,20 @@
 
             if isinstance(x, PipedagConfig):
                 # Config objects are not an allowed return type,
                 # because they might mess up caching.
                 raise TypeError(
                     "You can't return a PipedagConfig object from a materializing task."
                 )
+            if isinstance(x, ConfigContext):
+                # Config objects are not an allowed return type,
+                # because they might mess up caching.
+                raise TypeError(
+                    "You can't return a ConfigContext object from a materializing task."
+                )
 
             # Add missing metadata (if table was not already imperatively materialized)
             if (
                 isinstance(x, (Table, RawSql, Blob))
                 and id(x)
                 not in task_cache_info.imperative_materialization_state.table_ids
             ):
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/computation_tracing.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/computation_tracing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 
 import datetime as dt
 import json
 from enum import Enum
 from functools import cache
 from pathlib import Path
 
-from pydiverse.pipedag import Stage
+from pydiverse.pipedag import ConfigContext, Stage
 from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
 
 TYPE_KEY = "__pipedag_type__"
 
 
 class Type(str, Enum):
     # Pipedag types
     TABLE = "table"
     RAW_SQL = "raw_sql"
     BLOB = "blob"
     STAGE = "stage"
     PIPEDAG_CONFIG = "pipedag_config"
+    CONFIG_CONTEXT = "config_context"
 
     # Other types we want to support
     PATHLIB_PATH = "pathlib:path"
     DT_DATE = "dt:date"
     DT_DATETIME = "dt:datetime"
 
     def __str__(self):
@@ -82,17 +83,25 @@
     if isinstance(o, Stage):
         return {
             TYPE_KEY: Type.STAGE,
             "name": o.name,
         }
     if isinstance(o, PipedagConfig):
         return {
-            TYPE_KEY: Type.STAGE,
+            TYPE_KEY: Type.PIPEDAG_CONFIG,
             "config_dict": o.config_dict,
         }
+    if isinstance(o, ConfigContext):
+        return {
+            TYPE_KEY: Type.CONFIG_CONTEXT,
+            "config_dict": o._config_dict,
+            "pipedag_name": o.pipedag_name,
+            "flow_name": o.flow_name,
+            "instance_name": o.instance_name,
+        }
     if isinstance(o, Path):
         return {
             TYPE_KEY: Type.PATHLIB_PATH,
             "path": str(o),
         }
     if isinstance(o, dt.date):
         return {
@@ -143,18 +152,19 @@
         blob = Blob(name=d["name"])
         blob.stage = get_stage(d["stage"])
         blob.cache_key = d["cache_key"]
         return blob
     if type_ == Type.STAGE:
         return get_stage(d["name"])
     if type_ == Type.PIPEDAG_CONFIG:
-        # PipedagConfig objects are allowed as input to @materialize tasks,
-        # but it is not allowed as output since this might cause trouble
-        # for cache-invalidation
-        raise TypeError("PipedagConfig can't be deserialized.")
+        return PipedagConfig(d["config_dict"])
+    if type_ == Type.CONFIG_CONTEXT:
+        return ConfigContext.new(
+            d["config_dict"], d["pipedag_name"], d["flow_name"], d["instance_name"]
+        )
     if type_ == Type.PATHLIB_PATH:
         return Path(d["path"])
     if type_ == Type.DT_DATE:
         return dt.date.fromisoformat(d["date"])
     if type_ == Type.DT_DATETIME:
         return dt.datetime.fromisoformat(d["datetime"])
```

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.9.2/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.9.1/PKG-INFO` & `pydiverse_pipedag-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.9.1
+Version: 0.9.2
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

