# Comparing `tmp/bigframes-1.4.0.tar.gz` & `tmp/bigframes-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigframes-1.4.0.tar", last modified: Tue Apr 30 00:15:00 2024, max compression
+gzip compressed data, was "bigframes-1.5.0.tar", last modified: Tue May  7 06:49:32 2024, max compression
```

## Comparing `bigframes-1.4.0.tar` & `bigframes-1.5.0.tar`

### file list

```diff
@@ -1,379 +1,388 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.395885 bigframes-1.4.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      914 2024-04-30 00:12:25.000000 bigframes-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4785 2024-04-30 00:15:00.395885 bigframes-1.4.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2391 2024-04-30 00:12:25.000000 bigframes-1.4.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.315864 bigframes-1.4.0/bigframes/
--rw-rw-r--   0 root         (0)     1003     1111 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.319865 bigframes-1.4.0/bigframes/_config/
--rw-rw-r--   0 root         (0)     1003     2453 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     8953 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/bigquery_options.py
--rw-rw-r--   0 root         (0)     1003     2141 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/compute_options.py
--rw-rw-r--   0 root         (0)     1003     1661 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/display_options.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/_config/sampling_options.py
--rw-rw-r--   0 root         (0)     1003     7152 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/clients.py
--rw-rw-r--   0 root         (0)     1003     2709 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/constants.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.323866 bigframes-1.4.0/bigframes/core/
--rw-rw-r--   0 root         (0)     1003    17931 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/__init__.py
--rw-rw-r--   0 root         (0)     1003    30768 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/block_transforms.py
--rw-rw-r--   0 root         (0)     1003    95393 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/blocks.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/compile/
--rw-rw-r--   0 root         (0)     1003      832 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/__init__.py
--rw-rw-r--   0 root         (0)     1003    17475 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/aggregate_compiler.py
--rw-rw-r--   0 root         (0)     1003    52133 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/compiled.py
--rw-rw-r--   0 root         (0)     1003     6341 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/compiler.py
--rw-rw-r--   0 root         (0)     1003     3356 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/concat.py
--rw-rw-r--   0 root         (0)     1003    48955 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/scalar_op_compiler.py
--rw-rw-r--   0 root         (0)     1003     7121 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/compile/single_column.py
--rw-rw-r--   0 root         (0)     1003     2962 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/convert.py
--rw-rw-r--   0 root         (0)     1003     2495 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/eval.py
--rw-rw-r--   0 root         (0)     1003     6685 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/expression.py
--rw-rw-r--   0 root         (0)     1003     1846 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/global_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/groupby/
--rw-rw-r--   0 root         (0)     1003    23982 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/groupby/__init__.py
--rw-rw-r--   0 root         (0)     1003      716 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/guid.py
--rw-rw-r--   0 root         (0)     1003    18056 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/indexes/
--rw-rw-r--   0 root         (0)     1003      719 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003    16223 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     1720 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     1730 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/join_def.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/joins/
--rw-rw-r--   0 root         (0)     1003      691 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/joins/__init__.py
--rw-rw-r--   0 root         (0)     1003     2132 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/joins/merge.py
--rw-rw-r--   0 root         (0)     1003     2218 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/local_data.py
--rw-rw-r--   0 root         (0)     1003     2255 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/log_adapter.py
--rw-rw-r--   0 root         (0)     1003    18515 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/nodes.py
--rw-rw-r--   0 root         (0)     1003     9445 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/ordering.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/reshape/
--rw-rw-r--   0 root         (0)     1003     6872 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003    11714 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/rewrite.py
--rw-rw-r--   0 root         (0)     1003      746 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/scalar.py
--rw-rw-r--   0 root         (0)     1003     2144 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/schema.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/tools/
--rw-rw-r--   0 root         (0)     1003      664 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2515 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tools/datetimes.py
--rw-rw-r--   0 root         (0)     1003     3002 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/tree_properties.py
--rw-rw-r--   0 root         (0)     1003     5483 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/core/window/
--rw-rw-r--   0 root         (0)     1003     3075 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1286 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/core/window_spec.py
--rw-rw-r--   0 root         (0)     1003   132040 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/dataframe.py
--rw-rw-r--   0 root         (0)     1003    27597 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/dtypes.py
--rw-rw-r--   0 root         (0)     1003      666 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/exceptions.py
--rw-rw-r--   0 root         (0)     1003     1273 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/features.py
--rw-rw-r--   0 root         (0)     1003    11179 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/formatting_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.327867 bigframes-1.4.0/bigframes/functions/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003    42108 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/functions/remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/ml/
--rw-rw-r--   0 root         (0)     1003      877 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     8542 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/base.py
--rw-rw-r--   0 root         (0)     1003     6659 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/cluster.py
--rw-rw-r--   0 root         (0)     1003     7984 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/compose.py
--rw-rw-r--   0 root         (0)     1003    17724 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/core.py
--rw-rw-r--   0 root         (0)     1003     6807 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/decomposition.py
--rw-rw-r--   0 root         (0)     1003    24746 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/ensemble.py
--rw-rw-r--   0 root         (0)     1003    15998 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/forecasting.py
--rw-rw-r--   0 root         (0)     1003     1141 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/globals.py
--rw-rw-r--   0 root         (0)     1003    10844 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/imported.py
--rw-rw-r--   0 root         (0)     1003    13818 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/linear_model.py
--rw-rw-r--   0 root         (0)     1003    32246 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/llm.py
--rw-rw-r--   0 root         (0)     1003     4899 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/loader.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/ml/metrics/
--rw-rw-r--   0 root         (0)     1003     1066 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/__init__.py
--rw-rw-r--   0 root         (0)     1003    11096 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/_metrics.py
--rw-rw-r--   0 root         (0)     1003     2373 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     3748 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/model_selection.py
--rw-rw-r--   0 root         (0)     1003     5067 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/pipeline.py
--rw-rw-r--   0 root         (0)     1003    22667 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/preprocessing.py
--rw-rw-r--   0 root         (0)     1003     5773 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/remote.py
--rw-rw-r--   0 root         (0)     1003    14405 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/sql.py
--rw-rw-r--   0 root         (0)     1003     2403 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/ml/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/operations/
--rw-rw-r--   0 root         (0)     1003    23377 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.335869 bigframes-1.4.0/bigframes/operations/_matplotlib/
--rw-rw-r--   0 root         (0)     1003     1022 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/__init__.py
--rw-rw-r--   0 root         (0)     1003     4477 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/core.py
--rw-rw-r--   0 root         (0)     1003     5970 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/_matplotlib/hist.py
--rw-rw-r--   0 root         (0)     1003    13202 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/aggregations.py
--rw-rw-r--   0 root         (0)     1003     9321 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/base.py
--rw-rw-r--   0 root         (0)     1003     3079 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/datetimes.py
--rw-rw-r--   0 root         (0)     1003     2814 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/plotting.py
--rw-rw-r--   0 root         (0)     1003     9009 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/strings.py
--rw-rw-r--   0 root         (0)     1003     2089 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/structs.py
--rw-rw-r--   0 root         (0)     1003     7613 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/operations/type.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/pandas/
--rw-rw-r--   0 root         (0)     1003    23435 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/pandas/__init__.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/py.typed
--rw-rw-r--   0 root         (0)     1003    64464 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/session/
--rw-rw-r--   0 root         (0)     1003    83061 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/bigframes/session/_io/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/__init__.py
--rw-rw-r--   0 root         (0)     1003    11305 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/bigquery.py
--rw-rw-r--   0 root         (0)     1003     4345 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/_io/pandas.py
--rw-rw-r--   0 root         (0)     1003     8043 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/session/clients.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/typing.py
--rw-rw-r--   0 root         (0)     1003      597 2024-04-30 00:12:25.000000 bigframes-1.4.0/bigframes/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/bigframes.egg-info/
--rw-r--r--   0 root         (0)     1003     4785 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    12307 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      732 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       29 2024-04-30 00:15:00.000000 bigframes-1.4.0/bigframes.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       81 2024-04-30 00:12:25.000000 bigframes-1.4.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003       67 2024-04-30 00:15:00.395885 bigframes-1.4.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     4428 2024-04-30 00:12:25.000000 bigframes-1.4.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.339870 bigframes-1.4.0/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/data/
--rw-rw-r--   0 root         (0)     1003      619 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/hockey_players.json
--rw-rw-r--   0 root         (0)     1003     1250 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/hockey_players.jsonl
--rw-rw-r--   0 root         (0)     1003      340 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_2by3.json
--rw-rw-r--   0 root         (0)     1003       80 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_2by3.jsonl
--rw-rw-r--   0 root         (0)     1003      421 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_3by4.json
--rw-rw-r--   0 root         (0)     1003      154 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/matrix_3by4.jsonl
--rw-rw-r--   0 root         (0)     1003    33350 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/nested.jsonl
--rw-rw-r--   0 root         (0)     1003      966 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/nested_schema.json
--rw-rw-r--   0 root         (0)     1003    58869 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/penguins.jsonl
--rw-rw-r--   0 root         (0)     1003      636 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/penguins_schema.json
--rw-rw-r--   0 root         (0)     1003     3909 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/scalars.jsonl
--rw-rw-r--   0 root         (0)     1003     1458 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/scalars_schema.json
--rw-rw-r--   0 root         (0)     1003    23424 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/time_series.jsonl
--rw-rw-r--   0 root         (0)     1003      192 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/data/time_series_schema.json
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003    37000 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.343871 bigframes-1.4.0/tests/system/large/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.347872 bigframes-1.4.0/tests/system/large/ml/
--rw-rw-r--   0 root         (0)     1003     5411 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003     5391 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     6401 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6487 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    14451 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     4366 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     8408 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    30362 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003     4079 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_location.py
--rw-rw-r--   0 root         (0)     1003    52808 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003     1908 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/large/test_session.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.347872 bigframes-1.4.0/tests/system/load/
--rw-rw-r--   0 root         (0)     1003     3000 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/load/test_large_tables.py
--rw-rw-r--   0 root         (0)     1003     4559 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/load/test_llm.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.351873 bigframes-1.4.0/tests/system/small/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.355874 bigframes-1.4.0/tests/system/small/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003    11773 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/conftest.py
--rw-rw-r--   0 root         (0)     1003     7074 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_cluster.py
--rw-rw-r--   0 root         (0)     1003    13810 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_core.py
--rw-rw-r--   0 root         (0)     1003     6764 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_decomposition.py
--rw-rw-r--   0 root         (0)     1003    17015 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_ensemble.py
--rw-rw-r--   0 root         (0)     1003     6859 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_forecasting.py
--rw-rw-r--   0 root         (0)     1003     4983 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_imported.py
--rw-rw-r--   0 root         (0)     1003     8788 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_linear_model.py
--rw-rw-r--   0 root         (0)     1003    11541 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_llm.py
--rw-rw-r--   0 root         (0)     1003    25138 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_metrics.py
--rw-rw-r--   0 root         (0)     1003     2224 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_metrics_pairwise.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_model_selection.py
--rw-rw-r--   0 root         (0)     1003    27150 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_preprocessing.py
--rw-rw-r--   0 root         (0)     1003     2570 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_register.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/ml/test_remote.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/system/small/operations/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003    10399 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_datetimes.py
--rw-rw-r--   0 root         (0)     1003    12453 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_plotting.py
--rw-rw-r--   0 root         (0)     1003    15770 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/operations/test_strings.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/system/small/regression/
--rw-rw-r--   0 root         (0)     1003     1999 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/regression/test_issue355_merge_after_filter.py
--rw-rw-r--   0 root         (0)     1003   145083 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003    18961 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_dataframe_io.py
--rw-rw-r--   0 root         (0)     1003    10570 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_encryption.py
--rw-rw-r--   0 root         (0)     1003    13974 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_groupby.py
--rw-rw-r--   0 root         (0)     1003     1558 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_ibis.py
--rw-rw-r--   0 root         (0)     1003    13328 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_index.py
--rw-rw-r--   0 root         (0)     1003     1205 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_ipython.py
--rw-rw-r--   0 root         (0)     1003    41010 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_multiindex.py
--rw-rw-r--   0 root         (0)     1003     4190 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_numpy.py
--rw-rw-r--   0 root         (0)     1003    19608 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     9533 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_pandas_options.py
--rw-rw-r--   0 root         (0)     1003     4126 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_progress_bar.py
--rw-rw-r--   0 root         (0)     1003    26485 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_remote_function.py
--rw-rw-r--   0 root         (0)     1003      913 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_scalar.py
--rw-rw-r--   0 root         (0)     1003   111197 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_series.py
--rw-rw-r--   0 root         (0)     1003    40386 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_session.py
--rw-rw-r--   0 root         (0)     1003     3343 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/small/test_window.py
--rw-rw-r--   0 root         (0)     1003    12113 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/system/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.359876 bigframes-1.4.0/tests/unit/_config/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/_config/__init__.py
--rw-rw-r--   0 root         (0)     1003     4218 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/_config/test_bigquery_options.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/core/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/__init__.py
--rw-rw-r--   0 root         (0)     1003     1619 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_bf_utils.py
--rw-rw-r--   0 root         (0)     1003     2966 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_blocks.py
--rw-rw-r--   0 root         (0)     1003     1553 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_expression.py
--rw-rw-r--   0 root         (0)     1003     1813 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/core/test_log_adapter.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/ml/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/__init__.py
--rw-rw-r--   0 root         (0)     1003     2323 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_api_primitives.py
--rw-rw-r--   0 root         (0)     1003     6555 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_compose.py
--rw-rw-r--   0 root         (0)     1003     7422 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_golden_sql.py
--rw-rw-r--   0 root         (0)     1003     4058 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_pipeline.py
--rw-rw-r--   0 root         (0)     1003    14241 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/ml/test_sql.py
--rw-rw-r--   0 root         (0)     1003     5298 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.363877 bigframes-1.4.0/tests/unit/session/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/__init__.py
--rw-rw-r--   0 root         (0)     1003     4347 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_clients.py
--rw-rw-r--   0 root         (0)     1003     7809 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_io_bigquery.py
--rw-rw-r--   0 root         (0)     1003    18664 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_io_pandas.py
--rw-rw-r--   0 root         (0)     1003     8702 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/session/test_session.py
--rw-rw-r--   0 root         (0)     1003     1744 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_clients.py
--rw-rw-r--   0 root         (0)     1003     1056 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_compute_options.py
--rw-rw-r--   0 root         (0)     1003     6648 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_core.py
--rw-rw-r--   0 root         (0)     1003     2136 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_dataframe.py
--rw-rw-r--   0 root         (0)     1003     8819 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_dtypes.py
--rw-rw-r--   0 root         (0)     1003     1577 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_features.py
--rw-rw-r--   0 root         (0)     1003      528 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_formatting_helper.py
--rw-rw-r--   0 root         (0)     1003     1655 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_formatting_helpers.py
--rw-rw-r--   0 root         (0)     1003     4055 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_pandas.py
--rw-rw-r--   0 root         (0)     1003     1207 2024-04-30 00:12:25.000000 bigframes-1.4.0/tests/unit/test_remote_function.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.303861 bigframes-1.4.0/third_party/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/cpython/
--rw-rw-r--   0 root         (0)     1003     2339 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/__init__.py
--rw-rw-r--   0 root         (0)     1003    18854 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/cpython/_pprint.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     5290 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
--rw-rw-r--   0 root         (0)     1003      574 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    14045 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/ibis/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/LICENSE.txt
--rw-rw-r--   0 root         (0)     1003    11663 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.367878 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/
--rw-rw-r--   0 root         (0)     1003      184 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2091 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
--rw-rw-r--   0 root         (0)     1003     6600 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
--rw-rw-r--   0 root         (0)     1003     1892 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/
--rw-rw-r--   0 root         (0)     1003      464 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
--rw-rw-r--   0 root         (0)     1003      536 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
--rw-rw-r--   0 root         (0)     1003      276 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
--rw-rw-r--   0 root         (0)     1003      263 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
--rw-rw-r--   0 root         (0)     1003      690 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/pandas/
--rw-rw-r--   0 root         (0)     1003     2284 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/AUTHORS.md
--rw-rw-r--   0 root         (0)     1003     1634 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/LICENSE
--rw-rw-r--   0 root         (0)     1003    10620 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/README.md
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.371879 bigframes-1.4.0/third_party/bigframes_vendored/pandas/_config/
--rw-rw-r--   0 root         (0)     1003     1347 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/_config/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.375880 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
--rw-rw-r--   0 root         (0)     1003     3831 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
--rw-rw-r--   0 root         (0)     1003     3689 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
--rw-rw-r--   0 root         (0)     1003     2086 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/common.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/
--rw-rw-r--   0 root         (0)     1003     6944 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/align.py
--rw-rw-r--   0 root         (0)     1003     1543 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/common.py
--rw-rw-r--   0 root         (0)     1003     2295 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
--rw-rw-r--   0 root         (0)     1003    12685 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
--rw-rw-r--   0 root         (0)     1003    25132 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
--rw-rw-r--   0 root         (0)     1003    16244 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
--rw-rw-r--   0 root         (0)     1003     6477 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
--rw-rw-r--   0 root         (0)     1003    10303 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
--rw-rw-r--   0 root         (0)     1003     4394 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/config_init.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/
--rw-rw-r--   0 root         (0)     1003      707 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
--rw-rw-r--   0 root         (0)     1003   228180 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/frame.py
--rw-rw-r--   0 root         (0)     1003    40215 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/generic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/
--rw-rw-r--   0 root         (0)     1003    14023 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
--rw-rw-r--   0 root         (0)     1003     9589 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
--rw-rw-r--   0 root         (0)     1003    11461 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
--rw-rw-r--   0 root         (0)     1003     2941 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
--rw-rw-r--   0 root         (0)     1003     2909 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
--rw-rw-r--   0 root         (0)     1003     4372 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
--rw-rw-r--   0 root         (0)     1003     3804 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
--rw-rw-r--   0 root         (0)     1003     3220 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
--rw-rw-r--   0 root         (0)     1003     5844 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
--rw-rw-r--   0 root         (0)     1003   131177 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/series.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/
--rw-rw-r--   0 root         (0)     1003    37771 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.379881 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
--rw-rw-r--   0 root         (0)     1003     2964 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
--rw-rw-r--   0 root         (0)     1003     1350 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/__init__.py
--rw-rw-r--   0 root         (0)     1003     1269 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/common.py
--rw-rw-r--   0 root         (0)     1003     7071 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/gbq.py
--rw-rw-r--   0 root         (0)     1003     1428 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parquet.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
--rw-rw-r--   0 root         (0)     1003    10553 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
--rw-rw-r--   0 root         (0)     1003     3130 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/pickle.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/
--rw-rw-r--   0 root         (0)     1003    12353 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/_core.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/
--rw-rw-r--   0 root         (0)     1003      765 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
--rw-rw-r--   0 root         (0)     1003     1573 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_validators.py
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.383882 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/
--rw-rw-r--   0 root         (0)     1003     1532 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/COPYING
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/__init__.py
--rw-rw-r--   0 root         (0)     1003     6212 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/base.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/
--rw-rw-r--   0 root         (0)     1003     5924 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/
--rw-rw-r--   0 root         (0)     1003     2014 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/
--rw-rw-r--   0 root         (0)     1003     5387 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
--rw-rw-r--   0 root         (0)     1003     8977 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/
--rw-rw-r--   0 root         (0)     1003     5417 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
--rw-rw-r--   0 root         (0)     1003     4348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.387883 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/
--rw-rw-r--   0 root         (0)     1003     9783 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
--rw-rw-r--   0 root         (0)     1003     6347 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
--rw-rw-r--   0 root         (0)     1003     3550 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
--rw-rw-r--   0 root         (0)     1003     2124 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
--rw-rw-r--   0 root         (0)     1003     2977 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/pipeline.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/
--rw-rw-r--   0 root         (0)     1003     4980 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
--rw-rw-r--   0 root         (0)     1003     1523 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
--rw-rw-r--   0 root         (0)     1003     4059 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
--rw-rw-r--   0 root         (0)     1003     2085 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-30 00:15:00.391884 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/
--rw-rw-r--   0 root         (0)     1003    11348 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/LICENSE
--rw-rw-r--   0 root         (0)     1003        0 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/__init__.py
--rw-rw-r--   0 root         (0)     1003     6919 2024-04-30 00:12:25.000000 bigframes-1.4.0/third_party/bigframes_vendored/xgboost/sklearn.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.982660 bigframes-1.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 06:46:57.000000 bigframes-1.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      914 2024-05-07 06:46:57.000000 bigframes-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4785 2024-05-07 06:49:32.978659 bigframes-1.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2391 2024-05-07 06:46:57.000000 bigframes-1.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.902653 bigframes-1.5.0/bigframes/
+-rw-rw-r--   0 root         (0)     1003     1216 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.906654 bigframes-1.5.0/bigframes/_config/
+-rw-rw-r--   0 root         (0)     1003     4315 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8953 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/_config/bigquery_options.py
+-rw-rw-r--   0 root         (0)     1003     4369 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/_config/compute_options.py
+-rw-rw-r--   0 root         (0)     1003     1661 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/_config/display_options.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/_config/sampling_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.906654 bigframes-1.5.0/bigframes/bigquery/
+-rw-rw-r--   0 root         (0)     1003     1730 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7152 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/clients.py
+-rw-rw-r--   0 root         (0)     1003     2779 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/constants.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.910654 bigframes-1.5.0/bigframes/core/
+-rw-rw-r--   0 root         (0)     1003    18021 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30768 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/block_transforms.py
+-rw-rw-r--   0 root         (0)     1003    95833 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/blocks.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/compile/
+-rw-rw-r--   0 root         (0)     1003      832 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17475 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/aggregate_compiler.py
+-rw-rw-r--   0 root         (0)     1003    52133 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/compiled.py
+-rw-rw-r--   0 root         (0)     1003     6341 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/compiler.py
+-rw-rw-r--   0 root         (0)     1003     3356 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/concat.py
+-rw-rw-r--   0 root         (0)     1003    48955 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/scalar_op_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7121 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/compile/single_column.py
+-rw-rw-r--   0 root         (0)     1003     2962 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/convert.py
+-rw-rw-r--   0 root         (0)     1003     2495 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/eval.py
+-rw-rw-r--   0 root         (0)     1003     6685 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/expression.py
+-rw-rw-r--   0 root         (0)     1003     3887 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/global_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    23982 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/groupby/__init__.py
+-rw-rw-r--   0 root         (0)     1003      716 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/guid.py
+-rw-rw-r--   0 root         (0)     1003    18056 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/indexers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/indexes/
+-rw-rw-r--   0 root         (0)     1003      719 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16239 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     1720 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     1730 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/join_def.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/joins/
+-rw-rw-r--   0 root         (0)     1003      691 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/joins/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2132 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/joins/merge.py
+-rw-rw-r--   0 root         (0)     1003     2218 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/local_data.py
+-rw-rw-r--   0 root         (0)     1003     2255 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/log_adapter.py
+-rw-rw-r--   0 root         (0)     1003    18515 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/nodes.py
+-rw-rw-r--   0 root         (0)     1003     9445 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/ordering.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/reshape/
+-rw-rw-r--   0 root         (0)     1003     6872 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11714 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/rewrite.py
+-rw-rw-r--   0 root         (0)     1003      746 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/scalar.py
+-rw-rw-r--   0 root         (0)     1003     2144 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/schema.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/tools/
+-rw-rw-r--   0 root         (0)     1003      664 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2515 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/tools/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     3002 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/tree_properties.py
+-rw-rw-r--   0 root         (0)     1003     5483 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/core/window/
+-rw-rw-r--   0 root         (0)     1003     3075 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1286 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/core/window_spec.py
+-rw-rw-r--   0 root         (0)     1003   132153 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/dataframe.py
+-rw-rw-r--   0 root         (0)     1003    27597 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1029 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/enums.py
+-rw-rw-r--   0 root         (0)     1003      992 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1273 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/features.py
+-rw-rw-r--   0 root         (0)     1003    11179 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/formatting_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.914654 bigframes-1.5.0/bigframes/functions/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    43091 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/functions/remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.922655 bigframes-1.5.0/bigframes/ml/
+-rw-rw-r--   0 root         (0)     1003      877 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8542 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/base.py
+-rw-rw-r--   0 root         (0)     1003     6659 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/cluster.py
+-rw-rw-r--   0 root         (0)     1003     7984 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/compose.py
+-rw-rw-r--   0 root         (0)     1003    17897 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/core.py
+-rw-rw-r--   0 root         (0)     1003     6807 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/decomposition.py
+-rw-rw-r--   0 root         (0)     1003    24746 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/ensemble.py
+-rw-rw-r--   0 root         (0)     1003    16689 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/forecasting.py
+-rw-rw-r--   0 root         (0)     1003     1141 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/globals.py
+-rw-rw-r--   0 root         (0)     1003    10844 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/imported.py
+-rw-rw-r--   0 root         (0)     1003    13818 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/linear_model.py
+-rw-rw-r--   0 root         (0)     1003    32261 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/llm.py
+-rw-rw-r--   0 root         (0)     1003     4899 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/loader.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.922655 bigframes-1.5.0/bigframes/ml/metrics/
+-rw-rw-r--   0 root         (0)     1003     1066 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/metrics/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11096 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/metrics/_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2373 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     3748 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/model_selection.py
+-rw-rw-r--   0 root         (0)     1003     5067 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/pipeline.py
+-rw-rw-r--   0 root         (0)     1003    22667 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     5773 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/remote.py
+-rw-rw-r--   0 root         (0)     1003    14588 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/sql.py
+-rw-rw-r--   0 root         (0)     1003     2403 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/ml/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.922655 bigframes-1.5.0/bigframes/operations/
+-rw-rw-r--   0 root         (0)     1003    23377 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.922655 bigframes-1.5.0/bigframes/operations/_matplotlib/
+-rw-rw-r--   0 root         (0)     1003     1022 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/_matplotlib/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4477 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/_matplotlib/core.py
+-rw-rw-r--   0 root         (0)     1003     5970 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/_matplotlib/hist.py
+-rw-rw-r--   0 root         (0)     1003    13202 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/aggregations.py
+-rw-rw-r--   0 root         (0)     1003     9321 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/base.py
+-rw-rw-r--   0 root         (0)     1003     3079 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/datetimes.py
+-rw-rw-r--   0 root         (0)     1003     2814 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/plotting.py
+-rw-rw-r--   0 root         (0)     1003     9009 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/strings.py
+-rw-rw-r--   0 root         (0)     1003     2089 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/structs.py
+-rw-rw-r--   0 root         (0)     1003     7613 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/operations/type.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.926655 bigframes-1.5.0/bigframes/pandas/
+-rw-rw-r--   0 root         (0)     1003    25854 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/pandas/__init__.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/py.typed
+-rw-rw-r--   0 root         (0)     1003    64473 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.926655 bigframes-1.5.0/bigframes/session/
+-rw-rw-r--   0 root         (0)     1003    80817 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.926655 bigframes-1.5.0/bigframes/session/_io/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/_io/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.926655 bigframes-1.5.0/bigframes/session/_io/bigquery/
+-rw-rw-r--   0 root         (0)     1003    10605 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/_io/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16779 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/_io/bigquery/read_gbq_table.py
+-rw-rw-r--   0 root         (0)     1003     4345 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/_io/pandas.py
+-rw-rw-r--   0 root         (0)     1003     8043 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/session/clients.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/typing.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-05-07 06:46:57.000000 bigframes-1.5.0/bigframes/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.978659 bigframes-1.5.0/bigframes.egg-info/
+-rw-r--r--   0 root         (0)     1003     4785 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    12539 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      732 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       29 2024-05-07 06:49:32.000000 bigframes-1.5.0/bigframes.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       81 2024-05-07 06:46:57.000000 bigframes-1.5.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003       67 2024-05-07 06:49:32.982660 bigframes-1.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4428 2024-05-07 06:46:57.000000 bigframes-1.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.926655 bigframes-1.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.930656 bigframes-1.5.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003      619 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/hockey_players.json
+-rw-rw-r--   0 root         (0)     1003     1250 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/hockey_players.jsonl
+-rw-rw-r--   0 root         (0)     1003      340 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/matrix_2by3.json
+-rw-rw-r--   0 root         (0)     1003       80 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/matrix_2by3.jsonl
+-rw-rw-r--   0 root         (0)     1003      421 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/matrix_3by4.json
+-rw-rw-r--   0 root         (0)     1003      154 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/matrix_3by4.jsonl
+-rw-rw-r--   0 root         (0)     1003    33350 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/nested.jsonl
+-rw-rw-r--   0 root         (0)     1003      966 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/nested_schema.json
+-rw-rw-r--   0 root         (0)     1003    58869 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/penguins.jsonl
+-rw-rw-r--   0 root         (0)     1003      636 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/penguins_schema.json
+-rw-rw-r--   0 root         (0)     1003     3909 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/scalars.jsonl
+-rw-rw-r--   0 root         (0)     1003     1458 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/scalars_schema.json
+-rw-rw-r--   0 root         (0)     1003    23424 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/time_series.jsonl
+-rw-rw-r--   0 root         (0)     1003      192 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/data/time_series_schema.json
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.930656 bigframes-1.5.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37310 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.930656 bigframes-1.5.0/tests/system/large/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.934656 bigframes-1.5.0/tests/system/large/ml/
+-rw-rw-r--   0 root         (0)     1003     5411 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003     5391 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     6516 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6487 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    14552 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     4551 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     8408 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    30564 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003     4079 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/test_location.py
+-rw-rw-r--   0 root         (0)     1003    54220 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003     4573 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/large/test_session.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.934656 bigframes-1.5.0/tests/system/load/
+-rw-rw-r--   0 root         (0)     1003     3000 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/load/test_large_tables.py
+-rw-rw-r--   0 root         (0)     1003     4559 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/load/test_llm.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.938656 bigframes-1.5.0/tests/system/small/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.938656 bigframes-1.5.0/tests/system/small/bigquery/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1154 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/bigquery/test_array.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.942657 bigframes-1.5.0/tests/system/small/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11773 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/conftest.py
+-rw-rw-r--   0 root         (0)     1003     7074 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_cluster.py
+-rw-rw-r--   0 root         (0)     1003    13810 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_core.py
+-rw-rw-r--   0 root         (0)     1003     6764 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_decomposition.py
+-rw-rw-r--   0 root         (0)     1003    17015 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_ensemble.py
+-rw-rw-r--   0 root         (0)     1003     6859 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_forecasting.py
+-rw-rw-r--   0 root         (0)     1003     4983 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_imported.py
+-rw-rw-r--   0 root         (0)     1003     8788 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_linear_model.py
+-rw-rw-r--   0 root         (0)     1003    11929 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_llm.py
+-rw-rw-r--   0 root         (0)     1003    25138 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_metrics.py
+-rw-rw-r--   0 root         (0)     1003     2224 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_metrics_pairwise.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_model_selection.py
+-rw-rw-r--   0 root         (0)     1003    27150 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_preprocessing.py
+-rw-rw-r--   0 root         (0)     1003     2570 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_register.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/ml/test_remote.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.946657 bigframes-1.5.0/tests/system/small/operations/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10399 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/operations/test_datetimes.py
+-rw-rw-r--   0 root         (0)     1003    12453 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/operations/test_plotting.py
+-rw-rw-r--   0 root         (0)     1003    15770 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/operations/test_strings.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.946657 bigframes-1.5.0/tests/system/small/regression/
+-rw-rw-r--   0 root         (0)     1003     1999 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/regression/test_issue355_merge_after_filter.py
+-rw-rw-r--   0 root         (0)     1003   145044 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003    18968 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_dataframe_io.py
+-rw-rw-r--   0 root         (0)     1003    10446 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_encryption.py
+-rw-rw-r--   0 root         (0)     1003    13974 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_groupby.py
+-rw-rw-r--   0 root         (0)     1003     1558 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_ibis.py
+-rw-rw-r--   0 root         (0)     1003    13328 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_index.py
+-rw-rw-r--   0 root         (0)     1003     1205 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_ipython.py
+-rw-rw-r--   0 root         (0)     1003    41847 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_multiindex.py
+-rw-rw-r--   0 root         (0)     1003     4190 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_numpy.py
+-rw-rw-r--   0 root         (0)     1003    19608 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003    10425 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_pandas_options.py
+-rw-rw-r--   0 root         (0)     1003     5133 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_progress_bar.py
+-rw-rw-r--   0 root         (0)     1003    26485 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_remote_function.py
+-rw-rw-r--   0 root         (0)     1003      913 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_scalar.py
+-rw-rw-r--   0 root         (0)     1003   111197 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_series.py
+-rw-rw-r--   0 root         (0)     1003    40499 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_session.py
+-rw-rw-r--   0 root         (0)     1003     3343 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/small/test_window.py
+-rw-rw-r--   0 root         (0)     1003    12113 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/system/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.946657 bigframes-1.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.950657 bigframes-1.5.0/tests/unit/_config/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/_config/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4218 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/_config/test_bigquery_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.950657 bigframes-1.5.0/tests/unit/core/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/core/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1619 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/core/test_bf_utils.py
+-rw-rw-r--   0 root         (0)     1003     2966 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/core/test_blocks.py
+-rw-rw-r--   0 root         (0)     1003     1553 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/core/test_expression.py
+-rw-rw-r--   0 root         (0)     1003     1813 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/core/test_log_adapter.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.950657 bigframes-1.5.0/tests/unit/ml/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2323 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/test_api_primitives.py
+-rw-rw-r--   0 root         (0)     1003     6555 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/test_compose.py
+-rw-rw-r--   0 root         (0)     1003     7422 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/test_golden_sql.py
+-rw-rw-r--   0 root         (0)     1003     4058 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/test_pipeline.py
+-rw-rw-r--   0 root         (0)     1003    14554 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/ml/test_sql.py
+-rw-rw-r--   0 root         (0)     1003     5298 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/tests/unit/session/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4347 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     7193 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/test_io_bigquery.py
+-rw-rw-r--   0 root         (0)     1003    18664 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/test_io_pandas.py
+-rw-rw-r--   0 root         (0)     1003     1272 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/test_read_gbq_table.py
+-rw-rw-r--   0 root         (0)     1003    16158 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/session/test_session.py
+-rw-rw-r--   0 root         (0)     1003     1744 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_clients.py
+-rw-rw-r--   0 root         (0)     1003     1056 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_compute_options.py
+-rw-rw-r--   0 root         (0)     1003     6648 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_core.py
+-rw-rw-r--   0 root         (0)     1003     2136 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_dataframe.py
+-rw-rw-r--   0 root         (0)     1003     8819 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_dtypes.py
+-rw-rw-r--   0 root         (0)     1003     1577 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_features.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_formatting_helper.py
+-rw-rw-r--   0 root         (0)     1003     1655 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_formatting_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4055 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_pandas.py
+-rw-rw-r--   0 root         (0)     1003     1207 2024-05-07 06:46:57.000000 bigframes-1.5.0/tests/unit/test_remote_function.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.890652 bigframes-1.5.0/third_party/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/cpython/
+-rw-rw-r--   0 root         (0)     1003     2339 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/cpython/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/cpython/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18854 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/cpython/_pprint.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5290 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      574 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14045 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.954658 bigframes-1.5.0/third_party/bigframes_vendored/ibis/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/LICENSE.txt
+-rw-rw-r--   0 root         (0)     1003    11663 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/
+-rw-rw-r--   0 root         (0)     1003      184 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2091 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py
+-rw-rw-r--   0 root         (0)     1003     6600 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py
+-rw-rw-r--   0 root         (0)     1003     1892 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/
+-rw-rw-r--   0 root         (0)     1003      464 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      536 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py
+-rw-rw-r--   0 root         (0)     1003      276 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/generic.py
+-rw-rw-r--   0 root         (0)     1003      263 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/json.py
+-rw-rw-r--   0 root         (0)     1003      690 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/
+-rw-rw-r--   0 root         (0)     1003     2284 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/AUTHORS.md
+-rw-rw-r--   0 root         (0)     1003     1634 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/LICENSE
+-rw-rw-r--   0 root         (0)     1003    10620 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/README.md
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.958658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/_config/
+-rw-rw-r--   0 root         (0)     1003     2352 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/_config/config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.962658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.962658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.962658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3831 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py
+-rw-rw-r--   0 root         (0)     1003     3689 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py
+-rw-rw-r--   0 root         (0)     1003     2086 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/common.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/
+-rw-rw-r--   0 root         (0)     1003     6944 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/align.py
+-rw-rw-r--   0 root         (0)     1003     1543 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/common.py
+-rw-rw-r--   0 root         (0)     1003     2295 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/engines.py
+-rw-rw-r--   0 root         (0)     1003    12685 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/eval.py
+-rw-rw-r--   0 root         (0)     1003    25132 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/expr.py
+-rw-rw-r--   0 root         (0)     1003    16244 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/ops.py
+-rw-rw-r--   0 root         (0)     1003     6477 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py
+-rw-rw-r--   0 root         (0)     1003    10303 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/scope.py
+-rw-rw-r--   0 root         (0)     1003     4394 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/config_init.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/dtypes/
+-rw-rw-r--   0 root         (0)     1003      707 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py
+-rw-rw-r--   0 root         (0)     1003   228195 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/frame.py
+-rw-rw-r--   0 root         (0)     1003    40215 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/generic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/groupby/
+-rw-rw-r--   0 root         (0)     1003    14023 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9589 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py
+-rw-rw-r--   0 root         (0)     1003    11461 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/base.py
+-rw-rw-r--   0 root         (0)     1003     2941 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py
+-rw-rw-r--   0 root         (0)     1003     2909 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4372 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py
+-rw-rw-r--   0 root         (0)     1003     3804 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py
+-rw-rw-r--   0 root         (0)     1003     3220 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py
+-rw-rw-r--   0 root         (0)     1003     5844 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py
+-rw-rw-r--   0 root         (0)     1003   131177 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/series.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.966658 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/strings/
+-rw-rw-r--   0 root         (0)     1003    37771 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/tools/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/tools/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2964 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/window/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/window/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/window/rolling.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1269 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/common.py
+-rw-rw-r--   0 root         (0)     1003     8092 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/gbq.py
+-rw-rw-r--   0 root         (0)     1003     1428 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parquet.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parsers/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parsers/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10705 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py
+-rw-rw-r--   0 root         (0)     1003     3130 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/pickle.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/pandas/
+-rw-rw-r--   0 root         (0)     1003    12353 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/pandas/_typing.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/plotting/
+-rw-rw-r--   0 root         (0)     1003    11460 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/plotting/_core.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.970659 bigframes-1.5.0/third_party/bigframes_vendored/pandas/util/
+-rw-rw-r--   0 root         (0)     1003      765 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/util/_exceptions.py
+-rw-rw-r--   0 root         (0)     1003     1573 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/pandas/util/_validators.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/
+-rw-rw-r--   0 root         (0)     1003     1532 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/COPYING
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6212 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/base.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/cluster/
+-rw-rw-r--   0 root         (0)     1003     5924 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/compose/
+-rw-rw-r--   0 root         (0)     1003     2014 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/decomposition/
+-rw-rw-r--   0 root         (0)     1003     5387 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/ensemble/
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/ensemble/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8977 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/linear_model/
+-rw-rw-r--   0 root         (0)     1003     5417 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py
+-rw-rw-r--   0 root         (0)     1003     4348 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.974659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/
+-rw-rw-r--   0 root         (0)     1003     9783 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py
+-rw-rw-r--   0 root         (0)     1003     6347 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py
+-rw-rw-r--   0 root         (0)     1003     3550 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py
+-rw-rw-r--   0 root         (0)     1003     2124 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py
+-rw-rw-r--   0 root         (0)     1003     2977 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/pipeline.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.978659 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/
+-rw-rw-r--   0 root         (0)     1003     4980 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py
+-rw-rw-r--   0 root         (0)     1003     1523 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py
+-rw-rw-r--   0 root         (0)     1003     4059 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py
+-rw-rw-r--   0 root         (0)     1003     2085 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-07 06:49:32.978659 bigframes-1.5.0/third_party/bigframes_vendored/xgboost/
+-rw-rw-r--   0 root         (0)     1003    11348 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/xgboost/LICENSE
+-rw-rw-r--   0 root         (0)     1003        0 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/xgboost/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6919 2024-05-07 06:46:57.000000 bigframes-1.5.0/third_party/bigframes_vendored/xgboost/sklearn.py
```

### Comparing `bigframes-1.4.0/LICENSE` & `bigframes-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/MANIFEST.in` & `bigframes-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/PKG-INFO` & `bigframes-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.4.0
+Version: 1.5.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bigframes-1.4.0/README.rst` & `bigframes-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/__init__.py` & `bigframes-1.5.0/bigframes/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 # limitations under the License.
 
 """BigQuery DataFrames provides a DataFrame API scaled by the BigQuery engine."""
 
 from bigframes._config import option_context, options
 from bigframes._config.bigquery_options import BigQueryOptions
 from bigframes.core.global_session import close_session, get_global_session
+import bigframes.enums as enums
+import bigframes.exceptions as exceptions
 from bigframes.session import connect, Session
 from bigframes.version import __version__
 
 __all__ = [
     "options",
     "BigQueryOptions",
     "get_global_session",
     "close_session",
+    "enums",
+    "exceptions",
     "connect",
     "Session",
     "__version__",
     "option_context",
 ]
```

### Comparing `bigframes-1.4.0/bigframes/_config/bigquery_options.py` & `bigframes-1.5.0/bigframes/_config/bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/_config/display_options.py` & `bigframes-1.5.0/bigframes/_config/display_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/_config/sampling_options.py` & `bigframes-1.5.0/bigframes/_config/sampling_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/clients.py` & `bigframes-1.5.0/bigframes/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/constants.py` & `bigframes-1.5.0/bigframes/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ABSTRACT_METHOD_ERROR_MESSAGE = f"Abstract method. You have likely encountered a bug. Please share this stacktrace and how you reached it with the BigQuery DataFrames team. {FEEDBACK_LINK}"
 
 DEFAULT_EXPIRATION = datetime.timedelta(days=7)
 
 # https://cloud.google.com/bigquery/docs/locations
 ALL_BIGQUERY_LOCATIONS = frozenset(
     {
+        # regions
         "us-east5",
         "us-south1",
         "us-central1",
         "us-west4",
         "us-west2",
         "northamerica-northeast1",
         "us-east4",
@@ -70,14 +71,17 @@
         "me-central2",
         "me-central1",
         "me-west1",
         "me-central2",
         "me-central1",
         "me-west1",
         "africa-south1",
+        # multi-regions
+        "US",
+        "EU",
     }
 )
 
 # https://cloud.google.com/storage/docs/regional-endpoints
 REP_ENABLED_BIGQUERY_LOCATIONS = frozenset(
     {
         "me-central2",
```

### Comparing `bigframes-1.4.0/bigframes/core/__init__.py` & `bigframes-1.5.0/bigframes/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,18 @@
         col_ids: typing.Sequence[str],
     ) -> ArrayValue:
         """Create an ArrayValue from a list of label tuples."""
         rows = []
         for row_offset in range(len(former_column_labels)):
             row_label = former_column_labels[row_offset]
             row_label = (row_label,) if not isinstance(row_label, tuple) else row_label
-            row = {col_ids[i]: row_label[i] for i in range(len(col_ids))}
+            row = {
+                col_ids[i]: (row_label[i] if pandas.notnull(row_label[i]) else None)
+                for i in range(len(col_ids))
+            }
             rows.append(row)
 
         return ArrayValue.from_pyarrow(pa.Table.from_pylist(rows), session=self.session)
 
     def join(
         self,
         other: ArrayValue,
```

### Comparing `bigframes-1.4.0/bigframes/core/block_transforms.py` & `bigframes-1.5.0/bigframes/core/block_transforms.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/blocks.py` & `bigframes-1.5.0/bigframes/core/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,18 +112,28 @@
         index_columns = list(index_columns)
         if index_labels is not None:
             index_labels = list(index_labels)
             if len(index_labels) != len(index_columns):
                 raise ValueError(
                     f"'index_columns' (size {len(index_columns)}) and 'index_labels' (size {len(index_labels)}) must have equal length"
                 )
+
+        # If no index columns are set, create one.
+        #
+        # Note: get_index_cols_and_uniqueness in
+        # bigframes/session/_io/bigquery/read_gbq_table.py depends on this
+        # being as sequential integer index column. If this default behavior
+        # ever changes, please also update get_index_cols_and_uniqueness so
+        # that users who explicitly request a sequential integer index can
+        # still get one.
         if len(index_columns) == 0:
             new_index_col_id = guid.generate_guid()
             expr = expr.promote_offsets(new_index_col_id)
             index_columns = [new_index_col_id]
+
         self._index_columns = tuple(index_columns)
         # Index labels don't need complicated hierarchical access so can store as tuple
         self._index_labels = (
             tuple(index_labels)
             if index_labels
             else tuple([None for _ in index_columns])
         )
```

### Comparing `bigframes-1.4.0/bigframes/core/compile/__init__.py` & `bigframes-1.5.0/bigframes/core/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/aggregate_compiler.py` & `bigframes-1.5.0/bigframes/core/compile/aggregate_compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/compiled.py` & `bigframes-1.5.0/bigframes/core/compile/compiled.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/compiler.py` & `bigframes-1.5.0/bigframes/core/compile/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/concat.py` & `bigframes-1.5.0/bigframes/core/compile/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/scalar_op_compiler.py` & `bigframes-1.5.0/bigframes/core/compile/scalar_op_compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/compile/single_column.py` & `bigframes-1.5.0/bigframes/core/compile/single_column.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/convert.py` & `bigframes-1.5.0/bigframes/core/convert.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/eval.py` & `bigframes-1.5.0/bigframes/core/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/expression.py` & `bigframes-1.5.0/bigframes/core/expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/groupby/__init__.py` & `bigframes-1.5.0/bigframes/core/groupby/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/guid.py` & `bigframes-1.5.0/bigframes/core/guid.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/indexers.py` & `bigframes-1.5.0/bigframes/core/indexers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/indexes/__init__.py` & `bigframes-1.5.0/bigframes/core/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/indexes/base.py` & `bigframes-1.5.0/bigframes/core/indexes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         # TODO(swast): Add a timeout here? If the query is taking a long time,
         # maybe we just print the job metadata that we have so far?
         # TODO(swast): Avoid downloading the whole series by using job
         # metadata, like we do with DataFrame.
         opts = bigframes.options.display
         max_results = opts.max_rows
         if opts.repr_mode == "deferred":
-            return formatter.repr_query_job(self.query_job)
+            return formatter.repr_query_job(self._block._compute_dry_run())
 
         pandas_df, _, query_job = self._block.retrieve_repr_request_results(max_results)
         self._query_job = query_job
         return repr(pandas_df.index)
 
     def copy(self, name: Optional[Hashable] = None):
         copy_index = Index(self._block)
```

### Comparing `bigframes-1.4.0/bigframes/core/indexes/multi.py` & `bigframes-1.5.0/bigframes/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/join_def.py` & `bigframes-1.5.0/bigframes/core/join_def.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/joins/__init__.py` & `bigframes-1.5.0/bigframes/core/joins/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/joins/merge.py` & `bigframes-1.5.0/bigframes/core/joins/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/local_data.py` & `bigframes-1.5.0/bigframes/core/local_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/log_adapter.py` & `bigframes-1.5.0/bigframes/core/log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/nodes.py` & `bigframes-1.5.0/bigframes/core/nodes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/ordering.py` & `bigframes-1.5.0/bigframes/core/ordering.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/reshape/__init__.py` & `bigframes-1.5.0/bigframes/core/reshape/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/rewrite.py` & `bigframes-1.5.0/bigframes/core/rewrite.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/scalar.py` & `bigframes-1.5.0/bigframes/core/scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/schema.py` & `bigframes-1.5.0/bigframes/core/schema.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/tools/__init__.py` & `bigframes-1.5.0/bigframes/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/tools/datetimes.py` & `bigframes-1.5.0/bigframes/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/tree_properties.py` & `bigframes-1.5.0/bigframes/core/tree_properties.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/utils.py` & `bigframes-1.5.0/bigframes/core/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/window/__init__.py` & `bigframes-1.5.0/bigframes/core/window/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/core/window_spec.py` & `bigframes-1.5.0/bigframes/core/window_spec.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/dataframe.py` & `bigframes-1.5.0/bigframes/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
         """Converts a DataFrame to a string. Calls to_pandas.
 
         Only represents the first `bigframes.options.display.max_rows`.
         """
         opts = bigframes.options.display
         max_results = opts.max_rows
         if opts.repr_mode == "deferred":
-            return formatter.repr_query_job(self.query_job)
+            return formatter.repr_query_job(self._compute_dry_run())
 
         self._cached()
         # TODO(swast): pass max_columns and get the true column count back. Maybe
         # get 1 more column than we have requested so that pandas can add the
         # ... for us?
         pandas_df, row_count, query_job = self._block.retrieve_repr_request_results(
             max_results
@@ -628,17 +628,17 @@
     def _repr_html_(self) -> str:
         """
         Returns an html string primarily for use by notebooks for displaying
         a representation of the DataFrame. Displays 20 rows by default since
         many notebooks are not configured for large tables.
         """
         opts = bigframes.options.display
-        max_results = bigframes.options.display.max_rows
+        max_results = opts.max_rows
         if opts.repr_mode == "deferred":
-            return formatter.repr_query_job_html(self.query_job)
+            return formatter.repr_query_job(self._compute_dry_run())
 
         self._cached()
         # TODO(swast): pass max_columns and get the true column count back. Maybe
         # get 1 more column than we have requested so that pandas can add the
         # ... for us?
         pandas_df, row_count, query_job = self._block.retrieve_repr_request_results(
             max_results
@@ -2924,16 +2924,18 @@
                 raise ValueError(
                     f"Got invalid value {repr(if_exists)} for if_exists. "
                     "When no destination table is specified, a new table is always created. "
                     "None or 'replace' are the only valid options in this case."
                 )
             if_exists = "replace"
 
-            temp_table_ref = bigframes.session._io.bigquery.random_table(
-                self._session._anonymous_dataset
+            temp_table_ref = self._session._random_table(
+                # The client code owns this table reference now, so skip_cleanup=True
+                #  to not clean it up when we close the session.
+                skip_cleanup=True,
             )
             destination_table = f"{temp_table_ref.project}.{temp_table_ref.dataset_id}.{temp_table_ref.table_id}"
 
         table_parts = destination_table.split(".")
         default_project = self._block.expr.session.bqclient.project
 
         if len(table_parts) == 2:
```

### Comparing `bigframes-1.4.0/bigframes/dtypes.py` & `bigframes-1.5.0/bigframes/dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/exceptions.py` & `bigframes-1.5.0/bigframes/session/_io/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-
-class UnknownLocationWarning(Warning):
-    """The location is set to an unknown value."""
```

### Comparing `bigframes-1.4.0/bigframes/features.py` & `bigframes-1.5.0/bigframes/features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/formatting_helpers.py` & `bigframes-1.5.0/bigframes/formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/functions/__init__.py` & `bigframes-1.5.0/bigframes/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/functions/remote_function.py` & `bigframes-1.5.0/bigframes/functions/remote_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,20 @@
             f.write("\n".join(requirements))
 
         # main.py
         entry_point = self.generate_cloud_function_main_code(def_, dir)
         return entry_point
 
     def create_cloud_function(
-        self, def_, cf_name, package_requirements=None, cloud_function_timeout=600
+        self,
+        def_,
+        cf_name,
+        package_requirements=None,
+        timeout_seconds=600,
+        max_instance_count=None,
     ):
         """Create a cloud function from the given user defined function."""
 
         # Build and deploy folder structure containing cloud function
         with tempfile.TemporaryDirectory() as dir:
             entry_point = self.generate_cloud_function_code(
                 def_, dir, package_requirements
@@ -407,22 +412,24 @@
                 upload_url_response.storage_source.object_
             )
             function.build_config.docker_repository = (
                 self._cloud_function_docker_repository
             )
             function.service_config = functions_v2.ServiceConfig()
             function.service_config.available_memory = "1024M"
-            if cloud_function_timeout is not None:
-                if cloud_function_timeout > 1200:
+            if timeout_seconds is not None:
+                if timeout_seconds > 1200:
                     raise ValueError(
                         "BigQuery remote function can wait only up to 20 minutes"
                         ", see for more details "
                         "https://cloud.google.com/bigquery/quotas#remote_function_limits."
                     )
-                function.service_config.timeout_seconds = cloud_function_timeout
+                function.service_config.timeout_seconds = timeout_seconds
+            if max_instance_count is not None:
+                function.service_config.max_instance_count = max_instance_count
             function.service_config.service_account_email = (
                 self._cloud_function_service_account
             )
             function.kms_key_name = self._cloud_function_kms_key_name
             create_function_request.function = function
 
             # Create the cloud function and wait for it to be ready to use
@@ -462,14 +469,15 @@
         input_types,
         output_type,
         reuse,
         name,
         package_requirements,
         max_batching_rows,
         cloud_function_timeout,
+        cloud_function_max_instance_count,
     ):
         """Provision a BigQuery remote function."""
         # If reuse of any existing function with the same name (indicated by the
         # same hash of its source code) is not intended, then attach a unique
         # suffix to the intended function name to make it unique.
         uniq_suffix = None
         if not reuse:
@@ -483,15 +491,19 @@
             def_, uniq_suffix, package_requirements
         )
         cf_endpoint = self.get_cloud_function_endpoint(cloud_function_name)
 
         # Create the cloud function if it does not exist
         if not cf_endpoint:
             cf_endpoint = self.create_cloud_function(
-                def_, cloud_function_name, package_requirements, cloud_function_timeout
+                def_,
+                cloud_function_name,
+                package_requirements,
+                cloud_function_timeout,
+                cloud_function_max_instance_count,
             )
         else:
             logger.info(f"Cloud function {cloud_function_name} already exists.")
 
         # Derive the name of the remote function
         remote_function_name = name
         if not remote_function_name:
@@ -638,14 +650,15 @@
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
     max_batching_rows: Optional[int] = 1000,
     cloud_function_timeout: Optional[int] = 600,
+    cloud_function_max_instances: Optional[int] = None,
 ):
     """Decorator to turn a user defined function into a BigQuery remote function.
 
     .. deprecated:: 0.0.1
        This is an internal method. Please use :func:`bigframes.pandas.remote_function` instead.
 
     .. note::
@@ -774,14 +787,22 @@
             https://cloud.google.com/functions/docs/configuring/timeout.
             Please note that even though the cloud function (2nd gen) itself
             allows seeting up to 60 minutes of timeout, BigQuery remote
             function can wait only up to 20 minutes, see for more details
             https://cloud.google.com/bigquery/quotas#remote_function_limits.
             By default BigQuery DataFrames uses a 10 minute timeout. `None`
             can be passed to let the cloud functions default timeout take effect.
+        cloud_function_max_instances (int, Optional):
+            The maximumm instance count for the cloud function created. This
+            can be used to control how many cloud function instances can be
+            active at max at any given point of time. Lower setting can help
+            control the spike in the billing. Higher setting can help
+            support processing larger scale data. When not specified, cloud
+            function's default setting applies. For more details see
+            https://cloud.google.com/functions/docs/configuring/max-instances
     """
     if isinstance(input_types, type):
         input_types = [input_types]
 
     import bigframes.pandas as bpd
 
     session = session or bpd.get_global_session()
@@ -902,14 +923,15 @@
             ibis_signature.input_types,
             ibis_signature.output_type,
             reuse,
             name,
             packages,
             max_batching_rows,
             cloud_function_timeout,
+            cloud_function_max_instances,
         )
 
         # TODO: Move ibis logic to compiler step
         node = ibis.udf.scalar.builtin(
             f,
             name=rf_name,
             schema=f"{dataset_ref.project}.{dataset_ref.dataset_id}",
```

### Comparing `bigframes-1.4.0/bigframes/ml/__init__.py` & `bigframes-1.5.0/bigframes/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/base.py` & `bigframes-1.5.0/bigframes/ml/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/cluster.py` & `bigframes-1.5.0/bigframes/ml/cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/compose.py` & `bigframes-1.5.0/bigframes/ml/compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/core.py` & `bigframes-1.5.0/bigframes/ml/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,19 @@
     def arima_evaluate(self, show_all_candidate_models: bool = False):
         sql = self._model_manipulation_sql_generator.ml_arima_evaluate(
             show_all_candidate_models
         )
 
         return self._session.read_gbq(sql)
 
+    def arima_coefficients(self) -> bpd.DataFrame:
+        sql = self._model_manipulation_sql_generator.ml_arima_coefficients()
+
+        return self._session.read_gbq(sql)
+
     def centroids(self) -> bpd.DataFrame:
         assert self._model.model_type == "KMEANS"
 
         sql = self._model_manipulation_sql_generator.ml_centroids()
 
         return self._session.read_gbq(
             sql, index_col=["centroid_id", "feature"]
```

### Comparing `bigframes-1.4.0/bigframes/ml/decomposition.py` & `bigframes-1.5.0/bigframes/ml/decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/ensemble.py` & `bigframes-1.5.0/bigframes/ml/ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/forecasting.py` & `bigframes-1.5.0/bigframes/ml/forecasting.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,35 @@
         if not self._bqml_model:
             raise RuntimeError("A model must be fitted before predict")
 
         return self._bqml_model.forecast(
             options={"horizon": horizon, "confidence_level": confidence_level}
         )
 
+    @property
+    def coef_(
+        self,
+    ) -> bpd.DataFrame:
+        """Inspect the coefficients of the model.
+
+        ..note::
+
+            Output matches that of the ML.ARIMA_COEFFICIENTS function.
+            See: https://cloud.google.com/bigquery/docs/reference/standard-sql/bigqueryml-syntax-arima-coefficients
+            for the outputs relevant to this model type.
+
+        Returns:
+            bigframes.dataframe.DataFrame:
+                A DataFrame with the coefficients for the model.
+        """
+
+        if not self._bqml_model:
+            raise RuntimeError("A model must be fitted before inspect coefficients")
+        return self._bqml_model.arima_coefficients()
+
     def detect_anomalies(
         self,
         X: Union[bpd.DataFrame, bpd.Series],
         *,
         anomaly_prob_threshold: float = 0.95,
     ) -> bpd.DataFrame:
         """Detect the anomaly data points of the input.
```

### Comparing `bigframes-1.4.0/bigframes/ml/globals.py` & `bigframes-1.5.0/bigframes/ml/globals.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/imported.py` & `bigframes-1.5.0/bigframes/ml/imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/linear_model.py` & `bigframes-1.5.0/bigframes/ml/linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/llm.py` & `bigframes-1.5.0/bigframes/ml/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         model_connection = model._properties["remoteModelInfo"]["connection"]
         model_endpoint = bqml_endpoint.split("/")[-1]
 
         # Get the optional params
         kwargs: dict = {}
         last_fitting = model.training_runs[-1]["trainingOptions"]
 
-        dummy_text_generator = cls()
+        dummy_text_generator = cls(session=session)
         for bf_param, _ in dummy_text_generator.__dict__.items():
             bqml_param = _BQML_PARAMS_MAPPING.get(bf_param)
             if bqml_param in last_fitting:
                 # Convert types
                 if bf_param in ["max_iterations"]:
                     kwargs[bf_param] = int(last_fitting[bqml_param])
 
@@ -229,15 +229,15 @@
                 while higher temperatures can lead to more diverse or unexpected results. A temperature of 0 is deterministic:
                 the highest probability token is always selected. For most use cases, try starting with a temperature of 0.2.
                 Default 0. Possible values [0.0, 1.0].
 
             max_output_tokens (int, default 128):
                 Maximum number of tokens that can be generated in the response. Specify a lower value for shorter responses and a higher value for longer responses.
                 A token may be smaller than a word. A token is approximately four characters. 100 tokens correspond to roughly 60-80 words.
-                Default 128. For the 'text-bison' model, possible values are in the range [1, 1024]. For the 'text-bison-32k' model, possible values are in the range [1, 8196].
+                Default 128. For the 'text-bison' model, possible values are in the range [1, 1024]. For the 'text-bison-32k' model, possible values are in the range [1, 8192].
                 Please ensure that the specified value for max_output_tokens is within the appropriate range for the model being used.
 
             top_k (int, default 40):
                 Top-k changes how the model selects tokens for output. A top-k of 1 means the selected token is the most probable among all tokens
                 in the model's vocabulary (also called greedy decoding), while a top-k of 3 means that the next token is selected from among the 3 most probable tokens (using temperature).
                 For each token selection step, the top K tokens with the highest probabilities are sampled. Then tokens are further filtered based on topP with the final token selected using temperature sampling.
                 Specify a lower value for less random responses and a higher value for more random responses.
@@ -265,18 +265,18 @@
         ):
             raise ValueError(
                 f"max_output_token must be [1, 1024] for TextBison model, but is {max_output_tokens}."
             )
 
         if (
             self.model_name == _TEXT_GENERATOR_BISON_32K_ENDPOINT
-            and max_output_tokens not in range(1, 8197)
+            and max_output_tokens not in range(1, 8193)
         ):
             raise ValueError(
-                f"max_output_token must be [1, 8196] for TextBison 32k model, but is {max_output_tokens}."
+                f"max_output_token must be [1, 8192] for TextBison 32k model, but is {max_output_tokens}."
             )
 
         if top_k not in range(1, 41):
             raise ValueError(f"top_k must be [1, 40], but is {top_k}.")
 
         if top_p < 0.0 or top_p > 1.0:
             raise ValueError(f"top_p must be [0.0, 1.0], but is {top_p}.")
```

### Comparing `bigframes-1.4.0/bigframes/ml/loader.py` & `bigframes-1.5.0/bigframes/ml/loader.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/metrics/__init__.py` & `bigframes-1.5.0/bigframes/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/metrics/_metrics.py` & `bigframes-1.5.0/bigframes/ml/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/metrics/pairwise.py` & `bigframes-1.5.0/bigframes/ml/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/model_selection.py` & `bigframes-1.5.0/bigframes/ml/model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/pipeline.py` & `bigframes-1.5.0/bigframes/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/preprocessing.py` & `bigframes-1.5.0/bigframes/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/remote.py` & `bigframes-1.5.0/bigframes/ml/remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/ml/sql.py` & `bigframes-1.5.0/bigframes/ml/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,18 @@
 
         if source_sql is None:
             return f"""SELECT * FROM ML.EVALUATE(MODEL `{self._model_name}`)"""
         else:
             return f"""SELECT * FROM ML.EVALUATE(MODEL `{self._model_name}`,
   ({source_sql}))"""
 
+    def ml_arima_coefficients(self) -> str:
+        """Encode ML.ARIMA_COEFFICIENTS for BQML"""
+        return f"""SELECT * FROM ML.ARIMA_COEFFICIENTS(MODEL `{self._model_name}`)"""
+
     # ML evaluation TVFs
     def ml_llm_evaluate(
         self, source_df: bpd.DataFrame, task_type: Optional[str] = None
     ) -> str:
         """Encode ML.EVALUATE for BQML"""
         # Note: don't need index as evaluate returns a new table
         source_sql, _, _ = source_df._to_sql_query(include_index=False)
```

### Comparing `bigframes-1.4.0/bigframes/ml/utils.py` & `bigframes-1.5.0/bigframes/ml/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/__init__.py` & `bigframes-1.5.0/bigframes/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/_matplotlib/__init__.py` & `bigframes-1.5.0/bigframes/operations/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/_matplotlib/core.py` & `bigframes-1.5.0/bigframes/operations/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/_matplotlib/hist.py` & `bigframes-1.5.0/bigframes/operations/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/aggregations.py` & `bigframes-1.5.0/bigframes/operations/aggregations.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/base.py` & `bigframes-1.5.0/bigframes/operations/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/datetimes.py` & `bigframes-1.5.0/bigframes/operations/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/plotting.py` & `bigframes-1.5.0/bigframes/operations/plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/strings.py` & `bigframes-1.5.0/bigframes/operations/strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/structs.py` & `bigframes-1.5.0/bigframes/operations/structs.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/operations/type.py` & `bigframes-1.5.0/bigframes/operations/type.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/pandas/__init__.py` & `bigframes-1.5.0/bigframes/pandas/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 import bigframes.core.expression as ex
 import bigframes.core.global_session as global_session
 import bigframes.core.indexes
 import bigframes.core.joins
 import bigframes.core.reshape
 import bigframes.core.tools
 import bigframes.dataframe
+import bigframes.enums
 import bigframes.operations as ops
 import bigframes.series
 import bigframes.session
 import bigframes.session.clients
 
 
 # Include method definition so that the method appears in our docs for
@@ -419,15 +420,21 @@
     *,
     sep: Optional[str] = ",",
     header: Optional[int] = 0,
     names: Optional[
         Union[MutableSequence[Any], numpy.ndarray[Any, Any], Tuple[Any, ...], range]
     ] = None,
     index_col: Optional[
-        Union[int, str, Sequence[Union[str, int]], Literal[False]]
+        Union[
+            int,
+            str,
+            Sequence[Union[str, int]],
+            bigframes.enums.DefaultIndexKind,
+            Literal[False],
+        ]
     ] = None,
     usecols: Optional[
         Union[
             MutableSequence[str],
             Tuple[str, ...],
             Sequence[int],
             pandas.Series,
@@ -487,15 +494,15 @@
 
 read_json.__doc__ = inspect.getdoc(bigframes.session.Session.read_json)
 
 
 def read_gbq(
     query_or_table: str,
     *,
-    index_col: Iterable[str] | str = (),
+    index_col: Iterable[str] | str | bigframes.enums.DefaultIndexKind = (),
     columns: Iterable[str] = (),
     configuration: Optional[Dict] = None,
     max_results: Optional[int] = None,
     filters: vendored_pandas_gbq.FiltersType = (),
     use_cache: Optional[bool] = None,
     col_order: Iterable[str] = (),
 ) -> bigframes.dataframe.DataFrame:
@@ -525,15 +532,15 @@
 
 read_gbq_model.__doc__ = inspect.getdoc(bigframes.session.Session.read_gbq_model)
 
 
 def read_gbq_query(
     query: str,
     *,
-    index_col: Iterable[str] | str = (),
+    index_col: Iterable[str] | str | bigframes.enums.DefaultIndexKind = (),
     columns: Iterable[str] = (),
     configuration: Optional[Dict] = None,
     max_results: Optional[int] = None,
     use_cache: Optional[bool] = None,
     col_order: Iterable[str] = (),
 ) -> bigframes.dataframe.DataFrame:
     _set_default_session_location_if_possible(query)
@@ -551,15 +558,15 @@
 
 read_gbq_query.__doc__ = inspect.getdoc(bigframes.session.Session.read_gbq_query)
 
 
 def read_gbq_table(
     query: str,
     *,
-    index_col: Iterable[str] | str = (),
+    index_col: Iterable[str] | str | bigframes.enums.DefaultIndexKind = (),
     columns: Iterable[str] = (),
     max_results: Optional[int] = None,
     filters: vendored_pandas_gbq.FiltersType = (),
     use_cache: bool = True,
     col_order: Iterable[str] = (),
 ) -> bigframes.dataframe.DataFrame:
     _set_default_session_location_if_possible(query)
@@ -641,14 +648,15 @@
     name: Optional[str] = None,
     packages: Optional[Sequence[str]] = None,
     cloud_function_service_account: Optional[str] = None,
     cloud_function_kms_key_name: Optional[str] = None,
     cloud_function_docker_repository: Optional[str] = None,
     max_batching_rows: Optional[int] = 1000,
     cloud_function_timeout: Optional[int] = 600,
+    cloud_function_max_instances: Optional[int] = None,
 ):
     return global_session.with_default_session(
         bigframes.session.Session.remote_function,
         input_types=input_types,
         output_type=output_type,
         dataset=dataset,
         bigquery_connection=bigquery_connection,
@@ -656,14 +664,15 @@
         name=name,
         packages=packages,
         cloud_function_service_account=cloud_function_service_account,
         cloud_function_kms_key_name=cloud_function_kms_key_name,
         cloud_function_docker_repository=cloud_function_docker_repository,
         max_batching_rows=max_batching_rows,
         cloud_function_timeout=cloud_function_timeout,
+        cloud_function_max_instances=cloud_function_max_instances,
     )
 
 
 remote_function.__doc__ = inspect.getdoc(bigframes.session.Session.remote_function)
 
 
 def read_gbq_function(function_name: str):
@@ -695,14 +704,76 @@
         unit=unit,
     )
 
 
 to_datetime.__doc__ = vendored_pandas_datetimes.to_datetime.__doc__
 
 
+def get_default_session_id() -> str:
+    """Gets the session id that is used whenever a custom session
+    has not been provided.
+
+    It is the session id of the default global session. It is prefixed to
+    the table id of all temporary tables created in the global session.
+
+    Returns:
+        str, the default global session id, ex. 'sessiona1b2c'
+    """
+    return get_global_session().session_id
+
+
+def clean_up_by_session_id(
+    session_id: str,
+    location: Optional[str] = None,
+    project: Optional[str] = None,
+) -> None:
+    """Searches through table names in BigQuery and deletes tables
+    found matching the expected format.
+
+    This could be useful if the session object has been lost.
+    Calling `session.close()` or `bigframes.pandas.close_session()`
+    is preferred in most cases.
+
+    Args:
+        session_id (str):
+            The session id to clean up. Can be found using
+            session.session_id or get_default_session_id().
+
+        location (str, default None):
+            The location of the session to clean up. If given, used
+            together with project kwarg to determine the dataset
+            to search through for tables to clean up.
+
+        project (str, default None):
+            The project id associated with the session to clean up.
+            If given, used together with location kwarg to determine
+            the dataset to search through for tables to clean up.
+
+    Returns:
+        None
+    """
+    session = get_global_session()
+    client = session.bqclient
+
+    if (location is None) != (project is None):
+        raise ValueError(
+            "Only one of project or location was given. Must specify both or neither."
+        )
+    elif location is None and project is None:
+        dataset = session._anonymous_dataset
+    else:
+        dataset = bigframes.session._io.bigquery.create_bq_dataset_reference(
+            client, location=location, project=project
+        )
+
+    bigframes.session._io.bigquery.delete_tables_matching_session_id(
+        client, dataset, session_id
+    )
+
+
 # pandas dtype attributes
 NA = pandas.NA
 BooleanDtype = pandas.BooleanDtype
 Float64Dtype = pandas.Float64Dtype
 Int64Dtype = pandas.Int64Dtype
 StringDtype = pandas.StringDtype
 ArrowDtype = pandas.ArrowDtype
```

### Comparing `bigframes-1.4.0/bigframes/series.py` & `bigframes-1.5.0/bigframes/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         # TODO(swast): Add a timeout here? If the query is taking a long time,
         # maybe we just print the job metadata that we have so far?
         # TODO(swast): Avoid downloading the whole series by using job
         # metadata, like we do with DataFrame.
         opts = bigframes.options.display
         max_results = opts.max_rows
         if opts.repr_mode == "deferred":
-            return formatter.repr_query_job(self.query_job)
+            return formatter.repr_query_job(self._compute_dry_run())
 
         self._cached()
         pandas_df, _, query_job = self._block.retrieve_repr_request_results(max_results)
         self._set_internal_query_job(query_job)
 
         return repr(pandas_df.iloc[:, 0])
```

### Comparing `bigframes-1.4.0/bigframes/session/__init__.py` & `bigframes-1.5.0/bigframes/session/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,5156 +37,5016 @@
 00000240: 2222 5365 7373 696f 6e20 6d61 6e61 6765  ""Session manage
 00000250: 7320 7468 6520 636f 6e6e 6563 7469 6f6e  s the connection
 00000260: 2074 6f20 4269 6751 7565 7279 2e22 2222   to BigQuery."""
 00000270: 0a0a 6672 6f6d 205f 5f66 7574 7572 655f  ..from __future_
 00000280: 5f20 696d 706f 7274 2061 6e6e 6f74 6174  _ import annotat
 00000290: 696f 6e73 0a0a 696d 706f 7274 2063 6f70  ions..import cop
 000002a0: 790a 696d 706f 7274 2064 6174 6574 696d  y.import datetim
-000002b0: 650a 696d 706f 7274 2069 7465 7274 6f6f  e.import itertoo
-000002c0: 6c73 0a69 6d70 6f72 7420 6c6f 6767 696e  ls.import loggin
-000002d0: 670a 696d 706f 7274 206f 730a 696d 706f  g.import os.impo
-000002e0: 7274 2072 650a 696d 706f 7274 2074 7970  rt re.import typ
-000002f0: 696e 670a 6672 6f6d 2074 7970 696e 6720  ing.from typing 
-00000300: 696d 706f 7274 2028 0a20 2020 2041 6e79  import (.    Any
-00000310: 2c0a 2020 2020 4361 6c6c 6162 6c65 2c0a  ,.    Callable,.
-00000320: 2020 2020 4469 6374 2c0a 2020 2020 494f      Dict,.    IO
-00000330: 2c0a 2020 2020 4974 6572 6162 6c65 2c0a  ,.    Iterable,.
-00000340: 2020 2020 4c69 7374 2c0a 2020 2020 4c69      List,.    Li
-00000350: 7465 7261 6c2c 0a20 2020 204d 6170 7069  teral,.    Mappi
-00000360: 6e67 2c0a 2020 2020 4d75 7461 626c 6553  ng,.    MutableS
-00000370: 6571 7565 6e63 652c 0a20 2020 204f 7074  equence,.    Opt
-00000380: 696f 6e61 6c2c 0a20 2020 2053 6571 7565  ional,.    Seque
-00000390: 6e63 652c 0a20 2020 2054 7570 6c65 2c0a  nce,.    Tuple,.
-000003a0: 2020 2020 556e 696f 6e2c 0a29 0a69 6d70      Union,.).imp
-000003b0: 6f72 7420 7761 726e 696e 6773 0a0a 2320  ort warnings..# 
-000003c0: 4576 656e 2074 686f 7567 6820 7468 6520  Even though the 
-000003d0: 6962 6973 2e62 6163 6b65 6e64 732e 6269  ibis.backends.bi
-000003e0: 6771 7565 7279 2069 6d70 6f72 7420 6973  gquery import is
-000003f0: 2075 6e75 7365 642c 2069 7427 7320 6e65   unused, it's ne
-00000400: 6564 6564 0a23 2074 6f20 7265 6769 7374  eded.# to regist
-00000410: 6572 206e 6577 2061 6e64 2072 6570 6c61  er new and repla
-00000420: 6365 6d65 6e74 206f 7073 2077 6974 6820  cement ops with 
-00000430: 7468 6520 4962 6973 2042 6967 5175 6572  the Ibis BigQuer
-00000440: 7920 6261 636b 656e 642e 0a69 6d70 6f72  y backend..impor
-00000450: 7420 6269 6766 7261 6d65 735f 7665 6e64  t bigframes_vend
-00000460: 6f72 6564 2e69 6269 732e 6261 636b 656e  ored.ibis.backen
-00000470: 6473 2e62 6967 7175 6572 7920 2023 206e  ds.bigquery  # n
-00000480: 6f71 610a 696d 706f 7274 2062 6967 6672  oqa.import bigfr
-00000490: 616d 6573 5f76 656e 646f 7265 642e 6962  ames_vendored.ib
-000004a0: 6973 2e65 7870 722e 6f70 6572 6174 696f  is.expr.operatio
-000004b0: 6e73 2061 7320 7665 6e64 6f72 6564 5f69  ns as vendored_i
-000004c0: 6269 735f 6f70 730a 696d 706f 7274 2062  bis_ops.import b
-000004d0: 6967 6672 616d 6573 5f76 656e 646f 7265  igframes_vendore
-000004e0: 642e 7061 6e64 6173 2e69 6f2e 6762 7120  d.pandas.io.gbq 
-000004f0: 6173 2074 6869 7264 5f70 6172 7479 5f70  as third_party_p
-00000500: 616e 6461 735f 6762 710a 696d 706f 7274  andas_gbq.import
-00000510: 2062 6967 6672 616d 6573 5f76 656e 646f   bigframes_vendo
-00000520: 7265 642e 7061 6e64 6173 2e69 6f2e 7061  red.pandas.io.pa
-00000530: 7271 7565 7420 6173 2074 6869 7264 5f70  rquet as third_p
-00000540: 6172 7479 5f70 616e 6461 735f 7061 7271  arty_pandas_parq
-00000550: 7565 740a 696d 706f 7274 2062 6967 6672  uet.import bigfr
-00000560: 616d 6573 5f76 656e 646f 7265 642e 7061  ames_vendored.pa
-00000570: 6e64 6173 2e69 6f2e 7061 7273 6572 732e  ndas.io.parsers.
-00000580: 7265 6164 6572 7320 6173 2074 6869 7264  readers as third
-00000590: 5f70 6172 7479 5f70 616e 6461 735f 7265  _party_pandas_re
-000005a0: 6164 6572 730a 696d 706f 7274 2062 6967  aders.import big
-000005b0: 6672 616d 6573 5f76 656e 646f 7265 642e  frames_vendored.
-000005c0: 7061 6e64 6173 2e69 6f2e 7069 636b 6c65  pandas.io.pickle
-000005d0: 2061 7320 7468 6972 645f 7061 7274 795f   as third_party_
-000005e0: 7061 6e64 6173 5f70 6963 6b6c 650a 696d  pandas_pickle.im
-000005f0: 706f 7274 2067 6f6f 676c 652e 6170 695f  port google.api_
-00000600: 636f 7265 2e63 6c69 656e 745f 696e 666f  core.client_info
-00000610: 0a69 6d70 6f72 7420 676f 6f67 6c65 2e61  .import google.a
-00000620: 7069 5f63 6f72 652e 636c 6965 6e74 5f6f  pi_core.client_o
-00000630: 7074 696f 6e73 0a69 6d70 6f72 7420 676f  ptions.import go
-00000640: 6f67 6c65 2e61 7069 5f63 6f72 652e 6578  ogle.api_core.ex
-00000650: 6365 7074 696f 6e73 0a69 6d70 6f72 7420  ceptions.import 
-00000660: 676f 6f67 6c65 2e61 7069 5f63 6f72 652e  google.api_core.
-00000670: 6761 7069 635f 7631 2e63 6c69 656e 745f  gapic_v1.client_
-00000680: 696e 666f 0a69 6d70 6f72 7420 676f 6f67  info.import goog
-00000690: 6c65 2e61 7574 682e 6372 6564 656e 7469  le.auth.credenti
-000006a0: 616c 730a 696d 706f 7274 2067 6f6f 676c  als.import googl
-000006b0: 652e 636c 6f75 642e 6269 6771 7565 7279  e.cloud.bigquery
-000006c0: 2061 7320 6269 6771 7565 7279 0a69 6d70   as bigquery.imp
-000006d0: 6f72 7420 676f 6f67 6c65 2e63 6c6f 7564  ort google.cloud
-000006e0: 2e62 6967 7175 6572 792e 7461 626c 650a  .bigquery.table.
-000006f0: 696d 706f 7274 2067 6f6f 676c 652e 636c  import google.cl
-00000700: 6f75 642e 6269 6771 7565 7279 5f63 6f6e  oud.bigquery_con
-00000710: 6e65 6374 696f 6e5f 7631 0a69 6d70 6f72  nection_v1.impor
-00000720: 7420 676f 6f67 6c65 2e63 6c6f 7564 2e62  t google.cloud.b
-00000730: 6967 7175 6572 795f 7374 6f72 6167 655f  igquery_storage_
-00000740: 7631 0a69 6d70 6f72 7420 676f 6f67 6c65  v1.import google
-00000750: 2e63 6c6f 7564 2e66 756e 6374 696f 6e73  .cloud.functions
-00000760: 5f76 320a 696d 706f 7274 2067 6f6f 676c  _v2.import googl
-00000770: 652e 636c 6f75 642e 7265 736f 7572 6365  e.cloud.resource
-00000780: 6d61 6e61 6765 725f 7633 0a69 6d70 6f72  manager_v3.impor
-00000790: 7420 676f 6f67 6c65 2e63 6c6f 7564 2e73  t google.cloud.s
-000007a0: 746f 7261 6765 2061 7320 7374 6f72 6167  torage as storag
-000007b0: 6520 2023 2074 7970 653a 2069 676e 6f72  e  # type: ignor
-000007c0: 650a 696d 706f 7274 2069 6269 730a 696d  e.import ibis.im
-000007d0: 706f 7274 2069 6269 732e 6261 636b 656e  port ibis.backen
-000007e0: 6473 2e62 6967 7175 6572 7920 6173 2069  ds.bigquery as i
-000007f0: 6269 735f 6269 6771 7565 7279 0a69 6d70  bis_bigquery.imp
-00000800: 6f72 7420 6962 6973 2e65 7870 722e 6461  ort ibis.expr.da
-00000810: 7461 7479 7065 7320 6173 2069 6269 735f  tatypes as ibis_
-00000820: 6474 7970 6573 0a69 6d70 6f72 7420 6962  dtypes.import ib
-00000830: 6973 2e65 7870 722e 7479 7065 7320 6173  is.expr.types as
-00000840: 2069 6269 735f 7479 7065 730a 696d 706f   ibis_types.impo
-00000850: 7274 206e 756d 7079 2061 7320 6e70 0a69  rt numpy as np.i
-00000860: 6d70 6f72 7420 7061 6e64 6173 0a66 726f  mport pandas.fro
-00000870: 6d20 7061 6e64 6173 2e5f 7479 7069 6e67  m pandas._typing
-00000880: 2069 6d70 6f72 7420 280a 2020 2020 436f   import (.    Co
-00000890: 6d70 7265 7373 696f 6e4f 7074 696f 6e73  mpressionOptions
-000008a0: 2c0a 2020 2020 4669 6c65 5061 7468 2c0a  ,.    FilePath,.
-000008b0: 2020 2020 5265 6164 5069 636b 6c65 4275      ReadPickleBu
-000008c0: 6666 6572 2c0a 2020 2020 5374 6f72 6167  ffer,.    Storag
-000008d0: 654f 7074 696f 6e73 2c0a 290a 696d 706f  eOptions,.).impo
-000008e0: 7274 2070 7961 7272 6f77 2061 7320 7061  rt pyarrow as pa
-000008f0: 0a0a 696d 706f 7274 2062 6967 6672 616d  ..import bigfram
-00000900: 6573 2e5f 636f 6e66 6967 2e62 6967 7175  es._config.bigqu
-00000910: 6572 795f 6f70 7469 6f6e 7320 6173 2062  ery_options as b
-00000920: 6967 7175 6572 795f 6f70 7469 6f6e 730a  igquery_options.
-00000930: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
-00000940: 2e63 6c69 656e 7473 0a69 6d70 6f72 7420  .clients.import 
-00000950: 6269 6766 7261 6d65 732e 636f 6e73 7461  bigframes.consta
-00000960: 6e74 7320 6173 2063 6f6e 7374 616e 7473  nts as constants
-00000970: 0a69 6d70 6f72 7420 6269 6766 7261 6d65  .import bigframe
-00000980: 732e 636f 7265 2061 7320 636f 7265 0a69  s.core as core.i
-00000990: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
-000009a0: 636f 7265 2e62 6c6f 636b 7320 6173 2062  core.blocks as b
-000009b0: 6c6f 636b 730a 696d 706f 7274 2062 6967  locks.import big
-000009c0: 6672 616d 6573 2e63 6f72 652e 636f 6d70  frames.core.comp
-000009d0: 696c 650a 696d 706f 7274 2062 6967 6672  ile.import bigfr
-000009e0: 616d 6573 2e63 6f72 652e 6775 6964 2061  ames.core.guid a
-000009f0: 7320 6775 6964 0a69 6d70 6f72 7420 6269  s guid.import bi
-00000a00: 6766 7261 6d65 732e 636f 7265 2e6e 6f64  gframes.core.nod
-00000a10: 6573 2061 7320 6e6f 6465 730a 6672 6f6d  es as nodes.from
-00000a20: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
-00000a30: 6f72 6465 7269 6e67 2069 6d70 6f72 7420  ordering import 
-00000a40: 496e 7465 6765 7245 6e63 6f64 696e 670a  IntegerEncoding.
-00000a50: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
-00000a60: 2e63 6f72 652e 6f72 6465 7269 6e67 2061  .core.ordering a
-00000a70: 7320 6f72 6465 720a 696d 706f 7274 2062  s order.import b
-00000a80: 6967 6672 616d 6573 2e63 6f72 652e 7472  igframes.core.tr
-00000a90: 6565 5f70 726f 7065 7274 6965 7320 6173  ee_properties as
-00000aa0: 2074 7261 7665 7273 616c 730a 696d 706f   traversals.impo
-00000ab0: 7274 2062 6967 6672 616d 6573 2e63 6f72  rt bigframes.cor
-00000ac0: 652e 7472 6565 5f70 726f 7065 7274 6965  e.tree_propertie
-00000ad0: 7320 6173 2074 7265 655f 7072 6f70 6572  s as tree_proper
-00000ae0: 7469 6573 0a69 6d70 6f72 7420 6269 6766  ties.import bigf
-00000af0: 7261 6d65 732e 636f 7265 2e75 7469 6c73  rames.core.utils
-00000b00: 2061 7320 7574 696c 730a 696d 706f 7274   as utils.import
-00000b10: 2062 6967 6672 616d 6573 2e64 7479 7065   bigframes.dtype
-00000b20: 730a 696d 706f 7274 2062 6967 6672 616d  s.import bigfram
-00000b30: 6573 2e66 6f72 6d61 7474 696e 675f 6865  es.formatting_he
-00000b40: 6c70 6572 7320 6173 2066 6f72 6d61 7474  lpers as formatt
-00000b50: 696e 675f 6865 6c70 6572 730a 6672 6f6d  ing_helpers.from
-00000b60: 2062 6967 6672 616d 6573 2e66 756e 6374   bigframes.funct
-00000b70: 696f 6e73 2e72 656d 6f74 655f 6675 6e63  ions.remote_func
-00000b80: 7469 6f6e 2069 6d70 6f72 7420 7265 6164  tion import read
-00000b90: 5f67 6271 5f66 756e 6374 696f 6e20 6173  _gbq_function as
-00000ba0: 2062 6967 6672 616d 6573 5f72 6766 0a66   bigframes_rgf.f
-00000bb0: 726f 6d20 6269 6766 7261 6d65 732e 6675  rom bigframes.fu
-00000bc0: 6e63 7469 6f6e 732e 7265 6d6f 7465 5f66  nctions.remote_f
-00000bd0: 756e 6374 696f 6e20 696d 706f 7274 2072  unction import r
-00000be0: 656d 6f74 655f 6675 6e63 7469 6f6e 2061  emote_function a
-00000bf0: 7320 6269 6766 7261 6d65 735f 7266 0a69  s bigframes_rf.i
-00000c00: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
-00000c10: 7365 7373 696f 6e2e 5f69 6f2e 6269 6771  session._io.bigq
-00000c20: 7565 7279 2061 7320 6269 6766 7261 6d65  uery as bigframe
-00000c30: 735f 696f 0a69 6d70 6f72 7420 6269 6766  s_io.import bigf
-00000c40: 7261 6d65 732e 7365 7373 696f 6e2e 636c  rames.session.cl
-00000c50: 6965 6e74 730a 696d 706f 7274 2062 6967  ients.import big
-00000c60: 6672 616d 6573 2e76 6572 7369 6f6e 0a0a  frames.version..
-00000c70: 2320 4176 6f69 6420 6369 7263 756c 6172  # Avoid circular
-00000c80: 2069 6d70 6f72 7473 2e0a 6966 2074 7970   imports..if typ
-00000c90: 696e 672e 5459 5045 5f43 4845 434b 494e  ing.TYPE_CHECKIN
-00000ca0: 473a 0a20 2020 2069 6d70 6f72 7420 6269  G:.    import bi
-00000cb0: 6766 7261 6d65 732e 636f 7265 2e69 6e64  gframes.core.ind
-00000cc0: 6578 6573 0a20 2020 2069 6d70 6f72 7420  exes.    import 
-00000cd0: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
-00000ce0: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
-00000cf0: 0a20 2020 2069 6d70 6f72 7420 6269 6766  .    import bigf
-00000d00: 7261 6d65 732e 7365 7269 6573 0a0a 5f42  rames.series.._B
-00000d10: 4947 4652 414d 4553 5f44 4546 4155 4c54  IGFRAMES_DEFAULT
-00000d20: 5f43 4f4e 4e45 4354 494f 4e5f 4944 203d  _CONNECTION_ID =
-00000d30: 2022 6269 6766 7261 6d65 732d 6465 6661   "bigframes-defa
-00000d40: 756c 742d 636f 6e6e 6563 7469 6f6e 220a  ult-connection".
-00000d50: 0a5f 4d41 585f 434c 5553 5445 525f 434f  ._MAX_CLUSTER_CO
-00000d60: 4c55 4d4e 5320 3d20 340a 0a23 2054 4f44  LUMNS = 4..# TOD
-00000d70: 4f28 7377 6173 7429 3a20 4e65 6564 2074  O(swast): Need t
-00000d80: 6f20 636f 6e6e 6563 7420 746f 2072 6567  o connect to reg
-00000d90: 696f 6e61 6c20 656e 6470 6f69 6e74 7320  ional endpoints 
-00000da0: 7768 656e 2070 6572 666f 726d 696e 6720  when performing 
-00000db0: 7265 6d6f 7465 0a23 2066 756e 6374 696f  remote.# functio
-00000dc0: 6e73 206f 7065 7261 7469 6f6e 7320 2842  ns operations (B
-00000dd0: 5120 436f 6e6e 6563 7469 6f6e 2049 414d  Q Connection IAM
-00000de0: 2c20 436c 6f75 6420 5275 6e20 2f20 436c  , Cloud Run / Cl
-00000df0: 6f75 6420 4675 6e63 7469 6f6e 7329 2e0a  oud Functions)..
-00000e00: 2320 416c 736f 2073 6565 2069 6620 7265  # Also see if re
-00000e10: 736f 7572 6365 206d 616e 6167 6572 2063  source manager c
-00000e20: 6c69 656e 7420 6c69 6272 6172 7920 7375  lient library su
-00000e30: 7070 6f72 7473 2072 6567 696f 6e61 6c20  pports regional 
-00000e40: 656e 6470 6f69 6e74 732e 0a0a 5f56 414c  endpoints..._VAL
-00000e50: 4944 5f45 4e43 4f44 494e 4753 203d 207b  ID_ENCODINGS = {
-00000e60: 0a20 2020 2022 5554 462d 3822 2c0a 2020  .    "UTF-8",.  
-00000e70: 2020 2249 534f 2d38 3835 392d 3122 2c0a    "ISO-8859-1",.
-00000e80: 2020 2020 2255 5446 2d31 3642 4522 2c0a      "UTF-16BE",.
-00000e90: 2020 2020 2255 5446 2d31 364c 4522 2c0a      "UTF-16LE",.
-00000ea0: 2020 2020 2255 5446 2d33 3242 4522 2c0a      "UTF-32BE",.
-00000eb0: 2020 2020 2255 5446 2d33 324c 4522 2c0a      "UTF-32LE",.
-00000ec0: 7d0a 0a23 2042 6967 5175 6572 7920 6861  }..# BigQuery ha
-00000ed0: 7320 3120 4d42 2071 7565 7279 2073 697a  s 1 MB query siz
-00000ee0: 6520 6c69 6d69 742e 2044 6f6e 2774 2077  e limit. Don't w
-00000ef0: 616e 7420 746f 2074 616b 6520 7570 206d  ant to take up m
-00000f00: 6f72 6520 7468 616e 2061 2066 6577 2025  ore than a few %
-00000f10: 206f 6620 7468 6174 2069 6e6c 696e 696e   of that inlinin
-00000f20: 6720 6120 7461 626c 652e 0a23 2041 6c73  g a table..# Als
-00000f30: 6f20 6d75 7374 2061 7373 756d 6520 7468  o must assume th
-00000f40: 6174 2074 6578 7420 656e 636f 6469 6e67  at text encoding
-00000f50: 2061 7320 6c69 7465 7261 6c73 2069 7320   as literals is 
-00000f60: 6d75 6368 206c 6573 7320 6566 6669 6369  much less effici
-00000f70: 656e 7420 7468 616e 2069 6e2d 6d65 6d6f  ent than in-memo
-00000f80: 7279 2072 6570 7265 7365 6e74 6174 696f  ry representatio
-00000f90: 6e2e 0a4d 4158 5f49 4e4c 494e 455f 4446  n..MAX_INLINE_DF
-00000fa0: 5f42 5954 4553 203d 2035 3030 300a 0a23  _BYTES = 5000..#
-00000fb0: 204d 6178 2063 6f6d 706c 6578 6974 7920   Max complexity 
-00000fc0: 7468 6174 2073 686f 756c 6420 6265 2065  that should be e
-00000fd0: 7865 6375 7465 6420 6173 2061 2073 696e  xecuted as a sin
-00000fe0: 676c 6520 7175 6572 790a 5155 4552 595f  gle query.QUERY_
-00000ff0: 434f 4d50 4c45 5849 5459 5f4c 494d 4954  COMPLEXITY_LIMIT
-00001000: 203d 2031 6537 0a23 204e 756d 6265 7220   = 1e7.# Number 
-00001010: 6f66 2074 696d 6573 2074 6f20 6661 6374  of times to fact
-00001020: 6f72 206f 7574 2073 7562 7175 6572 6965  or out subquerie
-00001030: 7320 6265 666f 7265 2067 6976 696e 6720  s before giving 
-00001040: 7570 2e0a 4d41 585f 5355 4254 5245 455f  up..MAX_SUBTREE_
-00001050: 4641 4354 4f52 494e 4753 203d 2035 0a0a  FACTORINGS = 5..
-00001060: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
-00001070: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
-00001080: 655f 5f29 0a0a 2320 4578 636c 7564 6573  e__)..# Excludes
-00001090: 2067 656f 6772 6170 6879 2c20 6279 7465   geography, byte
-000010a0: 732c 2061 6e64 206e 6573 7465 6420 2861  s, and nested (a
-000010b0: 7272 6179 2c20 7374 7275 6374 2920 6461  rray, struct) da
-000010c0: 7461 7479 7065 730a 494e 4c49 4e41 424c  tatypes.INLINABL
-000010d0: 455f 4454 5950 4553 3a20 5365 7175 656e  E_DTYPES: Sequen
-000010e0: 6365 5b62 6967 6672 616d 6573 2e64 7479  ce[bigframes.dty
-000010f0: 7065 732e 4474 7970 655d 203d 2028 0a20  pes.Dtype] = (. 
-00001100: 2020 2070 616e 6461 732e 426f 6f6c 6561     pandas.Boolea
-00001110: 6e44 7479 7065 2829 2c0a 2020 2020 7061  nDtype(),.    pa
-00001120: 6e64 6173 2e46 6c6f 6174 3634 4474 7970  ndas.Float64Dtyp
-00001130: 6528 292c 0a20 2020 2070 616e 6461 732e  e(),.    pandas.
-00001140: 496e 7436 3444 7479 7065 2829 2c0a 2020  Int64Dtype(),.  
-00001150: 2020 7061 6e64 6173 2e53 7472 696e 6744    pandas.StringD
-00001160: 7479 7065 2873 746f 7261 6765 3d22 7079  type(storage="py
-00001170: 6172 726f 7722 292c 0a20 2020 2070 616e  arrow"),.    pan
-00001180: 6461 732e 4172 726f 7744 7479 7065 2870  das.ArrowDtype(p
-00001190: 612e 6461 7465 3332 2829 292c 0a20 2020  a.date32()),.   
-000011a0: 2070 616e 6461 732e 4172 726f 7744 7479   pandas.ArrowDty
-000011b0: 7065 2870 612e 7469 6d65 3634 2822 7573  pe(pa.time64("us
-000011c0: 2229 292c 0a20 2020 2070 616e 6461 732e  ")),.    pandas.
-000011d0: 4172 726f 7744 7479 7065 2870 612e 7469  ArrowDtype(pa.ti
-000011e0: 6d65 7374 616d 7028 2275 7322 2929 2c0a  mestamp("us")),.
-000011f0: 2020 2020 7061 6e64 6173 2e41 7272 6f77      pandas.Arrow
-00001200: 4474 7970 6528 7061 2e74 696d 6573 7461  Dtype(pa.timesta
-00001210: 6d70 2822 7573 222c 2074 7a3d 2255 5443  mp("us", tz="UTC
-00001220: 2229 292c 0a20 2020 2070 616e 6461 732e  ")),.    pandas.
-00001230: 4172 726f 7744 7479 7065 2870 612e 6465  ArrowDtype(pa.de
-00001240: 6369 6d61 6c31 3238 2833 382c 2039 2929  cimal128(38, 9))
-00001250: 2c0a 2020 2020 7061 6e64 6173 2e41 7272  ,.    pandas.Arr
-00001260: 6f77 4474 7970 6528 7061 2e64 6563 696d  owDtype(pa.decim
-00001270: 616c 3235 3628 3736 2c20 3338 2929 2c0a  al256(76, 38)),.
-00001280: 290a 0a0a 6465 6620 5f69 735f 7175 6572  )...def _is_quer
-00001290: 7928 7175 6572 795f 6f72 5f74 6162 6c65  y(query_or_table
-000012a0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
-000012b0: 2020 2020 2222 2244 6574 6572 6d69 6e65      """Determine
-000012c0: 2069 6620 6071 7565 7279 5f6f 725f 7461   if `query_or_ta
-000012d0: 626c 6560 2069 7320 6120 7461 626c 6520  ble` is a table 
-000012e0: 4944 206f 7220 6120 5351 4c20 7374 7269  ID or a SQL stri
-000012f0: 6e67 2222 220a 2020 2020 7265 7475 726e  ng""".    return
-00001300: 2072 652e 7365 6172 6368 2872 225c 7322   re.search(r"\s"
-00001310: 2c20 7175 6572 795f 6f72 5f74 6162 6c65  , query_or_table
-00001320: 2e73 7472 6970 2829 2c20 7265 2e4d 554c  .strip(), re.MUL
-00001330: 5449 4c49 4e45 2920 6973 206e 6f74 204e  TILINE) is not N
-00001340: 6f6e 650a 0a0a 6465 6620 5f69 735f 7461  one...def _is_ta
-00001350: 626c 655f 7769 7468 5f77 696c 6463 6172  ble_with_wildcar
-00001360: 645f 7375 6666 6978 2871 7565 7279 5f6f  d_suffix(query_o
-00001370: 725f 7461 626c 653a 2073 7472 2920 2d3e  r_table: str) ->
-00001380: 2062 6f6f 6c3a 0a20 2020 2022 2222 4465   bool:.    """De
-00001390: 7465 726d 696e 6520 6966 2060 7175 6572  termine if `quer
-000013a0: 795f 6f72 5f74 6162 6c65 6020 6973 2061  y_or_table` is a
-000013b0: 2074 6162 6c65 2061 6e64 2063 6f6e 7461   table and conta
-000013c0: 696e 7320 6120 7769 6c64 6361 7264 2073  ins a wildcard s
-000013d0: 7566 6669 782e 2222 220a 2020 2020 7265  uffix.""".    re
-000013e0: 7475 726e 206e 6f74 205f 6973 5f71 7565  turn not _is_que
-000013f0: 7279 2871 7565 7279 5f6f 725f 7461 626c  ry(query_or_tabl
-00001400: 6529 2061 6e64 2071 7565 7279 5f6f 725f  e) and query_or_
-00001410: 7461 626c 652e 656e 6473 7769 7468 2822  table.endswith("
-00001420: 2a22 290a 0a0a 636c 6173 7320 5365 7373  *")...class Sess
-00001430: 696f 6e28 0a20 2020 2074 6869 7264 5f70  ion(.    third_p
-00001440: 6172 7479 5f70 616e 6461 735f 6762 712e  arty_pandas_gbq.
-00001450: 4742 5149 4f4d 6978 696e 2c0a 2020 2020  GBQIOMixin,.    
-00001460: 7468 6972 645f 7061 7274 795f 7061 6e64  third_party_pand
-00001470: 6173 5f70 6172 7175 6574 2e50 6172 7175  as_parquet.Parqu
-00001480: 6574 494f 4d69 7869 6e2c 0a20 2020 2074  etIOMixin,.    t
-00001490: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
-000014a0: 735f 7069 636b 6c65 2e50 6963 6b6c 6549  s_pickle.PickleI
-000014b0: 4f4d 6978 696e 2c0a 2020 2020 7468 6972  OMixin,.    thir
-000014c0: 645f 7061 7274 795f 7061 6e64 6173 5f72  d_party_pandas_r
-000014d0: 6561 6465 7273 2e52 6561 6465 7249 4f4d  eaders.ReaderIOM
-000014e0: 6978 696e 2c0a 293a 0a20 2020 2022 2222  ixin,.):.    """
-000014f0: 4573 7461 626c 6973 6865 7320 6120 4269  Establishes a Bi
-00001500: 6751 7565 7279 2063 6f6e 6e65 6374 696f  gQuery connectio
-00001510: 6e20 746f 2063 6170 7475 7265 2061 2067  n to capture a g
-00001520: 726f 7570 206f 6620 6a6f 6220 6163 7469  roup of job acti
-00001530: 7669 7469 6573 2072 656c 6174 6564 2074  vities related t
-00001540: 6f0a 2020 2020 4461 7461 4672 616d 6573  o.    DataFrames
-00001550: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00001560: 2020 2020 2063 6f6e 7465 7874 2028 6269       context (bi
-00001570: 6766 7261 6d65 732e 5f63 6f6e 6669 672e  gframes._config.
-00001580: 6269 6771 7565 7279 5f6f 7074 696f 6e73  bigquery_options
-00001590: 2e42 6967 5175 6572 794f 7074 696f 6e73  .BigQueryOptions
-000015a0: 293a 0a20 2020 2020 2020 2020 2020 2043  ):.            C
-000015b0: 6f6e 6669 6775 7261 7469 6f6e 2061 646a  onfiguration adj
-000015c0: 7573 7469 6e67 2068 6f77 2074 6f20 636f  usting how to co
-000015d0: 6e6e 6563 7420 746f 2042 6967 5175 6572  nnect to BigQuer
-000015e0: 7920 616e 6420 7265 6c61 7465 640a 2020  y and related.  
-000015f0: 2020 2020 2020 2020 2020 4150 4973 2e20            APIs. 
-00001600: 4e6f 7465 2074 6861 7420 736f 6d65 206f  Note that some o
-00001610: 7074 696f 6e73 2061 7265 2069 676e 6f72  ptions are ignor
-00001620: 6564 2069 6620 6060 636c 6965 6e74 735f  ed if ``clients_
-00001630: 7072 6f76 6964 6572 6060 2069 730a 2020  provider`` is.  
-00001640: 2020 2020 2020 2020 2020 7365 742e 0a20            set.. 
-00001650: 2020 2020 2020 2063 6c69 656e 7473 5f70         clients_p
-00001660: 726f 7669 6465 7220 2862 6967 6672 616d  rovider (bigfram
-00001670: 6573 2e73 6573 7369 6f6e 2e63 6c69 656e  es.session.clien
-00001680: 7473 2e43 6c69 656e 7473 5072 6f76 6964  ts.ClientsProvid
-00001690: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-000016a0: 2041 6e20 6f62 6a65 6374 2070 726f 7669   An object provi
-000016b0: 6469 6e67 2063 6c69 656e 7420 6c69 6272  ding client libr
-000016c0: 6172 7920 6f62 6a65 6374 732e 0a20 2020  ary objects..   
-000016d0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-000016e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000016f0: 7365 6c66 2c0a 2020 2020 2020 2020 636f  self,.        co
-00001700: 6e74 6578 743a 204f 7074 696f 6e61 6c5b  ntext: Optional[
-00001710: 6269 6771 7565 7279 5f6f 7074 696f 6e73  bigquery_options
-00001720: 2e42 6967 5175 6572 794f 7074 696f 6e73  .BigQueryOptions
-00001730: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00001740: 2020 636c 6965 6e74 735f 7072 6f76 6964    clients_provid
-00001750: 6572 3a20 4f70 7469 6f6e 616c 5b62 6967  er: Optional[big
-00001760: 6672 616d 6573 2e73 6573 7369 6f6e 2e63  frames.session.c
-00001770: 6c69 656e 7473 2e43 6c69 656e 7473 5072  lients.ClientsPr
-00001780: 6f76 6964 6572 5d20 3d20 4e6f 6e65 2c0a  ovider] = None,.
-00001790: 2020 2020 293a 0a20 2020 2020 2020 2069      ):.        i
-000017a0: 6620 636f 6e74 6578 7420 6973 204e 6f6e  f context is Non
-000017b0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-000017c0: 6f6e 7465 7874 203d 2062 6967 7175 6572  ontext = bigquer
-000017d0: 795f 6f70 7469 6f6e 732e 4269 6751 7565  y_options.BigQue
-000017e0: 7279 4f70 7469 6f6e 7328 290a 0a20 2020  ryOptions()..   
-000017f0: 2020 2020 2023 2054 4f44 4f28 7377 6173       # TODO(swas
-00001800: 7429 3a20 4765 7420 6c6f 6361 7469 6f6e  t): Get location
-00001810: 2066 726f 6d20 7468 6520 656e 7669 726f   from the enviro
-00001820: 6e6d 656e 742e 0a20 2020 2020 2020 2069  nment..        i
-00001830: 6620 636f 6e74 6578 742e 6c6f 6361 7469  f context.locati
-00001840: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00001850: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00001860: 6361 7469 6f6e 203d 2022 5553 220a 2020  cation = "US".  
-00001870: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00001880: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-00001890: 2020 2020 2020 2020 2066 224e 6f20 6578           f"No ex
-000018a0: 706c 6963 6974 206c 6f63 6174 696f 6e20  plicit location 
-000018b0: 6973 2073 6574 2c20 736f 2075 7369 6e67  is set, so using
-000018c0: 206c 6f63 6174 696f 6e20 7b73 656c 662e   location {self.
-000018d0: 5f6c 6f63 6174 696f 6e7d 2066 6f72 2074  _location} for t
-000018e0: 6865 2073 6573 7369 6f6e 2e22 2c0a 2020  he session.",.  
-000018f0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00001900: 6163 6b6c 6576 656c 3d32 2c0a 2020 2020  acklevel=2,.    
-00001910: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001920: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001930: 2020 2020 7365 6c66 2e5f 6c6f 6361 7469      self._locati
-00001940: 6f6e 203d 2063 6f6e 7465 7874 2e6c 6f63  on = context.loc
-00001950: 6174 696f 6e0a 0a20 2020 2020 2020 2073  ation..        s
-00001960: 656c 662e 5f62 715f 6b6d 735f 6b65 795f  elf._bq_kms_key_
-00001970: 6e61 6d65 203d 2063 6f6e 7465 7874 2e6b  name = context.k
-00001980: 6d73 5f6b 6579 5f6e 616d 650a 0a20 2020  ms_key_name..   
-00001990: 2020 2020 2023 2049 6e73 7461 6e74 6961       # Instantia
-000019a0: 7465 2061 2063 6c69 656e 7473 2070 726f  te a clients pro
-000019b0: 7669 6465 7220 746f 2068 656c 7020 7769  vider to help wi
-000019c0: 7468 2063 6c6f 7564 2063 6c69 656e 7473  th cloud clients
-000019d0: 2074 6861 7420 7769 6c6c 2062 650a 2020   that will be.  
-000019e0: 2020 2020 2020 2320 7573 6564 2069 6e20        # used in 
-000019f0: 7468 6520 6675 7475 7265 206f 7065 7261  the future opera
-00001a00: 7469 6f6e 7320 696e 2074 6865 2073 6573  tions in the ses
-00001a10: 7369 6f6e 0a20 2020 2020 2020 2069 6620  sion.        if 
-00001a20: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
-00001a30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001a40: 6c66 2e5f 636c 6965 6e74 735f 7072 6f76  lf._clients_prov
-00001a50: 6964 6572 203d 2063 6c69 656e 7473 5f70  ider = clients_p
-00001a60: 726f 7669 6465 720a 2020 2020 2020 2020  rovider.        
-00001a70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00001a80: 2020 7365 6c66 2e5f 636c 6965 6e74 735f    self._clients_
-00001a90: 7072 6f76 6964 6572 203d 2062 6967 6672  provider = bigfr
-00001aa0: 616d 6573 2e73 6573 7369 6f6e 2e63 6c69  ames.session.cli
-00001ab0: 656e 7473 2e43 6c69 656e 7473 5072 6f76  ents.ClientsProv
-00001ac0: 6964 6572 280a 2020 2020 2020 2020 2020  ider(.          
-00001ad0: 2020 2020 2020 7072 6f6a 6563 743d 636f        project=co
-00001ae0: 6e74 6578 742e 7072 6f6a 6563 742c 0a20  ntext.project,. 
-00001af0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00001b00: 6f63 6174 696f 6e3d 7365 6c66 2e5f 6c6f  ocation=self._lo
-00001b10: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
-00001b20: 2020 2020 2020 2020 7573 655f 7265 6769          use_regi
-00001b30: 6f6e 616c 5f65 6e64 706f 696e 7473 3d63  onal_endpoints=c
-00001b40: 6f6e 7465 7874 2e75 7365 5f72 6567 696f  ontext.use_regio
-00001b50: 6e61 6c5f 656e 6470 6f69 6e74 732c 0a20  nal_endpoints,. 
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001b70: 7265 6465 6e74 6961 6c73 3d63 6f6e 7465  redentials=conte
-00001b80: 7874 2e63 7265 6465 6e74 6961 6c73 2c0a  xt.credentials,.
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 6170 706c 6963 6174 696f 6e5f 6e61 6d65  application_name
-00001bb0: 3d63 6f6e 7465 7874 2e61 7070 6c69 6361  =context.applica
-00001bc0: 7469 6f6e 5f6e 616d 652c 0a20 2020 2020  tion_name,.     
-00001bd0: 2020 2020 2020 2020 2020 2062 715f 6b6d             bq_km
-00001be0: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
-00001bf0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
-00001c00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00001c10: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00001c20: 7265 6174 655f 6271 5f64 6174 6173 6574  reate_bq_dataset
-00001c30: 7328 290a 0a20 2020 2020 2020 2023 2054  s()..        # T
-00001c40: 4f44 4f28 7368 6f62 7329 3a20 5265 6d6f  ODO(shobs): Remo
-00001c50: 7665 2074 6869 7320 6c6f 6769 6320 6166  ve this logic af
-00001c60: 7465 7220 6874 7470 733a 2f2f 6769 7468  ter https://gith
-00001c70: 7562 2e63 6f6d 2f69 6269 732d 7072 6f6a  ub.com/ibis-proj
-00001c80: 6563 742f 6962 6973 2f69 7373 7565 732f  ect/ibis/issues/
-00001c90: 3834 3934 0a20 2020 2020 2020 2023 2068  8494.        # h
-00001ca0: 6173 2062 6565 6e20 6669 7865 642e 2054  as been fixed. T
-00001cb0: 6865 2069 6269 7320 636c 6965 6e74 2063  he ibis client c
-00001cc0: 6861 6e67 6573 2074 6865 2064 6566 6175  hanges the defau
-00001cd0: 6c74 2071 7565 7279 206a 6f62 2063 6f6e  lt query job con
-00001ce0: 6669 670a 2020 2020 2020 2020 2320 736f  fig.        # so
-00001cf0: 2077 6520 6172 6520 676f 696e 6720 746f   we are going to
-00001d00: 2072 656d 656d 6265 7220 7468 6520 6375   remember the cu
-00001d10: 7272 656e 7420 636f 6e66 6967 2061 6e64  rrent config and
-00001d20: 2072 6573 746f 7265 2069 7420 6166 7465   restore it afte
-00001d30: 720a 2020 2020 2020 2020 2320 7468 6520  r.        # the 
-00001d40: 6962 6973 2063 6c69 656e 7420 6861 7320  ibis client has 
-00001d50: 6265 656e 2063 7265 6174 6564 0a20 2020  been created.   
-00001d60: 2020 2020 206f 7269 6769 6e61 6c5f 6465       original_de
-00001d70: 6661 756c 745f 7175 6572 795f 6a6f 625f  fault_query_job_
-00001d80: 636f 6e66 6967 203d 2073 656c 662e 6271  config = self.bq
-00001d90: 636c 6965 6e74 2e64 6566 6175 6c74 5f71  client.default_q
-00001da0: 7565 7279 5f6a 6f62 5f63 6f6e 6669 670a  uery_job_config.
-00001db0: 0a20 2020 2020 2020 2073 656c 662e 6962  .        self.ib
-00001dc0: 6973 5f63 6c69 656e 7420 3d20 7479 7069  is_client = typi
-00001dd0: 6e67 2e63 6173 7428 0a20 2020 2020 2020  ng.cast(.       
-00001de0: 2020 2020 2069 6269 735f 6269 6771 7565       ibis_bigque
-00001df0: 7279 2e42 6163 6b65 6e64 2c0a 2020 2020  ry.Backend,.    
-00001e00: 2020 2020 2020 2020 6962 6973 2e62 6967          ibis.big
-00001e10: 7175 6572 792e 636f 6e6e 6563 7428 0a20  query.connect(. 
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001e30: 726f 6a65 6374 5f69 643d 636f 6e74 6578  roject_id=contex
-00001e40: 742e 7072 6f6a 6563 742c 0a20 2020 2020  t.project,.     
-00001e50: 2020 2020 2020 2020 2020 2063 6c69 656e             clien
-00001e60: 743d 7365 6c66 2e62 7163 6c69 656e 742c  t=self.bqclient,
-00001e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e80: 2073 746f 7261 6765 5f63 6c69 656e 743d   storage_client=
-00001e90: 7365 6c66 2e62 7173 746f 7261 6765 7265  self.bqstoragere
-00001ea0: 6164 636c 6965 6e74 2c0a 2020 2020 2020  adclient,.      
-00001eb0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00001ec0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
-00001ed0: 2e62 7163 6c69 656e 742e 6465 6661 756c  .bqclient.defaul
-00001ee0: 745f 7175 6572 795f 6a6f 625f 636f 6e66  t_query_job_conf
-00001ef0: 6967 203d 206f 7269 6769 6e61 6c5f 6465  ig = original_de
-00001f00: 6661 756c 745f 7175 6572 795f 6a6f 625f  fault_query_job_
-00001f10: 636f 6e66 6967 0a0a 2020 2020 2020 2020  config..        
-00001f20: 2320 5265 736f 6c76 6520 7468 6520 4251  # Resolve the BQ
-00001f30: 2063 6f6e 6e65 6374 696f 6e20 666f 7220   connection for 
-00001f40: 7265 6d6f 7465 2066 756e 6374 696f 6e20  remote function 
-00001f50: 616e 6420 5665 7274 6578 2041 4920 696e  and Vertex AI in
-00001f60: 7465 6772 6174 696f 6e0a 2020 2020 2020  tegration.      
-00001f70: 2020 7365 6c66 2e5f 6271 5f63 6f6e 6e65    self._bq_conne
-00001f80: 6374 696f 6e20 3d20 636f 6e74 6578 742e  ction = context.
-00001f90: 6271 5f63 6f6e 6e65 6374 696f 6e20 6f72  bq_connection or
-00001fa0: 205f 4249 4746 5241 4d45 535f 4445 4641   _BIGFRAMES_DEFA
-00001fb0: 554c 545f 434f 4e4e 4543 5449 4f4e 5f49  ULT_CONNECTION_I
-00001fc0: 440a 2020 2020 2020 2020 7365 6c66 2e5f  D.        self._
-00001fd0: 736b 6970 5f62 715f 636f 6e6e 6563 7469  skip_bq_connecti
-00001fe0: 6f6e 5f63 6865 636b 203d 2063 6f6e 7465  on_check = conte
-00001ff0: 7874 2e5f 736b 6970 5f62 715f 636f 6e6e  xt._skip_bq_conn
-00002000: 6563 7469 6f6e 5f63 6865 636b 0a0a 2020  ection_check..  
-00002010: 2020 2020 2020 2320 4e6f 7720 7468 6174        # Now that
-00002020: 2077 6527 7265 2073 7461 7274 696e 6720   we're starting 
-00002030: 7468 6520 7365 7373 696f 6e2c 2064 6f6e  the session, don
-00002040: 2774 2061 6c6c 6f77 2074 6865 206f 7074  't allow the opt
-00002050: 696f 6e73 2074 6f20 6265 0a20 2020 2020  ions to be.     
-00002060: 2020 2023 2063 6861 6e67 6564 2e0a 2020     # changed..  
-00002070: 2020 2020 2020 636f 6e74 6578 742e 5f73        context._s
-00002080: 6573 7369 6f6e 5f73 7461 7274 6564 203d  ession_started =
-00002090: 2054 7275 650a 2020 2020 2020 2020 7365   True.        se
-000020a0: 6c66 2e5f 6466 5f73 6e61 7073 686f 743a  lf._df_snapshot:
-000020b0: 2044 6963 745b 0a20 2020 2020 2020 2020   Dict[.         
-000020c0: 2020 2062 6967 7175 6572 792e 5461 626c     bigquery.Tabl
-000020d0: 6552 6566 6572 656e 6365 2c20 5475 706c  eReference, Tupl
-000020e0: 655b 6461 7465 7469 6d65 2e64 6174 6574  e[datetime.datet
-000020f0: 696d 652c 2062 6967 7175 6572 792e 5461  ime, bigquery.Ta
-00002100: 626c 655d 0a20 2020 2020 2020 205d 203d  ble].        ] =
-00002110: 207b 7d0a 0a20 2020 2040 7072 6f70 6572   {}..    @proper
-00002120: 7479 0a20 2020 2064 6566 2062 7163 6c69  ty.    def bqcli
-00002130: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
-00002140: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00002150: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
-00002160: 2e62 7163 6c69 656e 740a 0a20 2020 2040  .bqclient..    @
-00002170: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00002180: 2062 7163 6f6e 6e65 6374 696f 6e63 6c69   bqconnectioncli
-00002190: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
-000021a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000021b0: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
-000021c0: 2e62 7163 6f6e 6e65 6374 696f 6e63 6c69  .bqconnectioncli
-000021d0: 656e 740a 0a20 2020 2040 7072 6f70 6572  ent..    @proper
-000021e0: 7479 0a20 2020 2064 6566 2062 7173 746f  ty.    def bqsto
-000021f0: 7261 6765 7265 6164 636c 6965 6e74 2873  ragereadclient(s
-00002200: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00002210: 7475 726e 2073 656c 662e 5f63 6c69 656e  turn self._clien
-00002220: 7473 5f70 726f 7669 6465 722e 6271 7374  ts_provider.bqst
-00002230: 6f72 6167 6572 6561 6463 6c69 656e 740a  oragereadclient.
-00002240: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00002250: 2020 2064 6566 2063 6c6f 7564 6675 6e63     def cloudfunc
-00002260: 7469 6f6e 7363 6c69 656e 7428 7365 6c66  tionsclient(self
-00002270: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00002280: 6e20 7365 6c66 2e5f 636c 6965 6e74 735f  n self._clients_
-00002290: 7072 6f76 6964 6572 2e63 6c6f 7564 6675  provider.cloudfu
-000022a0: 6e63 7469 6f6e 7363 6c69 656e 740a 0a20  nctionsclient.. 
-000022b0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000022c0: 2064 6566 2072 6573 6f75 7263 656d 616e   def resourceman
-000022d0: 6167 6572 636c 6965 6e74 2873 656c 6629  agerclient(self)
-000022e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000022f0: 2073 656c 662e 5f63 6c69 656e 7473 5f70   self._clients_p
-00002300: 726f 7669 6465 722e 7265 736f 7572 6365  rovider.resource
-00002310: 6d61 6e61 6765 7263 6c69 656e 740a 0a20  managerclient.. 
-00002320: 2020 205f 6271 5f63 6f6e 6e65 6374 696f     _bq_connectio
-00002330: 6e5f 6d61 6e61 6765 723a 204f 7074 696f  n_manager: Optio
-00002340: 6e61 6c5b 6269 6766 7261 6d65 732e 636c  nal[bigframes.cl
-00002350: 6965 6e74 732e 4271 436f 6e6e 6563 7469  ients.BqConnecti
-00002360: 6f6e 4d61 6e61 6765 725d 203d 204e 6f6e  onManager] = Non
-00002370: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+000002b0: 650a 696d 706f 7274 206c 6f67 6769 6e67  e.import logging
+000002c0: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
+000002d0: 7420 7265 0a69 6d70 6f72 7420 7365 6372  t re.import secr
+000002e0: 6574 730a 696d 706f 7274 2074 7970 696e  ets.import typin
+000002f0: 670a 6672 6f6d 2074 7970 696e 6720 696d  g.from typing im
+00000300: 706f 7274 2028 0a20 2020 2041 6e79 2c0a  port (.    Any,.
+00000310: 2020 2020 4361 6c6c 6162 6c65 2c0a 2020      Callable,.  
+00000320: 2020 4469 6374 2c0a 2020 2020 494f 2c0a    Dict,.    IO,.
+00000330: 2020 2020 4974 6572 6162 6c65 2c0a 2020      Iterable,.  
+00000340: 2020 4c69 7374 2c0a 2020 2020 4c69 7465    List,.    Lite
+00000350: 7261 6c2c 0a20 2020 204d 6170 7069 6e67  ral,.    Mapping
+00000360: 2c0a 2020 2020 4d75 7461 626c 6553 6571  ,.    MutableSeq
+00000370: 7565 6e63 652c 0a20 2020 204f 7074 696f  uence,.    Optio
+00000380: 6e61 6c2c 0a20 2020 2053 6571 7565 6e63  nal,.    Sequenc
+00000390: 652c 0a20 2020 2054 7570 6c65 2c0a 2020  e,.    Tuple,.  
+000003a0: 2020 556e 696f 6e2c 0a29 0a69 6d70 6f72    Union,.).impor
+000003b0: 7420 7575 6964 0a69 6d70 6f72 7420 7761  t uuid.import wa
+000003c0: 726e 696e 6773 0a0a 2320 4576 656e 2074  rnings..# Even t
+000003d0: 686f 7567 6820 7468 6520 6962 6973 2e62  hough the ibis.b
+000003e0: 6163 6b65 6e64 732e 6269 6771 7565 7279  ackends.bigquery
+000003f0: 2069 6d70 6f72 7420 6973 2075 6e75 7365   import is unuse
+00000400: 642c 2069 7427 7320 6e65 6564 6564 0a23  d, it's needed.#
+00000410: 2074 6f20 7265 6769 7374 6572 206e 6577   to register new
+00000420: 2061 6e64 2072 6570 6c61 6365 6d65 6e74   and replacement
+00000430: 206f 7073 2077 6974 6820 7468 6520 4962   ops with the Ib
+00000440: 6973 2042 6967 5175 6572 7920 6261 636b  is BigQuery back
+00000450: 656e 642e 0a69 6d70 6f72 7420 6269 6766  end..import bigf
+00000460: 7261 6d65 735f 7665 6e64 6f72 6564 2e69  rames_vendored.i
+00000470: 6269 732e 6261 636b 656e 6473 2e62 6967  bis.backends.big
+00000480: 7175 6572 7920 2023 206e 6f71 610a 696d  query  # noqa.im
+00000490: 706f 7274 2062 6967 6672 616d 6573 5f76  port bigframes_v
+000004a0: 656e 646f 7265 642e 7061 6e64 6173 2e69  endored.pandas.i
+000004b0: 6f2e 6762 7120 6173 2074 6869 7264 5f70  o.gbq as third_p
+000004c0: 6172 7479 5f70 616e 6461 735f 6762 710a  arty_pandas_gbq.
+000004d0: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+000004e0: 5f76 656e 646f 7265 642e 7061 6e64 6173  _vendored.pandas
+000004f0: 2e69 6f2e 7061 7271 7565 7420 6173 2074  .io.parquet as t
+00000500: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
+00000510: 735f 7061 7271 7565 740a 696d 706f 7274  s_parquet.import
+00000520: 2062 6967 6672 616d 6573 5f76 656e 646f   bigframes_vendo
+00000530: 7265 642e 7061 6e64 6173 2e69 6f2e 7061  red.pandas.io.pa
+00000540: 7273 6572 732e 7265 6164 6572 7320 6173  rsers.readers as
+00000550: 2074 6869 7264 5f70 6172 7479 5f70 616e   third_party_pan
+00000560: 6461 735f 7265 6164 6572 730a 696d 706f  das_readers.impo
+00000570: 7274 2062 6967 6672 616d 6573 5f76 656e  rt bigframes_ven
+00000580: 646f 7265 642e 7061 6e64 6173 2e69 6f2e  dored.pandas.io.
+00000590: 7069 636b 6c65 2061 7320 7468 6972 645f  pickle as third_
+000005a0: 7061 7274 795f 7061 6e64 6173 5f70 6963  party_pandas_pic
+000005b0: 6b6c 650a 696d 706f 7274 2067 6f6f 676c  kle.import googl
+000005c0: 652e 6170 695f 636f 7265 2e63 6c69 656e  e.api_core.clien
+000005d0: 745f 696e 666f 0a69 6d70 6f72 7420 676f  t_info.import go
+000005e0: 6f67 6c65 2e61 7069 5f63 6f72 652e 636c  ogle.api_core.cl
+000005f0: 6965 6e74 5f6f 7074 696f 6e73 0a69 6d70  ient_options.imp
+00000600: 6f72 7420 676f 6f67 6c65 2e61 7069 5f63  ort google.api_c
+00000610: 6f72 652e 6578 6365 7074 696f 6e73 0a69  ore.exceptions.i
+00000620: 6d70 6f72 7420 676f 6f67 6c65 2e61 7069  mport google.api
+00000630: 5f63 6f72 652e 6761 7069 635f 7631 2e63  _core.gapic_v1.c
+00000640: 6c69 656e 745f 696e 666f 0a69 6d70 6f72  lient_info.impor
+00000650: 7420 676f 6f67 6c65 2e61 7574 682e 6372  t google.auth.cr
+00000660: 6564 656e 7469 616c 730a 696d 706f 7274  edentials.import
+00000670: 2067 6f6f 676c 652e 636c 6f75 642e 6269   google.cloud.bi
+00000680: 6771 7565 7279 2061 7320 6269 6771 7565  gquery as bigque
+00000690: 7279 0a69 6d70 6f72 7420 676f 6f67 6c65  ry.import google
+000006a0: 2e63 6c6f 7564 2e62 6967 7175 6572 792e  .cloud.bigquery.
+000006b0: 7461 626c 650a 696d 706f 7274 2067 6f6f  table.import goo
+000006c0: 676c 652e 636c 6f75 642e 6269 6771 7565  gle.cloud.bigque
+000006d0: 7279 5f63 6f6e 6e65 6374 696f 6e5f 7631  ry_connection_v1
+000006e0: 0a69 6d70 6f72 7420 676f 6f67 6c65 2e63  .import google.c
+000006f0: 6c6f 7564 2e62 6967 7175 6572 795f 7374  loud.bigquery_st
+00000700: 6f72 6167 655f 7631 0a69 6d70 6f72 7420  orage_v1.import 
+00000710: 676f 6f67 6c65 2e63 6c6f 7564 2e66 756e  google.cloud.fun
+00000720: 6374 696f 6e73 5f76 320a 696d 706f 7274  ctions_v2.import
+00000730: 2067 6f6f 676c 652e 636c 6f75 642e 7265   google.cloud.re
+00000740: 736f 7572 6365 6d61 6e61 6765 725f 7633  sourcemanager_v3
+00000750: 0a69 6d70 6f72 7420 676f 6f67 6c65 2e63  .import google.c
+00000760: 6c6f 7564 2e73 746f 7261 6765 2061 7320  loud.storage as 
+00000770: 7374 6f72 6167 6520 2023 2074 7970 653a  storage  # type:
+00000780: 2069 676e 6f72 650a 696d 706f 7274 2069   ignore.import i
+00000790: 6269 730a 696d 706f 7274 2069 6269 732e  bis.import ibis.
+000007a0: 6261 636b 656e 6473 2e62 6967 7175 6572  backends.bigquer
+000007b0: 7920 6173 2069 6269 735f 6269 6771 7565  y as ibis_bigque
+000007c0: 7279 0a69 6d70 6f72 7420 6962 6973 2e65  ry.import ibis.e
+000007d0: 7870 722e 7479 7065 7320 6173 2069 6269  xpr.types as ibi
+000007e0: 735f 7479 7065 730a 696d 706f 7274 206e  s_types.import n
+000007f0: 756d 7079 2061 7320 6e70 0a69 6d70 6f72  umpy as np.impor
+00000800: 7420 7061 6e64 6173 0a66 726f 6d20 7061  t pandas.from pa
+00000810: 6e64 6173 2e5f 7479 7069 6e67 2069 6d70  ndas._typing imp
+00000820: 6f72 7420 280a 2020 2020 436f 6d70 7265  ort (.    Compre
+00000830: 7373 696f 6e4f 7074 696f 6e73 2c0a 2020  ssionOptions,.  
+00000840: 2020 4669 6c65 5061 7468 2c0a 2020 2020    FilePath,.    
+00000850: 5265 6164 5069 636b 6c65 4275 6666 6572  ReadPickleBuffer
+00000860: 2c0a 2020 2020 5374 6f72 6167 654f 7074  ,.    StorageOpt
+00000870: 696f 6e73 2c0a 290a 696d 706f 7274 2070  ions,.).import p
+00000880: 7961 7272 6f77 2061 7320 7061 0a0a 696d  yarrow as pa..im
+00000890: 706f 7274 2062 6967 6672 616d 6573 2e5f  port bigframes._
+000008a0: 636f 6e66 6967 2e62 6967 7175 6572 795f  config.bigquery_
+000008b0: 6f70 7469 6f6e 7320 6173 2062 6967 7175  options as bigqu
+000008c0: 6572 795f 6f70 7469 6f6e 730a 696d 706f  ery_options.impo
+000008d0: 7274 2062 6967 6672 616d 6573 2e63 6c69  rt bigframes.cli
+000008e0: 656e 7473 0a69 6d70 6f72 7420 6269 6766  ents.import bigf
+000008f0: 7261 6d65 732e 636f 6e73 7461 6e74 7320  rames.constants 
+00000900: 6173 2063 6f6e 7374 616e 7473 0a69 6d70  as constants.imp
+00000910: 6f72 7420 6269 6766 7261 6d65 732e 636f  ort bigframes.co
+00000920: 7265 2061 7320 636f 7265 0a69 6d70 6f72  re as core.impor
+00000930: 7420 6269 6766 7261 6d65 732e 636f 7265  t bigframes.core
+00000940: 2e62 6c6f 636b 7320 6173 2062 6c6f 636b  .blocks as block
+00000950: 730a 696d 706f 7274 2062 6967 6672 616d  s.import bigfram
+00000960: 6573 2e63 6f72 652e 636f 6d70 696c 650a  es.core.compile.
+00000970: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+00000980: 2e63 6f72 652e 6e6f 6465 7320 6173 206e  .core.nodes as n
+00000990: 6f64 6573 0a66 726f 6d20 6269 6766 7261  odes.from bigfra
+000009a0: 6d65 732e 636f 7265 2e6f 7264 6572 696e  mes.core.orderin
+000009b0: 6720 696d 706f 7274 2049 6e74 6567 6572  g import Integer
+000009c0: 456e 636f 6469 6e67 0a69 6d70 6f72 7420  Encoding.import 
+000009d0: 6269 6766 7261 6d65 732e 636f 7265 2e6f  bigframes.core.o
+000009e0: 7264 6572 696e 6720 6173 206f 7264 6572  rdering as order
+000009f0: 0a69 6d70 6f72 7420 6269 6766 7261 6d65  .import bigframe
+00000a00: 732e 636f 7265 2e74 7265 655f 7072 6f70  s.core.tree_prop
+00000a10: 6572 7469 6573 2061 7320 7472 6176 6572  erties as traver
+00000a20: 7361 6c73 0a69 6d70 6f72 7420 6269 6766  sals.import bigf
+00000a30: 7261 6d65 732e 636f 7265 2e74 7265 655f  rames.core.tree_
+00000a40: 7072 6f70 6572 7469 6573 2061 7320 7472  properties as tr
+00000a50: 6565 5f70 726f 7065 7274 6965 730a 696d  ee_properties.im
+00000a60: 706f 7274 2062 6967 6672 616d 6573 2e63  port bigframes.c
+00000a70: 6f72 652e 7574 696c 7320 6173 2075 7469  ore.utils as uti
+00000a80: 6c73 0a69 6d70 6f72 7420 6269 6766 7261  ls.import bigfra
+00000a90: 6d65 732e 6474 7970 6573 0a69 6d70 6f72  mes.dtypes.impor
+00000aa0: 7420 6269 6766 7261 6d65 732e 666f 726d  t bigframes.form
+00000ab0: 6174 7469 6e67 5f68 656c 7065 7273 2061  atting_helpers a
+00000ac0: 7320 666f 726d 6174 7469 6e67 5f68 656c  s formatting_hel
+00000ad0: 7065 7273 0a66 726f 6d20 6269 6766 7261  pers.from bigfra
+00000ae0: 6d65 732e 6675 6e63 7469 6f6e 732e 7265  mes.functions.re
+00000af0: 6d6f 7465 5f66 756e 6374 696f 6e20 696d  mote_function im
+00000b00: 706f 7274 2072 6561 645f 6762 715f 6675  port read_gbq_fu
+00000b10: 6e63 7469 6f6e 2061 7320 6269 6766 7261  nction as bigfra
+00000b20: 6d65 735f 7267 660a 6672 6f6d 2062 6967  mes_rgf.from big
+00000b30: 6672 616d 6573 2e66 756e 6374 696f 6e73  frames.functions
+00000b40: 2e72 656d 6f74 655f 6675 6e63 7469 6f6e  .remote_function
+00000b50: 2069 6d70 6f72 7420 7265 6d6f 7465 5f66   import remote_f
+00000b60: 756e 6374 696f 6e20 6173 2062 6967 6672  unction as bigfr
+00000b70: 616d 6573 5f72 660a 696d 706f 7274 2062  ames_rf.import b
+00000b80: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00000b90: 2e5f 696f 2e62 6967 7175 6572 7920 6173  ._io.bigquery as
+00000ba0: 2062 6967 6672 616d 6573 5f69 6f0a 696d   bigframes_io.im
+00000bb0: 706f 7274 2062 6967 6672 616d 6573 2e73  port bigframes.s
+00000bc0: 6573 7369 6f6e 2e5f 696f 2e62 6967 7175  ession._io.bigqu
+00000bd0: 6572 792e 7265 6164 5f67 6271 5f74 6162  ery.read_gbq_tab
+00000be0: 6c65 2061 7320 6266 5f72 6561 645f 6762  le as bf_read_gb
+00000bf0: 715f 7461 626c 650a 696d 706f 7274 2062  q_table.import b
+00000c00: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00000c10: 2e63 6c69 656e 7473 0a69 6d70 6f72 7420  .clients.import 
+00000c20: 6269 6766 7261 6d65 732e 7665 7273 696f  bigframes.versio
+00000c30: 6e0a 0a23 2041 766f 6964 2063 6972 6375  n..# Avoid circu
+00000c40: 6c61 7220 696d 706f 7274 732e 0a69 6620  lar imports..if 
+00000c50: 7479 7069 6e67 2e54 5950 455f 4348 4543  typing.TYPE_CHEC
+00000c60: 4b49 4e47 3a0a 2020 2020 696d 706f 7274  KING:.    import
+00000c70: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
+00000c80: 696e 6465 7865 730a 2020 2020 696d 706f  indexes.    impo
+00000c90: 7274 2062 6967 6672 616d 6573 2e64 6174  rt bigframes.dat
+00000ca0: 6166 7261 6d65 2061 7320 6461 7461 6672  aframe as datafr
+00000cb0: 616d 650a 2020 2020 696d 706f 7274 2062  ame.    import b
+00000cc0: 6967 6672 616d 6573 2e73 6572 6965 730a  igframes.series.
+00000cd0: 0a5f 4249 4746 5241 4d45 535f 4445 4641  ._BIGFRAMES_DEFA
+00000ce0: 554c 545f 434f 4e4e 4543 5449 4f4e 5f49  ULT_CONNECTION_I
+00000cf0: 4420 3d20 2262 6967 6672 616d 6573 2d64  D = "bigframes-d
+00000d00: 6566 6175 6c74 2d63 6f6e 6e65 6374 696f  efault-connectio
+00000d10: 6e22 0a0a 5f54 454d 505f 5441 424c 455f  n".._TEMP_TABLE_
+00000d20: 4944 5f46 4f52 4d41 5420 3d20 2262 7164  ID_FORMAT = "bqd
+00000d30: 667b 6461 7465 7d5f 7b73 6573 7369 6f6e  f{date}_{session
+00000d40: 5f69 647d 5f7b 7261 6e64 6f6d 5f69 647d  _id}_{random_id}
+00000d50: 220a 0a5f 4d41 585f 434c 5553 5445 525f  ".._MAX_CLUSTER_
+00000d60: 434f 4c55 4d4e 5320 3d20 340a 0a23 2054  COLUMNS = 4..# T
+00000d70: 4f44 4f28 7377 6173 7429 3a20 4e65 6564  ODO(swast): Need
+00000d80: 2074 6f20 636f 6e6e 6563 7420 746f 2072   to connect to r
+00000d90: 6567 696f 6e61 6c20 656e 6470 6f69 6e74  egional endpoint
+00000da0: 7320 7768 656e 2070 6572 666f 726d 696e  s when performin
+00000db0: 6720 7265 6d6f 7465 0a23 2066 756e 6374  g remote.# funct
+00000dc0: 696f 6e73 206f 7065 7261 7469 6f6e 7320  ions operations 
+00000dd0: 2842 5120 436f 6e6e 6563 7469 6f6e 2049  (BQ Connection I
+00000de0: 414d 2c20 436c 6f75 6420 5275 6e20 2f20  AM, Cloud Run / 
+00000df0: 436c 6f75 6420 4675 6e63 7469 6f6e 7329  Cloud Functions)
+00000e00: 2e0a 2320 416c 736f 2073 6565 2069 6620  ..# Also see if 
+00000e10: 7265 736f 7572 6365 206d 616e 6167 6572  resource manager
+00000e20: 2063 6c69 656e 7420 6c69 6272 6172 7920   client library 
+00000e30: 7375 7070 6f72 7473 2072 6567 696f 6e61  supports regiona
+00000e40: 6c20 656e 6470 6f69 6e74 732e 0a0a 5f56  l endpoints..._V
+00000e50: 414c 4944 5f45 4e43 4f44 494e 4753 203d  ALID_ENCODINGS =
+00000e60: 207b 0a20 2020 2022 5554 462d 3822 2c0a   {.    "UTF-8",.
+00000e70: 2020 2020 2249 534f 2d38 3835 392d 3122      "ISO-8859-1"
+00000e80: 2c0a 2020 2020 2255 5446 2d31 3642 4522  ,.    "UTF-16BE"
+00000e90: 2c0a 2020 2020 2255 5446 2d31 364c 4522  ,.    "UTF-16LE"
+00000ea0: 2c0a 2020 2020 2255 5446 2d33 3242 4522  ,.    "UTF-32BE"
+00000eb0: 2c0a 2020 2020 2255 5446 2d33 324c 4522  ,.    "UTF-32LE"
+00000ec0: 2c0a 7d0a 0a23 2042 6967 5175 6572 7920  ,.}..# BigQuery 
+00000ed0: 6861 7320 3120 4d42 2071 7565 7279 2073  has 1 MB query s
+00000ee0: 697a 6520 6c69 6d69 742e 2044 6f6e 2774  ize limit. Don't
+00000ef0: 2077 616e 7420 746f 2074 616b 6520 7570   want to take up
+00000f00: 206d 6f72 6520 7468 616e 2061 2066 6577   more than a few
+00000f10: 2025 206f 6620 7468 6174 2069 6e6c 696e   % of that inlin
+00000f20: 696e 6720 6120 7461 626c 652e 0a23 2041  ing a table..# A
+00000f30: 6c73 6f20 6d75 7374 2061 7373 756d 6520  lso must assume 
+00000f40: 7468 6174 2074 6578 7420 656e 636f 6469  that text encodi
+00000f50: 6e67 2061 7320 6c69 7465 7261 6c73 2069  ng as literals i
+00000f60: 7320 6d75 6368 206c 6573 7320 6566 6669  s much less effi
+00000f70: 6369 656e 7420 7468 616e 2069 6e2d 6d65  cient than in-me
+00000f80: 6d6f 7279 2072 6570 7265 7365 6e74 6174  mory representat
+00000f90: 696f 6e2e 0a4d 4158 5f49 4e4c 494e 455f  ion..MAX_INLINE_
+00000fa0: 4446 5f42 5954 4553 203d 2035 3030 300a  DF_BYTES = 5000.
+00000fb0: 0a23 204d 6178 2063 6f6d 706c 6578 6974  .# Max complexit
+00000fc0: 7920 7468 6174 2073 686f 756c 6420 6265  y that should be
+00000fd0: 2065 7865 6375 7465 6420 6173 2061 2073   executed as a s
+00000fe0: 696e 676c 6520 7175 6572 790a 5155 4552  ingle query.QUER
+00000ff0: 595f 434f 4d50 4c45 5849 5459 5f4c 494d  Y_COMPLEXITY_LIM
+00001000: 4954 203d 2031 6537 0a23 204e 756d 6265  IT = 1e7.# Numbe
+00001010: 7220 6f66 2074 696d 6573 2074 6f20 6661  r of times to fa
+00001020: 6374 6f72 206f 7574 2073 7562 7175 6572  ctor out subquer
+00001030: 6965 7320 6265 666f 7265 2067 6976 696e  ies before givin
+00001040: 6720 7570 2e0a 4d41 585f 5355 4254 5245  g up..MAX_SUBTRE
+00001050: 455f 4641 4354 4f52 494e 4753 203d 2035  E_FACTORINGS = 5
+00001060: 0a0a 6c6f 6767 6572 203d 206c 6f67 6769  ..logger = loggi
+00001070: 6e67 2e67 6574 4c6f 6767 6572 285f 5f6e  ng.getLogger(__n
+00001080: 616d 655f 5f29 0a0a 2320 4578 636c 7564  ame__)..# Exclud
+00001090: 6573 2067 656f 6772 6170 6879 2c20 6279  es geography, by
+000010a0: 7465 732c 2061 6e64 206e 6573 7465 6420  tes, and nested 
+000010b0: 2861 7272 6179 2c20 7374 7275 6374 2920  (array, struct) 
+000010c0: 6461 7461 7479 7065 730a 494e 4c49 4e41  datatypes.INLINA
+000010d0: 424c 455f 4454 5950 4553 3a20 5365 7175  BLE_DTYPES: Sequ
+000010e0: 656e 6365 5b62 6967 6672 616d 6573 2e64  ence[bigframes.d
+000010f0: 7479 7065 732e 4474 7970 655d 203d 2028  types.Dtype] = (
+00001100: 0a20 2020 2070 616e 6461 732e 426f 6f6c  .    pandas.Bool
+00001110: 6561 6e44 7479 7065 2829 2c0a 2020 2020  eanDtype(),.    
+00001120: 7061 6e64 6173 2e46 6c6f 6174 3634 4474  pandas.Float64Dt
+00001130: 7970 6528 292c 0a20 2020 2070 616e 6461  ype(),.    panda
+00001140: 732e 496e 7436 3444 7479 7065 2829 2c0a  s.Int64Dtype(),.
+00001150: 2020 2020 7061 6e64 6173 2e53 7472 696e      pandas.Strin
+00001160: 6744 7479 7065 2873 746f 7261 6765 3d22  gDtype(storage="
+00001170: 7079 6172 726f 7722 292c 0a20 2020 2070  pyarrow"),.    p
+00001180: 616e 6461 732e 4172 726f 7744 7479 7065  andas.ArrowDtype
+00001190: 2870 612e 6461 7465 3332 2829 292c 0a20  (pa.date32()),. 
+000011a0: 2020 2070 616e 6461 732e 4172 726f 7744     pandas.ArrowD
+000011b0: 7479 7065 2870 612e 7469 6d65 3634 2822  type(pa.time64("
+000011c0: 7573 2229 292c 0a20 2020 2070 616e 6461  us")),.    panda
+000011d0: 732e 4172 726f 7744 7479 7065 2870 612e  s.ArrowDtype(pa.
+000011e0: 7469 6d65 7374 616d 7028 2275 7322 2929  timestamp("us"))
+000011f0: 2c0a 2020 2020 7061 6e64 6173 2e41 7272  ,.    pandas.Arr
+00001200: 6f77 4474 7970 6528 7061 2e74 696d 6573  owDtype(pa.times
+00001210: 7461 6d70 2822 7573 222c 2074 7a3d 2255  tamp("us", tz="U
+00001220: 5443 2229 292c 0a20 2020 2070 616e 6461  TC")),.    panda
+00001230: 732e 4172 726f 7744 7479 7065 2870 612e  s.ArrowDtype(pa.
+00001240: 6465 6369 6d61 6c31 3238 2833 382c 2039  decimal128(38, 9
+00001250: 2929 2c0a 2020 2020 7061 6e64 6173 2e41  )),.    pandas.A
+00001260: 7272 6f77 4474 7970 6528 7061 2e64 6563  rrowDtype(pa.dec
+00001270: 696d 616c 3235 3628 3736 2c20 3338 2929  imal256(76, 38))
+00001280: 2c0a 290a 0a0a 6465 6620 5f69 735f 7175  ,.)...def _is_qu
+00001290: 6572 7928 7175 6572 795f 6f72 5f74 6162  ery(query_or_tab
+000012a0: 6c65 3a20 7374 7229 202d 3e20 626f 6f6c  le: str) -> bool
+000012b0: 3a0a 2020 2020 2222 2244 6574 6572 6d69  :.    """Determi
+000012c0: 6e65 2069 6620 6071 7565 7279 5f6f 725f  ne if `query_or_
+000012d0: 7461 626c 6560 2069 7320 6120 7461 626c  table` is a tabl
+000012e0: 6520 4944 206f 7220 6120 5351 4c20 7374  e ID or a SQL st
+000012f0: 7269 6e67 2222 220a 2020 2020 7265 7475  ring""".    retu
+00001300: 726e 2072 652e 7365 6172 6368 2872 225c  rn re.search(r"\
+00001310: 7322 2c20 7175 6572 795f 6f72 5f74 6162  s", query_or_tab
+00001320: 6c65 2e73 7472 6970 2829 2c20 7265 2e4d  le.strip(), re.M
+00001330: 554c 5449 4c49 4e45 2920 6973 206e 6f74  ULTILINE) is not
+00001340: 204e 6f6e 650a 0a0a 6465 6620 5f69 735f   None...def _is_
+00001350: 7461 626c 655f 7769 7468 5f77 696c 6463  table_with_wildc
+00001360: 6172 645f 7375 6666 6978 2871 7565 7279  ard_suffix(query
+00001370: 5f6f 725f 7461 626c 653a 2073 7472 2920  _or_table: str) 
+00001380: 2d3e 2062 6f6f 6c3a 0a20 2020 2022 2222  -> bool:.    """
+00001390: 4465 7465 726d 696e 6520 6966 2060 7175  Determine if `qu
+000013a0: 6572 795f 6f72 5f74 6162 6c65 6020 6973  ery_or_table` is
+000013b0: 2061 2074 6162 6c65 2061 6e64 2063 6f6e   a table and con
+000013c0: 7461 696e 7320 6120 7769 6c64 6361 7264  tains a wildcard
+000013d0: 2073 7566 6669 782e 2222 220a 2020 2020   suffix.""".    
+000013e0: 7265 7475 726e 206e 6f74 205f 6973 5f71  return not _is_q
+000013f0: 7565 7279 2871 7565 7279 5f6f 725f 7461  uery(query_or_ta
+00001400: 626c 6529 2061 6e64 2071 7565 7279 5f6f  ble) and query_o
+00001410: 725f 7461 626c 652e 656e 6473 7769 7468  r_table.endswith
+00001420: 2822 2a22 290a 0a0a 636c 6173 7320 5365  ("*")...class Se
+00001430: 7373 696f 6e28 0a20 2020 2074 6869 7264  ssion(.    third
+00001440: 5f70 6172 7479 5f70 616e 6461 735f 6762  _party_pandas_gb
+00001450: 712e 4742 5149 4f4d 6978 696e 2c0a 2020  q.GBQIOMixin,.  
+00001460: 2020 7468 6972 645f 7061 7274 795f 7061    third_party_pa
+00001470: 6e64 6173 5f70 6172 7175 6574 2e50 6172  ndas_parquet.Par
+00001480: 7175 6574 494f 4d69 7869 6e2c 0a20 2020  quetIOMixin,.   
+00001490: 2074 6869 7264 5f70 6172 7479 5f70 616e   third_party_pan
+000014a0: 6461 735f 7069 636b 6c65 2e50 6963 6b6c  das_pickle.Pickl
+000014b0: 6549 4f4d 6978 696e 2c0a 2020 2020 7468  eIOMixin,.    th
+000014c0: 6972 645f 7061 7274 795f 7061 6e64 6173  ird_party_pandas
+000014d0: 5f72 6561 6465 7273 2e52 6561 6465 7249  _readers.ReaderI
+000014e0: 4f4d 6978 696e 2c0a 293a 0a20 2020 2022  OMixin,.):.    "
+000014f0: 2222 4573 7461 626c 6973 6865 7320 6120  ""Establishes a 
+00001500: 4269 6751 7565 7279 2063 6f6e 6e65 6374  BigQuery connect
+00001510: 696f 6e20 746f 2063 6170 7475 7265 2061  ion to capture a
+00001520: 2067 726f 7570 206f 6620 6a6f 6220 6163   group of job ac
+00001530: 7469 7669 7469 6573 2072 656c 6174 6564  tivities related
+00001540: 2074 6f0a 2020 2020 4461 7461 4672 616d   to.    DataFram
+00001550: 6573 2e0a 0a20 2020 2041 7267 733a 0a20  es...    Args:. 
+00001560: 2020 2020 2020 2063 6f6e 7465 7874 2028         context (
+00001570: 6269 6766 7261 6d65 732e 5f63 6f6e 6669  bigframes._confi
+00001580: 672e 6269 6771 7565 7279 5f6f 7074 696f  g.bigquery_optio
+00001590: 6e73 2e42 6967 5175 6572 794f 7074 696f  ns.BigQueryOptio
+000015a0: 6e73 293a 0a20 2020 2020 2020 2020 2020  ns):.           
+000015b0: 2043 6f6e 6669 6775 7261 7469 6f6e 2061   Configuration a
+000015c0: 646a 7573 7469 6e67 2068 6f77 2074 6f20  djusting how to 
+000015d0: 636f 6e6e 6563 7420 746f 2042 6967 5175  connect to BigQu
+000015e0: 6572 7920 616e 6420 7265 6c61 7465 640a  ery and related.
+000015f0: 2020 2020 2020 2020 2020 2020 4150 4973              APIs
+00001600: 2e20 4e6f 7465 2074 6861 7420 736f 6d65  . Note that some
+00001610: 206f 7074 696f 6e73 2061 7265 2069 676e   options are ign
+00001620: 6f72 6564 2069 6620 6060 636c 6965 6e74  ored if ``client
+00001630: 735f 7072 6f76 6964 6572 6060 2069 730a  s_provider`` is.
+00001640: 2020 2020 2020 2020 2020 2020 7365 742e              set.
+00001650: 0a20 2020 2020 2020 2063 6c69 656e 7473  .        clients
+00001660: 5f70 726f 7669 6465 7220 2862 6967 6672  _provider (bigfr
+00001670: 616d 6573 2e73 6573 7369 6f6e 2e63 6c69  ames.session.cli
+00001680: 656e 7473 2e43 6c69 656e 7473 5072 6f76  ents.ClientsProv
+00001690: 6964 6572 293a 0a20 2020 2020 2020 2020  ider):.         
+000016a0: 2020 2041 6e20 6f62 6a65 6374 2070 726f     An object pro
+000016b0: 7669 6469 6e67 2063 6c69 656e 7420 6c69  viding client li
+000016c0: 6272 6172 7920 6f62 6a65 6374 732e 0a20  brary objects.. 
+000016d0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+000016e0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000016f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00001700: 636f 6e74 6578 743a 204f 7074 696f 6e61  context: Optiona
+00001710: 6c5b 6269 6771 7565 7279 5f6f 7074 696f  l[bigquery_optio
+00001720: 6e73 2e42 6967 5175 6572 794f 7074 696f  ns.BigQueryOptio
+00001730: 6e73 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ns] = None,.    
+00001740: 2020 2020 636c 6965 6e74 735f 7072 6f76      clients_prov
+00001750: 6964 6572 3a20 4f70 7469 6f6e 616c 5b62  ider: Optional[b
+00001760: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00001770: 2e63 6c69 656e 7473 2e43 6c69 656e 7473  .clients.Clients
+00001780: 5072 6f76 6964 6572 5d20 3d20 4e6f 6e65  Provider] = None
+00001790: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000017a0: 2069 6620 636f 6e74 6578 7420 6973 204e   if context is N
+000017b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000017c0: 2063 6f6e 7465 7874 203d 2062 6967 7175   context = bigqu
+000017d0: 6572 795f 6f70 7469 6f6e 732e 4269 6751  ery_options.BigQ
+000017e0: 7565 7279 4f70 7469 6f6e 7328 290a 0a20  ueryOptions().. 
+000017f0: 2020 2020 2020 2023 2054 4f44 4f28 7377         # TODO(sw
+00001800: 6173 7429 3a20 4765 7420 6c6f 6361 7469  ast): Get locati
+00001810: 6f6e 2066 726f 6d20 7468 6520 656e 7669  on from the envi
+00001820: 726f 6e6d 656e 742e 0a20 2020 2020 2020  ronment..       
+00001830: 2069 6620 636f 6e74 6578 742e 6c6f 6361   if context.loca
+00001840: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+00001850: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00001860: 6c6f 6361 7469 6f6e 203d 2022 5553 220a  location = "US".
+00001870: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+00001880: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
+00001890: 2020 2020 2020 2020 2020 2066 224e 6f20             f"No 
+000018a0: 6578 706c 6963 6974 206c 6f63 6174 696f  explicit locatio
+000018b0: 6e20 6973 2073 6574 2c20 736f 2075 7369  n is set, so usi
+000018c0: 6e67 206c 6f63 6174 696f 6e20 7b73 656c  ng location {sel
+000018d0: 662e 5f6c 6f63 6174 696f 6e7d 2066 6f72  f._location} for
+000018e0: 2074 6865 2073 6573 7369 6f6e 2e22 2c0a   the session.",.
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 7374 6163 6b6c 6576 656c 3d32 2c0a 2020  stacklevel=2,.  
+00001910: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00001920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001930: 2020 2020 2020 7365 6c66 2e5f 6c6f 6361        self._loca
+00001940: 7469 6f6e 203d 2063 6f6e 7465 7874 2e6c  tion = context.l
+00001950: 6f63 6174 696f 6e0a 0a20 2020 2020 2020  ocation..       
+00001960: 2073 656c 662e 5f62 715f 6b6d 735f 6b65   self._bq_kms_ke
+00001970: 795f 6e61 6d65 203d 2063 6f6e 7465 7874  y_name = context
+00001980: 2e6b 6d73 5f6b 6579 5f6e 616d 650a 0a20  .kms_key_name.. 
+00001990: 2020 2020 2020 2023 2049 6e73 7461 6e74         # Instant
+000019a0: 6961 7465 2061 2063 6c69 656e 7473 2070  iate a clients p
+000019b0: 726f 7669 6465 7220 746f 2068 656c 7020  rovider to help 
+000019c0: 7769 7468 2063 6c6f 7564 2063 6c69 656e  with cloud clien
+000019d0: 7473 2074 6861 7420 7769 6c6c 2062 650a  ts that will be.
+000019e0: 2020 2020 2020 2020 2320 7573 6564 2069          # used i
+000019f0: 6e20 7468 6520 6675 7475 7265 206f 7065  n the future ope
+00001a00: 7261 7469 6f6e 7320 696e 2074 6865 2073  rations in the s
+00001a10: 6573 7369 6f6e 0a20 2020 2020 2020 2069  ession.        i
+00001a20: 6620 636c 6965 6e74 735f 7072 6f76 6964  f clients_provid
+00001a30: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00001a40: 7365 6c66 2e5f 636c 6965 6e74 735f 7072  self._clients_pr
+00001a50: 6f76 6964 6572 203d 2063 6c69 656e 7473  ovider = clients
+00001a60: 5f70 726f 7669 6465 720a 2020 2020 2020  _provider.      
+00001a70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001a80: 2020 2020 7365 6c66 2e5f 636c 6965 6e74      self._client
+00001a90: 735f 7072 6f76 6964 6572 203d 2062 6967  s_provider = big
+00001aa0: 6672 616d 6573 2e73 6573 7369 6f6e 2e63  frames.session.c
+00001ab0: 6c69 656e 7473 2e43 6c69 656e 7473 5072  lients.ClientsPr
+00001ac0: 6f76 6964 6572 280a 2020 2020 2020 2020  ovider(.        
+00001ad0: 2020 2020 2020 2020 7072 6f6a 6563 743d          project=
+00001ae0: 636f 6e74 6578 742e 7072 6f6a 6563 742c  context.project,
+00001af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b00: 206c 6f63 6174 696f 6e3d 7365 6c66 2e5f   location=self._
+00001b10: 6c6f 6361 7469 6f6e 2c0a 2020 2020 2020  location,.      
+00001b20: 2020 2020 2020 2020 2020 7573 655f 7265            use_re
+00001b30: 6769 6f6e 616c 5f65 6e64 706f 696e 7473  gional_endpoints
+00001b40: 3d63 6f6e 7465 7874 2e75 7365 5f72 6567  =context.use_reg
+00001b50: 696f 6e61 6c5f 656e 6470 6f69 6e74 732c  ional_endpoints,
+00001b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b70: 2063 7265 6465 6e74 6961 6c73 3d63 6f6e   credentials=con
+00001b80: 7465 7874 2e63 7265 6465 6e74 6961 6c73  text.credentials
+00001b90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ba0: 2020 6170 706c 6963 6174 696f 6e5f 6e61    application_na
+00001bb0: 6d65 3d63 6f6e 7465 7874 2e61 7070 6c69  me=context.appli
+00001bc0: 6361 7469 6f6e 5f6e 616d 652c 0a20 2020  cation_name,.   
+00001bd0: 2020 2020 2020 2020 2020 2020 2062 715f               bq_
+00001be0: 6b6d 735f 6b65 795f 6e61 6d65 3d73 656c  kms_key_name=sel
+00001bf0: 662e 5f62 715f 6b6d 735f 6b65 795f 6e61  f._bq_kms_key_na
+00001c00: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00001c10: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00001c20: 5f61 6e6f 6e79 6d6f 7573 5f64 6174 6173  _anonymous_datas
+00001c30: 6574 203d 2028 0a20 2020 2020 2020 2020  et = (.         
+00001c40: 2020 2062 6967 6672 616d 6573 2e73 6573     bigframes.ses
+00001c50: 7369 6f6e 2e5f 696f 2e62 6967 7175 6572  sion._io.bigquer
+00001c60: 792e 6372 6561 7465 5f62 715f 6461 7461  y.create_bq_data
+00001c70: 7365 745f 7265 6665 7265 6e63 6528 0a20  set_reference(. 
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001c90: 656c 662e 6271 636c 6965 6e74 2c20 6c6f  elf.bqclient, lo
+00001ca0: 6361 7469 6f6e 3d73 656c 662e 5f6c 6f63  cation=self._loc
+00001cb0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+00001cc0: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+00001cd0: 2020 2020 2020 2023 2054 4f44 4f28 7368         # TODO(sh
+00001ce0: 6f62 7329 3a20 5265 6d6f 7665 2074 6869  obs): Remove thi
+00001cf0: 7320 6c6f 6769 6320 6166 7465 7220 6874  s logic after ht
+00001d00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001d10: 2f69 6269 732d 7072 6f6a 6563 742f 6962  /ibis-project/ib
+00001d20: 6973 2f69 7373 7565 732f 3834 3934 0a20  is/issues/8494. 
+00001d30: 2020 2020 2020 2023 2068 6173 2062 6565         # has bee
+00001d40: 6e20 6669 7865 642e 2054 6865 2069 6269  n fixed. The ibi
+00001d50: 7320 636c 6965 6e74 2063 6861 6e67 6573  s client changes
+00001d60: 2074 6865 2064 6566 6175 6c74 2071 7565   the default que
+00001d70: 7279 206a 6f62 2063 6f6e 6669 670a 2020  ry job config.  
+00001d80: 2020 2020 2020 2320 736f 2077 6520 6172        # so we ar
+00001d90: 6520 676f 696e 6720 746f 2072 656d 656d  e going to remem
+00001da0: 6265 7220 7468 6520 6375 7272 656e 7420  ber the current 
+00001db0: 636f 6e66 6967 2061 6e64 2072 6573 746f  config and resto
+00001dc0: 7265 2069 7420 6166 7465 720a 2020 2020  re it after.    
+00001dd0: 2020 2020 2320 7468 6520 6962 6973 2063      # the ibis c
+00001de0: 6c69 656e 7420 6861 7320 6265 656e 2063  lient has been c
+00001df0: 7265 6174 6564 0a20 2020 2020 2020 206f  reated.        o
+00001e00: 7269 6769 6e61 6c5f 6465 6661 756c 745f  riginal_default_
+00001e10: 7175 6572 795f 6a6f 625f 636f 6e66 6967  query_job_config
+00001e20: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
+00001e30: 2e64 6566 6175 6c74 5f71 7565 7279 5f6a  .default_query_j
+00001e40: 6f62 5f63 6f6e 6669 670a 0a20 2020 2020  ob_config..     
+00001e50: 2020 2073 656c 662e 6962 6973 5f63 6c69     self.ibis_cli
+00001e60: 656e 7420 3d20 7479 7069 6e67 2e63 6173  ent = typing.cas
+00001e70: 7428 0a20 2020 2020 2020 2020 2020 2069  t(.            i
+00001e80: 6269 735f 6269 6771 7565 7279 2e42 6163  bis_bigquery.Bac
+00001e90: 6b65 6e64 2c0a 2020 2020 2020 2020 2020  kend,.          
+00001ea0: 2020 6962 6973 2e62 6967 7175 6572 792e    ibis.bigquery.
+00001eb0: 636f 6e6e 6563 7428 0a20 2020 2020 2020  connect(.       
+00001ec0: 2020 2020 2020 2020 2070 726f 6a65 6374           project
+00001ed0: 5f69 643d 636f 6e74 6578 742e 7072 6f6a  _id=context.proj
+00001ee0: 6563 742c 0a20 2020 2020 2020 2020 2020  ect,.           
+00001ef0: 2020 2020 2063 6c69 656e 743d 7365 6c66       client=self
+00001f00: 2e62 7163 6c69 656e 742c 0a20 2020 2020  .bqclient,.     
+00001f10: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+00001f20: 6765 5f63 6c69 656e 743d 7365 6c66 2e62  ge_client=self.b
+00001f30: 7173 746f 7261 6765 7265 6164 636c 6965  qstoragereadclie
+00001f40: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+00001f50: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00001f60: 2020 2020 2020 7365 6c66 2e62 7163 6c69        self.bqcli
+00001f70: 656e 742e 6465 6661 756c 745f 7175 6572  ent.default_quer
+00001f80: 795f 6a6f 625f 636f 6e66 6967 203d 206f  y_job_config = o
+00001f90: 7269 6769 6e61 6c5f 6465 6661 756c 745f  riginal_default_
+00001fa0: 7175 6572 795f 6a6f 625f 636f 6e66 6967  query_job_config
+00001fb0: 0a0a 2020 2020 2020 2020 2320 5265 736f  ..        # Reso
+00001fc0: 6c76 6520 7468 6520 4251 2063 6f6e 6e65  lve the BQ conne
+00001fd0: 6374 696f 6e20 666f 7220 7265 6d6f 7465  ction for remote
+00001fe0: 2066 756e 6374 696f 6e20 616e 6420 5665   function and Ve
+00001ff0: 7274 6578 2041 4920 696e 7465 6772 6174  rtex AI integrat
+00002000: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+00002010: 2e5f 6271 5f63 6f6e 6e65 6374 696f 6e20  ._bq_connection 
+00002020: 3d20 636f 6e74 6578 742e 6271 5f63 6f6e  = context.bq_con
+00002030: 6e65 6374 696f 6e20 6f72 205f 4249 4746  nection or _BIGF
+00002040: 5241 4d45 535f 4445 4641 554c 545f 434f  RAMES_DEFAULT_CO
+00002050: 4e4e 4543 5449 4f4e 5f49 440a 2020 2020  NNECTION_ID.    
+00002060: 2020 2020 7365 6c66 2e5f 736b 6970 5f62      self._skip_b
+00002070: 715f 636f 6e6e 6563 7469 6f6e 5f63 6865  q_connection_che
+00002080: 636b 203d 2063 6f6e 7465 7874 2e5f 736b  ck = context._sk
+00002090: 6970 5f62 715f 636f 6e6e 6563 7469 6f6e  ip_bq_connection
+000020a0: 5f63 6865 636b 0a0a 2020 2020 2020 2020  _check..        
+000020b0: 2320 4e6f 7720 7468 6174 2077 6527 7265  # Now that we're
+000020c0: 2073 7461 7274 696e 6720 7468 6520 7365   starting the se
+000020d0: 7373 696f 6e2c 2064 6f6e 2774 2061 6c6c  ssion, don't all
+000020e0: 6f77 2074 6865 206f 7074 696f 6e73 2074  ow the options t
+000020f0: 6f20 6265 0a20 2020 2020 2020 2023 2063  o be.        # c
+00002100: 6861 6e67 6564 2e0a 2020 2020 2020 2020  hanged..        
+00002110: 636f 6e74 6578 742e 5f73 6573 7369 6f6e  context._session
+00002120: 5f73 7461 7274 6564 203d 2054 7275 650a  _started = True.
+00002130: 2020 2020 2020 2020 7365 6c66 2e5f 6466          self._df
+00002140: 5f73 6e61 7073 686f 743a 2044 6963 745b  _snapshot: Dict[
+00002150: 0a20 2020 2020 2020 2020 2020 2062 6967  .            big
+00002160: 7175 6572 792e 5461 626c 6552 6566 6572  query.TableRefer
+00002170: 656e 6365 2c20 5475 706c 655b 6461 7465  ence, Tuple[date
+00002180: 7469 6d65 2e64 6174 6574 696d 652c 2062  time.datetime, b
+00002190: 6967 7175 6572 792e 5461 626c 655d 0a20  igquery.Table]. 
+000021a0: 2020 2020 2020 205d 203d 207b 7d0a 0a20         ] = {}.. 
+000021b0: 2020 2020 2020 2023 2075 6e69 7175 6520         # unique 
+000021c0: 7365 7373 696f 6e20 6964 656e 7469 6669  session identifi
+000021d0: 6572 2c20 7368 6f72 7420 656e 6f75 6768  er, short enough
+000021e0: 2074 6f20 6265 2068 756d 616e 2072 6561   to be human rea
+000021f0: 6461 626c 650a 2020 2020 2020 2020 2320  dable.        # 
+00002200: 6f6e 6c79 206e 6565 6473 2074 6f20 6265  only needs to be
+00002210: 2075 6e69 7175 6520 616d 6f6e 6720 7365   unique among se
+00002220: 7373 696f 6e73 2063 7265 6174 6564 2062  ssions created b
+00002230: 7920 7468 6520 7361 6d65 2075 7365 720a  y the same user.
+00002240: 2020 2020 2020 2020 2320 6174 2074 6865          # at the
+00002250: 2073 616d 6520 7469 6d65 2069 6e20 7468   same time in th
+00002260: 6520 7361 6d65 2072 6567 696f 6e0a 2020  e same region.  
+00002270: 2020 2020 2020 7365 6c66 2e5f 7365 7373        self._sess
+00002280: 696f 6e5f 6964 3a20 7374 7220 3d20 2273  ion_id: str = "s
+00002290: 6573 7369 6f6e 2220 2b20 7365 6372 6574  ession" + secret
+000022a0: 732e 746f 6b65 6e5f 6865 7828 3329 0a20  s.token_hex(3). 
+000022b0: 2020 2020 2020 2073 656c 662e 5f74 6162         self._tab
+000022c0: 6c65 5f69 6473 3a20 4c69 7374 5b73 7472  le_ids: List[str
+000022d0: 5d20 3d20 5b5d 0a20 2020 2020 2020 2023  ] = [].        #
+000022e0: 2073 746f 7265 2074 6162 6c65 2069 6473   store table ids
+000022f0: 2061 6e64 2064 656c 6574 6520 7468 656d   and delete them
+00002300: 2077 6865 6e20 7468 6520 7365 7373 696f   when the sessio
+00002310: 6e20 6973 2063 6c6f 7365 640a 0a20 2020  n is closed..   
+00002320: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00002330: 6566 2062 7163 6c69 656e 7428 7365 6c66  ef bqclient(self
+00002340: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002350: 6e20 7365 6c66 2e5f 636c 6965 6e74 735f  n self._clients_
+00002360: 7072 6f76 6964 6572 2e62 7163 6c69 656e  provider.bqclien
+00002370: 740a 0a20 2020 2040 7072 6f70 6572 7479  t..    @property
 00002380: 0a20 2020 2064 6566 2062 7163 6f6e 6e65  .    def bqconne
-00002390: 6374 696f 6e6d 616e 6167 6572 2873 656c  ctionmanager(sel
-000023a0: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
-000023b0: 6f74 2073 656c 662e 5f73 6b69 705f 6271  ot self._skip_bq
-000023c0: 5f63 6f6e 6e65 6374 696f 6e5f 6368 6563  _connection_chec
-000023d0: 6b20 616e 6420 6e6f 7420 7365 6c66 2e5f  k and not self._
-000023e0: 6271 5f63 6f6e 6e65 6374 696f 6e5f 6d61  bq_connection_ma
-000023f0: 6e61 6765 723a 0a20 2020 2020 2020 2020  nager:.         
-00002400: 2020 2073 656c 662e 5f62 715f 636f 6e6e     self._bq_conn
-00002410: 6563 7469 6f6e 5f6d 616e 6167 6572 203d  ection_manager =
-00002420: 2062 6967 6672 616d 6573 2e63 6c69 656e   bigframes.clien
-00002430: 7473 2e42 7143 6f6e 6e65 6374 696f 6e4d  ts.BqConnectionM
-00002440: 616e 6167 6572 280a 2020 2020 2020 2020  anager(.        
-00002450: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-00002460: 6f6e 6e65 6374 696f 6e63 6c69 656e 742c  onnectionclient,
-00002470: 2073 656c 662e 7265 736f 7572 6365 6d61   self.resourcema
-00002480: 6e61 6765 7263 6c69 656e 740a 2020 2020  nagerclient.    
-00002490: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000024a0: 2020 7265 7475 726e 2073 656c 662e 5f62    return self._b
-000024b0: 715f 636f 6e6e 6563 7469 6f6e 5f6d 616e  q_connection_man
-000024c0: 6167 6572 0a0a 2020 2020 4070 726f 7065  ager..    @prope
-000024d0: 7274 790a 2020 2020 6465 6620 5f70 726f  rty.    def _pro
-000024e0: 6a65 6374 2873 656c 6629 3a0a 2020 2020  ject(self):.    
-000024f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002500: 6271 636c 6965 6e74 2e70 726f 6a65 6374  bqclient.project
-00002510: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
-00002520: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00002530: 2020 2320 5374 6162 6c65 2068 6173 6820    # Stable hash 
-00002540: 6e65 6564 6564 2074 6f20 7573 6520 696e  needed to use in
-00002550: 2065 7870 7265 7373 696f 6e20 7472 6565   expression tree
-00002560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002570: 6861 7368 2873 7472 2873 656c 662e 5f61  hash(str(self._a
-00002580: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
-00002590: 2929 0a0a 2020 2020 6465 6620 5f63 7265  ))..    def _cre
-000025a0: 6174 655f 6271 5f64 6174 6173 6574 7328  ate_bq_datasets(
-000025b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000025c0: 2222 4372 6561 7465 2061 6e64 2069 6465  ""Create and ide
-000025d0: 6e74 6966 7920 6461 7461 7365 7428 7329  ntify dataset(s)
-000025e0: 2066 6f72 2074 656d 706f 7261 7279 2042   for temporary B
-000025f0: 5120 7265 736f 7572 6365 732e 2222 220a  Q resources.""".
-00002600: 2020 2020 2020 2020 7175 6572 795f 6a6f          query_jo
-00002610: 6220 3d20 7365 6c66 2e62 7163 6c69 656e  b = self.bqclien
-00002620: 742e 7175 6572 7928 2253 454c 4543 5420  t.query("SELECT 
-00002630: 3122 2c20 6c6f 6361 7469 6f6e 3d73 656c  1", location=sel
-00002640: 662e 5f6c 6f63 6174 696f 6e29 0a20 2020  f._location).   
-00002650: 2020 2020 2071 7565 7279 5f6a 6f62 2e72       query_job.r
-00002660: 6573 756c 7428 2920 2023 2062 6c6f 636b  esult()  # block
-00002670: 7320 756e 7469 6c20 6669 6e69 7368 6564  s until finished
-00002680: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
-00002690: 616e 6f6e 796d 6f75 7320 6461 7461 7365  anonymous datase
-000026a0: 7420 6973 2075 7365 6420 6279 2042 6967  t is used by Big
-000026b0: 5175 6572 7920 746f 2077 7269 7465 2071  Query to write q
-000026c0: 7565 7279 2072 6573 756c 7473 2061 6e64  uery results and
-000026d0: 0a20 2020 2020 2020 2023 2073 6573 7369  .        # sessi
-000026e0: 6f6e 2074 6162 6c65 732e 2042 6967 5175  on tables. BigQu
-000026f0: 6572 7920 4461 7461 4672 616d 6573 2061  ery DataFrames a
-00002700: 6c73 6f20 7772 6974 6573 2074 656d 7020  lso writes temp 
-00002710: 7461 626c 6573 2064 6972 6563 746c 790a  tables directly.
-00002720: 2020 2020 2020 2020 2320 746f 2074 6865          # to the
-00002730: 2064 6174 6173 6574 2c20 6e6f 2042 6967   dataset, no Big
-00002740: 5175 6572 7920 5365 7373 696f 6e20 7265  Query Session re
-00002750: 7175 6972 6564 2e20 4e6f 7465 3a20 7468  quired. Note: th
-00002760: 6572 6520 6973 2061 0a20 2020 2020 2020  ere is a.       
-00002770: 2023 2064 6966 6665 7265 6e74 2061 6e6f   # different ano
-00002780: 6e79 6d6f 7573 2064 6174 6173 6574 2070  nymous dataset p
-00002790: 6572 206c 6f63 6174 696f 6e2e 2053 6565  er location. See
-000027a0: 3a0a 2020 2020 2020 2020 2320 6874 7470  :.        # http
-000027b0: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
-000027c0: 2e63 6f6d 2f62 6967 7175 6572 792f 646f  .com/bigquery/do
-000027d0: 6373 2f63 6163 6865 642d 7265 7375 6c74  cs/cached-result
-000027e0: 7323 686f 775f 6361 6368 6564 5f72 6573  s#how_cached_res
-000027f0: 756c 7473 5f61 7265 5f73 746f 7265 640a  ults_are_stored.
-00002800: 2020 2020 2020 2020 7175 6572 795f 6465          query_de
-00002810: 7374 696e 6174 696f 6e20 3d20 7175 6572  stination = quer
-00002820: 795f 6a6f 622e 6465 7374 696e 6174 696f  y_job.destinatio
-00002830: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
-00002840: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
-00002850: 7420 3d20 6269 6771 7565 7279 2e44 6174  t = bigquery.Dat
-00002860: 6173 6574 5265 6665 7265 6e63 6528 0a20  asetReference(. 
-00002870: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00002880: 5f64 6573 7469 6e61 7469 6f6e 2e70 726f  _destination.pro
-00002890: 6a65 6374 2c0a 2020 2020 2020 2020 2020  ject,.          
-000028a0: 2020 7175 6572 795f 6465 7374 696e 6174    query_destinat
-000028b0: 696f 6e2e 6461 7461 7365 745f 6964 2c0a  ion.dataset_id,.
-000028c0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-000028d0: 6566 2063 6c6f 7365 2873 656c 6629 3a0a  ef close(self):.
-000028e0: 2020 2020 2020 2020 2222 224e 6f2d 6f70          """No-op
-000028f0: 2e20 5465 6d70 6f72 6172 7920 7265 736f  . Temporary reso
-00002900: 7572 6365 7320 6172 6520 6465 6c65 7465  urces are delete
-00002910: 6420 6166 7465 7220 3720 6461 7973 2e22  d after 7 days."
-00002920: 2222 0a0a 2020 2020 6465 6620 7265 6164  ""..    def read
-00002930: 5f67 6271 280a 2020 2020 2020 2020 7365  _gbq(.        se
-00002940: 6c66 2c0a 2020 2020 2020 2020 7175 6572  lf,.        quer
-00002950: 795f 6f72 5f74 6162 6c65 3a20 7374 722c  y_or_table: str,
-00002960: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00002970: 2020 2020 696e 6465 785f 636f 6c3a 2049      index_col: I
-00002980: 7465 7261 626c 655b 7374 725d 207c 2073  terable[str] | s
-00002990: 7472 203d 2028 292c 0a20 2020 2020 2020  tr = (),.       
-000029a0: 2063 6f6c 756d 6e73 3a20 4974 6572 6162   columns: Iterab
-000029b0: 6c65 5b73 7472 5d20 3d20 2829 2c0a 2020  le[str] = (),.  
-000029c0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-000029d0: 696f 6e3a 204f 7074 696f 6e61 6c5b 4469  ion: Optional[Di
-000029e0: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-000029f0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
-00002a00: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00002a10: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
-00002a20: 696c 7465 7273 3a20 7468 6972 645f 7061  ilters: third_pa
-00002a30: 7274 795f 7061 6e64 6173 5f67 6271 2e46  rty_pandas_gbq.F
-00002a40: 696c 7465 7273 5479 7065 203d 2028 292c  iltersType = (),
-00002a50: 0a20 2020 2020 2020 2075 7365 5f63 6163  .        use_cac
-00002a60: 6865 3a20 4f70 7469 6f6e 616c 5b62 6f6f  he: Optional[boo
-00002a70: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
-00002a80: 2020 2063 6f6c 5f6f 7264 6572 3a20 4974     col_order: It
-00002a90: 6572 6162 6c65 5b73 7472 5d20 3d20 2829  erable[str] = ()
-00002aa0: 2c0a 2020 2020 2020 2020 2320 4164 6420  ,.        # Add 
-00002ab0: 6120 7665 7269 6679 2069 6e64 6578 2061  a verify index a
-00002ac0: 7267 756d 656e 7420 7468 6174 2066 6169  rgument that fai
-00002ad0: 6c73 2069 6620 7468 6520 696e 6465 7820  ls if the index 
-00002ae0: 6973 206e 6f74 2075 6e69 7175 652e 0a20  is not unique.. 
-00002af0: 2020 2029 202d 3e20 6461 7461 6672 616d     ) -> datafram
-00002b00: 652e 4461 7461 4672 616d 653a 0a20 2020  e.DataFrame:.   
-00002b10: 2020 2020 2023 2054 4f44 4f28 622f 3238       # TODO(b/28
-00002b20: 3135 3731 3231 3429 3a20 4765 6e65 7261  1571214): Genera
-00002b30: 7465 2070 726f 6d70 7420 746f 2073 686f  te prompt to sho
-00002b40: 7720 7468 6520 7072 6f67 7265 7373 206f  w the progress o
-00002b50: 6620 7265 6164 5f67 6271 2e0a 2020 2020  f read_gbq..    
-00002b60: 2020 2020 6966 2063 6f6c 756d 6e73 2061      if columns a
-00002b70: 6e64 2063 6f6c 5f6f 7264 6572 3a0a 2020  nd col_order:.  
-00002b80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002b90: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00002ba0: 2020 2020 2020 2020 2020 2020 224d 7573              "Mus
-00002bb0: 7420 7370 6563 6966 7920 6569 7468 6572  t specify either
-00002bc0: 2063 6f6c 756d 6e73 2028 7072 6566 6572   columns (prefer
-00002bd0: 7265 6429 206f 7220 636f 6c5f 6f72 6465  red) or col_orde
-00002be0: 722c 206e 6f74 2062 6f74 6822 0a20 2020  r, not both".   
-00002bf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00002c00: 2020 2065 6c69 6620 636f 6c5f 6f72 6465     elif col_orde
-00002c10: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
-00002c20: 6f6c 756d 6e73 203d 2063 6f6c 5f6f 7264  olumns = col_ord
-00002c30: 6572 0a0a 2020 2020 2020 2020 6669 6c74  er..        filt
-00002c40: 6572 7320 3d20 6c69 7374 2866 696c 7465  ers = list(filte
-00002c50: 7273 290a 2020 2020 2020 2020 6966 206c  rs).        if l
-00002c60: 656e 2866 696c 7465 7273 2920 213d 2030  en(filters) != 0
-00002c70: 206f 7220 5f69 735f 7461 626c 655f 7769   or _is_table_wi
-00002c80: 7468 5f77 696c 6463 6172 645f 7375 6666  th_wildcard_suff
-00002c90: 6978 2871 7565 7279 5f6f 725f 7461 626c  ix(query_or_tabl
-00002ca0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00002cb0: 7175 6572 795f 6f72 5f74 6162 6c65 203d  query_or_table =
-00002cc0: 2073 656c 662e 5f74 6f5f 7175 6572 7928   self._to_query(
-00002cd0: 7175 6572 795f 6f72 5f74 6162 6c65 2c20  query_or_table, 
-00002ce0: 636f 6c75 6d6e 732c 2066 696c 7465 7273  columns, filters
-00002cf0: 290a 0a20 2020 2020 2020 2069 6620 5f69  )..        if _i
-00002d00: 735f 7175 6572 7928 7175 6572 795f 6f72  s_query(query_or
-00002d10: 5f74 6162 6c65 293a 0a20 2020 2020 2020  _table):.       
-00002d20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002d30: 2e5f 7265 6164 5f67 6271 5f71 7565 7279  ._read_gbq_query
-00002d40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002d50: 2020 7175 6572 795f 6f72 5f74 6162 6c65    query_or_table
-00002d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002d70: 2020 696e 6465 785f 636f 6c3d 696e 6465    index_col=inde
-00002d80: 785f 636f 6c2c 0a20 2020 2020 2020 2020  x_col,.         
-00002d90: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
-00002da0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-00002db0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00002dc0: 6174 696f 6e3d 636f 6e66 6967 7572 6174  ation=configurat
-00002dd0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00002de0: 2020 2020 206d 6178 5f72 6573 756c 7473       max_results
-00002df0: 3d6d 6178 5f72 6573 756c 7473 2c0a 2020  =max_results,.  
-00002e00: 2020 2020 2020 2020 2020 2020 2020 6170                ap
-00002e10: 695f 6e61 6d65 3d22 7265 6164 5f67 6271  i_name="read_gbq
-00002e20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002e30: 2020 2075 7365 5f63 6163 6865 3d75 7365     use_cache=use
-00002e40: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
-00002e50: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-00002e60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00002e70: 2320 544f 444f 2873 7761 7374 293a 2051  # TODO(swast): Q
-00002e80: 7565 7279 2074 6865 2073 6e61 7073 686f  uery the snapsho
-00002e90: 7420 7461 626c 6520 6275 7420 6d61 726b  t table but mark
-00002ea0: 2069 7420 6173 2061 0a20 2020 2020 2020   it as a.       
-00002eb0: 2020 2020 2023 2064 6574 6572 6d69 6e69       # determini
-00002ec0: 7374 6963 2071 7565 7279 2073 6f20 7765  stic query so we
-00002ed0: 2063 616e 2061 766f 6964 2073 6572 6961   can avoid seria
-00002ee0: 6c69 7a69 6e67 2069 6620 7765 2068 6176  lizing if we hav
-00002ef0: 6520 610a 2020 2020 2020 2020 2020 2020  e a.            
-00002f00: 2320 756e 6971 7565 2069 6e64 6578 2e0a  # unique index..
-00002f10: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00002f20: 6f6e 6669 6775 7261 7469 6f6e 2069 7320  onfiguration is 
-00002f30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002f40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00002f50: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2254 6865 2027 636f 6e66 6967 7572 6174  "The 'configurat
-00002f80: 696f 6e27 2061 7267 756d 656e 7420 6973  ion' argument is
-00002f90: 206e 6f74 2061 6c6c 6f77 6564 2077 6865   not allowed whe
-00002fa0: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
-00002fb0: 2020 2020 2020 2020 2264 6972 6563 746c          "directl
-00002fc0: 7920 7265 6164 696e 6720 6672 6f6d 2061  y reading from a
-00002fd0: 2074 6162 6c65 2e20 506c 6561 7365 2072   table. Please r
-00002fe0: 656d 6f76 6520 220a 2020 2020 2020 2020  emove ".        
-00002ff0: 2020 2020 2020 2020 2020 2020 2227 636f              "'co
-00003000: 6e66 6967 7572 6174 696f 6e27 206f 7220  nfiguration' or 
-00003010: 7573 6520 6120 7175 6572 792e 220a 2020  use a query.".  
-00003020: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00003030: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00003040: 7572 6e20 7365 6c66 2e5f 7265 6164 5f67  urn self._read_g
-00003050: 6271 5f74 6162 6c65 280a 2020 2020 2020  bq_table(.      
-00003060: 2020 2020 2020 2020 2020 7175 6572 795f            query_
-00003070: 6f72 5f74 6162 6c65 2c0a 2020 2020 2020  or_table,.      
-00003080: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-00003090: 636f 6c3d 696e 6465 785f 636f 6c2c 0a20  col=index_col,. 
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000030b0: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 2c0a  olumns=columns,.
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 6d61 785f 7265 7375 6c74 733d 6d61 785f  max_results=max_
-000030e0: 7265 7375 6c74 732c 0a20 2020 2020 2020  results,.       
-000030f0: 2020 2020 2020 2020 2061 7069 5f6e 616d           api_nam
-00003100: 653d 2272 6561 645f 6762 7122 2c0a 2020  e="read_gbq",.  
-00003110: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00003120: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
-00003130: 6520 6966 2075 7365 5f63 6163 6865 2069  e if use_cache i
-00003140: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00003150: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00003160: 2020 290a 0a20 2020 2064 6566 205f 746f    )..    def _to
-00003170: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
-00003180: 7365 6c66 2c0a 2020 2020 2020 2020 7175  self,.        qu
-00003190: 6572 795f 6f72 5f74 6162 6c65 3a20 7374  ery_or_table: st
-000031a0: 722c 0a20 2020 2020 2020 2063 6f6c 756d  r,.        colum
-000031b0: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
-000031c0: 5d2c 0a20 2020 2020 2020 2066 696c 7465  ],.        filte
-000031d0: 7273 3a20 7468 6972 645f 7061 7274 795f  rs: third_party_
-000031e0: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
-000031f0: 7273 5479 7065 2c0a 2020 2020 2920 2d3e  rsType,.    ) ->
-00003200: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-00003210: 2243 6f6d 7069 6c65 2071 7565 7279 5f6f  "Compile query_o
-00003220: 725f 7461 626c 6520 7769 7468 2063 6f6e  r_table with con
-00003230: 6469 7469 6f6e 7328 6669 6c74 6572 732c  ditions(filters,
-00003240: 2077 696c 6463 6172 6473 2920 746f 2071   wildcards) to q
-00003250: 7565 7279 2e22 2222 0a20 2020 2020 2020  uery.""".       
-00003260: 2066 696c 7465 7273 203d 206c 6973 7428   filters = list(
-00003270: 6669 6c74 6572 7329 0a20 2020 2020 2020  filters).       
-00003280: 2073 7562 5f71 7565 7279 203d 2028 0a20   sub_query = (. 
-00003290: 2020 2020 2020 2020 2020 2066 2228 7b71             f"({q
-000032a0: 7565 7279 5f6f 725f 7461 626c 657d 2922  uery_or_table})"
-000032b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000032c0: 5f69 735f 7175 6572 7928 7175 6572 795f  _is_query(query_
-000032d0: 6f72 5f74 6162 6c65 290a 2020 2020 2020  or_table).      
-000032e0: 2020 2020 2020 656c 7365 2066 2260 7b71        else f"`{q
-000032f0: 7565 7279 5f6f 725f 7461 626c 657d 6022  uery_or_table}`"
-00003300: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00003310: 2020 2020 7365 6c65 6374 5f63 6c61 7573      select_claus
-00003320: 6520 3d20 2253 454c 4543 5420 2220 2b20  e = "SELECT " + 
-00003330: 280a 2020 2020 2020 2020 2020 2020 222c  (.            ",
-00003340: 2022 2e6a 6f69 6e28 6622 607b 636f 6c75   ".join(f"`{colu
-00003350: 6d6e 7d60 2220 666f 7220 636f 6c75 6d6e  mn}`" for column
-00003360: 2069 6e20 636f 6c75 6d6e 7329 2069 6620   in columns) if 
-00003370: 636f 6c75 6d6e 7320 656c 7365 2022 2a22  columns else "*"
-00003380: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00003390: 2020 2020 7768 6572 655f 636c 6175 7365      where_clause
-000033a0: 203d 2022 220a 2020 2020 2020 2020 6966   = "".        if
-000033b0: 2066 696c 7465 7273 3a0a 2020 2020 2020   filters:.      
-000033c0: 2020 2020 2020 7661 6c69 645f 6f70 6572        valid_oper
-000033d0: 6174 6f72 733a 204d 6170 7069 6e67 5b74  ators: Mapping[t
-000033e0: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
-000033f0: 735f 6762 712e 4669 6c74 6572 4f70 732c  s_gbq.FilterOps,
-00003400: 2073 7472 5d20 3d20 7b0a 2020 2020 2020   str] = {.      
-00003410: 2020 2020 2020 2020 2020 2269 6e22 3a20            "in": 
-00003420: 2249 4e22 2c0a 2020 2020 2020 2020 2020  "IN",.          
-00003430: 2020 2020 2020 226e 6f74 2069 6e22 3a20        "not in": 
-00003440: 224e 4f54 2049 4e22 2c0a 2020 2020 2020  "NOT IN",.      
-00003450: 2020 2020 2020 2020 2020 224c 494b 4522            "LIKE"
-00003460: 3a20 224c 494b 4522 2c0a 2020 2020 2020  : "LIKE",.      
-00003470: 2020 2020 2020 2020 2020 223d 3d22 3a20            "==": 
-00003480: 223d 222c 0a20 2020 2020 2020 2020 2020  "=",.           
-00003490: 2020 2020 2022 3e22 3a20 223e 222c 0a20       ">": ">",. 
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000034b0: 3c22 3a20 223c 222c 0a20 2020 2020 2020  <": "<",.       
-000034c0: 2020 2020 2020 2020 2022 3e3d 223a 2022           ">=": "
-000034d0: 3e3d 222c 0a20 2020 2020 2020 2020 2020  >=",.           
-000034e0: 2020 2020 2022 3c3d 223a 2022 3c3d 222c       "<=": "<=",
-000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003500: 2022 213d 223a 2022 213d 222c 0a20 2020   "!=": "!=",.   
-00003510: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00003520: 2020 2020 2020 2020 2320 4966 2073 696e          # If sin
-00003530: 676c 6520 6c61 7965 7220 6669 6c74 6572  gle layer filter
-00003540: 2c20 6164 6420 616e 6f74 6865 7220 7073  , add another ps
-00003550: 6575 646f 206c 6179 6572 2e20 536f 2074  eudo layer. So t
-00003560: 6865 2073 696e 676c 6520 6c61 7965 7220  he single layer 
-00003570: 7265 7072 6573 656e 7473 2022 616e 6422  represents "and"
-00003580: 206c 6f67 6963 2e0a 2020 2020 2020 2020   logic..        
-00003590: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000035a0: 6528 6669 6c74 6572 735b 305d 2c20 7475  e(filters[0], tu
-000035b0: 706c 6529 2061 6e64 2028 0a20 2020 2020  ple) and (.     
-000035c0: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
-000035d0: 696c 7465 7273 5b30 5d29 203d 3d20 3020  ilters[0]) == 0 
-000035e0: 6f72 206e 6f74 2069 7369 6e73 7461 6e63  or not isinstanc
-000035f0: 6528 6c69 7374 2866 696c 7465 7273 5b30  e(list(filters[0
-00003600: 5d29 5b30 5d2c 2074 7570 6c65 290a 2020  ])[0], tuple).  
-00003610: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00003620: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00003630: 7465 7273 203d 2074 7970 696e 672e 6361  ters = typing.ca
-00003640: 7374 2874 6869 7264 5f70 6172 7479 5f70  st(third_party_p
-00003650: 616e 6461 735f 6762 712e 4669 6c74 6572  andas_gbq.Filter
-00003660: 7354 7970 652c 205b 6669 6c74 6572 735d  sType, [filters]
-00003670: 290a 0a20 2020 2020 2020 2020 2020 206f  )..            o
-00003680: 725f 6578 7072 6573 7369 6f6e 7320 3d20  r_expressions = 
-00003690: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-000036a0: 6f72 2067 726f 7570 2069 6e20 6669 6c74  or group in filt
-000036b0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-000036c0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-000036d0: 7374 616e 6365 2867 726f 7570 2c20 4974  stance(group, It
-000036e0: 6572 6162 6c65 293a 0a20 2020 2020 2020  erable):.       
-000036f0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-00003700: 7570 203d 205b 6772 6f75 705d 0a0a 2020  up = [group]..  
-00003710: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00003720: 645f 6578 7072 6573 7369 6f6e 7320 3d20  d_expressions = 
-00003730: 5b5d 0a20 2020 2020 2020 2020 2020 2020  [].             
-00003740: 2020 2066 6f72 2066 696c 7465 725f 6974     for filter_it
-00003750: 656d 2069 6e20 6772 6f75 703a 0a20 2020  em in group:.   
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00003780: 6365 2866 696c 7465 725f 6974 656d 2c20  ce(filter_item, 
-00003790: 7475 706c 6529 206f 7220 286c 656e 2866  tuple) or (len(f
-000037a0: 696c 7465 725f 6974 656d 2920 213d 2033  ilter_item) != 3
-000037b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000037c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000037d0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 2020 2020 2020 2020 2066 2246 696c 7465           f"Filte
-00003800: 7220 636f 6e64 6974 696f 6e20 7368 6f75  r condition shou
-00003810: 6c64 2062 6520 6120 7475 706c 6520 6f66  ld be a tuple of
-00003820: 206c 656e 6774 6820 332c 207b 6669 6c74   length 3, {filt
-00003830: 6572 5f69 7465 6d7d 2069 7320 6e6f 7420  er_item} is not 
-00003840: 7661 6c69 642e 220a 2020 2020 2020 2020  valid.".        
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003870: 2020 2020 2020 2063 6f6c 756d 6e2c 206f         column, o
-00003880: 7065 7261 746f 722c 2076 616c 7565 203d  perator, value =
-00003890: 2066 696c 7465 725f 6974 656d 0a0a 2020   filter_item..  
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-000038c0: 6e63 6528 636f 6c75 6d6e 2c20 7374 7229  nce(column, str)
-000038d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000038e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000038f0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 2020 6622 436f 6c75 6d6e          f"Column
-00003920: 206e 616d 6520 7368 6f75 6c64 2062 6520   name should be 
-00003930: 6120 7374 7269 6e67 2c20 6275 7420 7265  a string, but re
-00003940: 6365 6976 6564 2027 7b63 6f6c 756d 6e7d  ceived '{column}
-00003950: 2720 6f66 2074 7970 6520 7b74 7970 6528  ' of type {type(
-00003960: 636f 6c75 6d6e 292e 5f5f 6e61 6d65 5f5f  column).__name__
-00003970: 7d2e 220a 2020 2020 2020 2020 2020 2020  }.".            
-00003980: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2069 6620 6f70 6572 6174 6f72 206e     if operator n
-000039b0: 6f74 2069 6e20 7661 6c69 645f 6f70 6572  ot in valid_oper
-000039c0: 6174 6f72 733a 0a20 2020 2020 2020 2020  ators:.         
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000039e0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000039f0: 6622 4f70 6572 6174 6f72 207b 6f70 6572  f"Operator {oper
-00003a00: 6174 6f72 7d20 6973 206e 6f74 2076 616c  ator} is not val
-00003a10: 6964 2e22 290a 0a20 2020 2020 2020 2020  id.")..         
-00003a20: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-00003a30: 746f 725f 7374 7220 3d20 7661 6c69 645f  tor_str = valid_
-00003a40: 6f70 6572 6174 6f72 735b 6f70 6572 6174  operators[operat
-00003a50: 6f72 5d0a 0a20 2020 2020 2020 2020 2020  or]..           
-00003a60: 2020 2020 2020 2020 2069 6620 6f70 6572           if oper
-00003a70: 6174 6f72 5f73 7472 2069 6e20 5b22 494e  ator_str in ["IN
-00003a80: 222c 2022 4e4f 5420 494e 225d 3a0a 2020  ", "NOT IN"]:.  
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 7661 6c75 655f 6c69 7374        value_list
-00003ab0: 203d 2022 2c20 222e 6a6f 696e 285b 7265   = ", ".join([re
-00003ac0: 7072 2876 2920 666f 7220 7620 696e 2076  pr(v) for v in v
-00003ad0: 616c 7565 5d29 0a20 2020 2020 2020 2020  alue]).         
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003af0: 7870 7265 7373 696f 6e20 3d20 6622 607b  xpression = f"`{
-00003b00: 636f 6c75 6d6e 7d60 207b 6f70 6572 6174  column}` {operat
-00003b10: 6f72 5f73 7472 7d20 287b 7661 6c75 655f  or_str} ({value_
-00003b20: 6c69 7374 7d29 220a 2020 2020 2020 2020  list})".        
-00003b30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003b50: 2020 2020 2020 2020 2020 6578 7072 6573            expres
-00003b60: 7369 6f6e 203d 2066 2260 7b63 6f6c 756d  sion = f"`{colum
-00003b70: 6e7d 6020 7b6f 7065 7261 746f 725f 7374  n}` {operator_st
-00003b80: 727d 207b 7265 7072 2876 616c 7565 297d  r} {repr(value)}
-00003b90: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003ba0: 2020 2020 2020 616e 645f 6578 7072 6573        and_expres
-00003bb0: 7369 6f6e 732e 6170 7065 6e64 2865 7870  sions.append(exp
-00003bc0: 7265 7373 696f 6e29 0a0a 2020 2020 2020  ression)..      
-00003bd0: 2020 2020 2020 2020 2020 6f72 5f65 7870            or_exp
-00003be0: 7265 7373 696f 6e73 2e61 7070 656e 6428  ressions.append(
-00003bf0: 2220 414e 4420 222e 6a6f 696e 2861 6e64  " AND ".join(and
-00003c00: 5f65 7870 7265 7373 696f 6e73 2929 0a0a  _expressions))..
-00003c10: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00003c20: 725f 6578 7072 6573 7369 6f6e 733a 0a20  r_expressions:. 
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00003c40: 6865 7265 5f63 6c61 7573 6520 3d20 2220  here_clause = " 
-00003c50: 5748 4552 4520 2220 2b20 2220 4f52 2022  WHERE " + " OR "
-00003c60: 2e6a 6f69 6e28 6f72 5f65 7870 7265 7373  .join(or_express
-00003c70: 696f 6e73 290a 0a20 2020 2020 2020 2066  ions)..        f
-00003c80: 756c 6c5f 7175 6572 7920 3d20 6622 7b73  ull_query = f"{s
-00003c90: 656c 6563 745f 636c 6175 7365 7d20 4652  elect_clause} FR
-00003ca0: 4f4d 207b 7375 625f 7175 6572 797d 2041  OM {sub_query} A
-00003cb0: 5320 7375 627b 7768 6572 655f 636c 6175  S sub{where_clau
-00003cc0: 7365 7d22 0a20 2020 2020 2020 2072 6574  se}".        ret
-00003cd0: 7572 6e20 6675 6c6c 5f71 7565 7279 0a0a  urn full_query..
-00003ce0: 2020 2020 6465 6620 5f71 7565 7279 5f74      def _query_t
-00003cf0: 6f5f 6465 7374 696e 6174 696f 6e28 0a20  o_destination(. 
-00003d00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00003d10: 2020 2020 2071 7565 7279 3a20 7374 722c       query: str,
-00003d20: 0a20 2020 2020 2020 2069 6e64 6578 5f63  .        index_c
-00003d30: 6f6c 733a 204c 6973 745b 7374 725d 2c0a  ols: List[str],.
-00003d40: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
-00003d50: 3a20 7374 722c 0a20 2020 2020 2020 2063  : str,.        c
-00003d60: 6f6e 6669 6775 7261 7469 6f6e 3a20 6469  onfiguration: di
-00003d70: 6374 203d 207b 2271 7565 7279 223a 207b  ct = {"query": {
-00003d80: 2275 7365 5175 6572 7943 6163 6865 223a  "useQueryCache":
-00003d90: 2054 7275 657d 7d2c 0a20 2020 2020 2020   True}},.       
-00003da0: 2064 6f5f 636c 7573 7465 7269 6e67 3d54   do_clustering=T
-00003db0: 7275 652c 0a20 2020 2029 202d 3e20 5475  rue,.    ) -> Tu
-00003dc0: 706c 655b 4f70 7469 6f6e 616c 5b62 6967  ple[Optional[big
-00003dd0: 7175 6572 792e 5461 626c 6552 6566 6572  query.TableRefer
-00003de0: 656e 6365 5d2c 2062 6967 7175 6572 792e  ence], bigquery.
-00003df0: 5175 6572 794a 6f62 5d3a 0a20 2020 2020  QueryJob]:.     
-00003e00: 2020 2023 2049 6620 6120 6472 795f 7275     # If a dry_ru
-00003e10: 6e20 696e 6469 6361 7465 7320 7468 6973  n indicates this
-00003e20: 2069 7320 6e6f 7420 6120 7175 6572 7920   is not a query 
-00003e30: 7479 7065 206a 6f62 2c20 7468 656e 2064  type job, then d
-00003e40: 6f6e 2774 0a20 2020 2020 2020 2023 2062  on't.        # b
-00003e50: 6f74 6865 7220 7472 7969 6e67 2074 6f20  other trying to 
-00003e60: 646f 2061 2043 5245 4154 4520 5445 4d50  do a CREATE TEMP
-00003e70: 2054 4142 4c45 202e 2e2e 2041 5320 5345   TABLE ... AS SE
-00003e80: 4c45 4354 202e 2e2e 2073 7461 7465 6d65  LECT ... stateme
-00003e90: 6e74 2e0a 2020 2020 2020 2020 6472 795f  nt..        dry_
-00003ea0: 7275 6e5f 636f 6e66 6967 203d 2062 6967  run_config = big
-00003eb0: 7175 6572 792e 5175 6572 794a 6f62 436f  query.QueryJobCo
-00003ec0: 6e66 6967 2829 0a20 2020 2020 2020 2064  nfig().        d
-00003ed0: 7279 5f72 756e 5f63 6f6e 6669 672e 6472  ry_run_config.dr
-00003ee0: 795f 7275 6e20 3d20 5472 7565 0a20 2020  y_run = True.   
-00003ef0: 2020 2020 205f 2c20 6472 795f 7275 6e5f       _, dry_run_
-00003f00: 6a6f 6220 3d20 7365 6c66 2e5f 7374 6172  job = self._star
-00003f10: 745f 7175 6572 7928 7175 6572 792c 206a  t_query(query, j
-00003f20: 6f62 5f63 6f6e 6669 673d 6472 795f 7275  ob_config=dry_ru
-00003f30: 6e5f 636f 6e66 6967 290a 2020 2020 2020  n_config).      
-00003f40: 2020 6966 2064 7279 5f72 756e 5f6a 6f62    if dry_run_job
-00003f50: 2e73 7461 7465 6d65 6e74 5f74 7970 6520  .statement_type 
-00003f60: 213d 2022 5345 4c45 4354 223a 0a20 2020  != "SELECT":.   
-00003f70: 2020 2020 2020 2020 205f 2c20 7175 6572           _, quer
-00003f80: 795f 6a6f 6220 3d20 7365 6c66 2e5f 7374  y_job = self._st
-00003f90: 6172 745f 7175 6572 7928 7175 6572 7929  art_query(query)
-00003fa0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00003fb0: 7572 6e20 7175 6572 795f 6a6f 622e 6465  urn query_job.de
-00003fc0: 7374 696e 6174 696f 6e2c 2071 7565 7279  stination, query
-00003fd0: 5f6a 6f62 0a0a 2020 2020 2020 2020 2320  _job..        # 
-00003fe0: 4372 6561 7465 2061 2074 6162 6c65 2074  Create a table t
-00003ff0: 6f20 776f 726b 6172 6f75 6e64 2042 6967  o workaround Big
-00004000: 5175 6572 7920 3130 2047 4220 7175 6572  Query 10 GB quer
-00004010: 7920 7265 7375 6c74 7320 6c69 6d69 742e  y results limit.
-00004020: 2053 6565 3a0a 2020 2020 2020 2020 2320   See:.        # 
-00004030: 696e 7465 726e 616c 2069 7373 7565 2033  internal issue 3
-00004040: 3033 3035 3733 3336 2e0a 2020 2020 2020  03057336..      
-00004050: 2020 2320 5369 6e63 6520 7765 2068 6176    # Since we hav
-00004060: 6520 6120 6073 7461 7465 6d65 6e74 5f74  e a `statement_t
-00004070: 7970 6520 3d3d 2027 5345 4c45 4354 2760  ype == 'SELECT'`
-00004080: 2c20 7363 6865 6d61 2073 686f 756c 6420  , schema should 
-00004090: 6265 2070 6f70 756c 6174 6564 2e0a 2020  be populated..  
-000040a0: 2020 2020 2020 7363 6865 6d61 203d 2074        schema = t
-000040b0: 7970 696e 672e 6361 7374 2849 7465 7261  yping.cast(Itera
-000040c0: 626c 655b 6269 6771 7565 7279 2e53 6368  ble[bigquery.Sch
-000040d0: 656d 6146 6965 6c64 5d2c 2064 7279 5f72  emaField], dry_r
-000040e0: 756e 5f6a 6f62 2e73 6368 656d 6129 0a20  un_job.schema). 
-000040f0: 2020 2020 2020 2069 6620 646f 5f63 6c75         if do_clu
-00004100: 7374 6572 696e 673a 0a20 2020 2020 2020  stering:.       
-00004110: 2020 2020 2063 6c75 7374 6572 5f63 6f6c       cluster_col
-00004120: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00004130: 2020 2020 2020 6974 656d 2e6e 616d 650a        item.name.
-00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004150: 666f 7220 6974 656d 2069 6e20 7363 6865  for item in sche
-00004160: 6d61 0a20 2020 2020 2020 2020 2020 2020  ma.             
-00004170: 2020 2069 6620 2869 7465 6d2e 6e61 6d65     if (item.name
-00004180: 2069 6e20 696e 6465 785f 636f 6c73 2920   in index_cols) 
-00004190: 616e 6420 5f63 616e 5f63 6c75 7374 6572  and _can_cluster
-000041a0: 5f62 7128 6974 656d 290a 2020 2020 2020  _bq(item).      
-000041b0: 2020 2020 2020 5d5b 3a5f 4d41 585f 434c        ][:_MAX_CL
-000041c0: 5553 5445 525f 434f 4c55 4d4e 535d 0a20  USTER_COLUMNS]. 
-000041d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000041e0: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
-000041f0: 5f63 6f6c 7320 3d20 5b5d 0a20 2020 2020  _cols = [].     
-00004200: 2020 2074 656d 705f 7461 626c 6520 3d20     temp_table = 
-00004210: 7365 6c66 2e5f 6372 6561 7465 5f65 6d70  self._create_emp
-00004220: 7479 5f74 656d 705f 7461 626c 6528 7363  ty_temp_table(sc
-00004230: 6865 6d61 2c20 636c 7573 7465 725f 636f  hema, cluster_co
-00004240: 6c73 290a 0a20 2020 2020 2020 2074 696d  ls)..        tim
-00004250: 656f 7574 5f6d 7320 3d20 636f 6e66 6967  eout_ms = config
-00004260: 7572 6174 696f 6e2e 6765 7428 226a 6f62  uration.get("job
-00004270: 5469 6d65 6f75 744d 7322 2920 6f72 2063  TimeoutMs") or c
-00004280: 6f6e 6669 6775 7261 7469 6f6e 5b22 7175  onfiguration["qu
-00004290: 6572 7922 5d2e 6765 7428 0a20 2020 2020  ery"].get(.     
-000042a0: 2020 2020 2020 2022 7469 6d65 6f75 744d         "timeoutM
-000042b0: 7322 0a20 2020 2020 2020 2029 0a0a 2020  s".        )..  
-000042c0: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
-000042d0: 7469 6d65 6f75 745f 6d73 2074 6f20 7365  timeout_ms to se
-000042e0: 636f 6e64 732c 2065 6e73 7572 696e 6720  conds, ensuring 
-000042f0: 6120 6d69 6e69 6d75 6d20 6f66 2030 2e31  a minimum of 0.1
-00004300: 2073 6563 6f6e 6473 2074 6f20 6176 6f69   seconds to avoi
-00004310: 640a 2020 2020 2020 2020 2320 7468 6520  d.        # the 
-00004320: 7072 6f67 7261 6d20 6765 7474 696e 6720  program getting 
-00004330: 7374 7563 6b20 6f6e 2074 6f6f 2d73 686f  stuck on too-sho
-00004340: 7274 2074 696d 656f 7574 732e 0a20 2020  rt timeouts..   
-00004350: 2020 2020 2074 696d 656f 7574 203d 206d       timeout = m
-00004360: 6178 2869 6e74 2874 696d 656f 7574 5f6d  ax(int(timeout_m
-00004370: 7329 202a 2031 652d 332c 2030 2e31 2920  s) * 1e-3, 0.1) 
-00004380: 6966 2074 696d 656f 7574 5f6d 7320 656c  if timeout_ms el
-00004390: 7365 204e 6f6e 650a 0a20 2020 2020 2020  se None..       
-000043a0: 206a 6f62 5f63 6f6e 6669 6720 3d20 7479   job_config = ty
-000043b0: 7069 6e67 2e63 6173 7428 0a20 2020 2020  ping.cast(.     
-000043c0: 2020 2020 2020 2062 6967 7175 6572 792e         bigquery.
-000043d0: 5175 6572 794a 6f62 436f 6e66 6967 2c0a  QueryJobConfig,.
-000043e0: 2020 2020 2020 2020 2020 2020 6269 6771              bigq
-000043f0: 7565 7279 2e51 7565 7279 4a6f 6243 6f6e  uery.QueryJobCon
-00004400: 6669 672e 6672 6f6d 5f61 7069 5f72 6570  fig.from_api_rep
-00004410: 7228 636f 6e66 6967 7572 6174 696f 6e29  r(configuration)
-00004420: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00004430: 2020 2020 6a6f 625f 636f 6e66 6967 2e6c      job_config.l
-00004440: 6162 656c 735b 2262 6967 6672 616d 6573  abels["bigframes
-00004450: 2d61 7069 225d 203d 2061 7069 5f6e 616d  -api"] = api_nam
-00004460: 650a 2020 2020 2020 2020 6a6f 625f 636f  e.        job_co
-00004470: 6e66 6967 2e64 6573 7469 6e61 7469 6f6e  nfig.destination
-00004480: 203d 2074 656d 705f 7461 626c 650a 0a20   = temp_table.. 
-00004490: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000044a0: 2020 2020 2020 2020 2320 5772 6974 6520          # Write 
-000044b0: 746f 2074 656d 7020 7461 626c 6520 746f  to temp table to
-000044c0: 2077 6f72 6b61 726f 756e 6420 4269 6751   workaround BigQ
-000044d0: 7565 7279 2031 3020 4742 2071 7565 7279  uery 10 GB query
-000044e0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
-000044f0: 2020 2020 2023 206c 696d 6974 2e20 5365       # limit. Se
-00004500: 653a 2069 6e74 6572 6e61 6c20 6973 7375  e: internal issu
-00004510: 6520 3330 3330 3537 3333 362e 0a20 2020  e 303057336..   
-00004520: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-00004530: 6669 672e 6c61 6265 6c73 5b22 6572 726f  fig.labels["erro
-00004540: 725f 6361 7567 6874 225d 203d 2022 7472  r_caught"] = "tr
-00004550: 7565 220a 2020 2020 2020 2020 2020 2020  ue".            
-00004560: 5f2c 2071 7565 7279 5f6a 6f62 203d 2073  _, query_job = s
-00004570: 656c 662e 5f73 7461 7274 5f71 7565 7279  elf._start_query
-00004580: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004590: 2020 7175 6572 792c 206a 6f62 5f63 6f6e    query, job_con
-000045a0: 6669 673d 6a6f 625f 636f 6e66 6967 2c20  fig=job_config, 
-000045b0: 7469 6d65 6f75 743d 7469 6d65 6f75 740a  timeout=timeout.
-000045c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000045d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000045e0: 2071 7565 7279 5f6a 6f62 2e64 6573 7469   query_job.desti
-000045f0: 6e61 7469 6f6e 2c20 7175 6572 795f 6a6f  nation, query_jo
-00004600: 620a 2020 2020 2020 2020 6578 6365 7074  b.        except
-00004610: 2067 6f6f 676c 652e 6170 695f 636f 7265   google.api_core
-00004620: 2e65 7863 6570 7469 6f6e 732e 4261 6452  .exceptions.BadR
-00004630: 6571 7565 7374 3a0a 2020 2020 2020 2020  equest:.        
-00004640: 2020 2020 2320 536f 6d65 2053 454c 4543      # Some SELEC
-00004650: 5420 7374 6174 656d 656e 7473 2073 7469  T statements sti
-00004660: 6c6c 2061 7265 6e27 7420 636f 6d70 6174  ll aren't compat
-00004670: 6962 6c65 2077 6974 6820 636c 7573 7465  ible with cluste
-00004680: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
-00004690: 7461 626c 6573 2061 7320 7468 6520 6465  tables as the de
-000046a0: 7374 696e 6174 696f 6e2e 2046 6f72 2065  stination. For e
-000046b0: 7861 6d70 6c65 2c20 6966 2074 6865 2071  xample, if the q
-000046c0: 7565 7279 2068 6173 2061 0a20 2020 2020  uery has a.     
-000046d0: 2020 2020 2020 2023 2074 6f70 2d6c 6576         # top-lev
-000046e0: 656c 204f 5244 4552 2042 592c 2074 6869  el ORDER BY, thi
-000046f0: 7320 636f 6e66 6c69 6374 7320 7769 7468  s conflicts with
-00004700: 206f 7572 2061 6269 6c69 7479 2074 6f20   our ability to 
-00004710: 636c 7573 7465 720a 2020 2020 2020 2020  cluster.        
-00004720: 2020 2020 2320 7468 6520 7461 626c 6520      # the table 
-00004730: 6279 2074 6865 2069 6e64 6578 2063 6f6c  by the index col
-00004740: 756d 6e28 7329 2e0a 2020 2020 2020 2020  umn(s)..        
-00004750: 2020 2020 5f2c 2071 7565 7279 5f6a 6f62      _, query_job
-00004760: 203d 2073 656c 662e 5f73 7461 7274 5f71   = self._start_q
-00004770: 7565 7279 2871 7565 7279 2c20 7469 6d65  uery(query, time
-00004780: 6f75 743d 7469 6d65 6f75 7429 0a20 2020  out=timeout).   
-00004790: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000047a0: 7175 6572 795f 6a6f 622e 6465 7374 696e  query_job.destin
-000047b0: 6174 696f 6e2c 2071 7565 7279 5f6a 6f62  ation, query_job
-000047c0: 0a0a 2020 2020 6465 6620 7265 6164 5f67  ..    def read_g
-000047d0: 6271 5f71 7565 7279 280a 2020 2020 2020  bq_query(.      
-000047e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000047f0: 7175 6572 793a 2073 7472 2c0a 2020 2020  query: str,.    
-00004800: 2020 2020 2a2c 0a20 2020 2020 2020 2069      *,.        i
-00004810: 6e64 6578 5f63 6f6c 3a20 4974 6572 6162  ndex_col: Iterab
-00004820: 6c65 5b73 7472 5d20 7c20 7374 7220 3d20  le[str] | str = 
-00004830: 2829 2c0a 2020 2020 2020 2020 636f 6c75  (),.        colu
-00004840: 6d6e 733a 2049 7465 7261 626c 655b 7374  mns: Iterable[st
-00004850: 725d 203d 2028 292c 0a20 2020 2020 2020  r] = (),.       
-00004860: 2063 6f6e 6669 6775 7261 7469 6f6e 3a20   configuration: 
-00004870: 4f70 7469 6f6e 616c 5b44 6963 745d 203d  Optional[Dict] =
-00004880: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
-00004890: 6178 5f72 6573 756c 7473 3a20 4f70 7469  ax_results: Opti
-000048a0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000048b0: 2c0a 2020 2020 2020 2020 7573 655f 6361  ,.        use_ca
-000048c0: 6368 653a 204f 7074 696f 6e61 6c5b 626f  che: Optional[bo
-000048d0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-000048e0: 2020 2020 636f 6c5f 6f72 6465 723a 2049      col_order: I
-000048f0: 7465 7261 626c 655b 7374 725d 203d 2028  terable[str] = (
-00004900: 292c 0a20 2020 2029 202d 3e20 6461 7461  ),.    ) -> data
-00004910: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
-00004920: 0a20 2020 2020 2020 2022 2222 5475 726e  .        """Turn
-00004930: 2061 2053 514c 2071 7565 7279 2069 6e74   a SQL query int
-00004940: 6f20 6120 4461 7461 4672 616d 652e 0a0a  o a DataFrame...
-00004950: 2020 2020 2020 2020 4e6f 7465 3a20 4265          Note: Be
-00004960: 6361 7573 6520 7468 6520 7265 7375 6c74  cause the result
-00004970: 7320 6172 6520 7772 6974 7465 6e20 746f  s are written to
-00004980: 2061 2074 656d 706f 7261 7279 2074 6162   a temporary tab
-00004990: 6c65 2c20 6f72 6465 7269 6e67 2062 790a  le, ordering by.
-000049a0: 2020 2020 2020 2020 6060 4f52 4445 5220          ``ORDER 
-000049b0: 4259 6060 2069 7320 6e6f 7420 7072 6573  BY`` is not pres
-000049c0: 6572 7665 642e 2041 2075 6e69 7175 6520  erved. A unique 
-000049d0: 6069 6e64 6578 5f63 6f6c 6020 6973 2072  `index_col` is r
-000049e0: 6563 6f6d 6d65 6e64 6564 2e20 5573 650a  ecommended. Use.
-000049f0: 2020 2020 2020 2020 6060 726f 775f 6e75          ``row_nu
-00004a00: 6d62 6572 2829 206f 7665 7220 2829 6060  mber() over ()``
-00004a10: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
-00004a20: 6e61 7475 7261 6c20 756e 6971 7565 2069  natural unique i
-00004a30: 6e64 6578 206f 7220 796f 750a 2020 2020  ndex or you.    
-00004a40: 2020 2020 7761 6e74 2074 6f20 7072 6573      want to pres
-00004a50: 6572 7665 206f 7264 6572 696e 672e 0a0a  erve ordering...
-00004a60: 2020 2020 2020 2020 2a2a 4578 616d 706c          **Exampl
-00004a70: 6573 3a2a 2a0a 0a20 2020 2020 2020 2020  es:**..         
-00004a80: 2020 203e 3e3e 2069 6d70 6f72 7420 6269     >>> import bi
-00004a90: 6766 7261 6d65 732e 7061 6e64 6173 2061  gframes.pandas a
-00004aa0: 7320 6270 640a 2020 2020 2020 2020 2020  s bpd.          
-00004ab0: 2020 3e3e 3e20 6270 642e 6f70 7469 6f6e    >>> bpd.option
-00004ac0: 732e 6469 7370 6c61 792e 7072 6f67 7265  s.display.progre
-00004ad0: 7373 5f62 6172 203d 204e 6f6e 650a 0a20  ss_bar = None.. 
-00004ae0: 2020 2020 2020 2053 696d 706c 6520 7175         Simple qu
-00004af0: 6572 7920 696e 7075 743a 0a0a 2020 2020  ery input:..    
-00004b00: 2020 2020 2020 2020 3e3e 3e20 6466 203d          >>> df =
-00004b10: 2062 7064 2e72 6561 645f 6762 715f 7175   bpd.read_gbq_qu
-00004b20: 6572 7928 2727 270a 2020 2020 2020 2020  ery('''.        
-00004b30: 2020 2020 2e2e 2e20 2020 2053 454c 4543      ...    SELEC
-00004b40: 540a 2020 2020 2020 2020 2020 2020 2e2e  T.            ..
-00004b50: 2e20 2020 2020 2020 7069 7463 6865 7246  .       pitcherF
-00004b60: 6972 7374 4e61 6d65 2c0a 2020 2020 2020  irstName,.      
-00004b70: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-00004b80: 7069 7463 6865 724c 6173 744e 616d 652c  pitcherLastName,
-00004b90: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00004ba0: 2020 2020 2020 2070 6974 6368 5370 6565         pitchSpee
-00004bb0: 642c 0a20 2020 2020 2020 2020 2020 202e  d,.            .
-00004bc0: 2e2e 2020 2020 4652 4f4d 2060 6269 6771  ..    FROM `bigq
-00004bd0: 7565 7279 2d70 7562 6c69 632d 6461 7461  uery-public-data
-00004be0: 2e62 6173 6562 616c 6c2e 6761 6d65 735f  .baseball.games_
-00004bf0: 7769 6465 600a 2020 2020 2020 2020 2020  wide`.          
-00004c00: 2020 2e2e 2e20 2727 2729 0a0a 2020 2020    ... ''')..    
-00004c10: 2020 2020 5072 6573 6572 7665 206f 7264      Preserve ord
-00004c20: 6572 696e 6720 696e 2061 2071 7565 7279  ering in a query
-00004c30: 2069 6e70 7574 2e0a 0a20 2020 2020 2020   input...       
-00004c40: 2020 2020 203e 3e3e 2064 6620 3d20 6270       >>> df = bp
-00004c50: 642e 7265 6164 5f67 6271 5f71 7565 7279  d.read_gbq_query
-00004c60: 2827 2727 0a20 2020 2020 2020 2020 2020  ('''.           
-00004c70: 202e 2e2e 2020 2020 5345 4c45 4354 0a20   ...    SELECT. 
-00004c80: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00004c90: 2020 2020 202d 2d20 496e 7374 6561 6420       -- Instead 
-00004ca0: 6f66 2061 6e20 4f52 4445 5220 4259 2063  of an ORDER BY c
-00004cb0: 6c61 7573 6520 6f6e 2074 6865 2071 7565  lause on the que
-00004cc0: 7279 2c20 7573 650a 2020 2020 2020 2020  ry, use.        
-00004cd0: 2020 2020 2e2e 2e20 2020 2020 2020 2d2d      ...       --
-00004ce0: 2052 4f57 5f4e 554d 4245 5228 2920 746f   ROW_NUMBER() to
-00004cf0: 2063 7265 6174 6520 616e 206f 7264 6572   create an order
-00004d00: 6564 2044 6174 6146 7261 6d65 2e0a 2020  ed DataFrame..  
-00004d10: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004d20: 2020 2020 524f 575f 4e55 4d42 4552 2829      ROW_NUMBER()
-00004d30: 204f 5645 5220 284f 5244 4552 2042 5920   OVER (ORDER BY 
-00004d40: 4156 4728 7069 7463 6853 7065 6564 2920  AVG(pitchSpeed) 
-00004d50: 4445 5343 290a 2020 2020 2020 2020 2020  DESC).          
-00004d60: 2020 2e2e 2e20 2020 2020 2020 2020 4153    ...         AS
-00004d70: 2072 6f77 696e 6465 782c 0a20 2020 2020   rowindex,.     
-00004d80: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-00004d90: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
-00004da0: 2070 6974 6368 6572 4669 7273 744e 616d   pitcherFirstNam
-00004db0: 652c 0a20 2020 2020 2020 2020 2020 202e  e,.            .
-00004dc0: 2e2e 2020 2020 2020 2070 6974 6368 6572  ..       pitcher
-00004dd0: 4c61 7374 4e61 6d65 2c0a 2020 2020 2020  LastName,.      
-00004de0: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-00004df0: 4156 4728 7069 7463 6853 7065 6564 2920  AVG(pitchSpeed) 
-00004e00: 4153 2061 7665 7261 6765 5069 7463 6853  AS averagePitchS
-00004e10: 7065 6564 0a20 2020 2020 2020 2020 2020  peed.           
-00004e20: 202e 2e2e 2020 2020 2046 524f 4d20 6062   ...     FROM `b
-00004e30: 6967 7175 6572 792d 7075 626c 6963 2d64  igquery-public-d
-00004e40: 6174 612e 6261 7365 6261 6c6c 2e67 616d  ata.baseball.gam
-00004e50: 6573 5f77 6964 6560 0a20 2020 2020 2020  es_wide`.       
-00004e60: 2020 2020 202e 2e2e 2020 2020 2057 4845       ...     WHE
-00004e70: 5245 2079 6561 7220 3d20 3230 3136 0a20  RE year = 2016. 
-00004e80: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00004e90: 2020 2047 524f 5550 2042 5920 7069 7463     GROUP BY pitc
-00004ea0: 6865 7246 6972 7374 4e61 6d65 2c20 7069  herFirstName, pi
-00004eb0: 7463 6865 724c 6173 744e 616d 650a 2020  tcherLastName.  
-00004ec0: 2020 2020 2020 2020 2020 2e2e 2e20 2727            ... ''
-00004ed0: 272c 2069 6e64 6578 5f63 6f6c 3d22 726f  ', index_col="ro
-00004ee0: 7769 6e64 6578 2229 0a20 2020 2020 2020  windex").       
-00004ef0: 2020 2020 203e 3e3e 2064 662e 6865 6164       >>> df.head
-00004f00: 2832 290a 2020 2020 2020 2020 2020 2020  (2).            
-00004f10: 2020 2020 2020 2020 2070 6974 6368 6572           pitcher
-00004f20: 4669 7273 744e 616d 6520 7069 7463 6865  FirstName pitche
-00004f30: 724c 6173 744e 616d 6520 2061 7665 7261  rLastName  avera
-00004f40: 6765 5069 7463 6853 7065 6564 0a20 2020  gePitchSpeed.   
-00004f50: 2020 2020 2020 2020 2072 6f77 696e 6465           rowinde
-00004f60: 780a 2020 2020 2020 2020 2020 2020 3120  x.            1 
-00004f70: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00004f80: 6c62 6572 7469 6e20 2020 2020 2020 2020  lbertin         
-00004f90: 4368 6170 6d61 6e20 2020 2020 2020 2020  Chapman         
-00004fa0: 2039 362e 3531 3431 3133 0a20 2020 2020   96.514113.     
-00004fb0: 2020 2020 2020 2032 2020 2020 2020 2020         2        
-00004fc0: 2020 2020 2020 2020 205a 6163 6861 7279           Zachary
-00004fd0: 2020 2020 2020 2020 2042 7269 7474 6f6e           Britton
-00004fe0: 2020 2020 2020 2020 2020 3934 2e35 3931            94.591
-00004ff0: 3033 390a 2020 2020 2020 2020 2020 2020  039.            
-00005000: 3c42 4c41 4e4b 4c49 4e45 3e0a 2020 2020  <BLANKLINE>.    
-00005010: 2020 2020 2020 2020 5b32 2072 6f77 7320          [2 rows 
-00005020: 7820 3320 636f 6c75 6d6e 735d 0a0a 2020  x 3 columns]..  
-00005030: 2020 2020 2020 5365 6520 616c 736f 3a20        See also: 
-00005040: 3a6d 6574 683a 6053 6573 7369 6f6e 2e72  :meth:`Session.r
-00005050: 6561 645f 6762 7160 2e0a 2020 2020 2020  ead_gbq`..      
-00005060: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-00005070: 4e4f 5445 3a20 5468 6973 206d 6574 686f  NOTE: This metho
-00005080: 6420 646f 6573 6e27 7420 2879 6574 2920  d doesn't (yet) 
-00005090: 6578 6973 7420 696e 2070 616e 6461 7320  exist in pandas 
-000050a0: 6f72 2070 616e 6461 732d 6762 712c 2073  or pandas-gbq, s
-000050b0: 6f0a 2020 2020 2020 2020 2320 7468 6573  o.        # thes
-000050c0: 6520 646f 6373 7472 696e 6773 2061 7265  e docstrings are
-000050d0: 2069 6e6c 696e 652e 0a20 2020 2020 2020   inline..       
-000050e0: 2069 6620 636f 6c75 6d6e 7320 616e 6420   if columns and 
-000050f0: 636f 6c5f 6f72 6465 723a 0a20 2020 2020  col_order:.     
-00005100: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00005110: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00005120: 2020 2020 2020 2020 2022 4d75 7374 2073           "Must s
-00005130: 7065 6369 6679 2065 6974 6865 7220 636f  pecify either co
-00005140: 6c75 6d6e 7320 2870 7265 6665 7272 6564  lumns (preferred
-00005150: 2920 6f72 2063 6f6c 5f6f 7264 6572 2c20  ) or col_order, 
-00005160: 6e6f 7420 626f 7468 220a 2020 2020 2020  not both".      
-00005170: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005180: 656c 6966 2063 6f6c 5f6f 7264 6572 3a0a  elif col_order:.
-00005190: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-000051a0: 6d6e 7320 3d20 636f 6c5f 6f72 6465 720a  mns = col_order.
-000051b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000051c0: 7365 6c66 2e5f 7265 6164 5f67 6271 5f71  self._read_gbq_q
-000051d0: 7565 7279 280a 2020 2020 2020 2020 2020  uery(.          
-000051e0: 2020 7175 6572 793d 7175 6572 792c 0a20    query=query,. 
-000051f0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00005200: 5f63 6f6c 3d69 6e64 6578 5f63 6f6c 2c0a  _col=index_col,.
-00005210: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00005220: 6d6e 733d 636f 6c75 6d6e 732c 0a20 2020  mns=columns,.   
-00005230: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
-00005240: 7261 7469 6f6e 3d63 6f6e 6669 6775 7261  ration=configura
-00005250: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00005260: 2020 6d61 785f 7265 7375 6c74 733d 6d61    max_results=ma
-00005270: 785f 7265 7375 6c74 732c 0a20 2020 2020  x_results,.     
-00005280: 2020 2020 2020 2061 7069 5f6e 616d 653d         api_name=
-00005290: 2272 6561 645f 6762 715f 7175 6572 7922  "read_gbq_query"
-000052a0: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-000052b0: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
-000052c0: 652c 0a20 2020 2020 2020 2029 0a0a 2020  e,.        )..  
-000052d0: 2020 6465 6620 5f72 6561 645f 6762 715f    def _read_gbq_
-000052e0: 7175 6572 7928 0a20 2020 2020 2020 2073  query(.        s
-000052f0: 656c 662c 0a20 2020 2020 2020 2071 7565  elf,.        que
-00005300: 7279 3a20 7374 722c 0a20 2020 2020 2020  ry: str,.       
-00005310: 202a 2c0a 2020 2020 2020 2020 696e 6465   *,.        inde
-00005320: 785f 636f 6c3a 2049 7465 7261 626c 655b  x_col: Iterable[
-00005330: 7374 725d 207c 2073 7472 203d 2028 292c  str] | str = (),
-00005340: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-00005350: 3a20 4974 6572 6162 6c65 5b73 7472 5d20  : Iterable[str] 
-00005360: 3d20 2829 2c0a 2020 2020 2020 2020 636f  = (),.        co
-00005370: 6e66 6967 7572 6174 696f 6e3a 204f 7074  nfiguration: Opt
-00005380: 696f 6e61 6c5b 4469 6374 5d20 3d20 4e6f  ional[Dict] = No
-00005390: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
-000053a0: 7265 7375 6c74 733a 204f 7074 696f 6e61  results: Optiona
-000053b0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
-000053c0: 2020 2020 2020 2061 7069 5f6e 616d 653a         api_name:
-000053d0: 2073 7472 203d 2022 7265 6164 5f67 6271   str = "read_gbq
-000053e0: 5f71 7565 7279 222c 0a20 2020 2020 2020  _query",.       
-000053f0: 2075 7365 5f63 6163 6865 3a20 4f70 7469   use_cache: Opti
-00005400: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00005410: 652c 0a20 2020 2029 202d 3e20 6461 7461  e,.    ) -> data
-00005420: 6672 616d 652e 4461 7461 4672 616d 653a  frame.DataFrame:
-00005430: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00005440: 6269 6766 7261 6d65 732e 6461 7461 6672  bigframes.datafr
-00005450: 616d 6520 6173 2064 6174 6166 7261 6d65  ame as dataframe
-00005460: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-00005470: 7572 6174 696f 6e20 3d20 5f74 7261 6e73  uration = _trans
-00005480: 666f 726d 5f72 6561 645f 6762 715f 636f  form_read_gbq_co
-00005490: 6e66 6967 7572 6174 696f 6e28 636f 6e66  nfiguration(conf
-000054a0: 6967 7572 6174 696f 6e29 0a0a 2020 2020  iguration)..    
-000054b0: 2020 2020 6966 2022 7175 6572 7922 206e      if "query" n
-000054c0: 6f74 2069 6e20 636f 6e66 6967 7572 6174  ot in configurat
-000054d0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-000054e0: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
-000054f0: 7175 6572 7922 5d20 3d20 7b7d 0a0a 2020  query"] = {}..  
-00005500: 2020 2020 2020 6966 2022 7175 6572 7922        if "query"
-00005510: 2069 6e20 636f 6e66 6967 7572 6174 696f   in configuratio
-00005520: 6e5b 2271 7565 7279 225d 3a0a 2020 2020  n["query"]:.    
-00005530: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00005540: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00005550: 2020 2020 2020 2020 2020 2254 6865 2071            "The q
-00005560: 7565 7279 2073 7461 7465 6d65 6e74 206d  uery statement m
-00005570: 7573 7420 6e6f 7420 6265 2069 6e63 6c75  ust not be inclu
-00005580: 6465 6420 696e 2074 6865 2022 2c0a 2020  ded in the ",.  
-00005590: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-000055a0: 636f 6e66 6967 7572 6174 696f 6e27 2062  configuration' b
-000055b0: 6563 6175 7365 2069 7420 6973 2061 6c72  ecause it is alr
-000055c0: 6561 6479 2070 726f 7669 6465 6420 6173  eady provided as
-000055d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000055e0: 2020 2022 2061 2073 6570 6172 6174 6520     " a separate 
-000055f0: 7061 7261 6d65 7465 722e 222c 0a20 2020  parameter.",.   
-00005600: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00005610: 2020 2020 6966 2022 7573 6551 7565 7279      if "useQuery
-00005620: 4361 6368 6522 2069 6e20 636f 6e66 6967  Cache" in config
-00005630: 7572 6174 696f 6e5b 2271 7565 7279 225d  uration["query"]
-00005640: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005650: 2075 7365 5f63 6163 6865 2069 7320 6e6f   use_cache is no
-00005660: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00005670: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00005680: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00005690: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-000056a0: 7573 6551 7565 7279 4361 6368 6527 2069  useQueryCache' i
-000056b0: 6e20 2763 6f6e 6669 6775 7261 7469 6f6e  n 'configuration
-000056c0: 2720 636f 6e66 6c69 6374 7320 7769 7468  ' conflicts with
-000056d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000056e0: 2020 2020 2020 2220 2775 7365 5f63 6163        " 'use_cac
-000056f0: 6865 2720 7061 7261 6d65 7465 722e 2050  he' parameter. P
-00005700: 6c65 6173 6520 7370 6563 6966 7920 6f6e  lease specify on
-00005710: 6c79 206f 6e65 2e22 0a20 2020 2020 2020  ly one.".       
-00005720: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00005730: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005740: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-00005750: 6f6e 5b22 7175 6572 7922 5d5b 2275 7365  on["query"]["use
-00005760: 5175 6572 7943 6163 6865 225d 203d 2028  QueryCache"] = (
-00005770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005780: 2054 7275 6520 6966 2075 7365 5f63 6163   True if use_cac
-00005790: 6865 2069 7320 4e6f 6e65 2065 6c73 6520  he is None else 
-000057a0: 7573 655f 6361 6368 650a 2020 2020 2020  use_cache.      
-000057b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000057c0: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
-000057d0: 6e64 6578 5f63 6f6c 2c20 7374 7229 3a0a  ndex_col, str):.
-000057e0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-000057f0: 785f 636f 6c73 203d 205b 696e 6465 785f  x_cols = [index_
-00005800: 636f 6c5d 0a20 2020 2020 2020 2065 6c73  col].        els
-00005810: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00005820: 6e64 6578 5f63 6f6c 7320 3d20 6c69 7374  ndex_cols = list
-00005830: 2869 6e64 6578 5f63 6f6c 290a 0a20 2020  (index_col)..   
-00005840: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00005850: 2c20 7175 6572 795f 6a6f 6220 3d20 7365  , query_job = se
-00005860: 6c66 2e5f 7175 6572 795f 746f 5f64 6573  lf._query_to_des
-00005870: 7469 6e61 7469 6f6e 280a 2020 2020 2020  tination(.      
-00005880: 2020 2020 2020 7175 6572 792c 0a20 2020        query,.   
-00005890: 2020 2020 2020 2020 2069 6e64 6578 5f63           index_c
-000058a0: 6f6c 732c 0a20 2020 2020 2020 2020 2020  ols,.           
-000058b0: 2061 7069 5f6e 616d 653d 6170 695f 6e61   api_name=api_na
-000058c0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000058d0: 636f 6e66 6967 7572 6174 696f 6e3d 636f  configuration=co
-000058e0: 6e66 6967 7572 6174 696f 6e2c 0a20 2020  nfiguration,.   
-000058f0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00005900: 2320 4966 2074 6865 7265 2077 6173 206e  # If there was n
-00005910: 6f20 6465 7374 696e 6174 696f 6e20 7461  o destination ta
-00005920: 626c 652c 2074 6861 7420 6d65 616e 7320  ble, that means 
-00005930: 7468 6520 7175 6572 7920 6d75 7374 2068  the query must h
-00005940: 6176 650a 2020 2020 2020 2020 2320 6265  ave.        # be
-00005950: 656e 2044 444c 206f 7220 444d 4c2e 2052  en DDL or DML. R
-00005960: 6574 7572 6e20 736f 6d65 206a 6f62 206d  eturn some job m
-00005970: 6574 6164 6174 612c 2069 6e73 7465 6164  etadata, instead
-00005980: 2e0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00005990: 2064 6573 7469 6e61 7469 6f6e 3a0a 2020   destination:.  
-000059a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000059b0: 2064 6174 6166 7261 6d65 2e44 6174 6146   dataframe.DataF
-000059c0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
-000059d0: 2020 2020 2020 6461 7461 3d70 616e 6461        data=panda
-000059e0: 732e 4461 7461 4672 616d 6528 0a20 2020  s.DataFrame(.   
-000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00005a10: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
-00005a20: 656d 656e 745f 7479 7065 223a 205b 0a20  ement_type": [. 
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a40: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00005a50: 5f6a 6f62 2e73 7461 7465 6d65 6e74 5f74  _job.statement_t
-00005a60: 7970 6520 6966 2071 7565 7279 5f6a 6f62  ype if query_job
-00005a70: 2065 6c73 6520 2275 6e6b 6e6f 776e 220a   else "unknown".
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2022 6a6f 625f 6964 223a 205b 7175     "job_id": [qu
-00005ac0: 6572 795f 6a6f 622e 6a6f 625f 6964 2069  ery_job.job_id i
-00005ad0: 6620 7175 6572 795f 6a6f 6220 656c 7365  f query_job else
-00005ae0: 2022 756e 6b6e 6f77 6e22 5d2c 0a20 2020   "unknown"],.   
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2022 6c6f 6361 7469 6f6e 223a       "location":
-00005b10: 205b 7175 6572 795f 6a6f 622e 6c6f 6361   [query_job.loca
-00005b20: 7469 6f6e 2069 6620 7175 6572 795f 6a6f  tion if query_jo
-00005b30: 6220 656c 7365 2022 756e 6b6e 6f77 6e22  b else "unknown"
-00005b40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00005b50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00005b60: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00005b70: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-00005b80: 696f 6e3d 7365 6c66 2c0a 2020 2020 2020  ion=self,.      
-00005b90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00005ba0: 2072 6574 7572 6e20 7365 6c66 2e72 6561   return self.rea
-00005bb0: 645f 6762 715f 7461 626c 6528 0a20 2020  d_gbq_table(.   
-00005bc0: 2020 2020 2020 2020 2066 227b 6465 7374           f"{dest
-00005bd0: 696e 6174 696f 6e2e 7072 6f6a 6563 747d  ination.project}
-00005be0: 2e7b 6465 7374 696e 6174 696f 6e2e 6461  .{destination.da
-00005bf0: 7461 7365 745f 6964 7d2e 7b64 6573 7469  taset_id}.{desti
-00005c00: 6e61 7469 6f6e 2e74 6162 6c65 5f69 647d  nation.table_id}
-00005c10: 222c 0a20 2020 2020 2020 2020 2020 2069  ",.            i
-00005c20: 6e64 6578 5f63 6f6c 3d69 6e64 6578 5f63  ndex_col=index_c
-00005c30: 6f6c 732c 0a20 2020 2020 2020 2020 2020  ols,.           
-00005c40: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-00005c50: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00005c60: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
-00005c70: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
-00005c80: 2020 2075 7365 5f63 6163 6865 3d63 6f6e     use_cache=con
-00005c90: 6669 6775 7261 7469 6f6e 5b22 7175 6572  figuration["quer
-00005ca0: 7922 5d5b 2275 7365 5175 6572 7943 6163  y"]["useQueryCac
-00005cb0: 6865 225d 2c0a 2020 2020 2020 2020 290a  he"],.        ).
-00005cc0: 0a20 2020 2064 6566 2072 6561 645f 6762  .    def read_gb
-00005cd0: 715f 7461 626c 6528 0a20 2020 2020 2020  q_table(.       
-00005ce0: 2073 656c 662c 0a20 2020 2020 2020 2071   self,.        q
-00005cf0: 7565 7279 3a20 7374 722c 0a20 2020 2020  uery: str,.     
-00005d00: 2020 202a 2c0a 2020 2020 2020 2020 696e     *,.        in
-00005d10: 6465 785f 636f 6c3a 2049 7465 7261 626c  dex_col: Iterabl
-00005d20: 655b 7374 725d 207c 2073 7472 203d 2028  e[str] | str = (
-00005d30: 292c 0a20 2020 2020 2020 2063 6f6c 756d  ),.        colum
-00005d40: 6e73 3a20 4974 6572 6162 6c65 5b73 7472  ns: Iterable[str
-00005d50: 5d20 3d20 2829 2c0a 2020 2020 2020 2020  ] = (),.        
-00005d60: 6d61 785f 7265 7375 6c74 733a 204f 7074  max_results: Opt
-00005d70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00005d80: 652c 0a20 2020 2020 2020 2066 696c 7465  e,.        filte
-00005d90: 7273 3a20 7468 6972 645f 7061 7274 795f  rs: third_party_
-00005da0: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
-00005db0: 7273 5479 7065 203d 2028 292c 0a20 2020  rsType = (),.   
-00005dc0: 2020 2020 2075 7365 5f63 6163 6865 3a20       use_cache: 
-00005dd0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-00005de0: 2020 2020 2063 6f6c 5f6f 7264 6572 3a20       col_order: 
-00005df0: 4974 6572 6162 6c65 5b73 7472 5d20 3d20  Iterable[str] = 
-00005e00: 2829 2c0a 2020 2020 2920 2d3e 2064 6174  (),.    ) -> dat
-00005e10: 6166 7261 6d65 2e44 6174 6146 7261 6d65  aframe.DataFrame
-00005e20: 3a0a 2020 2020 2020 2020 2222 2254 7572  :.        """Tur
-00005e30: 6e20 6120 4269 6751 7565 7279 2074 6162  n a BigQuery tab
-00005e40: 6c65 2069 6e74 6f20 6120 4461 7461 4672  le into a DataFr
-00005e50: 616d 652e 0a0a 2020 2020 2020 2020 2a2a  ame...        **
-00005e60: 4578 616d 706c 6573 3a2a 2a0a 0a20 2020  Examples:**..   
-00005e70: 2020 2020 2020 2020 203e 3e3e 2069 6d70           >>> imp
-00005e80: 6f72 7420 6269 6766 7261 6d65 732e 7061  ort bigframes.pa
-00005e90: 6e64 6173 2061 7320 6270 640a 2020 2020  ndas as bpd.    
-00005ea0: 2020 2020 2020 2020 3e3e 3e20 6270 642e          >>> bpd.
-00005eb0: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
-00005ec0: 7072 6f67 7265 7373 5f62 6172 203d 204e  progress_bar = N
-00005ed0: 6f6e 650a 0a20 2020 2020 2020 2052 6561  one..        Rea
-00005ee0: 6420 6120 7768 6f6c 6520 7461 626c 652c  d a whole table,
-00005ef0: 2077 6974 6820 6172 6269 7472 6172 7920   with arbitrary 
-00005f00: 6f72 6465 7269 6e67 206f 7220 6f72 6465  ordering or orde
-00005f10: 7269 6e67 2063 6f72 7265 7370 6f6e 6469  ring correspondi
-00005f20: 6e67 2074 6f20 7468 6520 7072 696d 6172  ng to the primar
-00005f30: 7920 6b65 7928 7329 2e0a 0a20 2020 2020  y key(s)...     
-00005f40: 2020 2020 2020 203e 3e3e 2064 6620 3d20         >>> df = 
-00005f50: 6270 642e 7265 6164 5f67 6271 5f74 6162  bpd.read_gbq_tab
-00005f60: 6c65 2822 6269 6771 7565 7279 2d70 7562  le("bigquery-pub
-00005f70: 6c69 632d 6461 7461 2e6d 6c5f 6461 7461  lic-data.ml_data
-00005f80: 7365 7473 2e70 656e 6775 696e 7322 290a  sets.penguins").
-00005f90: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
-00005fa0: 6f3a 203a 6d65 7468 3a60 5365 7373 696f  o: :meth:`Sessio
-00005fb0: 6e2e 7265 6164 5f67 6271 602e 0a20 2020  n.read_gbq`..   
-00005fc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005fd0: 2023 204e 4f54 453a 2054 6869 7320 6d65   # NOTE: This me
-00005fe0: 7468 6f64 2064 6f65 736e 2774 2028 7965  thod doesn't (ye
-00005ff0: 7429 2065 7869 7374 2069 6e20 7061 6e64  t) exist in pand
-00006000: 6173 206f 7220 7061 6e64 6173 2d67 6271  as or pandas-gbq
-00006010: 2c20 736f 0a20 2020 2020 2020 2023 2074  , so.        # t
-00006020: 6865 7365 2064 6f63 7374 7269 6e67 7320  hese docstrings 
-00006030: 6172 6520 696e 6c69 6e65 2e0a 2020 2020  are inline..    
-00006040: 2020 2020 6966 2063 6f6c 756d 6e73 2061      if columns a
-00006050: 6e64 2063 6f6c 5f6f 7264 6572 3a0a 2020  nd col_order:.  
-00006060: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006070: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00006080: 2020 2020 2020 2020 2020 2020 224d 7573              "Mus
-00006090: 7420 7370 6563 6966 7920 6569 7468 6572  t specify either
-000060a0: 2063 6f6c 756d 6e73 2028 7072 6566 6572   columns (prefer
-000060b0: 7265 6429 206f 7220 636f 6c5f 6f72 6465  red) or col_orde
-000060c0: 722c 206e 6f74 2062 6f74 6822 0a20 2020  r, not both".   
-000060d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000060e0: 2020 2065 6c69 6620 636f 6c5f 6f72 6465     elif col_orde
-000060f0: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
-00006100: 6f6c 756d 6e73 203d 2063 6f6c 5f6f 7264  olumns = col_ord
-00006110: 6572 0a0a 2020 2020 2020 2020 6669 6c74  er..        filt
-00006120: 6572 7320 3d20 6c69 7374 2866 696c 7465  ers = list(filte
-00006130: 7273 290a 2020 2020 2020 2020 6966 206c  rs).        if l
-00006140: 656e 2866 696c 7465 7273 2920 213d 2030  en(filters) != 0
-00006150: 206f 7220 5f69 735f 7461 626c 655f 7769   or _is_table_wi
-00006160: 7468 5f77 696c 6463 6172 645f 7375 6666  th_wildcard_suff
-00006170: 6978 2871 7565 7279 293a 0a20 2020 2020  ix(query):.     
-00006180: 2020 2020 2020 2071 7565 7279 203d 2073         query = s
-00006190: 656c 662e 5f74 6f5f 7175 6572 7928 7175  elf._to_query(qu
-000061a0: 6572 792c 2063 6f6c 756d 6e73 2c20 6669  ery, columns, fi
-000061b0: 6c74 6572 7329 0a0a 2020 2020 2020 2020  lters)..        
-000061c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000061d0: 5f72 6561 645f 6762 715f 7175 6572 7928  _read_gbq_query(
-000061e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000061f0: 2071 7565 7279 2c0a 2020 2020 2020 2020   query,.        
-00006200: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
-00006210: 6c3d 696e 6465 785f 636f 6c2c 0a20 2020  l=index_col,.   
-00006220: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00006230: 756d 6e73 3d63 6f6c 756d 6e73 2c0a 2020  umns=columns,.  
-00006240: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00006250: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
-00006260: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
-00006270: 2020 2020 2020 2061 7069 5f6e 616d 653d         api_name=
-00006280: 2272 6561 645f 6762 715f 7461 626c 6522  "read_gbq_table"
-00006290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000062a0: 2020 7573 655f 6361 6368 653d 7573 655f    use_cache=use_
-000062b0: 6361 6368 652c 0a20 2020 2020 2020 2020  cache,.         
-000062c0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-000062d0: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
-000062e0: 6762 715f 7461 626c 6528 0a20 2020 2020  gbq_table(.     
-000062f0: 2020 2020 2020 2071 7565 7279 3d71 7565         query=que
-00006300: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-00006310: 696e 6465 785f 636f 6c3d 696e 6465 785f  index_col=index_
-00006320: 636f 6c2c 0a20 2020 2020 2020 2020 2020  col,.           
-00006330: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-00006340: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00006350: 785f 7265 7375 6c74 733d 6d61 785f 7265  x_results=max_re
-00006360: 7375 6c74 732c 0a20 2020 2020 2020 2020  sults,.         
-00006370: 2020 2061 7069 5f6e 616d 653d 2272 6561     api_name="rea
-00006380: 645f 6762 715f 7461 626c 6522 2c0a 2020  d_gbq_table",.  
-00006390: 2020 2020 2020 2020 2020 7573 655f 6361            use_ca
-000063a0: 6368 653d 7573 655f 6361 6368 652c 0a20  che=use_cache,. 
-000063b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-000063c0: 6620 5f67 6574 5f73 6e61 7073 686f 745f  f _get_snapshot_
-000063d0: 7371 6c5f 616e 645f 7072 696d 6172 795f  sql_and_primary_
-000063e0: 6b65 7928 0a20 2020 2020 2020 2073 656c  key(.        sel
-000063f0: 662c 0a20 2020 2020 2020 2074 6162 6c65  f,.        table
-00006400: 3a20 676f 6f67 6c65 2e63 6c6f 7564 2e62  : google.cloud.b
-00006410: 6967 7175 6572 792e 7461 626c 652e 5461  igquery.table.Ta
-00006420: 626c 652c 0a20 2020 2020 2020 202a 2c0a  ble,.        *,.
-00006430: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
-00006440: 3a20 7374 722c 0a20 2020 2020 2020 2075  : str,.        u
-00006450: 7365 5f63 6163 6865 3a20 626f 6f6c 203d  se_cache: bool =
-00006460: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
-00006470: 5475 706c 655b 6962 6973 5f74 7970 6573  Tuple[ibis_types
-00006480: 2e54 6162 6c65 2c20 4f70 7469 6f6e 616c  .Table, Optional
-00006490: 5b53 6571 7565 6e63 655b 7374 725d 5d5d  [Sequence[str]]]
-000064a0: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
-000064b0: 6174 6520 6120 7265 6164 2d6f 6e6c 7920  ate a read-only 
-000064c0: 4962 6973 2074 6162 6c65 2065 7870 7265  Ibis table expre
-000064d0: 7373 696f 6e20 7265 7072 6573 656e 7469  ssion representi
-000064e0: 6e67 2061 2074 6162 6c65 2e0a 0a20 2020  ng a table...   
-000064f0: 2020 2020 2049 6620 7765 2063 616e 2067       If we can g
-00006500: 6574 2061 2074 6f74 616c 206f 7264 6572  et a total order
-00006510: 696e 6720 6672 6f6d 2074 6865 2074 6162  ing from the tab
-00006520: 6c65 2c20 7375 6368 2061 7320 7669 6120  le, such as via 
-00006530: 7072 696d 6172 7920 6b65 790a 2020 2020  primary key.    
-00006540: 2020 2020 636f 6c75 6d6e 2873 292c 2074      column(s), t
-00006550: 6865 6e20 7265 7475 726e 2074 686f 7365  hen return those
-00006560: 2074 6f6f 2073 6f20 7468 6174 206f 7264   too so that ord
-00006570: 6572 696e 6720 6765 6e65 7261 7469 6f6e  ering generation
-00006580: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
-00006590: 6176 6f69 6465 642e 0a20 2020 2020 2020  avoided..       
-000065a0: 2022 2222 0a20 2020 2020 2020 2028 0a20   """.        (. 
-000065b0: 2020 2020 2020 2020 2020 2073 6e61 7073             snaps
-000065c0: 686f 745f 7469 6d65 7374 616d 702c 0a20  hot_timestamp,. 
-000065d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-000065e0: 2c0a 2020 2020 2020 2020 2920 3d20 6269  ,.        ) = bi
-000065f0: 6766 7261 6d65 735f 696f 2e67 6574 5f73  gframes_io.get_s
-00006600: 6e61 7073 686f 745f 6461 7465 7469 6d65  napshot_datetime
-00006610: 5f61 6e64 5f74 6162 6c65 5f6d 6574 6164  _and_table_metad
-00006620: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
-00006630: 2073 656c 662e 6271 636c 6965 6e74 2c0a   self.bqclient,.
-00006640: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00006650: 655f 7265 663d 7461 626c 652e 7265 6665  e_ref=table.refe
-00006660: 7265 6e63 652c 0a20 2020 2020 2020 2020  rence,.         
-00006670: 2020 2061 7069 5f6e 616d 653d 6170 695f     api_name=api_
-00006680: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00006690: 2020 6361 6368 653d 7365 6c66 2e5f 6466    cache=self._df
-000066a0: 5f73 6e61 7073 686f 742c 0a20 2020 2020  _snapshot,.     
-000066b0: 2020 2020 2020 2075 7365 5f63 6163 6865         use_cache
-000066c0: 3d75 7365 5f63 6163 6865 2c0a 2020 2020  =use_cache,.    
-000066d0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-000066e0: 6620 7461 626c 652e 6c6f 6361 7469 6f6e  f table.location
-000066f0: 2e63 6173 6566 6f6c 6428 2920 213d 2073  .casefold() != s
-00006700: 656c 662e 5f6c 6f63 6174 696f 6e2e 6361  elf._location.ca
-00006710: 7365 666f 6c64 2829 3a0a 2020 2020 2020  sefold():.      
-00006720: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00006730: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00006740: 2020 2020 2020 2020 6622 4375 7272 656e          f"Curren
-00006750: 7420 7365 7373 696f 6e20 6973 2069 6e20  t session is in 
-00006760: 7b73 656c 662e 5f6c 6f63 6174 696f 6e7d  {self._location}
-00006770: 2062 7574 2064 6174 6173 6574 2027 7b74   but dataset '{t
-00006780: 6162 6c65 2e70 726f 6a65 6374 7d2e 7b74  able.project}.{t
-00006790: 6162 6c65 2e64 6174 6173 6574 5f69 647d  able.dataset_id}
-000067a0: 2720 6973 206c 6f63 6174 6564 2069 6e20  ' is located in 
-000067b0: 7b74 6162 6c65 2e6c 6f63 6174 696f 6e7d  {table.location}
-000067c0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-000067d0: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
-000067e0: 6572 6520 6172 6520 7072 696d 6172 7920  ere are primary 
-000067f0: 6b65 7973 2064 6566 696e 6564 2c20 7468  keys defined, th
-00006800: 6520 7175 6572 7920 656e 6769 6e65 2061  e query engine a
-00006810: 7373 756d 6573 2074 6865 7365 0a20 2020  ssumes these.   
-00006820: 2020 2020 2023 2063 6f6c 756d 6e73 2061       # columns a
-00006830: 7265 2075 6e69 7175 652c 2065 7665 6e20  re unique, even 
-00006840: 6966 2074 6865 2063 6f6e 7374 7261 696e  if the constrain
-00006850: 7420 6973 206e 6f74 2065 6e66 6f72 6365  t is not enforce
-00006860: 642e 2057 6520 6d61 6b65 0a20 2020 2020  d. We make.     
-00006870: 2020 2023 2074 6865 2073 616d 6520 6173     # the same as
-00006880: 7375 6d70 7469 6f6e 2061 6e64 2075 7365  sumption and use
-00006890: 2074 6865 7365 2063 6f6c 756d 6e73 2061   these columns a
-000068a0: 7320 7468 6520 746f 7461 6c20 6f72 6465  s the total orde
-000068b0: 7269 6e67 206b 6579 732e 0a20 2020 2020  ring keys..     
-000068c0: 2020 2070 7269 6d61 7279 5f6b 6579 7320     primary_keys 
-000068d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-000068e0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-000068f0: 2874 6162 6c65 5f63 6f6e 7374 7261 696e  (table_constrain
-00006900: 7473 203a 3d20 6765 7461 7474 7228 7461  ts := getattr(ta
-00006910: 626c 652c 2022 7461 626c 655f 636f 6e73  ble, "table_cons
-00006920: 7472 6169 6e74 7322 2c20 4e6f 6e65 2929  traints", None))
-00006930: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00006940: 2020 2020 2020 2020 2061 6e64 2028 7072           and (pr
-00006950: 696d 6172 795f 6b65 7920 3a3d 2074 6162  imary_key := tab
-00006960: 6c65 5f63 6f6e 7374 7261 696e 7473 2e70  le_constraints.p
-00006970: 7269 6d61 7279 5f6b 6579 2920 6973 206e  rimary_key) is n
-00006980: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-00006990: 2020 2020 2320 5468 6973 2077 696c 6c20      # This will 
-000069a0: 6265 2046 616c 7365 2066 6f72 2065 6974  be False for eit
-000069b0: 6865 7220 4e6f 6e65 206f 7220 656d 7074  her None or empt
-000069c0: 7920 6c69 7374 2e0a 2020 2020 2020 2020  y list..        
-000069d0: 2020 2020 2320 5765 2077 616e 7420 7072      # We want pr
-000069e0: 696d 6172 795f 6b65 7973 203d 204e 6f6e  imary_keys = Non
-000069f0: 6520 6966 206e 6f20 7072 696d 6172 7920  e if no primary 
-00006a00: 6b65 7973 2061 7265 2073 6574 2e0a 2020  keys are set..  
-00006a10: 2020 2020 2020 2020 2020 616e 6420 2863            and (c
-00006a20: 6f6c 756d 6e73 203a 3d20 7072 696d 6172  olumns := primar
-00006a30: 795f 6b65 792e 636f 6c75 6d6e 7329 0a20  y_key.columns). 
-00006a40: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00006a50: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
-00006a60: 7973 203d 2063 6f6c 756d 6e73 0a0a 2020  ys = columns..  
-00006a70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00006a80: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
-00006a90: 7265 7373 696f 6e20 3d20 7365 6c66 2e69  ression = self.i
-00006aa0: 6269 735f 636c 6965 6e74 2e73 716c 280a  bis_client.sql(.
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 6269 6766 7261 6d65 735f 696f 2e63 7265  bigframes_io.cre
-00006ad0: 6174 655f 736e 6170 7368 6f74 5f73 716c  ate_snapshot_sql
-00006ae0: 2874 6162 6c65 2e72 6566 6572 656e 6365  (table.reference
-00006af0: 2c20 736e 6170 7368 6f74 5f74 696d 6573  , snapshot_times
-00006b00: 7461 6d70 290a 2020 2020 2020 2020 2020  tamp).          
-00006b10: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
-00006b20: 7074 2067 6f6f 676c 652e 6170 695f 636f  pt google.api_co
-00006b30: 7265 2e65 7863 6570 7469 6f6e 732e 466f  re.exceptions.Fo
-00006b40: 7262 6964 6465 6e20 6173 2065 783a 0a20  rbidden as ex:. 
-00006b50: 2020 2020 2020 2020 2020 2069 6620 2244             if "D
-00006b60: 7269 7665 2063 7265 6465 6e74 6961 6c73  rive credentials
-00006b70: 2220 696e 2065 782e 6d65 7373 6167 653a  " in ex.message:
-00006b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b90: 2065 782e 6d65 7373 6167 6520 2b3d 2022   ex.message += "
-00006ba0: 5c6e 4368 6563 6b20 6874 7470 733a 2f2f  \nCheck https://
-00006bb0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
-00006bc0: 2f62 6967 7175 6572 792f 646f 6373 2f71  /bigquery/docs/q
-00006bd0: 7565 7279 2d64 7269 7665 2d64 6174 6123  uery-drive-data#
-00006be0: 476f 6f67 6c65 5f44 7269 7665 5f70 6572  Google_Drive_per
-00006bf0: 6d69 7373 696f 6e73 2e22 0a20 2020 2020  missions.".     
-00006c00: 2020 2020 2020 2072 6169 7365 0a0a 2020         raise..  
-00006c10: 2020 2020 2020 7265 7475 726e 2074 6162        return tab
-00006c20: 6c65 5f65 7870 7265 7373 696f 6e2c 2070  le_expression, p
-00006c30: 7269 6d61 7279 5f6b 6579 730a 0a20 2020  rimary_keys..   
-00006c40: 2064 6566 205f 7265 6164 5f67 6271 5f74   def _read_gbq_t
-00006c50: 6162 6c65 280a 2020 2020 2020 2020 7365  able(.        se
-00006c60: 6c66 2c0a 2020 2020 2020 2020 7175 6572  lf,.        quer
-00006c70: 793a 2073 7472 2c0a 2020 2020 2020 2020  y: str,.        
-00006c80: 2a2c 0a20 2020 2020 2020 2069 6e64 6578  *,.        index
-00006c90: 5f63 6f6c 3a20 4974 6572 6162 6c65 5b73  _col: Iterable[s
-00006ca0: 7472 5d20 7c20 7374 7220 3d20 2829 2c0a  tr] | str = (),.
-00006cb0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
-00006cc0: 2049 7465 7261 626c 655b 7374 725d 203d   Iterable[str] =
-00006cd0: 2028 292c 0a20 2020 2020 2020 206d 6178   (),.        max
-00006ce0: 5f72 6573 756c 7473 3a20 4f70 7469 6f6e  _results: Option
-00006cf0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00006d00: 2020 2020 2020 2020 6170 695f 6e61 6d65          api_name
-00006d10: 3a20 7374 722c 0a20 2020 2020 2020 2075  : str,.        u
-00006d20: 7365 5f63 6163 6865 3a20 626f 6f6c 203d  se_cache: bool =
-00006d30: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
-00006d40: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00006d50: 616d 653a 0a20 2020 2020 2020 2069 6d70  ame:.        imp
-00006d60: 6f72 7420 6269 6766 7261 6d65 732e 6461  ort bigframes.da
-00006d70: 7461 6672 616d 6520 6173 2064 6174 6166  taframe as dataf
-00006d80: 7261 6d65 0a0a 2020 2020 2020 2020 6966  rame..        if
-00006d90: 206d 6178 5f72 6573 756c 7473 2061 6e64   max_results and
-00006da0: 206d 6178 5f72 6573 756c 7473 203c 3d20   max_results <= 
-00006db0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00006dc0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00006dd0: 2260 6d61 785f 7265 7375 6c74 7360 2073  "`max_results` s
-00006de0: 686f 756c 6420 6265 2061 2070 6f73 6974  hould be a posit
-00006df0: 6976 6520 6e75 6d62 6572 2e22 290a 0a20  ive number.").. 
-00006e00: 2020 2020 2020 2074 6162 6c65 5f72 6566         table_ref
-00006e10: 203d 2062 6967 7175 6572 792e 7461 626c   = bigquery.tabl
-00006e20: 652e 5461 626c 6552 6566 6572 656e 6365  e.TableReference
-00006e30: 2e66 726f 6d5f 7374 7269 6e67 280a 2020  .from_string(.  
-00006e40: 2020 2020 2020 2020 2020 7175 6572 792c            query,
-00006e50: 2064 6566 6175 6c74 5f70 726f 6a65 6374   default_project
-00006e60: 3d73 656c 662e 6271 636c 6965 6e74 2e70  =self.bqclient.p
-00006e70: 726f 6a65 6374 0a20 2020 2020 2020 2029  roject.        )
-00006e80: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
-00006e90: 3d20 7365 6c66 2e62 7163 6c69 656e 742e  = self.bqclient.
-00006ea0: 6765 745f 7461 626c 6528 7461 626c 655f  get_table(table_
-00006eb0: 7265 6629 0a20 2020 2020 2020 2028 7461  ref).        (ta
-00006ec0: 626c 655f 6578 7072 6573 7369 6f6e 2c20  ble_expression, 
-00006ed0: 7072 696d 6172 795f 6b65 7973 2c29 203d  primary_keys,) =
-00006ee0: 2073 656c 662e 5f67 6574 5f73 6e61 7073   self._get_snaps
-00006ef0: 686f 745f 7371 6c5f 616e 645f 7072 696d  hot_sql_and_prim
-00006f00: 6172 795f 6b65 7928 0a20 2020 2020 2020  ary_key(.       
-00006f10: 2020 2020 2074 6162 6c65 2c20 6170 695f       table, api_
-00006f20: 6e61 6d65 3d61 7069 5f6e 616d 652c 2075  name=api_name, u
-00006f30: 7365 5f63 6163 6865 3d75 7365 5f63 6163  se_cache=use_cac
-00006f40: 6865 0a20 2020 2020 2020 2029 0a20 2020  he.        ).   
-00006f50: 2020 2020 2074 6f74 616c 5f6f 7264 6572       total_order
-00006f60: 696e 675f 636f 6c73 203d 2070 7269 6d61  ing_cols = prima
-00006f70: 7279 5f6b 6579 730a 0a20 2020 2020 2020  ry_keys..       
-00006f80: 2069 6620 6e6f 7420 696e 6465 785f 636f   if not index_co
-00006f90: 6c20 616e 6420 7072 696d 6172 795f 6b65  l and primary_ke
-00006fa0: 7973 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ys is not None:.
-00006fb0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00006fc0: 785f 636f 6c20 3d20 7072 696d 6172 795f  x_col = primary_
-00006fd0: 6b65 7973 0a0a 2020 2020 2020 2020 666f  keys..        fo
-00006fe0: 7220 6b65 7920 696e 2063 6f6c 756d 6e73  r key in columns
-00006ff0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00007000: 206b 6579 206e 6f74 2069 6e20 7461 626c   key not in tabl
-00007010: 655f 6578 7072 6573 7369 6f6e 2e63 6f6c  e_expression.col
-00007020: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
-00007030: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00007040: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00007050: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
-00007060: 6c75 6d6e 2027 7b6b 6579 7d27 206f 6620  lumn '{key}' of 
-00007070: 6063 6f6c 756d 6e73 6020 6e6f 7420 666f  `columns` not fo
-00007080: 756e 6420 696e 2074 6869 7320 7461 626c  und in this tabl
-00007090: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
-000070a0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-000070b0: 6620 6973 696e 7374 616e 6365 2869 6e64  f isinstance(ind
-000070c0: 6578 5f63 6f6c 2c20 7374 7229 3a0a 2020  ex_col, str):.  
-000070d0: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-000070e0: 636f 6c73 3a20 4c69 7374 5b73 7472 5d20  cols: List[str] 
-000070f0: 3d20 5b69 6e64 6578 5f63 6f6c 5d0a 2020  = [index_col].  
-00007100: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00007110: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
-00007120: 6c73 203d 206c 6973 7428 696e 6465 785f  ls = list(index_
-00007130: 636f 6c29 0a0a 2020 2020 2020 2020 666f  col)..        fo
-00007140: 7220 6b65 7920 696e 2069 6e64 6578 5f63  r key in index_c
-00007150: 6f6c 733a 0a20 2020 2020 2020 2020 2020  ols:.           
-00007160: 2069 6620 6b65 7920 6e6f 7420 696e 2074   if key not in t
-00007170: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
-00007180: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
-00007190: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000071a0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000071c0: 2243 6f6c 756d 6e20 607b 6b65 797d 6020  "Column `{key}` 
-000071d0: 6f66 2060 696e 6465 785f 636f 6c60 206e  of `index_col` n
-000071e0: 6f74 2066 6f75 6e64 2069 6e20 7468 6973  ot found in this
-000071f0: 2074 6162 6c65 2e22 0a20 2020 2020 2020   table.".       
-00007200: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00007210: 2020 2020 6966 2063 6f6c 756d 6e73 3a0a      if columns:.
-00007220: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00007230: 655f 6578 7072 6573 7369 6f6e 203d 2074  e_expression = t
-00007240: 6162 6c65 5f65 7870 7265 7373 696f 6e2e  able_expression.
-00007250: 7365 6c65 6374 285b 2a69 6e64 6578 5f63  select([*index_c
-00007260: 6f6c 732c 202a 636f 6c75 6d6e 735d 290a  ols, *columns]).
-00007270: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
-00007280: 6520 696e 6465 7820 6973 2075 6e69 7175  e index is uniqu
-00007290: 6520 616e 6420 736f 7274 6162 6c65 2c20  e and sortable, 
-000072a0: 7468 656e 2077 6520 646f 6e27 7420 6e65  then we don't ne
-000072b0: 6564 2074 6f20 6765 6e65 7261 7465 0a20  ed to generate. 
-000072c0: 2020 2020 2020 2023 2061 6e20 6f72 6465         # an orde
-000072d0: 7269 6e67 2063 6f6c 756d 6e2e 0a20 2020  ring column..   
-000072e0: 2020 2020 206f 7264 6572 696e 6720 3d20       ordering = 
-000072f0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00007300: 746f 7461 6c5f 6f72 6465 7269 6e67 5f63  total_ordering_c
-00007310: 6f6c 7320 6973 206e 6f74 204e 6f6e 653a  ols is not None:
-00007320: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
-00007330: 6f74 653a 2063 7572 7265 6e74 6c79 2c20  ote: currently, 
-00007340: 6120 7461 626c 6520 6861 7320 6120 746f  a table has a to
-00007350: 7461 6c20 6f72 6465 7269 6e67 206f 6e6c  tal ordering onl
-00007360: 7920 7768 656e 2074 6865 0a20 2020 2020  y when the.     
-00007370: 2020 2020 2020 2023 2070 7269 6d61 7279         # primary
-00007380: 206b 6579 2873 2920 6172 6520 7365 7420   key(s) are set 
-00007390: 6f6e 2061 2074 6162 6c65 2e20 5468 6520  on a table. The 
-000073a0: 7175 6572 7920 656e 6769 6e65 2061 7373  query engine ass
-000073b0: 756d 6573 2073 7563 680a 2020 2020 2020  umes such.      
-000073c0: 2020 2020 2020 2320 636f 6c75 6d6e 7320        # columns 
-000073d0: 6172 6520 756e 6971 7565 2c20 6576 656e  are unique, even
-000073e0: 2069 6620 6e6f 7420 656e 666f 7263 6564   if not enforced
-000073f0: 2e0a 2020 2020 2020 2020 2020 2020 6f72  ..            or
-00007400: 6465 7269 6e67 203d 206f 7264 6572 2e45  dering = order.E
-00007410: 7870 7265 7373 696f 6e4f 7264 6572 696e  xpressionOrderin
-00007420: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
-00007430: 2020 206f 7264 6572 696e 675f 7661 6c75     ordering_valu
-00007440: 655f 636f 6c75 6d6e 733d 7475 706c 6528  e_columns=tuple(
-00007450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007460: 2020 2020 206f 7264 6572 2e61 7363 656e       order.ascen
-00007470: 6469 6e67 5f6f 7665 7228 636f 6c75 6d6e  ding_over(column
-00007480: 5f69 6429 2066 6f72 2063 6f6c 756d 6e5f  _id) for column_
-00007490: 6964 2069 6e20 746f 7461 6c5f 6f72 6465  id in total_orde
-000074a0: 7269 6e67 5f63 6f6c 730a 2020 2020 2020  ring_cols.      
-000074b0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000074c0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-000074d0: 616c 5f6f 7264 6572 696e 675f 636f 6c75  al_ordering_colu
-000074e0: 6d6e 733d 6672 6f7a 656e 7365 7428 746f  mns=frozenset(to
-000074f0: 7461 6c5f 6f72 6465 7269 6e67 5f63 6f6c  tal_ordering_col
-00007500: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
-00007510: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
-00007520: 6c75 6d6e 5f76 616c 7565 7320 3d20 5b74  lumn_values = [t
-00007530: 6162 6c65 5f65 7870 7265 7373 696f 6e5b  able_expression[
-00007540: 636f 6c5d 2066 6f72 2063 6f6c 2069 6e20  col] for col in 
-00007550: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-00007560: 2e63 6f6c 756d 6e73 5d0a 2020 2020 2020  .columns].      
-00007570: 2020 2020 2020 6172 7261 795f 7661 6c75        array_valu
-00007580: 6520 3d20 636f 7265 2e41 7272 6179 5661  e = core.ArrayVa
-00007590: 6c75 652e 6672 6f6d 5f69 6269 7328 0a20  lue.from_ibis(. 
-000075a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000075b0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000075c0: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-000075d0: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
-000075e0: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
-000075f0: 6f6c 756d 6e5f 7661 6c75 6573 2c0a 2020  olumn_values,.  
-00007600: 2020 2020 2020 2020 2020 2020 2020 6869                hi
-00007610: 6464 656e 5f6f 7264 6572 696e 675f 636f  dden_ordering_co
-00007620: 6c75 6d6e 733d 5b5d 2c0a 2020 2020 2020  lumns=[],.      
-00007630: 2020 2020 2020 2020 2020 6f72 6465 7269            orderi
-00007640: 6e67 3d6f 7264 6572 696e 672c 0a20 2020  ng=ordering,.   
-00007650: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00007660: 2020 2020 656c 6966 206c 656e 2869 6e64      elif len(ind
-00007670: 6578 5f63 6f6c 7329 2021 3d20 303a 0a20  ex_cols) != 0:. 
-00007680: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-00007690: 6861 7665 2069 6e64 6578 2063 6f6c 756d  have index colum
-000076a0: 6e73 2c20 6c65 7473 2073 6565 2069 6620  ns, lets see if 
-000076b0: 7468 6f73 6520 6172 6520 6163 7475 616c  those are actual
-000076c0: 6c79 2074 6f74 616c 5f6f 7264 6572 5f63  ly total_order_c
-000076d0: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
-000076e0: 2020 206f 7264 6572 696e 6720 3d20 6f72     ordering = or
-000076f0: 6465 722e 4578 7072 6573 7369 6f6e 4f72  der.ExpressionOr
-00007700: 6465 7269 6e67 280a 2020 2020 2020 2020  dering(.        
-00007710: 2020 2020 2020 2020 6f72 6465 7269 6e67          ordering
-00007720: 5f76 616c 7565 5f63 6f6c 756d 6e73 3d74  _value_columns=t
-00007730: 7570 6c65 280a 2020 2020 2020 2020 2020  uple(.          
-00007740: 2020 2020 2020 2020 2020 5b6f 7264 6572            [order
-00007750: 2e61 7363 656e 6469 6e67 5f6f 7665 7228  .ascending_over(
-00007760: 636f 6c75 6d6e 5f69 6429 2066 6f72 2063  column_id) for c
-00007770: 6f6c 756d 6e5f 6964 2069 6e20 696e 6465  olumn_id in inde
-00007780: 785f 636f 6c73 5d0a 2020 2020 2020 2020  x_cols].        
-00007790: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000077a0: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-000077b0: 5f6f 7264 6572 696e 675f 636f 6c75 6d6e  _ordering_column
-000077c0: 733d 6672 6f7a 656e 7365 7428 696e 6465  s=frozenset(inde
-000077d0: 785f 636f 6c73 292c 0a20 2020 2020 2020  x_cols),.       
-000077e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000077f0: 2020 2069 735f 746f 7461 6c5f 6f72 6465     is_total_orde
-00007800: 7269 6e67 203d 2073 656c 662e 5f63 6865  ring = self._che
-00007810: 636b 5f69 6e64 6578 5f75 6e69 7175 656e  ck_index_uniquen
-00007820: 6573 7328 0a20 2020 2020 2020 2020 2020  ess(.           
-00007830: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-00007840: 7373 696f 6e2c 2069 6e64 6578 5f63 6f6c  ssion, index_col
-00007850: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
-00007860: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00007870: 735f 746f 7461 6c5f 6f72 6465 7269 6e67  s_total_ordering
-00007880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007890: 2020 636f 6c75 6d6e 5f76 616c 7565 7320    column_values 
-000078a0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-000078b0: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
-000078c0: 7072 6573 7369 6f6e 5b63 6f6c 5d20 666f  pression[col] fo
-000078d0: 7220 636f 6c20 696e 2074 6162 6c65 5f65  r col in table_e
-000078e0: 7870 7265 7373 696f 6e2e 636f 6c75 6d6e  xpression.column
-000078f0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00007900: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00007910: 2020 2020 6172 7261 795f 7661 6c75 6520      array_value 
-00007920: 3d20 636f 7265 2e41 7272 6179 5661 6c75  = core.ArrayValu
-00007930: 652e 6672 6f6d 5f69 6269 7328 0a20 2020  e.from_ibis(.   
-00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007950: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-00007960: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00007970: 5f65 7870 7265 7373 696f 6e2c 0a20 2020  _expression,.   
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e5f   columns=column_
-000079a0: 7661 6c75 6573 2c0a 2020 2020 2020 2020  values,.        
-000079b0: 2020 2020 2020 2020 2020 2020 6869 6464              hidd
-000079c0: 656e 5f6f 7264 6572 696e 675f 636f 6c75  en_ordering_colu
-000079d0: 6d6e 733d 5b5d 2c0a 2020 2020 2020 2020  mns=[],.        
-000079e0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-000079f0: 7269 6e67 3d6f 7264 6572 696e 672c 0a20  ring=ordering,. 
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007a10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00007a20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007a30: 2020 2061 7272 6179 5f76 616c 7565 203d     array_value =
-00007a40: 2073 656c 662e 5f63 7265 6174 655f 746f   self._create_to
-00007a50: 7461 6c5f 6f72 6465 7269 6e67 280a 2020  tal_ordering(.  
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
-00007a80: 6f6e 2c20 7461 626c 655f 726f 7773 3d74  on, table_rows=t
-00007a90: 6162 6c65 2e6e 756d 5f72 6f77 730a 2020  able.num_rows.  
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00007ab0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00007ac0: 2020 2020 2020 2020 2020 6172 7261 795f            array_
-00007ad0: 7661 6c75 6520 3d20 7365 6c66 2e5f 6372  value = self._cr
-00007ae0: 6561 7465 5f74 6f74 616c 5f6f 7264 6572  eate_total_order
-00007af0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00007b00: 2020 2020 2074 6162 6c65 5f65 7870 7265       table_expre
-00007b10: 7373 696f 6e2c 2074 6162 6c65 5f72 6f77  ssion, table_row
-00007b20: 733d 7461 626c 652e 6e75 6d5f 726f 7773  s=table.num_rows
-00007b30: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00007b40: 2020 2020 2020 2020 7661 6c75 655f 636f          value_co
-00007b50: 6c75 6d6e 7320 3d20 5b63 6f6c 2066 6f72  lumns = [col for
-00007b60: 2063 6f6c 2069 6e20 6172 7261 795f 7661   col in array_va
-00007b70: 6c75 652e 636f 6c75 6d6e 5f69 6473 2069  lue.column_ids i
-00007b80: 6620 636f 6c20 6e6f 7420 696e 2069 6e64  f col not in ind
-00007b90: 6578 5f63 6f6c 735d 0a20 2020 2020 2020  ex_cols].       
-00007ba0: 2062 6c6f 636b 203d 2062 6c6f 636b 732e   block = blocks.
-00007bb0: 426c 6f63 6b28 0a20 2020 2020 2020 2020  Block(.         
-00007bc0: 2020 2061 7272 6179 5f76 616c 7565 2c0a     array_value,.
-00007bd0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00007be0: 785f 636f 6c75 6d6e 733d 696e 6465 785f  x_columns=index_
-00007bf0: 636f 6c73 2c0a 2020 2020 2020 2020 2020  cols,.          
-00007c00: 2020 636f 6c75 6d6e 5f6c 6162 656c 733d    column_labels=
-00007c10: 7661 6c75 655f 636f 6c75 6d6e 732c 0a20  value_columns,. 
-00007c20: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00007c30: 5f6c 6162 656c 733d 696e 6465 785f 636f  _labels=index_co
-00007c40: 6c73 2c0a 2020 2020 2020 2020 290a 2020  ls,.        ).  
-00007c50: 2020 2020 2020 6966 206d 6178 5f72 6573        if max_res
-00007c60: 756c 7473 3a0a 2020 2020 2020 2020 2020  ults:.          
-00007c70: 2020 626c 6f63 6b20 3d20 626c 6f63 6b2e    block = block.
-00007c80: 736c 6963 6528 7374 6f70 3d6d 6178 5f72  slice(stop=max_r
-00007c90: 6573 756c 7473 290a 2020 2020 2020 2020  esults).        
-00007ca0: 6466 203d 2064 6174 6166 7261 6d65 2e44  df = dataframe.D
-00007cb0: 6174 6146 7261 6d65 2862 6c6f 636b 290a  ataFrame(block).
-00007cc0: 0a20 2020 2020 2020 2023 2049 6620 7573  .        # If us
-00007cd0: 6572 2070 726f 7669 6465 6420 696e 6465  er provided inde
-00007ce0: 7820 636f 6c75 6d6e 732c 2073 686f 756c  x columns, shoul
-00007cf0: 6420 736f 7274 206f 7665 7220 6974 0a20  d sort over it. 
-00007d00: 2020 2020 2020 2069 6620 6c65 6e28 696e         if len(in
-00007d10: 6465 785f 636f 6c73 2920 3e20 303a 0a20  dex_cols) > 0:. 
-00007d20: 2020 2020 2020 2020 2020 2064 662e 736f             df.so
-00007d30: 7274 5f69 6e64 6578 2829 0a20 2020 2020  rt_index().     
-00007d40: 2020 2072 6574 7572 6e20 6466 0a0a 2020     return df..  
-00007d50: 2020 6465 6620 5f63 6865 636b 5f69 6e64    def _check_ind
-00007d60: 6578 5f75 6e69 7175 656e 6573 7328 0a20  ex_uniqueness(. 
-00007d70: 2020 2020 2020 2073 656c 662c 2074 6162         self, tab
-00007d80: 6c65 3a20 6962 6973 5f74 7970 6573 2e54  le: ibis_types.T
-00007d90: 6162 6c65 2c20 696e 6465 785f 636f 6c73  able, index_cols
-00007da0: 3a20 4c69 7374 5b73 7472 5d0a 2020 2020  : List[str].    
-00007db0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00007dc0: 2020 2064 6973 7469 6e63 745f 7461 626c     distinct_tabl
-00007dd0: 6520 3d20 7461 626c 652e 7365 6c65 6374  e = table.select
-00007de0: 282a 696e 6465 785f 636f 6c73 292e 6469  (*index_cols).di
-00007df0: 7374 696e 6374 2829 0a20 2020 2020 2020  stinct().       
-00007e00: 2069 735f 756e 6971 7565 5f73 716c 203d   is_unique_sql =
-00007e10: 2066 2222 2257 4954 4820 6675 6c6c 5f74   f"""WITH full_t
-00007e20: 6162 6c65 2041 5320 280a 2020 2020 2020  able AS (.      
-00007e30: 2020 2020 2020 7b73 656c 662e 6962 6973        {self.ibis
-00007e40: 5f63 6c69 656e 742e 636f 6d70 696c 6528  _client.compile(
-00007e50: 7461 626c 6529 7d0a 2020 2020 2020 2020  table)}.        
-00007e60: 292c 0a20 2020 2020 2020 2064 6973 7469  ),.        disti
-00007e70: 6e63 745f 7461 626c 6520 4153 2028 0a20  nct_table AS (. 
-00007e80: 2020 2020 2020 2020 2020 207b 7365 6c66             {self
-00007e90: 2e69 6269 735f 636c 6965 6e74 2e63 6f6d  .ibis_client.com
-00007ea0: 7069 6c65 2864 6973 7469 6e63 745f 7461  pile(distinct_ta
-00007eb0: 626c 6529 7d0a 2020 2020 2020 2020 290a  ble)}.        ).
-00007ec0: 0a20 2020 2020 2020 2053 454c 4543 5420  .        SELECT 
-00007ed0: 2853 454c 4543 5420 434f 554e 5428 2a29  (SELECT COUNT(*)
-00007ee0: 2046 524f 4d20 6675 6c6c 5f74 6162 6c65   FROM full_table
-00007ef0: 2920 4153 2060 746f 7461 6c5f 636f 756e  ) AS `total_coun
-00007f00: 7460 2c0a 2020 2020 2020 2020 2853 454c  t`,.        (SEL
-00007f10: 4543 5420 434f 554e 5428 2a29 2046 524f  ECT COUNT(*) FRO
-00007f20: 4d20 6469 7374 696e 6374 5f74 6162 6c65  M distinct_table
-00007f30: 2920 4153 2060 6469 7374 696e 6374 5f63  ) AS `distinct_c
-00007f40: 6f75 6e74 600a 2020 2020 2020 2020 2222  ount`.        ""
-00007f50: 220a 2020 2020 2020 2020 7265 7375 6c74  ".        result
-00007f60: 732c 205f 203d 2073 656c 662e 5f73 7461  s, _ = self._sta
-00007f70: 7274 5f71 7565 7279 2869 735f 756e 6971  rt_query(is_uniq
-00007f80: 7565 5f73 716c 290a 2020 2020 2020 2020  ue_sql).        
-00007f90: 726f 7720 3d20 6e65 7874 2869 7465 7228  row = next(iter(
-00007fa0: 7265 7375 6c74 7329 290a 0a20 2020 2020  results))..     
-00007fb0: 2020 2074 6f74 616c 5f63 6f75 6e74 203d     total_count =
-00007fc0: 2072 6f77 5b22 746f 7461 6c5f 636f 756e   row["total_coun
-00007fd0: 7422 5d0a 2020 2020 2020 2020 6469 7374  t"].        dist
-00007fe0: 696e 6374 5f63 6f75 6e74 203d 2072 6f77  inct_count = row
-00007ff0: 5b22 6469 7374 696e 6374 5f63 6f75 6e74  ["distinct_count
-00008000: 225d 0a20 2020 2020 2020 2072 6574 7572  "].        retur
-00008010: 6e20 746f 7461 6c5f 636f 756e 7420 3d3d  n total_count ==
-00008020: 2064 6973 7469 6e63 745f 636f 756e 740a   distinct_count.
-00008030: 0a20 2020 2064 6566 205f 7265 6164 5f62  .    def _read_b
-00008040: 6967 7175 6572 795f 6c6f 6164 5f6a 6f62  igquery_load_job
-00008050: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00008060: 2020 2020 2020 2020 6669 6c65 7061 7468          filepath
-00008070: 5f6f 725f 6275 6666 6572 3a20 7374 7220  _or_buffer: str 
-00008080: 7c20 494f 5b22 6279 7465 7322 5d2c 0a20  | IO["bytes"],. 
-00008090: 2020 2020 2020 2074 6162 6c65 3a20 556e         table: Un
-000080a0: 696f 6e5b 6269 6771 7565 7279 2e54 6162  ion[bigquery.Tab
-000080b0: 6c65 2c20 6269 6771 7565 7279 2e54 6162  le, bigquery.Tab
-000080c0: 6c65 5265 6665 7265 6e63 655d 2c0a 2020  leReference],.  
-000080d0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-000080e0: 206a 6f62 5f63 6f6e 6669 673a 2062 6967   job_config: big
-000080f0: 7175 6572 792e 4c6f 6164 4a6f 6243 6f6e  query.LoadJobCon
-00008100: 6669 672c 0a20 2020 2020 2020 2069 6e64  fig,.        ind
-00008110: 6578 5f63 6f6c 3a20 4974 6572 6162 6c65  ex_col: Iterable
-00008120: 5b73 7472 5d20 7c20 7374 7220 3d20 2829  [str] | str = ()
-00008130: 2c0a 2020 2020 2020 2020 636f 6c75 6d6e  ,.        column
-00008140: 733a 2049 7465 7261 626c 655b 7374 725d  s: Iterable[str]
-00008150: 203d 2028 292c 0a20 2020 2029 202d 3e20   = (),.    ) -> 
-00008160: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00008170: 616d 653a 0a20 2020 2020 2020 2069 6620  ame:.        if 
-00008180: 6973 696e 7374 616e 6365 2869 6e64 6578  isinstance(index
-00008190: 5f63 6f6c 2c20 7374 7229 3a0a 2020 2020  _col, str):.    
-000081a0: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
-000081b0: 6c73 203d 205b 696e 6465 785f 636f 6c5d  ls = [index_col]
-000081c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000081d0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-000081e0: 5f63 6f6c 7320 3d20 6c69 7374 2869 6e64  _cols = list(ind
-000081f0: 6578 5f63 6f6c 290a 0a20 2020 2020 2020  ex_col)..       
-00008200: 2069 6620 6e6f 7420 6a6f 625f 636f 6e66   if not job_conf
-00008210: 6967 2e63 6c75 7374 6572 696e 675f 6669  ig.clustering_fi
-00008220: 656c 6473 2061 6e64 2069 6e64 6578 5f63  elds and index_c
-00008230: 6f6c 733a 0a20 2020 2020 2020 2020 2020  ols:.           
-00008240: 206a 6f62 5f63 6f6e 6669 672e 636c 7573   job_config.clus
-00008250: 7465 7269 6e67 5f66 6965 6c64 7320 3d20  tering_fields = 
-00008260: 696e 6465 785f 636f 6c73 5b3a 5f4d 4158  index_cols[:_MAX
-00008270: 5f43 4c55 5354 4552 5f43 4f4c 554d 4e53  _CLUSTER_COLUMNS
-00008280: 5d0a 0a20 2020 2020 2020 2069 6620 6973  ]..        if is
-00008290: 696e 7374 616e 6365 2866 696c 6570 6174  instance(filepat
-000082a0: 685f 6f72 5f62 7566 6665 722c 2073 7472  h_or_buffer, str
-000082b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-000082c0: 6620 6669 6c65 7061 7468 5f6f 725f 6275  f filepath_or_bu
-000082d0: 6666 6572 2e73 7461 7274 7377 6974 6828  ffer.startswith(
-000082e0: 2267 733a 2f2f 2229 3a0a 2020 2020 2020  "gs://"):.      
-000082f0: 2020 2020 2020 2020 2020 6c6f 6164 5f6a            load_j
-00008300: 6f62 203d 2073 656c 662e 6271 636c 6965  ob = self.bqclie
-00008310: 6e74 2e6c 6f61 645f 7461 626c 655f 6672  nt.load_table_fr
-00008320: 6f6d 5f75 7269 280a 2020 2020 2020 2020  om_uri(.        
-00008330: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00008340: 7061 7468 5f6f 725f 6275 6666 6572 2c20  path_or_buffer, 
-00008350: 7461 626c 652c 206a 6f62 5f63 6f6e 6669  table, job_confi
-00008360: 673d 6a6f 625f 636f 6e66 6967 0a20 2020  g=job_config.   
-00008370: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00008380: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083a0: 2077 6974 6820 6f70 656e 2866 696c 6570   with open(filep
-000083b0: 6174 685f 6f72 5f62 7566 6665 722c 2022  ath_or_buffer, "
-000083c0: 7262 2229 2061 7320 736f 7572 6365 5f66  rb") as source_f
-000083d0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-000083e0: 2020 2020 2020 2020 206c 6f61 645f 6a6f           load_jo
-000083f0: 6220 3d20 7365 6c66 2e62 7163 6c69 656e  b = self.bqclien
-00008400: 742e 6c6f 6164 5f74 6162 6c65 5f66 726f  t.load_table_fro
-00008410: 6d5f 6669 6c65 280a 2020 2020 2020 2020  m_file(.        
-00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 736f 7572 6365 5f66 696c 652c 2074 6162  source_file, tab
-00008440: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
-00008450: 6f62 5f63 6f6e 6669 670a 2020 2020 2020  ob_config.      
-00008460: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008470: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008480: 2020 2020 2020 2020 2020 6c6f 6164 5f6a            load_j
-00008490: 6f62 203d 2073 656c 662e 6271 636c 6965  ob = self.bqclie
-000084a0: 6e74 2e6c 6f61 645f 7461 626c 655f 6672  nt.load_table_fr
-000084b0: 6f6d 5f66 696c 6528 0a20 2020 2020 2020  om_file(.       
-000084c0: 2020 2020 2020 2020 2066 696c 6570 6174           filepat
-000084d0: 685f 6f72 5f62 7566 6665 722c 2074 6162  h_or_buffer, tab
-000084e0: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
-000084f0: 6f62 5f63 6f6e 6669 670a 2020 2020 2020  ob_config.      
-00008500: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00008510: 2073 656c 662e 5f73 7461 7274 5f67 656e   self._start_gen
-00008520: 6572 6963 5f6a 6f62 286c 6f61 645f 6a6f  eric_job(load_jo
-00008530: 6229 0a20 2020 2020 2020 2074 6162 6c65  b).        table
-00008540: 5f69 6420 3d20 6622 7b74 6162 6c65 2e70  _id = f"{table.p
-00008550: 726f 6a65 6374 7d2e 7b74 6162 6c65 2e64  roject}.{table.d
-00008560: 6174 6173 6574 5f69 647d 2e7b 7461 626c  ataset_id}.{tabl
-00008570: 652e 7461 626c 655f 6964 7d22 0a0a 2020  e.table_id}"..  
-00008580: 2020 2020 2020 2320 5570 6461 7465 2074        # Update t
-00008590: 6865 2074 6162 6c65 2065 7870 6972 6174  he table expirat
-000085a0: 696f 6e20 736f 2077 6520 6172 656e 2774  ion so we aren't
-000085b0: 206c 696d 6974 6564 2074 6f20 7468 6520   limited to the 
-000085c0: 6465 6661 756c 7420 3234 0a20 2020 2020  default 24.     
-000085d0: 2020 2023 2068 6f75 7273 206f 6620 7468     # hours of th
-000085e0: 6520 616e 6f6e 796d 6f75 7320 6461 7461  e anonymous data
-000085f0: 7365 742e 0a20 2020 2020 2020 2074 6162  set..        tab
-00008600: 6c65 5f65 7870 6972 6174 696f 6e20 3d20  le_expiration = 
-00008610: 6269 6771 7565 7279 2e54 6162 6c65 2874  bigquery.Table(t
-00008620: 6162 6c65 5f69 6429 0a20 2020 2020 2020  able_id).       
-00008630: 2074 6162 6c65 5f65 7870 6972 6174 696f   table_expiratio
-00008640: 6e2e 6578 7069 7265 7320 3d20 280a 2020  n.expires = (.  
-00008650: 2020 2020 2020 2020 2020 6461 7465 7469            dateti
-00008660: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
-00008670: 6461 7465 7469 6d65 2e74 696d 657a 6f6e  datetime.timezon
-00008680: 652e 7574 6329 202b 2063 6f6e 7374 616e  e.utc) + constan
-00008690: 7473 2e44 4546 4155 4c54 5f45 5850 4952  ts.DEFAULT_EXPIR
-000086a0: 4154 494f 4e0a 2020 2020 2020 2020 290a  ATION.        ).
-000086b0: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-000086c0: 6c69 656e 742e 7570 6461 7465 5f74 6162  lient.update_tab
-000086d0: 6c65 2874 6162 6c65 5f65 7870 6972 6174  le(table_expirat
-000086e0: 696f 6e2c 205b 2265 7870 6972 6573 225d  ion, ["expires"]
-000086f0: 290a 0a20 2020 2020 2020 2023 2054 6865  )..        # The
-00008700: 2042 6967 5175 6572 7920 5245 5354 2041   BigQuery REST A
-00008710: 5049 2066 6f72 2074 6162 6c65 732e 6765  PI for tables.ge
-00008720: 7420 646f 6573 6e27 7420 7461 6b65 2061  t doesn't take a
-00008730: 2073 6573 7369 6f6e 2049 442c 2073 6f20   session ID, so 
-00008740: 7765 0a20 2020 2020 2020 2023 2063 616e  we.        # can
-00008750: 2774 2067 6574 2074 6865 2073 6368 656d  't get the schem
-00008760: 6120 666f 7220 6120 7465 6d70 2074 6162  a for a temp tab
-00008770: 6c65 2074 6861 7420 7761 792e 0a20 2020  le that way..   
-00008780: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008790: 2e72 6561 645f 6762 715f 7461 626c 6528  .read_gbq_table(
-000087a0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-000087b0: 6c65 5f69 642c 0a20 2020 2020 2020 2020  le_id,.         
-000087c0: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
-000087d0: 6578 5f63 6f6c 2c0a 2020 2020 2020 2020  ex_col,.        
-000087e0: 2020 2020 636f 6c75 6d6e 733d 636f 6c75      columns=colu
-000087f0: 6d6e 732c 0a20 2020 2020 2020 2029 0a0a  mns,.        )..
-00008800: 2020 2020 6465 6620 7265 6164 5f67 6271      def read_gbq
-00008810: 5f6d 6f64 656c 2873 656c 662c 206d 6f64  _model(self, mod
-00008820: 656c 5f6e 616d 653a 2073 7472 293a 0a20  el_name: str):. 
-00008830: 2020 2020 2020 2022 2222 4c6f 6164 7320         """Loads 
-00008840: 6120 4269 6751 7565 7279 204d 4c20 6d6f  a BigQuery ML mo
-00008850: 6465 6c20 6672 6f6d 2042 6967 5175 6572  del from BigQuer
-00008860: 792e 0a0a 2020 2020 2020 2020 2a2a 4578  y...        **Ex
-00008870: 616d 706c 6573 3a2a 2a0a 0a20 2020 2020  amples:**..     
-00008880: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
-00008890: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
-000088a0: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
-000088b0: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
-000088c0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
-000088d0: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
-000088e0: 650a 0a20 2020 2020 2020 2052 6561 6420  e..        Read 
-000088f0: 616e 2065 7869 7374 696e 6720 4269 6751  an existing BigQ
-00008900: 7565 7279 204d 4c20 6d6f 6465 6c2e 0a0a  uery ML model...
-00008910: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00008920: 6d6f 6465 6c5f 6e61 6d65 203d 2022 6269  model_name = "bi
-00008930: 6766 7261 6d65 732d 6465 762e 6271 6d6c  gframes-dev.bqml
-00008940: 5f74 7574 6f72 6961 6c2e 7065 6e67 7569  _tutorial.pengui
-00008950: 6e73 5f6d 6f64 656c 220a 2020 2020 2020  ns_model".      
-00008960: 2020 2020 2020 3e3e 3e20 6d6f 6465 6c20        >>> model 
-00008970: 3d20 6270 642e 7265 6164 5f67 6271 5f6d  = bpd.read_gbq_m
-00008980: 6f64 656c 286d 6f64 656c 5f6e 616d 6529  odel(model_name)
-00008990: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000089a0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000089b0: 6c5f 6e61 6d65 2028 7374 7229 3a0a 2020  l_name (str):.  
-000089c0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-000089d0: 6520 6d6f 6465 6c27 7320 6e61 6d65 2069  e model's name i
-000089e0: 6e20 4269 6751 7565 7279 2069 6e20 7468  n BigQuery in th
-000089f0: 6520 666f 726d 6174 0a20 2020 2020 2020  e format.       
-00008a00: 2020 2020 2020 2020 2060 7072 6f6a 6563           `projec
-00008a10: 745f 6964 2e64 6174 6173 6574 5f69 642e  t_id.dataset_id.
-00008a20: 6d6f 6465 6c5f 6964 602c 206f 7220 6a75  model_id`, or ju
-00008a30: 7374 2060 6461 7461 7365 745f 6964 2e6d  st `dataset_id.m
-00008a40: 6f64 656c 5f69 6460 0a20 2020 2020 2020  odel_id`.       
-00008a50: 2020 2020 2020 2020 2074 6f20 6c6f 6164           to load
-00008a60: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
-00008a70: 7420 7072 6f6a 6563 742e 0a0a 2020 2020  t project...    
-00008a80: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00008a90: 2020 2020 2020 2020 2041 2062 6967 6672           A bigfr
-00008aa0: 616d 6573 2e6d 6c20 4d6f 6465 6c2c 2054  ames.ml Model, T
-00008ab0: 7261 6e73 666f 726d 6572 206f 7220 5069  ransformer or Pi
-00008ac0: 7065 6c69 6e65 2077 7261 7070 696e 6720  peline wrapping 
-00008ad0: 7468 6520 6d6f 6465 6c2e 0a20 2020 2020  the model..     
-00008ae0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00008af0: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
-00008b00: 6d6c 2e6c 6f61 6465 720a 0a20 2020 2020  ml.loader..     
-00008b10: 2020 206d 6f64 656c 5f72 6566 203d 2062     model_ref = b
-00008b20: 6967 7175 6572 792e 4d6f 6465 6c52 6566  igquery.ModelRef
-00008b30: 6572 656e 6365 2e66 726f 6d5f 7374 7269  erence.from_stri
-00008b40: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-00008b50: 6d6f 6465 6c5f 6e61 6d65 2c20 6465 6661  model_name, defa
-00008b60: 756c 745f 7072 6f6a 6563 743d 7365 6c66  ult_project=self
-00008b70: 2e62 7163 6c69 656e 742e 7072 6f6a 6563  .bqclient.projec
-00008b80: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
-00008b90: 2020 2020 6d6f 6465 6c20 3d20 7365 6c66      model = self
-00008ba0: 2e62 7163 6c69 656e 742e 6765 745f 6d6f  .bqclient.get_mo
-00008bb0: 6465 6c28 6d6f 6465 6c5f 7265 6629 0a20  del(model_ref). 
-00008bc0: 2020 2020 2020 2072 6574 7572 6e20 6269         return bi
-00008bd0: 6766 7261 6d65 732e 6d6c 2e6c 6f61 6465  gframes.ml.loade
-00008be0: 722e 6672 6f6d 5f62 7128 7365 6c66 2c20  r.from_bq(self, 
-00008bf0: 6d6f 6465 6c29 0a0a 2020 2020 4074 7970  model)..    @typ
-00008c00: 696e 672e 6f76 6572 6c6f 6164 0a20 2020  ing.overload.   
-00008c10: 2064 6566 2072 6561 645f 7061 6e64 6173   def read_pandas
-00008c20: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00008c30: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-00008c40: 3a20 7061 6e64 6173 2e49 6e64 6578 0a20  : pandas.Index. 
-00008c50: 2020 2029 202d 3e20 6269 6766 7261 6d65     ) -> bigframe
-00008c60: 732e 636f 7265 2e69 6e64 6578 6573 2e49  s.core.indexes.I
-00008c70: 6e64 6578 3a0a 2020 2020 2020 2020 2e2e  ndex:.        ..
-00008c80: 2e0a 0a20 2020 2040 7479 7069 6e67 2e6f  ...    @typing.o
-00008c90: 7665 726c 6f61 640a 2020 2020 6465 6620  verload.    def 
-00008ca0: 7265 6164 5f70 616e 6461 7328 7365 6c66  read_pandas(self
-00008cb0: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
-00008cc0: 6d65 3a20 7061 6e64 6173 2e53 6572 6965  me: pandas.Serie
-00008cd0: 7329 202d 3e20 6269 6766 7261 6d65 732e  s) -> bigframes.
-00008ce0: 7365 7269 6573 2e53 6572 6965 733a 0a20  series.Series:. 
-00008cf0: 2020 2020 2020 202e 2e2e 0a0a 2020 2020         .....    
-00008d00: 4074 7970 696e 672e 6f76 6572 6c6f 6164  @typing.overload
-00008d10: 0a20 2020 2064 6566 2072 6561 645f 7061  .    def read_pa
-00008d20: 6e64 6173 2873 656c 662c 2070 616e 6461  ndas(self, panda
-00008d30: 735f 6461 7461 6672 616d 653a 2070 616e  s_dataframe: pan
-00008d40: 6461 732e 4461 7461 4672 616d 6529 202d  das.DataFrame) -
-00008d50: 3e20 6461 7461 6672 616d 652e 4461 7461  > dataframe.Data
-00008d60: 4672 616d 653a 0a20 2020 2020 2020 202e  Frame:.        .
-00008d70: 2e2e 0a0a 2020 2020 6465 6620 7265 6164  ....    def read
-00008d80: 5f70 616e 6461 7328 0a20 2020 2020 2020  _pandas(.       
-00008d90: 2073 656c 662c 2070 616e 6461 735f 6461   self, pandas_da
-00008da0: 7461 6672 616d 653a 2055 6e69 6f6e 5b70  taframe: Union[p
-00008db0: 616e 6461 732e 4461 7461 4672 616d 652c  andas.DataFrame,
-00008dc0: 2070 616e 6461 732e 5365 7269 6573 2c20   pandas.Series, 
-00008dd0: 7061 6e64 6173 2e49 6e64 6578 5d0a 2020  pandas.Index].  
-00008de0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00008df0: 4c6f 6164 7320 4461 7461 4672 616d 6520  Loads DataFrame 
-00008e00: 6672 6f6d 2061 2070 616e 6461 7320 4461  from a pandas Da
-00008e10: 7461 4672 616d 652e 0a0a 2020 2020 2020  taFrame...      
-00008e20: 2020 5468 6520 7061 6e64 6173 2044 6174    The pandas Dat
-00008e30: 6146 7261 6d65 2077 696c 6c20 6265 2070  aFrame will be p
-00008e40: 6572 7369 7374 6564 2061 7320 6120 7465  ersisted as a te
-00008e50: 6d70 6f72 6172 7920 4269 6751 7565 7279  mporary BigQuery
-00008e60: 2074 6162 6c65 2c20 7768 6963 6820 6361   table, which ca
-00008e70: 6e20 6265 0a20 2020 2020 2020 2061 7574  n be.        aut
-00008e80: 6f6d 6174 6963 616c 6c79 2072 6563 7963  omatically recyc
-00008e90: 6c65 6420 6166 7465 7220 7468 6520 5365  led after the Se
-00008ea0: 7373 696f 6e20 6973 2063 6c6f 7365 642e  ssion is closed.
-00008eb0: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
-00008ec0: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
-00008ed0: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
-00008ee0: 6269 6766 7261 6d65 732e 7061 6e64 6173  bigframes.pandas
-00008ef0: 2061 7320 6270 640a 2020 2020 2020 2020   as bpd.        
-00008f00: 2020 2020 3e3e 3e20 696d 706f 7274 2070      >>> import p
-00008f10: 616e 6461 7320 6173 2070 640a 2020 2020  andas as pd.    
-00008f20: 2020 2020 2020 2020 3e3e 3e20 6270 642e          >>> bpd.
-00008f30: 6f70 7469 6f6e 732e 6469 7370 6c61 792e  options.display.
-00008f40: 7072 6f67 7265 7373 5f62 6172 203d 204e  progress_bar = N
-00008f50: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
-00008f60: 203e 3e3e 2064 203d 207b 2763 6f6c 3127   >>> d = {'col1'
-00008f70: 3a20 5b31 2c20 325d 2c20 2763 6f6c 3227  : [1, 2], 'col2'
-00008f80: 3a20 5b33 2c20 345d 7d0a 2020 2020 2020  : [3, 4]}.      
-00008f90: 2020 2020 2020 3e3e 3e20 7061 6e64 6173        >>> pandas
-00008fa0: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
-00008fb0: 6d65 2864 6174 613d 6429 0a20 2020 2020  me(data=d).     
-00008fc0: 2020 2020 2020 203e 3e3e 2064 6620 3d20         >>> df = 
-00008fd0: 6270 642e 7265 6164 5f70 616e 6461 7328  bpd.read_pandas(
-00008fe0: 7061 6e64 6173 5f64 6629 0a20 2020 2020  pandas_df).     
-00008ff0: 2020 2020 2020 203e 3e3e 2064 660a 2020         >>> df.  
-00009000: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00009010: 3120 2063 6f6c 320a 2020 2020 2020 2020  1  col2.        
-00009020: 2020 2020 3020 2020 2020 3120 2020 2020      0     1     
-00009030: 330a 2020 2020 2020 2020 2020 2020 3120  3.            1 
-00009040: 2020 2020 3220 2020 2020 340a 2020 2020      2     4.    
-00009050: 2020 2020 2020 2020 3c42 4c41 4e4b 4c49          <BLANKLI
-00009060: 4e45 3e0a 2020 2020 2020 2020 2020 2020  NE>.            
-00009070: 5b32 2072 6f77 7320 7820 3220 636f 6c75  [2 rows x 2 colu
-00009080: 6d6e 735d 0a0a 2020 2020 2020 2020 4172  mns]..        Ar
-00009090: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000090a0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-000090b0: 2028 7061 6e64 6173 2e44 6174 6146 7261   (pandas.DataFra
-000090c0: 6d65 2c20 7061 6e64 6173 2e53 6572 6965  me, pandas.Serie
-000090d0: 732c 206f 7220 7061 6e64 6173 2e49 6e64  s, or pandas.Ind
-000090e0: 6578 293a 0a20 2020 2020 2020 2020 2020  ex):.           
-000090f0: 2020 2020 2061 2070 616e 6461 7320 4461       a pandas Da
-00009100: 7461 4672 616d 652f 5365 7269 6573 2f49  taFrame/Series/I
-00009110: 6e64 6578 206f 626a 6563 7420 746f 2062  ndex object to b
-00009120: 6520 6c6f 6164 6564 2e0a 0a20 2020 2020  e loaded...     
-00009130: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00009140: 2020 2020 2020 2020 416e 2065 7175 6976          An equiv
-00009150: 616c 656e 7420 6269 6766 7261 6d65 732e  alent bigframes.
-00009160: 7061 6e64 6173 2e28 4461 7461 4672 616d  pandas.(DataFram
-00009170: 652f 5365 7269 6573 2f49 6e64 6578 2920  e/Series/Index) 
-00009180: 6f62 6a65 6374 0a20 2020 2020 2020 2022  object.        "
-00009190: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
-000091a0: 7420 6269 6766 7261 6d65 732e 7365 7269  t bigframes.seri
-000091b0: 6573 2061 7320 7365 7269 6573 0a0a 2020  es as series..  
-000091c0: 2020 2020 2020 2320 5472 7920 746f 2068        # Try to h
-000091d0: 616e 646c 6520 6e6f 6e2d 6461 7461 6672  andle non-datafr
-000091e0: 616d 6520 7061 6e64 6173 206f 626a 6563  ame pandas objec
-000091f0: 7473 2061 7320 7765 6c6c 0a20 2020 2020  ts as well.     
-00009200: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00009210: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
-00009220: 652c 2070 616e 6461 732e 5365 7269 6573  e, pandas.Series
-00009230: 293a 0a20 2020 2020 2020 2020 2020 2062  ):.            b
-00009240: 665f 6466 203d 2073 656c 662e 5f72 6561  f_df = self._rea
-00009250: 645f 7061 6e64 6173 2870 616e 6461 732e  d_pandas(pandas.
-00009260: 4461 7461 4672 616d 6528 7061 6e64 6173  DataFrame(pandas
-00009270: 5f64 6174 6166 7261 6d65 292c 2022 7265  _dataframe), "re
-00009280: 6164 5f70 616e 6461 7322 290a 2020 2020  ad_pandas").    
-00009290: 2020 2020 2020 2020 6266 5f73 6572 6965          bf_serie
-000092a0: 7320 3d20 7479 7069 6e67 2e63 6173 7428  s = typing.cast(
-000092b0: 7365 7269 6573 2e53 6572 6965 732c 2062  series.Series, b
-000092c0: 665f 6466 5b62 665f 6466 2e63 6f6c 756d  f_df[bf_df.colum
-000092d0: 6e73 5b30 5d5d 290a 2020 2020 2020 2020  ns[0]]).        
-000092e0: 2020 2020 2320 7772 6170 7069 6e67 2069      # wrapping i
-000092f0: 6e74 6f20 6466 2063 616e 2073 6574 206e  nto df can set n
-00009300: 616d 6520 746f 2030 2073 6f20 7265 7365  ame to 0 so rese
-00009310: 7420 746f 206f 7269 6769 6e61 6c20 6f62  t to original ob
-00009320: 6a65 6374 206e 616d 650a 2020 2020 2020  ject name.      
-00009330: 2020 2020 2020 6266 5f73 6572 6965 732e        bf_series.
-00009340: 6e61 6d65 203d 2070 616e 6461 735f 6461  name = pandas_da
-00009350: 7461 6672 616d 652e 6e61 6d65 0a20 2020  taframe.name.   
-00009360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009370: 6266 5f73 6572 6965 730a 2020 2020 2020  bf_series.      
-00009380: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00009390: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-000093a0: 2c20 7061 6e64 6173 2e49 6e64 6578 293a  , pandas.Index):
-000093b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000093c0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f70  urn self._read_p
-000093d0: 616e 6461 7328 0a20 2020 2020 2020 2020  andas(.         
-000093e0: 2020 2020 2020 2070 616e 6461 732e 4461         pandas.Da
-000093f0: 7461 4672 616d 6528 696e 6465 783d 7061  taFrame(index=pa
-00009400: 6e64 6173 5f64 6174 6166 7261 6d65 292c  ndas_dataframe),
-00009410: 2022 7265 6164 5f70 616e 6461 7322 0a20   "read_pandas". 
-00009420: 2020 2020 2020 2020 2020 2029 2e69 6e64             ).ind
-00009430: 6578 0a20 2020 2020 2020 2069 6620 6973  ex.        if is
-00009440: 696e 7374 616e 6365 2870 616e 6461 735f  instance(pandas_
-00009450: 6461 7461 6672 616d 652c 2070 616e 6461  dataframe, panda
-00009460: 732e 4461 7461 4672 616d 6529 3a0a 2020  s.DataFrame):.  
-00009470: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009480: 2073 656c 662e 5f72 6561 645f 7061 6e64   self._read_pand
-00009490: 6173 2870 616e 6461 735f 6461 7461 6672  as(pandas_datafr
-000094a0: 616d 652c 2022 7265 6164 5f70 616e 6461  ame, "read_panda
-000094b0: 7322 290a 2020 2020 2020 2020 656c 7365  s").        else
-000094c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000094d0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 6622 7265 6164 5f70 616e 6461 7328 2920  f"read_pandas() 
-00009500: 6578 7065 6374 7320 6120 7061 6e64 6173  expects a pandas
-00009510: 2e44 6174 6146 7261 6d65 2c20 6275 7420  .DataFrame, but 
-00009520: 676f 7420 6120 7b74 7970 6528 7061 6e64  got a {type(pand
-00009530: 6173 5f64 6174 6166 7261 6d65 297d 220a  as_dataframe)}".
-00009540: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00009550: 2020 2064 6566 205f 7265 6164 5f70 616e     def _read_pan
-00009560: 6461 7328 0a20 2020 2020 2020 2073 656c  das(.        sel
-00009570: 662c 2070 616e 6461 735f 6461 7461 6672  f, pandas_datafr
-00009580: 616d 653a 2070 616e 6461 732e 4461 7461  ame: pandas.Data
-00009590: 4672 616d 652c 2061 7069 5f6e 616d 653a  Frame, api_name:
-000095a0: 2073 7472 0a20 2020 2029 202d 3e20 6461   str.    ) -> da
-000095b0: 7461 6672 616d 652e 4461 7461 4672 616d  taframe.DataFram
-000095c0: 653a 0a20 2020 2020 2020 2069 6d70 6f72  e:.        impor
-000095d0: 7420 6269 6766 7261 6d65 732e 6461 7461  t bigframes.data
-000095e0: 6672 616d 6520 6173 2064 6174 6166 7261  frame as datafra
-000095f0: 6d65 0a0a 2020 2020 2020 2020 6966 2069  me..        if i
-00009600: 7369 6e73 7461 6e63 6528 7061 6e64 6173  sinstance(pandas
-00009610: 5f64 6174 6166 7261 6d65 2c20 6461 7461  _dataframe, data
-00009620: 6672 616d 652e 4461 7461 4672 616d 6529  frame.DataFrame)
-00009630: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00009640: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 2272 6561 645f 7061 6e64 6173 2829 2065  "read_pandas() e
-00009670: 7870 6563 7473 2061 2070 616e 6461 732e  xpects a pandas.
-00009680: 4461 7461 4672 616d 652c 2062 7574 2067  DataFrame, but g
-00009690: 6f74 2061 2022 0a20 2020 2020 2020 2020  ot a ".         
-000096a0: 2020 2020 2020 2022 6269 6766 7261 6d65         "bigframe
-000096b0: 732e 7061 6e64 6173 2e44 6174 6146 7261  s.pandas.DataFra
-000096c0: 6d65 2e22 0a20 2020 2020 2020 2020 2020  me.".           
-000096d0: 2029 0a0a 2020 2020 2020 2020 696e 6c69   )..        inli
-000096e0: 6e65 5f64 6620 3d20 7365 6c66 2e5f 7265  ne_df = self._re
-000096f0: 6164 5f70 616e 6461 735f 696e 6c69 6e65  ad_pandas_inline
-00009700: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
-00009710: 6529 0a20 2020 2020 2020 2069 6620 696e  e).        if in
-00009720: 6c69 6e65 5f64 6620 6973 206e 6f74 204e  line_df is not N
-00009730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00009740: 2072 6574 7572 6e20 696e 6c69 6e65 5f64   return inline_d
-00009750: 660a 2020 2020 2020 2020 7472 793a 0a20  f.        try:. 
-00009760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009770: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
-00009780: 6461 735f 6c6f 6164 5f6a 6f62 2870 616e  das_load_job(pan
-00009790: 6461 735f 6461 7461 6672 616d 652c 2061  das_dataframe, a
-000097a0: 7069 5f6e 616d 6529 0a20 2020 2020 2020  pi_name).       
-000097b0: 2065 7863 6570 7420 7061 2e41 7272 6f77   except pa.Arrow
-000097c0: 496e 7661 6c69 6420 6173 2065 3a0a 2020  Invalid as e:.  
-000097d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000097e0: 7061 2e41 7272 6f77 496e 7661 6c69 6428  pa.ArrowInvalid(
-000097f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009800: 2066 2243 6f75 6c64 206e 6f74 2063 6f6e   f"Could not con
-00009810: 7665 7274 2077 6974 6820 6120 4269 6751  vert with a BigQ
-00009820: 7565 7279 2074 7970 653a 2060 7b65 7d60  uery type: `{e}`
-00009830: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00009840: 2920 6672 6f6d 2065 0a0a 2020 2020 6465  ) from e..    de
-00009850: 6620 5f72 6561 645f 7061 6e64 6173 5f69  f _read_pandas_i
-00009860: 6e6c 696e 6528 0a20 2020 2020 2020 2073  nline(.        s
-00009870: 656c 662c 2070 616e 6461 735f 6461 7461  elf, pandas_data
-00009880: 6672 616d 653a 2070 616e 6461 732e 4461  frame: pandas.Da
-00009890: 7461 4672 616d 650a 2020 2020 2920 2d3e  taFrame.    ) ->
-000098a0: 204f 7074 696f 6e61 6c5b 6461 7461 6672   Optional[datafr
-000098b0: 616d 652e 4461 7461 4672 616d 655d 3a0a  ame.DataFrame]:.
-000098c0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
-000098d0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
-000098e0: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
-000098f0: 0a20 2020 2020 2020 2069 6620 7061 6e64  .        if pand
-00009900: 6173 5f64 6174 6166 7261 6d65 2e6d 656d  as_dataframe.mem
-00009910: 6f72 795f 7573 6167 6528 6465 6570 3d54  ory_usage(deep=T
-00009920: 7275 6529 2e73 756d 2829 203e 204d 4158  rue).sum() > MAX
-00009930: 5f49 4e4c 494e 455f 4446 5f42 5954 4553  _INLINE_DF_BYTES
-00009940: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009950: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
-00009960: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00009970: 2020 2020 696e 6c69 6e65 5f64 6620 3d20      inline_df = 
-00009980: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
-00009990: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
-000099a0: 2020 2020 2062 6c6f 636b 732e 426c 6f63       blocks.Bloc
-000099b0: 6b2e 6672 6f6d 5f6c 6f63 616c 2870 616e  k.from_local(pan
-000099c0: 6461 735f 6461 7461 6672 616d 652c 2073  das_dataframe, s
-000099d0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-000099e0: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
-000099f0: 7420 7061 2e41 7272 6f77 496e 7661 6c69  t pa.ArrowInvali
-00009a00: 6420 6173 2065 3a0a 2020 2020 2020 2020  d as e:.        
-00009a10: 2020 2020 7261 6973 6520 7061 2e41 7272      raise pa.Arr
-00009a20: 6f77 496e 7661 6c69 6428 0a20 2020 2020  owInvalid(.     
-00009a30: 2020 2020 2020 2020 2020 2066 2243 6f75             f"Cou
-00009a40: 6c64 206e 6f74 2063 6f6e 7665 7274 2077  ld not convert w
-00009a50: 6974 6820 6120 4269 6751 7565 7279 2074  ith a BigQuery t
-00009a60: 7970 653a 2060 7b65 7d60 2e20 220a 2020  ype: `{e}`. ".  
-00009a70: 2020 2020 2020 2020 2020 2920 6672 6f6d            ) from
-00009a80: 2065 0a20 2020 2020 2020 2065 7863 6570   e.        excep
-00009a90: 7420 5661 6c75 6545 7272 6f72 3a20 2023  t ValueError:  #
-00009aa0: 2054 6872 6f77 6e20 6279 2069 6269 7320   Thrown by ibis 
-00009ab0: 666f 7220 736f 6d65 2075 6e68 616e 646c  for some unhandl
-00009ac0: 6564 2074 7970 6573 0a20 2020 2020 2020  ed types.       
-00009ad0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00009ae0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00009af0: 7061 2e41 7272 6f77 5479 7065 4572 726f  pa.ArrowTypeErro
-00009b00: 723a 2020 2320 5468 726f 776e 2062 7920  r:  # Thrown by 
-00009b10: 6172 726f 7720 666f 7220 7479 7065 7320  arrow for types 
-00009b20: 7769 7468 6f75 7420 6d61 7070 696e 6720  without mapping 
-00009b30: 2867 656f 292e 0a20 2020 2020 2020 2020  (geo)..         
-00009b40: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00009b50: 2020 2020 2020 2020 696e 6c69 6e65 5f74          inline_t
-00009b60: 7970 6573 203d 2069 6e6c 696e 655f 6466  ypes = inline_df
-00009b70: 2e5f 626c 6f63 6b2e 6578 7072 2e73 6368  ._block.expr.sch
-00009b80: 656d 612e 6474 7970 6573 0a20 2020 2020  ema.dtypes.     
-00009b90: 2020 2023 2049 6269 7320 6861 7320 7072     # Ibis has pr
-00009ba0: 6f62 6c65 6d73 2065 7363 6170 696e 6720  oblems escaping 
-00009bb0: 6279 7465 7320 6c69 7465 7261 6c73 2c20  bytes literals, 
-00009bc0: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
-00009bd0: 2073 796e 7461 7820 6572 726f 7273 2073   syntax errors s
-00009be0: 6572 7665 722d 7369 6465 2e0a 2020 2020  erver-side..    
-00009bf0: 2020 2020 6966 2061 6c6c 2864 7479 7065      if all(dtype
-00009c00: 2069 6e20 494e 4c49 4e41 424c 455f 4454   in INLINABLE_DT
-00009c10: 5950 4553 2066 6f72 2064 7479 7065 2069  YPES for dtype i
-00009c20: 6e20 696e 6c69 6e65 5f74 7970 6573 293a  n inline_types):
-00009c30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009c40: 7572 6e20 696e 6c69 6e65 5f64 660a 2020  urn inline_df.  
-00009c50: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00009c60: 650a 0a20 2020 2064 6566 205f 7265 6164  e..    def _read
-00009c70: 5f70 616e 6461 735f 6c6f 6164 5f6a 6f62  _pandas_load_job
-00009c80: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00009c90: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
-00009ca0: 3a20 7061 6e64 6173 2e44 6174 6146 7261  : pandas.DataFra
-00009cb0: 6d65 2c20 6170 695f 6e61 6d65 3a20 7374  me, api_name: st
-00009cc0: 720a 2020 2020 2920 2d3e 2064 6174 6166  r.    ) -> dataf
-00009cd0: 7261 6d65 2e44 6174 6146 7261 6d65 3a0a  rame.DataFrame:.
-00009ce0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
-00009cf0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
-00009d00: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
-00009d10: 0a20 2020 2020 2020 2063 6f6c 5f69 6e64  .        col_ind
-00009d20: 6578 203d 2070 616e 6461 735f 6461 7461  ex = pandas_data
-00009d30: 6672 616d 652e 636f 6c75 6d6e 732e 636f  frame.columns.co
-00009d40: 7079 2829 0a20 2020 2020 2020 2063 6f6c  py().        col
-00009d50: 5f6c 6162 656c 732c 2069 6478 5f6c 6162  _labels, idx_lab
-00009d60: 656c 7320 3d20 280a 2020 2020 2020 2020  els = (.        
-00009d70: 2020 2020 636f 6c5f 696e 6465 782e 746f      col_index.to
-00009d80: 5f6c 6973 7428 292c 0a20 2020 2020 2020  _list(),.       
-00009d90: 2020 2020 2070 616e 6461 735f 6461 7461       pandas_data
-00009da0: 6672 616d 652e 696e 6465 782e 6e61 6d65  frame.index.name
-00009db0: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
-00009dc0: 2020 2020 206e 6577 5f63 6f6c 5f69 6473       new_col_ids
-00009dd0: 2c20 6e65 775f 6964 785f 6964 7320 3d20  , new_idx_ids = 
-00009de0: 7574 696c 732e 6765 745f 7374 616e 6461  utils.get_standa
-00009df0: 7264 697a 6564 5f69 6473 280a 2020 2020  rdized_ids(.    
-00009e00: 2020 2020 2020 2020 636f 6c5f 6c61 6265          col_labe
-00009e10: 6c73 2c0a 2020 2020 2020 2020 2020 2020  ls,.            
-00009e20: 6964 785f 6c61 6265 6c73 2c0a 2020 2020  idx_labels,.    
-00009e30: 2020 2020 2020 2020 2320 4c6f 6164 696e          # Loadin
-00009e40: 6720 7061 7271 7565 7420 6669 6c65 7320  g parquet files 
-00009e50: 696e 746f 2042 6967 5175 6572 7920 7769  into BigQuery wi
-00009e60: 7468 2073 7065 6369 616c 2063 6f6c 756d  th special colum
-00009e70: 6e20 6e61 6d65 730a 2020 2020 2020 2020  n names.        
-00009e80: 2020 2020 2320 6973 206f 6e6c 7920 7375      # is only su
-00009e90: 7070 6f72 7465 6420 756e 6465 7220 616e  pported under an
-00009ea0: 2061 6c6c 6f77 6c69 7374 2e0a 2020 2020   allowlist..    
-00009eb0: 2020 2020 2020 2020 7374 7269 6374 3d54          strict=T
-00009ec0: 7275 652c 0a20 2020 2020 2020 2029 0a0a  rue,.        )..
-00009ed0: 2020 2020 2020 2020 2320 4164 6420 6f72          # Add or
-00009ee0: 6465 7220 636f 6c75 6d6e 2074 6f20 7061  der column to pa
-00009ef0: 6e64 6173 2044 6174 6146 7261 6d65 2074  ndas DataFrame t
-00009f00: 6f20 7072 6573 6572 7665 206f 7264 6572  o preserve order
-00009f10: 2069 6e20 4269 6751 7565 7279 0a20 2020   in BigQuery.   
-00009f20: 2020 2020 206f 7264 6572 696e 675f 636f       ordering_co
-00009f30: 6c20 3d20 2272 6f77 6964 220a 2020 2020  l = "rowid".    
-00009f40: 2020 2020 636f 6c75 6d6e 7320 3d20 6672      columns = fr
-00009f50: 6f7a 656e 7365 7428 636f 6c5f 6c61 6265  ozenset(col_labe
-00009f60: 6c73 202b 2069 6478 5f6c 6162 656c 7329  ls + idx_labels)
-00009f70: 0a20 2020 2020 2020 2073 7566 6669 7820  .        suffix 
-00009f80: 3d20 320a 2020 2020 2020 2020 7768 696c  = 2.        whil
-00009f90: 6520 6f72 6465 7269 6e67 5f63 6f6c 2069  e ordering_col i
-00009fa0: 6e20 636f 6c75 6d6e 733a 0a20 2020 2020  n columns:.     
-00009fb0: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
-00009fc0: 636f 6c20 3d20 6622 726f 7769 645f 7b73  col = f"rowid_{s
-00009fd0: 7566 6669 787d 220a 2020 2020 2020 2020  uffix}".        
-00009fe0: 2020 2020 7375 6666 6978 202b 3d20 310a      suffix += 1.
-00009ff0: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
-0000a000: 6461 7461 6672 616d 655f 636f 7079 203d  dataframe_copy =
-0000a010: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-0000a020: 652e 636f 7079 2829 0a20 2020 2020 2020  e.copy().       
-0000a030: 2070 616e 6461 735f 6461 7461 6672 616d   pandas_datafram
-0000a040: 655f 636f 7079 2e69 6e64 6578 2e6e 616d  e_copy.index.nam
-0000a050: 6573 203d 206e 6577 5f69 6478 5f69 6473  es = new_idx_ids
-0000a060: 0a20 2020 2020 2020 2070 616e 6461 735f  .        pandas_
-0000a070: 6461 7461 6672 616d 655f 636f 7079 2e63  dataframe_copy.c
-0000a080: 6f6c 756d 6e73 203d 2070 616e 6461 732e  olumns = pandas.
-0000a090: 496e 6465 7828 6e65 775f 636f 6c5f 6964  Index(new_col_id
-0000a0a0: 7329 0a20 2020 2020 2020 2070 616e 6461  s).        panda
-0000a0b0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
-0000a0c0: 5b6f 7264 6572 696e 675f 636f 6c5d 203d  [ordering_col] =
-0000a0d0: 206e 702e 6172 616e 6765 2870 616e 6461   np.arange(panda
-0000a0e0: 735f 6461 7461 6672 616d 655f 636f 7079  s_dataframe_copy
-0000a0f0: 2e73 6861 7065 5b30 5d29 0a0a 2020 2020  .shape[0])..    
-0000a100: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
-0000a110: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
-0000a120: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
-0000a130: 0a0a 2020 2020 2020 2020 2320 5370 6563  ..        # Spec
-0000a140: 6966 7920 7468 6520 6461 7465 7469 6d65  ify the datetime
-0000a150: 2064 7479 7065 732c 2077 6869 6368 2069   dtypes, which i
-0000a160: 7320 6175 746f 2d64 6574 6563 7465 6420  s auto-detected 
-0000a170: 6173 2074 696d 6573 7461 6d70 2074 7970  as timestamp typ
-0000a180: 6573 2e0a 2020 2020 2020 2020 7363 6865  es..        sche
-0000a190: 6d61 3a20 6c69 7374 5b62 6967 7175 6572  ma: list[bigquer
-0000a1a0: 792e 5363 6865 6d61 4669 656c 645d 203d  y.SchemaField] =
-0000a1b0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0000a1c0: 636f 6c75 6d6e 2c20 6474 7970 6520 696e  column, dtype in
-0000a1d0: 207a 6970 286e 6577 5f63 6f6c 5f69 6473   zip(new_col_ids
-0000a1e0: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
-0000a1f0: 6d65 2e64 7479 7065 7329 3a0a 2020 2020  me.dtypes):.    
-0000a200: 2020 2020 2020 2020 6966 2064 7479 7065          if dtype
-0000a210: 203d 3d20 2274 696d 6573 7461 6d70 5b75   == "timestamp[u
-0000a220: 735d 5b70 7961 7272 6f77 5d22 3a0a 2020  s][pyarrow]":.  
-0000a230: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0000a240: 6865 6d61 2e61 7070 656e 6428 0a20 2020  hema.append(.   
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2062 6967 7175 6572 792e 5363 6865 6d61   bigquery.Schema
-0000a270: 4669 656c 6428 636f 6c75 6d6e 2c20 6269  Field(column, bi
-0000a280: 6771 7565 7279 2e65 6e75 6d73 2e53 716c  gquery.enums.Sql
-0000a290: 5479 7065 4e61 6d65 732e 4441 5445 5449  TypeNames.DATETI
-0000a2a0: 4d45 290a 2020 2020 2020 2020 2020 2020  ME).            
-0000a2b0: 2020 2020 290a 2020 2020 2020 2020 6a6f      ).        jo
-0000a2c0: 625f 636f 6e66 6967 2e73 6368 656d 6120  b_config.schema 
-0000a2d0: 3d20 7363 6865 6d61 0a0a 2020 2020 2020  = schema..      
-0000a2e0: 2020 2320 436c 7573 7465 7269 6e67 2070    # Clustering p
-0000a2f0: 726f 6261 626c 7920 6e6f 7420 6e65 6564  robably not need
-0000a300: 6564 2061 6e79 7761 7973 2061 7320 7061  ed anyways as pa
-0000a310: 6e64 6173 2074 6162 6c65 7320 6172 6520  ndas tables are 
-0000a320: 736d 616c 6c0a 2020 2020 2020 2020 636c  small.        cl
-0000a330: 7573 7465 725f 636f 6c73 203d 205b 6f72  uster_cols = [or
-0000a340: 6465 7269 6e67 5f63 6f6c 5d0a 2020 2020  dering_col].    
-0000a350: 2020 2020 6a6f 625f 636f 6e66 6967 2e63      job_config.c
-0000a360: 6c75 7374 6572 696e 675f 6669 656c 6473  lustering_fields
-0000a370: 203d 2063 6c75 7374 6572 5f63 6f6c 730a   = cluster_cols.
-0000a380: 0a20 2020 2020 2020 206a 6f62 5f63 6f6e  .        job_con
-0000a390: 6669 672e 6c61 6265 6c73 203d 207b 2262  fig.labels = {"b
-0000a3a0: 6967 6672 616d 6573 2d61 7069 223a 2061  igframes-api": a
-0000a3b0: 7069 5f6e 616d 657d 0a0a 2020 2020 2020  pi_name}..      
-0000a3c0: 2020 6c6f 6164 5f74 6162 6c65 5f64 6573    load_table_des
-0000a3d0: 7469 6e61 7469 6f6e 203d 2062 6967 6672  tination = bigfr
-0000a3e0: 616d 6573 5f69 6f2e 7261 6e64 6f6d 5f74  ames_io.random_t
-0000a3f0: 6162 6c65 2873 656c 662e 5f61 6e6f 6e79  able(self._anony
-0000a400: 6d6f 7573 5f64 6174 6173 6574 290a 2020  mous_dataset).  
-0000a410: 2020 2020 2020 6c6f 6164 5f6a 6f62 203d        load_job =
-0000a420: 2073 656c 662e 6271 636c 6965 6e74 2e6c   self.bqclient.l
-0000a430: 6f61 645f 7461 626c 655f 6672 6f6d 5f64  oad_table_from_d
-0000a440: 6174 6166 7261 6d65 280a 2020 2020 2020  ataframe(.      
-0000a450: 2020 2020 2020 7061 6e64 6173 5f64 6174        pandas_dat
-0000a460: 6166 7261 6d65 5f63 6f70 792c 0a20 2020  aframe_copy,.   
-0000a470: 2020 2020 2020 2020 206c 6f61 645f 7461           load_ta
-0000a480: 626c 655f 6465 7374 696e 6174 696f 6e2c  ble_destination,
-0000a490: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000a4a0: 5f63 6f6e 6669 673d 6a6f 625f 636f 6e66  _config=job_conf
-0000a4b0: 6967 2c0a 2020 2020 2020 2020 290a 2020  ig,.        ).  
-0000a4c0: 2020 2020 2020 7365 6c66 2e5f 7374 6172        self._star
-0000a4d0: 745f 6765 6e65 7269 635f 6a6f 6228 6c6f  t_generic_job(lo
-0000a4e0: 6164 5f6a 6f62 290a 0a20 2020 2020 2020  ad_job)..       
-0000a4f0: 206f 7264 6572 696e 6720 3d20 6f72 6465   ordering = orde
-0000a500: 722e 4578 7072 6573 7369 6f6e 4f72 6465  r.ExpressionOrde
-0000a510: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
-0000a520: 2020 6f72 6465 7269 6e67 5f76 616c 7565    ordering_value
-0000a530: 5f63 6f6c 756d 6e73 3d74 7570 6c65 285b  _columns=tuple([
-0000a540: 6f72 6465 722e 6173 6365 6e64 696e 675f  order.ascending_
-0000a550: 6f76 6572 286f 7264 6572 696e 675f 636f  over(ordering_co
-0000a560: 6c29 5d29 2c0a 2020 2020 2020 2020 2020  l)]),.          
-0000a570: 2020 746f 7461 6c5f 6f72 6465 7269 6e67    total_ordering
-0000a580: 5f63 6f6c 756d 6e73 3d66 726f 7a65 6e73  _columns=frozens
-0000a590: 6574 285b 6f72 6465 7269 6e67 5f63 6f6c  et([ordering_col
-0000a5a0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0000a5b0: 696e 7465 6765 725f 656e 636f 6469 6e67  integer_encoding
-0000a5c0: 3d49 6e74 6567 6572 456e 636f 6469 6e67  =IntegerEncoding
-0000a5d0: 2854 7275 652c 2069 735f 7365 7175 656e  (True, is_sequen
-0000a5e0: 7469 616c 3d54 7275 6529 2c0a 2020 2020  tial=True),.    
-0000a5f0: 2020 2020 290a 2020 2020 2020 2020 7461      ).        ta
-0000a600: 626c 655f 6578 7072 6573 7369 6f6e 203d  ble_expression =
-0000a610: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
-0000a620: 742e 7461 626c 6528 2020 2320 7479 7065  t.table(  # type
-0000a630: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
-0000a640: 2020 2020 206c 6f61 645f 7461 626c 655f       load_table_
-0000a650: 6465 7374 696e 6174 696f 6e2e 7461 626c  destination.tabl
-0000a660: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-0000a670: 2020 7363 6865 6d61 3d6c 6f61 645f 7461    schema=load_ta
-0000a680: 626c 655f 6465 7374 696e 6174 696f 6e2e  ble_destination.
-0000a690: 6461 7461 7365 745f 6964 2c0a 2020 2020  dataset_id,.    
-0000a6a0: 2020 2020 2020 2020 6461 7461 6261 7365          database
-0000a6b0: 3d6c 6f61 645f 7461 626c 655f 6465 7374  =load_table_dest
-0000a6c0: 696e 6174 696f 6e2e 7072 6f6a 6563 742c  ination.project,
-0000a6d0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000a6e0: 2020 2020 2320 622f 3239 3735 3930 3137      # b/29759017
-0000a6f0: 3820 506f 7465 6e74 6961 6c6c 7920 6120  8 Potentially a 
-0000a700: 6275 6720 696e 2062 7163 6c69 656e 742e  bug in bqclient.
-0000a710: 6c6f 6164 5f74 6162 6c65 5f66 726f 6d5f  load_table_from_
-0000a720: 6461 7461 6672 616d 6528 292c 2074 6861  dataframe(), tha
-0000a730: 7420 6f6e 6c79 2077 6865 6e20 7468 6520  t only when the 
-0000a740: 4446 2069 7320 656d 7074 792c 2074 6865  DF is empty, the
-0000a750: 2069 6e64 6578 2063 6f6c 756d 6e73 2064   index columns d
-0000a760: 6973 6170 7065 6172 2069 6e20 7461 626c  isappear in tabl
-0000a770: 655f 6578 7072 6573 7369 6f6e 2e0a 2020  e_expression..  
-0000a780: 2020 2020 2020 6966 2061 6e79 280a 2020        if any(.  
-0000a790: 2020 2020 2020 2020 2020 5b6e 6577 5f69            [new_i
-0000a7a0: 6478 5f69 6420 6e6f 7420 696e 2074 6162  dx_id not in tab
-0000a7b0: 6c65 5f65 7870 7265 7373 696f 6e2e 636f  le_expression.co
-0000a7c0: 6c75 6d6e 7320 666f 7220 6e65 775f 6964  lumns for new_id
-0000a7d0: 785f 6964 2069 6e20 6e65 775f 6964 785f  x_id in new_idx_
-0000a7e0: 6964 735d 0a20 2020 2020 2020 2029 3a0a  ids].        ):.
-0000a7f0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000a800: 6964 785f 6964 732c 2069 6478 5f6c 6162  idx_ids, idx_lab
-0000a810: 656c 7320 3d20 5b5d 2c20 5b5d 0a0a 2020  els = [], []..  
-0000a820: 2020 2020 2020 636f 6c75 6d6e 5f76 616c        column_val
-0000a830: 7565 7320 3d20 5b0a 2020 2020 2020 2020  ues = [.        
-0000a840: 2020 2020 7461 626c 655f 6578 7072 6573      table_expres
-0000a850: 7369 6f6e 5b63 6f6c 5d0a 2020 2020 2020  sion[col].      
-0000a860: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-0000a870: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
-0000a880: 6e2e 636f 6c75 6d6e 730a 2020 2020 2020  n.columns.      
-0000a890: 2020 2020 2020 6966 2063 6f6c 2021 3d20        if col != 
-0000a8a0: 6f72 6465 7269 6e67 5f63 6f6c 0a20 2020  ordering_col.   
-0000a8b0: 2020 2020 205d 0a20 2020 2020 2020 2061       ].        a
-0000a8c0: 7272 6179 5f76 616c 7565 203d 2063 6f72  rray_value = cor
-0000a8d0: 652e 4172 7261 7956 616c 7565 2e66 726f  e.ArrayValue.fro
-0000a8e0: 6d5f 6962 6973 280a 2020 2020 2020 2020  m_ibis(.        
-0000a8f0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000a900: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
-0000a910: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
-0000a920: 2020 2020 636f 6c75 6d6e 733d 636f 6c75      columns=colu
-0000a930: 6d6e 5f76 616c 7565 732c 0a20 2020 2020  mn_values,.     
-0000a940: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
-0000a950: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d5b  dering_columns=[
-0000a960: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
-0000a970: 5b6f 7264 6572 696e 675f 636f 6c5d 5d2c  [ordering_col]],
-0000a980: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-0000a990: 6572 696e 673d 6f72 6465 7269 6e67 2c0a  ering=ordering,.
-0000a9a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000a9b0: 2020 2062 6c6f 636b 203d 2062 6c6f 636b     block = block
-0000a9c0: 732e 426c 6f63 6b28 0a20 2020 2020 2020  s.Block(.       
-0000a9d0: 2020 2020 2061 7272 6179 5f76 616c 7565       array_value
-0000a9e0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
-0000a9f0: 6465 785f 636f 6c75 6d6e 733d 6e65 775f  dex_columns=new_
-0000aa00: 6964 785f 6964 732c 0a20 2020 2020 2020  idx_ids,.       
-0000aa10: 2020 2020 2063 6f6c 756d 6e5f 6c61 6265       column_labe
-0000aa20: 6c73 3d63 6f6c 5f69 6e64 6578 2c0a 2020  ls=col_index,.  
-0000aa30: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-0000aa40: 6c61 6265 6c73 3d69 6478 5f6c 6162 656c  labels=idx_label
-0000aa50: 732c 0a20 2020 2020 2020 2029 0a20 2020  s,.        ).   
-0000aa60: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-0000aa70: 6672 616d 652e 4461 7461 4672 616d 6528  frame.DataFrame(
-0000aa80: 626c 6f63 6b29 0a0a 2020 2020 6465 6620  block)..    def 
-0000aa90: 7265 6164 5f63 7376 280a 2020 2020 2020  read_csv(.      
-0000aaa0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000aab0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
-0000aac0: 6572 3a20 7374 7220 7c20 494f 5b22 6279  er: str | IO["by
-0000aad0: 7465 7322 5d2c 0a20 2020 2020 2020 202a  tes"],.        *
-0000aae0: 2c0a 2020 2020 2020 2020 7365 703a 204f  ,.        sep: O
-0000aaf0: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-0000ab00: 2c22 2c0a 2020 2020 2020 2020 6865 6164  ,",.        head
-0000ab10: 6572 3a20 4f70 7469 6f6e 616c 5b69 6e74  er: Optional[int
-0000ab20: 5d20 3d20 302c 0a20 2020 2020 2020 206e  ] = 0,.        n
-0000ab30: 616d 6573 3a20 4f70 7469 6f6e 616c 5b0a  ames: Optional[.
-0000ab40: 2020 2020 2020 2020 2020 2020 556e 696f              Unio
-0000ab50: 6e5b 4d75 7461 626c 6553 6571 7565 6e63  n[MutableSequenc
-0000ab60: 655b 416e 795d 2c20 6e70 2e6e 6461 7272  e[Any], np.ndarr
-0000ab70: 6179 5b41 6e79 2c20 416e 795d 2c20 5475  ay[Any, Any], Tu
-0000ab80: 706c 655b 416e 792c 202e 2e2e 5d2c 2072  ple[Any, ...], r
-0000ab90: 616e 6765 5d0a 2020 2020 2020 2020 5d20  ange].        ] 
-0000aba0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000abb0: 696e 6465 785f 636f 6c3a 204f 7074 696f  index_col: Optio
-0000abc0: 6e61 6c5b 0a20 2020 2020 2020 2020 2020  nal[.           
-0000abd0: 2055 6e69 6f6e 5b69 6e74 2c20 7374 722c   Union[int, str,
-0000abe0: 2053 6571 7565 6e63 655b 556e 696f 6e5b   Sequence[Union[
-0000abf0: 7374 722c 2069 6e74 5d5d 2c20 4c69 7465  str, int]], Lite
-0000ac00: 7261 6c5b 4661 6c73 655d 5d0a 2020 2020  ral[False]].    
-0000ac10: 2020 2020 5d20 3d20 4e6f 6e65 2c0a 2020      ] = None,.  
-0000ac20: 2020 2020 2020 7573 6563 6f6c 733a 204f        usecols: O
-0000ac30: 7074 696f 6e61 6c5b 0a20 2020 2020 2020  ptional[.       
-0000ac40: 2020 2020 2055 6e69 6f6e 5b0a 2020 2020       Union[.    
-0000ac50: 2020 2020 2020 2020 2020 2020 4d75 7461              Muta
-0000ac60: 626c 6553 6571 7565 6e63 655b 7374 725d  bleSequence[str]
-0000ac70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ac80: 2020 5475 706c 655b 7374 722c 202e 2e2e    Tuple[str, ...
-0000ac90: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000aca0: 2020 2053 6571 7565 6e63 655b 696e 745d     Sequence[int]
-0000acb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000acc0: 2020 7061 6e64 6173 2e53 6572 6965 732c    pandas.Series,
-0000acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ace0: 2070 616e 6461 732e 496e 6465 782c 0a20   pandas.Index,. 
-0000acf0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000ad00: 702e 6e64 6172 7261 795b 416e 792c 2041  p.ndarray[Any, A
-0000ad10: 6e79 5d2c 0a20 2020 2020 2020 2020 2020  ny],.           
-0000ad20: 2020 2020 2043 616c 6c61 626c 655b 5b41       Callable[[A
-0000ad30: 6e79 5d2c 2062 6f6f 6c5d 2c0a 2020 2020  ny], bool],.    
-0000ad40: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000ad50: 2020 5d20 3d20 4e6f 6e65 2c0a 2020 2020    ] = None,.    
-0000ad60: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
-0000ad70: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
-0000ad80: 2c0a 2020 2020 2020 2020 656e 6769 6e65  ,.        engine
-0000ad90: 3a20 4f70 7469 6f6e 616c 5b0a 2020 2020  : Optional[.    
-0000ada0: 2020 2020 2020 2020 4c69 7465 7261 6c5b          Literal[
-0000adb0: 2263 222c 2022 7079 7468 6f6e 222c 2022  "c", "python", "
-0000adc0: 7079 6172 726f 7722 2c20 2270 7974 686f  pyarrow", "pytho
-0000add0: 6e2d 6677 6622 2c20 2262 6967 7175 6572  n-fwf", "bigquer
-0000ade0: 7922 5d0a 2020 2020 2020 2020 5d20 3d20  y"].        ] = 
-0000adf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
-0000ae00: 636f 6469 6e67 3a20 4f70 7469 6f6e 616c  coding: Optional
-0000ae10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000ae20: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
-0000ae30: 2020 2020 2920 2d3e 2064 6174 6166 7261      ) -> datafra
-0000ae40: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
-0000ae50: 2020 2020 2020 7461 626c 6520 3d20 6269        table = bi
-0000ae60: 6766 7261 6d65 735f 696f 2e72 616e 646f  gframes_io.rando
-0000ae70: 6d5f 7461 626c 6528 7365 6c66 2e5f 616e  m_table(self._an
-0000ae80: 6f6e 796d 6f75 735f 6461 7461 7365 7429  onymous_dataset)
-0000ae90: 0a0a 2020 2020 2020 2020 6966 2065 6e67  ..        if eng
-0000aea0: 696e 6520 6973 206e 6f74 204e 6f6e 6520  ine is not None 
-0000aeb0: 616e 6420 656e 6769 6e65 203d 3d20 2262  and engine == "b
-0000aec0: 6967 7175 6572 7922 3a0a 2020 2020 2020  igquery":.      
-0000aed0: 2020 2020 2020 6966 2061 6e79 2870 6172        if any(par
-0000aee0: 616d 2069 7320 6e6f 7420 4e6f 6e65 2066  am is not None f
-0000aef0: 6f72 2070 6172 616d 2069 6e20 2864 7479  or param in (dty
-0000af00: 7065 2c20 6e61 6d65 7329 293a 0a20 2020  pe, names)):.   
-0000af10: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-0000af20: 5f73 7570 706f 7274 6564 203d 2028 2264  _supported = ("d
-0000af30: 7479 7065 222c 2022 6e61 6d65 7322 290a  type", "names").
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
-0000af60: 6e74 6564 4572 726f 7228 0a20 2020 2020  ntedError(.     
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000af80: 2242 6967 5175 6572 7920 656e 6769 6e65  "BigQuery engine
-0000af90: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-0000afa0: 7420 7468 6573 6520 6172 6775 6d65 6e74  t these argument
-0000afb0: 733a 207b 6e6f 745f 7375 7070 6f72 7465  s: {not_supporte
-0000afc0: 647d 2e20 220a 2020 2020 2020 2020 2020  d}. ".          
-0000afd0: 2020 2020 2020 2020 2020 6622 7b63 6f6e            f"{con
-0000afe0: 7374 616e 7473 2e46 4545 4442 4143 4b5f  stants.FEEDBACK_
-0000aff0: 4c49 4e4b 7d22 0a20 2020 2020 2020 2020  LINK}".         
-0000b000: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000b010: 2020 2020 2020 6966 2069 6e64 6578 5f63        if index_c
-0000b020: 6f6c 2069 7320 6e6f 7420 4e6f 6e65 2061  ol is not None a
-0000b030: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
-0000b040: 2020 2020 206e 6f74 2069 6e64 6578 5f63       not index_c
-0000b050: 6f6c 206f 7220 6e6f 7420 6973 696e 7374  ol or not isinst
-0000b060: 616e 6365 2869 6e64 6578 5f63 6f6c 2c20  ance(index_col, 
-0000b070: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
-0000b080: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000b090: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-0000b0a0: 6c65 6d65 6e74 6564 4572 726f 7228 0a20  lementedError(. 
-0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0c0: 2020 2022 4269 6751 7565 7279 2065 6e67     "BigQuery eng
-0000b0d0: 696e 6520 6f6e 6c79 2073 7570 706f 7274  ine only support
-0000b0e0: 7320 6120 7369 6e67 6c65 2063 6f6c 756d  s a single colum
-0000b0f0: 6e20 6e61 6d65 2066 6f72 2060 696e 6465  n name for `inde
-0000b100: 785f 636f 6c60 2e20 220a 2020 2020 2020  x_col`. ".      
-0000b110: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b120: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
-0000b130: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
-0000b140: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000b150: 2020 2020 2020 2020 2020 2320 4e6f 6e65            # None
-0000b160: 2076 616c 7565 2066 6f72 2069 6e64 6578   value for index
-0000b170: 5f63 6f6c 2063 616e 6e6f 7420 6265 2070  _col cannot be p
-0000b180: 6173 7365 6420 746f 2072 6561 645f 6762  assed to read_gb
-0000b190: 710a 2020 2020 2020 2020 2020 2020 6966  q.            if
-0000b1a0: 2069 6e64 6578 5f63 6f6c 2069 7320 4e6f   index_col is No
-0000b1b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b1c0: 2020 2020 696e 6465 785f 636f 6c20 3d20      index_col = 
-0000b1d0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0000b1e0: 2320 7573 6563 6f6c 7320 7368 6f75 6c64  # usecols should
-0000b1f0: 206f 6e6c 7920 6265 2061 6e20 6974 6572   only be an iter
-0000b200: 6162 6c65 206f 6620 7374 7269 6e67 7320  able of strings 
-0000b210: 2863 6f6c 756d 6e20 6e61 6d65 7329 2066  (column names) f
-0000b220: 6f72 2075 7365 2061 7320 636f 6c75 6d6e  or use as column
-0000b230: 7320 696e 2072 6561 645f 6762 712e 0a20  s in read_gbq.. 
-0000b240: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000b250: 6e73 3a20 5475 706c 655b 416e 792c 202e  ns: Tuple[Any, .
-0000b260: 2e2e 5d20 3d20 7475 706c 6528 290a 2020  ..] = tuple().  
-0000b270: 2020 2020 2020 2020 2020 6966 2075 7365            if use
-0000b280: 636f 6c73 2069 7320 6e6f 7420 4e6f 6e65  cols is not None
-0000b290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b2a0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000b2b0: 7573 6563 6f6c 732c 2049 7465 7261 626c  usecols, Iterabl
-0000b2c0: 6529 2061 6e64 2061 6c6c 280a 2020 2020  e) and all(.    
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 6973 696e 7374 616e 6365 2863 6f6c 2c20  isinstance(col, 
-0000b2f0: 7374 7229 2066 6f72 2063 6f6c 2069 6e20  str) for col in 
-0000b300: 7573 6563 6f6c 730a 2020 2020 2020 2020  usecols.        
-0000b310: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000b320: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000b330: 6f6c 756d 6e73 203d 2074 7570 6c65 2863  olumns = tuple(c
-0000b340: 6f6c 2066 6f72 2063 6f6c 2069 6e20 7573  ol for col in us
-0000b350: 6563 6f6c 7329 0a20 2020 2020 2020 2020  ecols).         
-0000b360: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b380: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000b390: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 2020 2242 6967 5175 6572 7920 656e      "BigQuery en
-0000b3c0: 6769 6e65 206f 6e6c 7920 7375 7070 6f72  gine only suppor
-0000b3d0: 7473 2061 6e20 6974 6572 6162 6c65 206f  ts an iterable o
-0000b3e0: 6620 7374 7269 6e67 7320 666f 7220 6075  f strings for `u
-0000b3f0: 7365 636f 6c73 602e 2022 0a20 2020 2020  secols`. ".     
-0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b410: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
-0000b420: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000b450: 2020 2069 6620 656e 636f 6469 6e67 2069     if encoding i
-0000b460: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2065  s not None and e
-0000b470: 6e63 6f64 696e 6720 6e6f 7420 696e 205f  ncoding not in _
-0000b480: 5641 4c49 445f 454e 434f 4449 4e47 533a  VALID_ENCODINGS:
-0000b490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b4a0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000b4b0: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4d0: 6622 4269 6751 7565 7279 2065 6e67 696e  f"BigQuery engin
-0000b4e0: 6520 6f6e 6c79 2073 7570 706f 7274 7320  e only supports 
-0000b4f0: 7468 6520 666f 6c6c 6f77 696e 6720 656e  the following en
-0000b500: 636f 6469 6e67 733a 207b 5f56 414c 4944  codings: {_VALID
-0000b510: 5f45 4e43 4f44 494e 4753 7d2e 2022 0a20  _ENCODINGS}. ". 
-0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2066 227b 636f 6e73 7461 6e74 732e     f"{constants.
-0000b540: 4645 4544 4241 434b 5f4c 494e 4b7d 220a  FEEDBACK_LINK}".
-0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 290a 0a20 2020 2020 2020 2020 2020 206a  )..            j
-0000b570: 6f62 5f63 6f6e 6669 6720 3d20 7365 6c66  ob_config = self
-0000b580: 2e5f 7072 6570 6172 655f 6c6f 6164 5f6a  ._prepare_load_j
-0000b590: 6f62 5f63 6f6e 6669 6728 290a 2020 2020  ob_config().    
-0000b5a0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000b5b0: 6967 2e63 7265 6174 655f 6469 7370 6f73  ig.create_dispos
-0000b5c0: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
-0000b5d0: 2e43 7265 6174 6544 6973 706f 7369 7469  .CreateDispositi
-0000b5e0: 6f6e 2e43 5245 4154 455f 4946 5f4e 4545  on.CREATE_IF_NEE
-0000b5f0: 4445 440a 2020 2020 2020 2020 2020 2020  DED.            
-0000b600: 6a6f 625f 636f 6e66 6967 2e73 6f75 7263  job_config.sourc
-0000b610: 655f 666f 726d 6174 203d 2062 6967 7175  e_format = bigqu
-0000b620: 6572 792e 536f 7572 6365 466f 726d 6174  ery.SourceFormat
-0000b630: 2e43 5356 0a20 2020 2020 2020 2020 2020  .CSV.           
-0000b640: 206a 6f62 5f63 6f6e 6669 672e 7772 6974   job_config.writ
-0000b650: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
-0000b660: 6269 6771 7565 7279 2e57 7269 7465 4469  bigquery.WriteDi
-0000b670: 7370 6f73 6974 696f 6e2e 5752 4954 455f  sposition.WRITE_
-0000b680: 454d 5054 590a 2020 2020 2020 2020 2020  EMPTY.          
-0000b690: 2020 6a6f 625f 636f 6e66 6967 2e61 7574    job_config.aut
-0000b6a0: 6f64 6574 6563 7420 3d20 5472 7565 0a20  odetect = True. 
-0000b6b0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000b6c0: 6f6e 6669 672e 6669 656c 645f 6465 6c69  onfig.field_deli
-0000b6d0: 6d69 7465 7220 3d20 7365 700a 2020 2020  miter = sep.    
-0000b6e0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000b6f0: 6967 2e65 6e63 6f64 696e 6720 3d20 656e  ig.encoding = en
-0000b700: 636f 6469 6e67 0a20 2020 2020 2020 2020  coding.         
-0000b710: 2020 206a 6f62 5f63 6f6e 6669 672e 6c61     job_config.la
-0000b720: 6265 6c73 203d 207b 2262 6967 6672 616d  bels = {"bigfram
-0000b730: 6573 2d61 7069 223a 2022 7265 6164 5f63  es-api": "read_c
-0000b740: 7376 227d 0a0a 2020 2020 2020 2020 2020  sv"}..          
-0000b750: 2020 2320 5765 2077 616e 7420 746f 206d    # We want to m
-0000b760: 6174 6368 2070 616e 6461 7320 6265 6861  atch pandas beha
-0000b770: 7669 6f72 2e20 4966 2068 6561 6465 7220  vior. If header 
-0000b780: 6973 2030 2c20 6e6f 2072 6f77 7320 7368  is 0, no rows sh
-0000b790: 6f75 6c64 2062 6520 736b 6970 7065 642c  ould be skipped,
-0000b7a0: 2073 6f20 7765 0a20 2020 2020 2020 2020   so we.         
-0000b7b0: 2020 2023 2064 6f20 6e6f 7420 6e65 6564     # do not need
-0000b7c0: 2074 6f20 7365 7420 6073 6b69 705f 6c65   to set `skip_le
-0000b7d0: 6164 696e 675f 726f 7773 602e 2049 6620  ading_rows`. If 
-0000b7e0: 6865 6164 6572 2069 7320 4e6f 6e65 2c20  header is None, 
-0000b7f0: 7468 656e 2074 6865 7265 2069 7320 6e6f  then there is no
-0000b800: 2068 6561 6465 722e 0a20 2020 2020 2020   header..       
-0000b810: 2020 2020 2023 2053 6574 7469 6e67 2073       # Setting s
-0000b820: 6b69 705f 6c65 6164 696e 675f 726f 7773  kip_leading_rows
-0000b830: 2074 6f20 3020 646f 6573 2074 6861 742e   to 0 does that.
-0000b840: 2049 6620 6865 6164 6572 3d4e 2061 6e64   If header=N and
-0000b850: 204e 3e30 2c20 7765 2077 616e 7420 746f   N>0, we want to
-0000b860: 2073 6b69 7020 4e20 726f 7773 2e0a 2020   skip N rows..  
-0000b870: 2020 2020 2020 2020 2020 6966 2068 6561            if hea
-0000b880: 6465 7220 6973 204e 6f6e 653a 0a20 2020  der is None:.   
-0000b890: 2020 2020 2020 2020 2020 2020 206a 6f62               job
-0000b8a0: 5f63 6f6e 6669 672e 736b 6970 5f6c 6561  _config.skip_lea
-0000b8b0: 6469 6e67 5f72 6f77 7320 3d20 300a 2020  ding_rows = 0.  
-0000b8c0: 2020 2020 2020 2020 2020 656c 6966 2068            elif h
-0000b8d0: 6561 6465 7220 3e20 303a 0a20 2020 2020  eader > 0:.     
-0000b8e0: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
-0000b8f0: 6f6e 6669 672e 736b 6970 5f6c 6561 6469  onfig.skip_leadi
-0000b900: 6e67 5f72 6f77 7320 3d20 6865 6164 6572  ng_rows = header
-0000b910: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0000b920: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
-0000b930: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
-0000b940: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
-0000b950: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
-0000b960: 7566 6665 722c 0a20 2020 2020 2020 2020  uffer,.         
-0000b970: 2020 2020 2020 2074 6162 6c65 2c0a 2020         table,.  
-0000b980: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-0000b990: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
-0000b9a0: 6669 672c 0a20 2020 2020 2020 2020 2020  fig,.           
-0000b9b0: 2020 2020 2069 6e64 6578 5f63 6f6c 3d69       index_col=i
-0000b9c0: 6e64 6578 5f63 6f6c 2c0a 2020 2020 2020  ndex_col,.      
-0000b9d0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-0000b9e0: 733d 636f 6c75 6d6e 732c 0a20 2020 2020  s=columns,.     
-0000b9f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000ba00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000ba10: 2020 2069 6620 616e 7928 6172 6720 696e     if any(arg in
-0000ba20: 206b 7761 7267 7320 666f 7220 6172 6720   kwargs for arg 
-0000ba30: 696e 2028 2263 6875 6e6b 7369 7a65 222c  in ("chunksize",
-0000ba40: 2022 6974 6572 6174 6f72 2229 293a 0a20   "iterator")):. 
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000ba60: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000ba70: 7465 6445 7272 6f72 280a 2020 2020 2020  tedError(.      
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-0000ba90: 6368 756e 6b73 697a 6527 2061 6e64 2027  chunksize' and '
-0000baa0: 6974 6572 6174 6f72 2720 6172 6775 6d65  iterator' argume
-0000bab0: 6e74 7320 6172 6520 6e6f 7420 7375 7070  nts are not supp
-0000bac0: 6f72 7465 642e 2022 0a20 2020 2020 2020  orted. ".       
-0000bad0: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0000bae0: 636f 6e73 7461 6e74 732e 4645 4544 4241  constants.FEEDBA
-0000baf0: 434b 5f4c 494e 4b7d 220a 2020 2020 2020  CK_LINK}".      
-0000bb00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000bb10: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000bb20: 7374 616e 6365 2866 696c 6570 6174 685f  stance(filepath_
-0000bb30: 6f72 5f62 7566 6665 722c 2073 7472 293a  or_buffer, str):
-0000bb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb50: 2073 656c 662e 5f63 6865 636b 5f66 696c   self._check_fil
-0000bb60: 655f 7369 7a65 2866 696c 6570 6174 685f  e_size(filepath_
-0000bb70: 6f72 5f62 7566 6665 7229 0a20 2020 2020  or_buffer).     
-0000bb80: 2020 2020 2020 2070 616e 6461 735f 6466         pandas_df
-0000bb90: 203d 2070 616e 6461 732e 7265 6164 5f63   = pandas.read_c
-0000bba0: 7376 280a 2020 2020 2020 2020 2020 2020  sv(.            
-0000bbb0: 2020 2020 6669 6c65 7061 7468 5f6f 725f      filepath_or_
-0000bbc0: 6275 6666 6572 2c0a 2020 2020 2020 2020  buffer,.        
-0000bbd0: 2020 2020 2020 2020 7365 703d 7365 702c          sep=sep,
-0000bbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbf0: 2068 6561 6465 723d 6865 6164 6572 2c0a   header=header,.
-0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc10: 6e61 6d65 733d 6e61 6d65 732c 0a20 2020  names=names,.   
-0000bc20: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-0000bc30: 6578 5f63 6f6c 3d69 6e64 6578 5f63 6f6c  ex_col=index_col
-0000bc40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bc50: 2020 7573 6563 6f6c 733d 7573 6563 6f6c    usecols=usecol
-0000bc60: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000bc70: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-0000bc80: 2020 2064 7479 7065 3d64 7479 7065 2c0a     dtype=dtype,.
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 656e 6769 6e65 3d65 6e67 696e 652c 0a20  engine=engine,. 
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000bcc0: 6e63 6f64 696e 673d 656e 636f 6469 6e67  ncoding=encoding
-0000bcd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bce0: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-0000bcf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000bd00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000bd10: 662e 5f72 6561 645f 7061 6e64 6173 2870  f._read_pandas(p
-0000bd20: 616e 6461 735f 6466 2c20 2272 6561 645f  andas_df, "read_
-0000bd30: 6373 7622 2920 2023 2074 7970 653a 2069  csv")  # type: i
-0000bd40: 676e 6f72 650a 0a20 2020 2064 6566 2072  gnore..    def r
-0000bd50: 6561 645f 7069 636b 6c65 280a 2020 2020  ead_pickle(.    
-0000bd60: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000bd70: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
-0000bd80: 6666 6572 3a20 4669 6c65 5061 7468 207c  ffer: FilePath |
-0000bd90: 2052 6561 6450 6963 6b6c 6542 7566 6665   ReadPickleBuffe
-0000bda0: 722c 0a20 2020 2020 2020 2063 6f6d 7072  r,.        compr
-0000bdb0: 6573 7369 6f6e 3a20 436f 6d70 7265 7373  ession: Compress
-0000bdc0: 696f 6e4f 7074 696f 6e73 203d 2022 696e  ionOptions = "in
-0000bdd0: 6665 7222 2c0a 2020 2020 2020 2020 7374  fer",.        st
-0000bde0: 6f72 6167 655f 6f70 7469 6f6e 733a 2053  orage_options: S
-0000bdf0: 746f 7261 6765 4f70 7469 6f6e 7320 3d20  torageOptions = 
-0000be00: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000be10: 2020 2020 2070 616e 6461 735f 6f62 6a20       pandas_obj 
-0000be20: 3d20 7061 6e64 6173 2e72 6561 645f 7069  = pandas.read_pi
-0000be30: 636b 6c65 280a 2020 2020 2020 2020 2020  ckle(.          
-0000be40: 2020 6669 6c65 7061 7468 5f6f 725f 6275    filepath_or_bu
-0000be50: 6666 6572 2c0a 2020 2020 2020 2020 2020  ffer,.          
-0000be60: 2020 636f 6d70 7265 7373 696f 6e3d 636f    compression=co
-0000be70: 6d70 7265 7373 696f 6e2c 0a20 2020 2020  mpression,.     
-0000be80: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0000be90: 7074 696f 6e73 3d73 746f 7261 6765 5f6f  ptions=storage_o
-0000bea0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
-0000beb0: 290a 0a20 2020 2020 2020 2069 6620 6973  )..        if is
-0000bec0: 696e 7374 616e 6365 2870 616e 6461 735f  instance(pandas_
-0000bed0: 6f62 6a2c 2070 616e 6461 732e 5365 7269  obj, pandas.Seri
-0000bee0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-0000bef0: 2069 6620 7061 6e64 6173 5f6f 626a 2e6e   if pandas_obj.n
-0000bf00: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
-0000bf10: 2020 2020 2020 2020 2020 2020 2070 616e               pan
-0000bf20: 6461 735f 6f62 6a2e 6e61 6d65 203d 2022  das_obj.name = "
-0000bf30: 3022 0a20 2020 2020 2020 2020 2020 2062  0".            b
-0000bf40: 6967 6672 616d 6573 5f64 6620 3d20 7365  igframes_df = se
-0000bf50: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
-0000bf60: 7061 6e64 6173 5f6f 626a 2e74 6f5f 6672  pandas_obj.to_fr
-0000bf70: 616d 6528 292c 2022 7265 6164 5f70 6963  ame(), "read_pic
-0000bf80: 6b6c 6522 290a 2020 2020 2020 2020 2020  kle").          
-0000bf90: 2020 7265 7475 726e 2062 6967 6672 616d    return bigfram
-0000bfa0: 6573 5f64 665b 6269 6766 7261 6d65 735f  es_df[bigframes_
-0000bfb0: 6466 2e63 6f6c 756d 6e73 5b30 5d5d 0a20  df.columns[0]]. 
-0000bfc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000bfd0: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
-0000bfe0: 7061 6e64 6173 5f6f 626a 2c20 2272 6561  pandas_obj, "rea
-0000bff0: 645f 7069 636b 6c65 2229 0a0a 2020 2020  d_pickle")..    
-0000c000: 6465 6620 7265 6164 5f70 6172 7175 6574  def read_parquet
-0000c010: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000c020: 2020 2020 2020 2020 7061 7468 3a20 7374          path: st
-0000c030: 7220 7c20 494f 5b22 6279 7465 7322 5d2c  r | IO["bytes"],
-0000c040: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000c050: 2020 2020 656e 6769 6e65 3a20 7374 7220      engine: str 
-0000c060: 3d20 2261 7574 6f22 2c0a 2020 2020 2920  = "auto",.    ) 
-0000c070: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
-0000c080: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-0000c090: 7461 626c 6520 3d20 6269 6766 7261 6d65  table = bigframe
-0000c0a0: 735f 696f 2e72 616e 646f 6d5f 7461 626c  s_io.random_tabl
-0000c0b0: 6528 7365 6c66 2e5f 616e 6f6e 796d 6f75  e(self._anonymou
-0000c0c0: 735f 6461 7461 7365 7429 0a0a 2020 2020  s_dataset)..    
-0000c0d0: 2020 2020 6966 2065 6e67 696e 6520 3d3d      if engine ==
-0000c0e0: 2022 6269 6771 7565 7279 223a 0a20 2020   "bigquery":.   
-0000c0f0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000c100: 6669 6720 3d20 7365 6c66 2e5f 7072 6570  fig = self._prep
-0000c110: 6172 655f 6c6f 6164 5f6a 6f62 5f63 6f6e  are_load_job_con
-0000c120: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
-0000c130: 2020 6a6f 625f 636f 6e66 6967 2e63 7265    job_config.cre
-0000c140: 6174 655f 6469 7370 6f73 6974 696f 6e20  ate_disposition 
-0000c150: 3d20 6269 6771 7565 7279 2e43 7265 6174  = bigquery.Creat
-0000c160: 6544 6973 706f 7369 7469 6f6e 2e43 5245  eDisposition.CRE
-0000c170: 4154 455f 4946 5f4e 4545 4445 440a 2020  ATE_IF_NEEDED.  
-0000c180: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
-0000c190: 6e66 6967 2e73 6f75 7263 655f 666f 726d  nfig.source_form
-0000c1a0: 6174 203d 2062 6967 7175 6572 792e 536f  at = bigquery.So
-0000c1b0: 7572 6365 466f 726d 6174 2e50 4152 5155  urceFormat.PARQU
-0000c1c0: 4554 0a20 2020 2020 2020 2020 2020 206a  ET.            j
-0000c1d0: 6f62 5f63 6f6e 6669 672e 7772 6974 655f  ob_config.write_
-0000c1e0: 6469 7370 6f73 6974 696f 6e20 3d20 6269  disposition = bi
-0000c1f0: 6771 7565 7279 2e57 7269 7465 4469 7370  gquery.WriteDisp
-0000c200: 6f73 6974 696f 6e2e 5752 4954 455f 454d  osition.WRITE_EM
-0000c210: 5054 590a 2020 2020 2020 2020 2020 2020  PTY.            
-0000c220: 6a6f 625f 636f 6e66 6967 2e6c 6162 656c  job_config.label
-0000c230: 7320 3d20 7b22 6269 6766 7261 6d65 732d  s = {"bigframes-
-0000c240: 6170 6922 3a20 2272 6561 645f 7061 7271  api": "read_parq
-0000c250: 7565 7422 7d0a 0a20 2020 2020 2020 2020  uet"}..         
-0000c260: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000c270: 7265 6164 5f62 6967 7175 6572 795f 6c6f  read_bigquery_lo
-0000c280: 6164 5f6a 6f62 2870 6174 682c 2074 6162  ad_job(path, tab
-0000c290: 6c65 2c20 6a6f 625f 636f 6e66 6967 3d6a  le, job_config=j
-0000c2a0: 6f62 5f63 6f6e 6669 6729 0a20 2020 2020  ob_config).     
-0000c2b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c2c0: 2020 2020 2072 6561 645f 7061 7271 7565       read_parque
-0000c2d0: 745f 6b77 6172 6773 3a20 4469 6374 5b73  t_kwargs: Dict[s
-0000c2e0: 7472 2c20 416e 795d 203d 207b 7d0a 2020  tr, Any] = {}.  
-0000c2f0: 2020 2020 2020 2020 2020 6966 2070 616e            if pan
-0000c300: 6461 732e 5f5f 7665 7273 696f 6e5f 5f2e  das.__version__.
-0000c310: 7374 6172 7473 7769 7468 2822 312e 2229  startswith("1.")
-0000c320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c330: 2020 7265 6164 5f70 6172 7175 6574 5f6b    read_parquet_k
-0000c340: 7761 7267 735b 2275 7365 5f6e 756c 6c61  wargs["use_nulla
-0000c350: 626c 655f 6474 7970 6573 225d 203d 2054  ble_dtypes"] = T
-0000c360: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000c370: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c380: 2020 2020 2020 7265 6164 5f70 6172 7175        read_parqu
-0000c390: 6574 5f6b 7761 7267 735b 2264 7479 7065  et_kwargs["dtype
-0000c3a0: 5f62 6163 6b65 6e64 225d 203d 2022 7079  _backend"] = "py
-0000c3b0: 6172 726f 7722 0a0a 2020 2020 2020 2020  arrow"..        
-0000c3c0: 2020 2020 7061 6e64 6173 5f6f 626a 203d      pandas_obj =
-0000c3d0: 2070 616e 6461 732e 7265 6164 5f70 6172   pandas.read_par
-0000c3e0: 7175 6574 280a 2020 2020 2020 2020 2020  quet(.          
-0000c3f0: 2020 2020 2020 7061 7468 2c0a 2020 2020        path,.    
-0000c400: 2020 2020 2020 2020 2020 2020 656e 6769              engi
-0000c410: 6e65 3d65 6e67 696e 652c 2020 2320 7479  ne=engine,  # ty
-0000c420: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
-0000c430: 2020 2020 2020 2020 2020 202a 2a72 6561             **rea
-0000c440: 645f 7061 7271 7565 745f 6b77 6172 6773  d_parquet_kwargs
-0000c450: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000c460: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c470: 726e 2073 656c 662e 5f72 6561 645f 7061  rn self._read_pa
-0000c480: 6e64 6173 2870 616e 6461 735f 6f62 6a2c  ndas(pandas_obj,
-0000c490: 2022 7265 6164 5f70 6172 7175 6574 2229   "read_parquet")
-0000c4a0: 0a0a 2020 2020 6465 6620 7265 6164 5f6a  ..    def read_j
-0000c4b0: 736f 6e28 0a20 2020 2020 2020 2073 656c  son(.        sel
-0000c4c0: 662c 0a20 2020 2020 2020 2070 6174 685f  f,.        path_
-0000c4d0: 6f72 5f62 7566 3a20 7374 7220 7c20 494f  or_buf: str | IO
-0000c4e0: 5b22 6279 7465 7322 5d2c 0a20 2020 2020  ["bytes"],.     
-0000c4f0: 2020 202a 2c0a 2020 2020 2020 2020 6f72     *,.        or
-0000c500: 6965 6e74 3a20 4c69 7465 7261 6c5b 0a20  ient: Literal[. 
-0000c510: 2020 2020 2020 2020 2020 2022 7370 6c69             "spli
-0000c520: 7422 2c20 2272 6563 6f72 6473 222c 2022  t", "records", "
-0000c530: 696e 6465 7822 2c20 2263 6f6c 756d 6e73  index", "columns
-0000c540: 222c 2022 7661 6c75 6573 222c 2022 7461  ", "values", "ta
-0000c550: 626c 6522 0a20 2020 2020 2020 205d 203d  ble".        ] =
-0000c560: 2022 636f 6c75 6d6e 7322 2c0a 2020 2020   "columns",.    
-0000c570: 2020 2020 6474 7970 653a 204f 7074 696f      dtype: Optio
-0000c580: 6e61 6c5b 4469 6374 5d20 3d20 4e6f 6e65  nal[Dict] = None
-0000c590: 2c0a 2020 2020 2020 2020 656e 636f 6469  ,.        encodi
-0000c5a0: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
-0000c5b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000c5c0: 2020 6c69 6e65 733a 2062 6f6f 6c20 3d20    lines: bool = 
-0000c5d0: 4661 6c73 652c 0a20 2020 2020 2020 2065  False,.        e
-0000c5e0: 6e67 696e 653a 204c 6974 6572 616c 5b22  ngine: Literal["
-0000c5f0: 756a 736f 6e22 2c20 2270 7961 7272 6f77  ujson", "pyarrow
-0000c600: 222c 2022 6269 6771 7565 7279 225d 203d  ", "bigquery"] =
-0000c610: 2022 756a 736f 6e22 2c0a 2020 2020 2020   "ujson",.      
-0000c620: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
-0000c630: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
-0000c640: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
-0000c650: 2020 7461 626c 6520 3d20 6269 6766 7261    table = bigfra
-0000c660: 6d65 735f 696f 2e72 616e 646f 6d5f 7461  mes_io.random_ta
-0000c670: 626c 6528 7365 6c66 2e5f 616e 6f6e 796d  ble(self._anonym
-0000c680: 6f75 735f 6461 7461 7365 7429 0a0a 2020  ous_dataset)..  
-0000c690: 2020 2020 2020 6966 2065 6e67 696e 6520        if engine 
-0000c6a0: 3d3d 2022 6269 6771 7565 7279 223a 0a0a  == "bigquery":..
-0000c6b0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-0000c6c0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-0000c6d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c6e0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000c6f0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c710: 2022 4269 6751 7565 7279 2065 6e67 696e   "BigQuery engin
-0000c720: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
-0000c730: 7274 2074 6865 2064 7479 7065 2061 7267  rt the dtype arg
-0000c740: 756d 656e 7473 2e22 0a20 2020 2020 2020  uments.".       
-0000c750: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000c760: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
-0000c770: 696e 6573 3a0a 2020 2020 2020 2020 2020  ines:.          
-0000c780: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-0000c790: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-0000c7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c7b0: 2020 2020 2022 4f6e 6c79 206e 6577 6c69       "Only newli
-0000c7c0: 6e65 2064 656c 696d 6974 6564 204a 534f  ne delimited JSO
-0000c7d0: 4e20 666f 726d 6174 2069 7320 7375 7070  N format is supp
-0000c7e0: 6f72 7465 642e 220a 2020 2020 2020 2020  orted.".        
-0000c7f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000c800: 2020 2020 2020 2069 6620 656e 636f 6469         if encodi
-0000c810: 6e67 2069 7320 6e6f 7420 4e6f 6e65 2061  ng is not None a
-0000c820: 6e64 2065 6e63 6f64 696e 6720 6e6f 7420  nd encoding not 
-0000c830: 696e 205f 5641 4c49 445f 454e 434f 4449  in _VALID_ENCODI
-0000c840: 4e47 533a 0a20 2020 2020 2020 2020 2020  NGS:.           
-0000c850: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-0000c860: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c880: 2020 2020 6622 4269 6751 7565 7279 2065      f"BigQuery e
-0000c890: 6e67 696e 6520 6f6e 6c79 2073 7570 706f  ngine only suppo
-0000c8a0: 7274 7320 7468 6520 666f 6c6c 6f77 696e  rts the followin
-0000c8b0: 6720 656e 636f 6469 6e67 733a 207b 5f56  g encodings: {_V
-0000c8c0: 414c 4944 5f45 4e43 4f44 494e 4753 7d22  ALID_ENCODINGS}"
-0000c8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8e0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000c8f0: 6966 206c 696e 6573 2061 6e64 206f 7269  if lines and ori
-0000c900: 656e 7420 213d 2022 7265 636f 7264 7322  ent != "records"
-0000c910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c920: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000c930: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000c940: 2020 2020 2020 2020 2227 6c69 6e65 7327          "'lines'
-0000c950: 206b 6579 776f 7264 2069 7320 6f6e 6c79   keyword is only
-0000c960: 2076 616c 6964 2077 6865 6e20 276f 7269   valid when 'ori
-0000c970: 656e 7427 2069 7320 2772 6563 6f72 6473  ent' is 'records
-0000c980: 272e 220a 2020 2020 2020 2020 2020 2020  '.".            
-0000c990: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000c9a0: 2020 206a 6f62 5f63 6f6e 6669 6720 3d20     job_config = 
-0000c9b0: 7365 6c66 2e5f 7072 6570 6172 655f 6c6f  self._prepare_lo
-0000c9c0: 6164 5f6a 6f62 5f63 6f6e 6669 6728 290a  ad_job_config().
-0000c9d0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-0000c9e0: 636f 6e66 6967 2e63 7265 6174 655f 6469  config.create_di
-0000c9f0: 7370 6f73 6974 696f 6e20 3d20 6269 6771  sposition = bigq
-0000ca00: 7565 7279 2e43 7265 6174 6544 6973 706f  uery.CreateDispo
-0000ca10: 7369 7469 6f6e 2e43 5245 4154 455f 4946  sition.CREATE_IF
-0000ca20: 5f4e 4545 4445 440a 2020 2020 2020 2020  _NEEDED.        
-0000ca30: 2020 2020 6a6f 625f 636f 6e66 6967 2e73      job_config.s
-0000ca40: 6f75 7263 655f 666f 726d 6174 203d 2062  ource_format = b
-0000ca50: 6967 7175 6572 792e 536f 7572 6365 466f  igquery.SourceFo
-0000ca60: 726d 6174 2e4e 4557 4c49 4e45 5f44 454c  rmat.NEWLINE_DEL
-0000ca70: 494d 4954 4544 5f4a 534f 4e0a 2020 2020  IMITED_JSON.    
-0000ca80: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
-0000ca90: 6967 2e77 7269 7465 5f64 6973 706f 7369  ig.write_disposi
-0000caa0: 7469 6f6e 203d 2062 6967 7175 6572 792e  tion = bigquery.
-0000cab0: 5772 6974 6544 6973 706f 7369 7469 6f6e  WriteDisposition
-0000cac0: 2e57 5249 5445 5f45 4d50 5459 0a20 2020  .WRITE_EMPTY.   
-0000cad0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-0000cae0: 6669 672e 6175 746f 6465 7465 6374 203d  fig.autodetect =
-0000caf0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000cb00: 2020 6a6f 625f 636f 6e66 6967 2e65 6e63    job_config.enc
-0000cb10: 6f64 696e 6720 3d20 656e 636f 6469 6e67  oding = encoding
-0000cb20: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
-0000cb30: 5f63 6f6e 6669 672e 6c61 6265 6c73 203d  _config.labels =
-0000cb40: 207b 2262 6967 6672 616d 6573 2d61 7069   {"bigframes-api
-0000cb50: 223a 2022 7265 6164 5f6a 736f 6e22 7d0a  ": "read_json"}.
-0000cb60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cb70: 7572 6e20 7365 6c66 2e5f 7265 6164 5f62  urn self._read_b
-0000cb80: 6967 7175 6572 795f 6c6f 6164 5f6a 6f62  igquery_load_job
-0000cb90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000cba0: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000cbc0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
-0000cbd0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-0000cbe0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
-0000cbf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000cc00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000cc10: 2020 2020 2069 6620 616e 7928 6172 6720       if any(arg 
-0000cc20: 696e 206b 7761 7267 7320 666f 7220 6172  in kwargs for ar
-0000cc30: 6720 696e 2028 2263 6875 6e6b 7369 7a65  g in ("chunksize
-0000cc40: 222c 2022 6974 6572 6174 6f72 2229 293a  ", "iterator")):
-0000cc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc60: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000cc70: 656e 7465 6445 7272 6f72 280a 2020 2020  entedError(.    
-0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2227 6368 756e 6b73 697a 6527 2061 6e64  "'chunksize' and
-0000cca0: 2027 6974 6572 6174 6f72 2720 6172 6775   'iterator' argu
-0000ccb0: 6d65 6e74 7320 6172 6520 6e6f 7420 7375  ments are not su
-0000ccc0: 7070 6f72 7465 642e 220a 2020 2020 2020  pported.".      
-0000ccd0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000cce0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000ccf0: 7374 616e 6365 2870 6174 685f 6f72 5f62  stance(path_or_b
-0000cd00: 7566 2c20 7374 7229 3a0a 2020 2020 2020  uf, str):.      
-0000cd10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000cd20: 6368 6563 6b5f 6669 6c65 5f73 697a 6528  check_file_size(
-0000cd30: 7061 7468 5f6f 725f 6275 6629 0a0a 2020  path_or_buf)..  
-0000cd40: 2020 2020 2020 2020 2020 6966 2065 6e67            if eng
-0000cd50: 696e 6520 3d3d 2022 756a 736f 6e22 3a0a  ine == "ujson":.
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 7061 6e64 6173 5f64 6620 3d20 7061 6e64  pandas_df = pand
-0000cd80: 6173 2e72 6561 645f 6a73 6f6e 2820 2023  as.read_json(  #
-0000cd90: 2074 7970 653a 2069 676e 6f72 650a 2020   type: ignore.  
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2020 7061 7468 5f6f 725f 6275 662c 0a20    path_or_buf,. 
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 206f 7269 656e 743d 6f72 6965 6e74     orient=orient
-0000cde0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cdf0: 2020 2020 2020 6474 7970 653d 6474 7970        dtype=dtyp
-0000ce00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000ce10: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
-0000ce20: 656e 636f 6469 6e67 2c0a 2020 2020 2020  encoding,.      
-0000ce30: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000ce40: 6e65 733d 6c69 6e65 732c 0a20 2020 2020  nes=lines,.     
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000ce60: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
-0000ce70: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000ce80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0000cea0: 6e64 6173 5f64 6620 3d20 7061 6e64 6173  ndas_df = pandas
-0000ceb0: 2e72 6561 645f 6a73 6f6e 2820 2023 2074  .read_json(  # t
-0000cec0: 7970 653a 2069 676e 6f72 650a 2020 2020  ype: ignore.    
-0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cee0: 7061 7468 5f6f 725f 6275 662c 0a20 2020  path_or_buf,.   
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 206f 7269 656e 743d 6f72 6965 6e74 2c0a   orient=orient,.
-0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf20: 2020 2020 6474 7970 653d 6474 7970 652c      dtype=dtype,
-0000cf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf40: 2020 2020 2065 6e63 6f64 696e 673d 656e       encoding=en
-0000cf50: 636f 6469 6e67 2c0a 2020 2020 2020 2020  coding,.        
-0000cf60: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000cf70: 733d 6c69 6e65 732c 0a20 2020 2020 2020  s=lines,.       
-0000cf80: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
-0000cf90: 696e 653d 656e 6769 6e65 2c0a 2020 2020  ine=engine,.    
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
-0000cfc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000cfd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000cfe0: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
-0000cff0: 2870 616e 6461 735f 6466 2c20 2272 6561  (pandas_df, "rea
-0000d000: 645f 6a73 6f6e 2229 0a0a 2020 2020 6465  d_json")..    de
-0000d010: 6620 5f63 6865 636b 5f66 696c 655f 7369  f _check_file_si
-0000d020: 7a65 2873 656c 662c 2066 696c 6570 6174  ze(self, filepat
-0000d030: 683a 2073 7472 293a 0a20 2020 2020 2020  h: str):.       
-0000d040: 206d 6178 5f73 697a 6520 3d20 3130 3234   max_size = 1024
-0000d050: 202a 2031 3032 3420 2a20 3130 3234 2020   * 1024 * 1024  
-0000d060: 2320 3120 4742 2069 6e20 6279 7465 730a  # 1 GB in bytes.
-0000d070: 2020 2020 2020 2020 6966 2066 696c 6570          if filep
-0000d080: 6174 682e 7374 6172 7473 7769 7468 2822  ath.startswith("
-0000d090: 6773 3a2f 2f22 293a 2020 2320 4743 5320  gs://"):  # GCS 
-0000d0a0: 6669 6c65 2070 6174 680a 2020 2020 2020  file path.      
-0000d0b0: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
-0000d0c0: 746f 7261 6765 2e43 6c69 656e 7428 290a  torage.Client().
-0000d0d0: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-0000d0e0: 6574 5f6e 616d 652c 2062 6c6f 625f 6e61  et_name, blob_na
-0000d0f0: 6d65 203d 2066 696c 6570 6174 682e 7370  me = filepath.sp
-0000d100: 6c69 7428 222f 222c 2033 295b 323a 5d0a  lit("/", 3)[2:].
-0000d110: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-0000d120: 6574 203d 2063 6c69 656e 742e 6275 636b  et = client.buck
-0000d130: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-0000d140: 2020 2020 2020 2020 2020 2020 626c 6f62              blob
-0000d150: 203d 2062 7563 6b65 742e 626c 6f62 2862   = bucket.blob(b
-0000d160: 6c6f 625f 6e61 6d65 290a 2020 2020 2020  lob_name).      
-0000d170: 2020 2020 2020 626c 6f62 2e72 656c 6f61        blob.reloa
-0000d180: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-0000d190: 6669 6c65 5f73 697a 6520 3d20 626c 6f62  file_size = blob
-0000d1a0: 2e73 697a 650a 2020 2020 2020 2020 656c  .size.        el
-0000d1b0: 7365 3a20 2023 206c 6f63 616c 2066 696c  se:  # local fil
-0000d1c0: 6520 7061 7468 0a20 2020 2020 2020 2020  e path.         
-0000d1d0: 2020 2066 696c 655f 7369 7a65 203d 206f     file_size = o
-0000d1e0: 732e 7061 7468 2e67 6574 7369 7a65 2866  s.path.getsize(f
-0000d1f0: 696c 6570 6174 6829 0a0a 2020 2020 2020  ilepath)..      
-0000d200: 2020 6966 2066 696c 655f 7369 7a65 203e    if file_size >
-0000d210: 206d 6178 5f73 697a 653a 0a20 2020 2020   max_size:.     
-0000d220: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-0000d230: 2074 6f20 4742 0a20 2020 2020 2020 2020   to GB.         
-0000d240: 2020 2066 696c 655f 7369 7a65 203d 2072     file_size = r
-0000d250: 6f75 6e64 2866 696c 655f 7369 7a65 202f  ound(file_size /
-0000d260: 2028 3130 3234 2a2a 3329 2c20 3129 0a20   (1024**3), 1). 
-0000d270: 2020 2020 2020 2020 2020 206d 6178 5f73             max_s
-0000d280: 697a 6520 3d20 696e 7428 6d61 785f 7369  ize = int(max_si
-0000d290: 7a65 202f 2031 3032 342a 2a33 290a 2020  ze / 1024**3).  
-0000d2a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d2b0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
-0000d2c0: 2020 2020 2020 2020 2020 6622 4669 6c65            f"File
-0000d2d0: 2073 697a 6520 7b66 696c 655f 7369 7a65   size {file_size
-0000d2e0: 7d47 4220 6578 6365 6564 7320 7b6d 6178  }GB exceeds {max
-0000d2f0: 5f73 697a 657d 4742 2e20 220a 2020 2020  _size}GB. ".    
-0000d300: 2020 2020 2020 2020 2020 2020 2249 7420              "It 
-0000d310: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
-0000d320: 6f20 7573 6520 656e 6769 6e65 3d27 6269  o use engine='bi
-0000d330: 6771 7565 7279 2720 220a 2020 2020 2020  gquery' ".      
-0000d340: 2020 2020 2020 2020 2020 2266 6f72 206c            "for l
-0000d350: 6172 6765 2066 696c 6573 2074 6f20 6176  arge files to av
-0000d360: 6f69 6420 6c6f 6164 696e 6720 7468 6520  oid loading the 
-0000d370: 6669 6c65 2069 6e74 6f20 6c6f 6361 6c20  file into local 
-0000d380: 6d65 6d6f 7279 2e22 0a20 2020 2020 2020  memory.".       
-0000d390: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000d3a0: 5f63 7265 6174 655f 656d 7074 795f 7465  _create_empty_te
-0000d3b0: 6d70 5f74 6162 6c65 280a 2020 2020 2020  mp_table(.      
-0000d3c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000d3d0: 7363 6865 6d61 3a20 4974 6572 6162 6c65  schema: Iterable
-0000d3e0: 5b62 6967 7175 6572 792e 5363 6865 6d61  [bigquery.Schema
-0000d3f0: 4669 656c 645d 2c0a 2020 2020 2020 2020  Field],.        
-0000d400: 636c 7573 7465 725f 636f 6c73 3a20 4c69  cluster_cols: Li
-0000d410: 7374 5b73 7472 5d2c 0a20 2020 2029 202d  st[str],.    ) -
-0000d420: 3e20 6269 6771 7565 7279 2e54 6162 6c65  > bigquery.Table
-0000d430: 5265 6665 7265 6e63 653a 0a20 2020 2020  Reference:.     
-0000d440: 2020 2023 2043 616e 2774 2073 6574 2061     # Can't set a
-0000d450: 2074 6162 6c65 2069 6e20 5f53 4553 5349   table in _SESSI
-0000d460: 4f4e 2061 7320 6465 7374 696e 6174 696f  ON as destinatio
-0000d470: 6e20 7669 6120 7175 6572 7920 6a6f 6220  n via query job 
-0000d480: 4150 492c 2073 6f20 7765 0a20 2020 2020  API, so we.     
-0000d490: 2020 2023 2072 756e 2044 444c 2c20 696e     # run DDL, in
-0000d4a0: 7374 6561 642e 0a20 2020 2020 2020 2064  stead..        d
-0000d4b0: 6174 6173 6574 203d 2073 656c 662e 5f61  ataset = self._a
-0000d4c0: 6e6f 6e79 6d6f 7573 5f64 6174 6173 6574  nonymous_dataset
-0000d4d0: 0a20 2020 2020 2020 2065 7870 6972 6174  .        expirat
-0000d4e0: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
-0000d4f0: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
-0000d500: 6574 696d 652e 6e6f 7728 6461 7465 7469  etime.now(dateti
-0000d510: 6d65 2e74 696d 657a 6f6e 652e 7574 6329  me.timezone.utc)
-0000d520: 202b 2063 6f6e 7374 616e 7473 2e44 4546   + constants.DEF
-0000d530: 4155 4c54 5f45 5850 4952 4154 494f 4e0a  AULT_EXPIRATION.
-0000d540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d550: 2020 2074 6162 6c65 203d 2062 6967 6672     table = bigfr
-0000d560: 616d 6573 5f69 6f2e 6372 6561 7465 5f74  ames_io.create_t
-0000d570: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
-0000d580: 2020 2020 2020 2073 656c 662e 6271 636c         self.bqcl
-0000d590: 6965 6e74 2c0a 2020 2020 2020 2020 2020  ient,.          
-0000d5a0: 2020 6461 7461 7365 742c 0a20 2020 2020    dataset,.     
-0000d5b0: 2020 2020 2020 2065 7870 6972 6174 696f         expiratio
-0000d5c0: 6e2c 0a20 2020 2020 2020 2020 2020 2073  n,.            s
-0000d5d0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-0000d5e0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-0000d5f0: 725f 636f 6c75 6d6e 733d 636c 7573 7465  r_columns=cluste
-0000d600: 725f 636f 6c73 2c0a 2020 2020 2020 2020  r_cols,.        
-0000d610: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d620: 2062 6967 7175 6572 792e 5461 626c 6552   bigquery.TableR
-0000d630: 6566 6572 656e 6365 2e66 726f 6d5f 7374  eference.from_st
-0000d640: 7269 6e67 2874 6162 6c65 290a 0a20 2020  ring(table)..   
-0000d650: 2064 6566 205f 6372 6561 7465 5f74 6f74   def _create_tot
-0000d660: 616c 5f6f 7264 6572 696e 6728 0a20 2020  al_ordering(.   
-0000d670: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000d680: 2020 2074 6162 6c65 3a20 6962 6973 5f74     table: ibis_t
-0000d690: 7970 6573 2e54 6162 6c65 2c0a 2020 2020  ypes.Table,.    
-0000d6a0: 2020 2020 7461 626c 655f 726f 7773 3a20      table_rows: 
-0000d6b0: 4f70 7469 6f6e 616c 5b69 6e74 5d2c 0a20  Optional[int],. 
-0000d6c0: 2020 2029 202d 3e20 636f 7265 2e41 7272     ) -> core.Arr
-0000d6d0: 6179 5661 6c75 653a 0a20 2020 2020 2020  ayValue:.       
-0000d6e0: 2023 2053 696e 6365 2074 6869 7320 6d69   # Since this mi
-0000d6f0: 6768 7420 616c 736f 2062 6520 7573 6564  ght also be used
-0000d700: 2061 7320 7468 6520 696e 6465 782c 2064   as the index, d
-0000d710: 6f6e 2774 2075 7365 2074 6865 2064 6566  on't use the def
-0000d720: 6175 6c74 0a20 2020 2020 2020 2023 2022  ault.        # "
-0000d730: 6f72 6465 7269 6e67 2049 4422 206e 616d  ordering ID" nam
-0000d740: 652e 0a0a 2020 2020 2020 2020 2320 466f  e...        # Fo
-0000d750: 7220 736d 616c 6c20 7461 626c 6573 2c20  r small tables, 
-0000d760: 3634 2062 6974 7320 6973 2065 6e6f 7567  64 bits is enoug
-0000d770: 6820 746f 2061 766f 6964 2063 6f6c 6c69  h to avoid colli
-0000d780: 7369 6f6e 732c 2031 3238 2062 6974 7320  sions, 128 bits 
-0000d790: 7769 6c6c 206e 6576 6572 2065 7665 7220  will never ever 
-0000d7a0: 636f 6c6c 6964 6520 6e6f 206d 6174 7465  collide no matte
-0000d7b0: 7220 7768 6174 0a20 2020 2020 2020 2023  r what.        #
-0000d7c0: 2041 7373 756d 6520 7461 626c 6520 6973   Assume table is
-0000d7d0: 206c 6172 6765 2069 6620 7461 626c 6520   large if table 
-0000d7e0: 726f 7720 636f 756e 7420 6973 2075 6e6b  row count is unk
-0000d7f0: 6e6f 776e 0a20 2020 2020 2020 2075 7365  nown.        use
-0000d800: 5f64 6f75 626c 655f 6861 7368 203d 2028  _double_hash = (
-0000d810: 0a20 2020 2020 2020 2020 2020 2028 7461  .            (ta
-0000d820: 626c 655f 726f 7773 2069 7320 4e6f 6e65  ble_rows is None
-0000d830: 2920 6f72 2028 7461 626c 655f 726f 7773  ) or (table_rows
-0000d840: 203d 3d20 3029 206f 7220 2874 6162 6c65   == 0) or (table
-0000d850: 5f72 6f77 7320 3e20 3130 3030 3030 290a  _rows > 100000).
-0000d860: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000d870: 2020 206f 7264 6572 696e 675f 6861 7368     ordering_hash
-0000d880: 5f70 6172 7420 3d20 6775 6964 2e67 656e  _part = guid.gen
-0000d890: 6572 6174 655f 6775 6964 2822 6269 6766  erate_guid("bigf
-0000d8a0: 7261 6d65 735f 6f72 6465 7269 6e67 5f22  rames_ordering_"
-0000d8b0: 290a 2020 2020 2020 2020 6f72 6465 7269  ).        orderi
-0000d8c0: 6e67 5f68 6173 685f 7061 7274 3220 3d20  ng_hash_part2 = 
-0000d8d0: 6775 6964 2e67 656e 6572 6174 655f 6775  guid.generate_gu
-0000d8e0: 6964 2822 6269 6766 7261 6d65 735f 6f72  id("bigframes_or
-0000d8f0: 6465 7269 6e67 5f22 290a 2020 2020 2020  dering_").      
-0000d900: 2020 6f72 6465 7269 6e67 5f72 616e 645f    ordering_rand_
-0000d910: 7061 7274 203d 2067 7569 642e 6765 6e65  part = guid.gene
-0000d920: 7261 7465 5f67 7569 6428 2262 6967 6672  rate_guid("bigfr
-0000d930: 616d 6573 5f6f 7264 6572 696e 675f 2229  ames_ordering_")
-0000d940: 0a0a 2020 2020 2020 2020 2320 416c 6c20  ..        # All 
-0000d950: 696e 7075 7473 2069 6e74 6f20 6861 7368  inputs into hash
-0000d960: 206d 7573 7420 6265 206e 6f6e 2d6e 756c   must be non-nul
-0000d970: 6c20 6f72 2072 6573 756c 7469 6e67 2068  l or resulting h
-0000d980: 6173 6820 7769 6c6c 2062 6520 6e75 6c6c  ash will be null
-0000d990: 0a20 2020 2020 2020 2073 7472 5f76 616c  .        str_val
-0000d9a0: 7565 7320 3d20 6c69 7374 280a 2020 2020  ues = list(.    
-0000d9b0: 2020 2020 2020 2020 6d61 7028 6c61 6d62          map(lamb
-0000d9c0: 6461 2063 6f6c 3a20 5f63 6f6e 7665 7274  da col: _convert
-0000d9d0: 5f74 6f5f 6e6f 6e6e 756c 6c5f 7374 7269  _to_nonnull_stri
-0000d9e0: 6e67 2874 6162 6c65 5b63 6f6c 5d29 2c20  ng(table[col]), 
-0000d9f0: 7461 626c 652e 636f 6c75 6d6e 7329 0a20  table.columns). 
-0000da00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000da10: 2066 756c 6c5f 726f 775f 7374 7220 3d20   full_row_str = 
-0000da20: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-0000da30: 725f 7661 6c75 6573 5b30 5d2e 636f 6e63  r_values[0].conc
-0000da40: 6174 282a 7374 725f 7661 6c75 6573 5b31  at(*str_values[1
-0000da50: 3a5d 290a 2020 2020 2020 2020 2020 2020  :]).            
-0000da60: 6966 206c 656e 2873 7472 5f76 616c 7565  if len(str_value
-0000da70: 7329 203e 2031 0a20 2020 2020 2020 2020  s) > 1.         
-0000da80: 2020 2065 6c73 6520 7374 725f 7661 6c75     else str_valu
-0000da90: 6573 5b30 5d0a 2020 2020 2020 2020 290a  es[0].        ).
-0000daa0: 2020 2020 2020 2020 6675 6c6c 5f72 6f77          full_row
-0000dab0: 5f68 6173 6820 3d20 6675 6c6c 5f72 6f77  _hash = full_row
-0000dac0: 5f73 7472 2e68 6173 6828 292e 6e61 6d65  _str.hash().name
-0000dad0: 286f 7264 6572 696e 675f 6861 7368 5f70  (ordering_hash_p
-0000dae0: 6172 7429 0a20 2020 2020 2020 2023 2042  art).        # B
-0000daf0: 7920 6d6f 6469 6679 696e 6720 7661 6c75  y modifying valu
-0000db00: 6520 736c 6967 6874 6c79 2c20 7765 2067  e slightly, we g
-0000db10: 6574 2061 6e6f 7468 6572 2068 6173 6820  et another hash 
-0000db20: 756e 636f 7272 656c 6174 6564 2077 6974  uncorrelated wit
-0000db30: 6820 7468 6520 6669 7273 740a 2020 2020  h the first.    
-0000db40: 2020 2020 6675 6c6c 5f72 6f77 5f68 6173      full_row_has
-0000db50: 685f 7032 203d 2028 6675 6c6c 5f72 6f77  h_p2 = (full_row
-0000db60: 5f73 7472 202b 2022 5f22 292e 6861 7368  _str + "_").hash
-0000db70: 2829 2e6e 616d 6528 6f72 6465 7269 6e67  ().name(ordering
-0000db80: 5f68 6173 685f 7061 7274 3229 0a20 2020  _hash_part2).   
-0000db90: 2020 2020 2023 2055 7365 6420 746f 2064       # Used to d
-0000dba0: 6973 616d 6269 6775 6174 6520 6265 7477  isambiguate betw
-0000dbb0: 6565 6e20 6964 656e 7469 6361 6c20 726f  een identical ro
-0000dbc0: 7773 2028 7768 6963 6820 7769 6c6c 2068  ws (which will h
-0000dbd0: 6176 6520 6964 656e 7469 6361 6c20 6861  ave identical ha
-0000dbe0: 7368 290a 2020 2020 2020 2020 7261 6e64  sh).        rand
-0000dbf0: 6f6d 5f76 616c 7565 203d 2069 6269 732e  om_value = ibis.
-0000dc00: 7261 6e64 6f6d 2829 2e6e 616d 6528 6f72  random().name(or
-0000dc10: 6465 7269 6e67 5f72 616e 645f 7061 7274  dering_rand_part
-0000dc20: 290a 0a20 2020 2020 2020 206f 7264 6572  )..        order
-0000dc30: 5f76 616c 7565 7320 3d20 280a 2020 2020  _values = (.    
-0000dc40: 2020 2020 2020 2020 5b66 756c 6c5f 726f          [full_ro
-0000dc50: 775f 6861 7368 2c20 6675 6c6c 5f72 6f77  w_hash, full_row
-0000dc60: 5f68 6173 685f 7032 2c20 7261 6e64 6f6d  _hash_p2, random
-0000dc70: 5f76 616c 7565 5d0a 2020 2020 2020 2020  _value].        
-0000dc80: 2020 2020 6966 2075 7365 5f64 6f75 626c      if use_doubl
-0000dc90: 655f 6861 7368 0a20 2020 2020 2020 2020  e_hash.         
-0000dca0: 2020 2065 6c73 6520 5b66 756c 6c5f 726f     else [full_ro
-0000dcb0: 775f 6861 7368 2c20 7261 6e64 6f6d 5f76  w_hash, random_v
-0000dcc0: 616c 7565 5d0a 2020 2020 2020 2020 290a  alue].        ).
-0000dcd0: 0a20 2020 2020 2020 206f 7269 6769 6e61  .        origina
-0000dce0: 6c5f 636f 6c75 6d6e 5f69 6473 203d 2074  l_column_ids = t
-0000dcf0: 6162 6c65 2e63 6f6c 756d 6e73 0a20 2020  able.columns.   
-0000dd00: 2020 2020 2074 6162 6c65 5f77 6974 685f       table_with_
-0000dd10: 6f72 6465 7269 6e67 203d 2074 6162 6c65  ordering = table
-0000dd20: 2e73 656c 6563 7428 0a20 2020 2020 2020  .select(.       
-0000dd30: 2020 2020 2069 7465 7274 6f6f 6c73 2e63       itertools.c
-0000dd40: 6861 696e 286f 7269 6769 6e61 6c5f 636f  hain(original_co
-0000dd50: 6c75 6d6e 5f69 6473 2c20 6f72 6465 725f  lumn_ids, order_
-0000dd60: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
-0000dd70: 290a 0a20 2020 2020 2020 206f 7264 6572  )..        order
-0000dd80: 696e 6720 3d20 6f72 6465 722e 4578 7072  ing = order.Expr
-0000dd90: 6573 7369 6f6e 4f72 6465 7269 6e67 280a  essionOrdering(.
-0000dda0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0000ddb0: 7269 6e67 5f76 616c 7565 5f63 6f6c 756d  ring_value_colum
-0000ddc0: 6e73 3d74 7570 6c65 280a 2020 2020 2020  ns=tuple(.      
-0000ddd0: 2020 2020 2020 2020 2020 6f72 6465 722e            order.
-0000dde0: 6173 6365 6e64 696e 675f 6f76 6572 2863  ascending_over(c
-0000ddf0: 6f6c 2e67 6574 5f6e 616d 6528 2929 2066  ol.get_name()) f
-0000de00: 6f72 2063 6f6c 2069 6e20 6f72 6465 725f  or col in order_
-0000de10: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
-0000de20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-0000de30: 2020 746f 7461 6c5f 6f72 6465 7269 6e67    total_ordering
-0000de40: 5f63 6f6c 756d 6e73 3d66 726f 7a65 6e73  _columns=frozens
-0000de50: 6574 2863 6f6c 2e67 6574 5f6e 616d 6528  et(col.get_name(
-0000de60: 2920 666f 7220 636f 6c20 696e 206f 7264  ) for col in ord
-0000de70: 6572 5f76 616c 7565 7329 2c0a 2020 2020  er_values),.    
-0000de80: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-0000de90: 6c75 6d6e 7320 3d20 5b74 6162 6c65 5f77  lumns = [table_w
-0000dea0: 6974 685f 6f72 6465 7269 6e67 5b63 6f6c  ith_ordering[col
-0000deb0: 5d20 666f 7220 636f 6c20 696e 206f 7269  ] for col in ori
-0000dec0: 6769 6e61 6c5f 636f 6c75 6d6e 5f69 6473  ginal_column_ids
-0000ded0: 5d0a 2020 2020 2020 2020 6869 6464 656e  ].        hidden
-0000dee0: 5f63 6f6c 756d 6e73 203d 205b 7461 626c  _columns = [tabl
-0000def0: 655f 7769 7468 5f6f 7264 6572 696e 675b  e_with_ordering[
-0000df00: 636f 6c2e 6765 745f 6e61 6d65 2829 5d20  col.get_name()] 
-0000df10: 666f 7220 636f 6c20 696e 206f 7264 6572  for col in order
-0000df20: 5f76 616c 7565 735d 0a20 2020 2020 2020  _values].       
-0000df30: 2072 6574 7572 6e20 636f 7265 2e41 7272   return core.Arr
-0000df40: 6179 5661 6c75 652e 6672 6f6d 5f69 6269  ayValue.from_ibi
-0000df50: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
-0000df60: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000df70: 2074 6162 6c65 5f77 6974 685f 6f72 6465   table_with_orde
-0000df80: 7269 6e67 2c0a 2020 2020 2020 2020 2020  ring,.          
-0000df90: 2020 636f 6c75 6d6e 732c 0a20 2020 2020    columns,.     
-0000dfa0: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
-0000dfb0: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d68  dering_columns=h
-0000dfc0: 6964 6465 6e5f 636f 6c75 6d6e 732c 0a20  idden_columns,. 
-0000dfd0: 2020 2020 2020 2020 2020 206f 7264 6572             order
-0000dfe0: 696e 673d 6f72 6465 7269 6e67 2c0a 2020  ing=ordering,.  
-0000dff0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000e000: 205f 6962 6973 5f74 6f5f 7465 6d70 5f74   _ibis_to_temp_t
-0000e010: 6162 6c65 280a 2020 2020 2020 2020 7365  able(.        se
-0000e020: 6c66 2c0a 2020 2020 2020 2020 7461 626c  lf,.        tabl
-0000e030: 653a 2069 6269 735f 7479 7065 732e 5461  e: ibis_types.Ta
-0000e040: 626c 652c 0a20 2020 2020 2020 2063 6c75  ble,.        clu
-0000e050: 7374 6572 5f63 6f6c 733a 2049 7465 7261  ster_cols: Itera
-0000e060: 626c 655b 7374 725d 2c0a 2020 2020 2020  ble[str],.      
-0000e070: 2020 6170 695f 6e61 6d65 3a20 7374 722c    api_name: str,
-0000e080: 0a20 2020 2029 202d 3e20 6269 6771 7565  .    ) -> bigque
-0000e090: 7279 2e54 6162 6c65 5265 6665 7265 6e63  ry.TableReferenc
-0000e0a0: 653a 0a20 2020 2020 2020 2064 6573 7469  e:.        desti
-0000e0b0: 6e61 7469 6f6e 2c20 5f20 3d20 7365 6c66  nation, _ = self
-0000e0c0: 2e5f 7175 6572 795f 746f 5f64 6573 7469  ._query_to_desti
-0000e0d0: 6e61 7469 6f6e 280a 2020 2020 2020 2020  nation(.        
-0000e0e0: 2020 2020 7365 6c66 2e69 6269 735f 636c      self.ibis_cl
-0000e0f0: 6965 6e74 2e63 6f6d 7069 6c65 2874 6162  ient.compile(tab
-0000e100: 6c65 292c 0a20 2020 2020 2020 2020 2020  le),.           
-0000e110: 2069 6e64 6578 5f63 6f6c 733d 6c69 7374   index_cols=list
-0000e120: 2863 6c75 7374 6572 5f63 6f6c 7329 2c0a  (cluster_cols),.
-0000e130: 2020 2020 2020 2020 2020 2020 6170 695f              api_
-0000e140: 6e61 6d65 3d61 7069 5f6e 616d 652c 0a20  name=api_name,. 
-0000e150: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e160: 2023 2054 6865 7265 2073 686f 756c 6420   # There should 
-0000e170: 616c 7761 7973 2062 6520 6120 6465 7374  always be a dest
-0000e180: 696e 6174 696f 6e20 7461 626c 6520 666f  ination table fo
-0000e190: 7220 7468 6973 2071 7565 7279 2074 7970  r this query typ
-0000e1a0: 652e 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-0000e1b0: 6e20 7479 7069 6e67 2e63 6173 7428 6269  n typing.cast(bi
-0000e1c0: 6771 7565 7279 2e54 6162 6c65 5265 6665  gquery.TableRefe
-0000e1d0: 7265 6e63 652c 2064 6573 7469 6e61 7469  rence, destinati
-0000e1e0: 6f6e 290a 0a20 2020 2064 6566 2072 656d  on)..    def rem
-0000e1f0: 6f74 655f 6675 6e63 7469 6f6e 280a 2020  ote_function(.  
-0000e200: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000e210: 2020 2020 696e 7075 745f 7479 7065 733a      input_types:
-0000e220: 2055 6e69 6f6e 5b74 7970 652c 2053 6571   Union[type, Seq
-0000e230: 7565 6e63 655b 7479 7065 5d5d 2c0a 2020  uence[type]],.  
-0000e240: 2020 2020 2020 6f75 7470 7574 5f74 7970        output_typ
-0000e250: 653a 2074 7970 652c 0a20 2020 2020 2020  e: type,.       
-0000e260: 2064 6174 6173 6574 3a20 4f70 7469 6f6e   dataset: Option
-0000e270: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000e280: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
-0000e290: 5f63 6f6e 6e65 6374 696f 6e3a 204f 7074  _connection: Opt
-0000e2a0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e2b0: 652c 0a20 2020 2020 2020 2072 6575 7365  e,.        reuse
-0000e2c0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-0000e2d0: 2020 2020 2020 206e 616d 653a 204f 7074         name: Opt
-0000e2e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e2f0: 652c 0a20 2020 2020 2020 2070 6163 6b61  e,.        packa
-0000e300: 6765 733a 204f 7074 696f 6e61 6c5b 5365  ges: Optional[Se
-0000e310: 7175 656e 6365 5b73 7472 5d5d 203d 204e  quence[str]] = N
-0000e320: 6f6e 652c 0a20 2020 2020 2020 2063 6c6f  one,.        clo
-0000e330: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
-0000e340: 6963 655f 6163 636f 756e 743a 204f 7074  ice_account: Opt
-0000e350: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e360: 652c 0a20 2020 2020 2020 2063 6c6f 7564  e,.        cloud
-0000e370: 5f66 756e 6374 696f 6e5f 6b6d 735f 6b65  _function_kms_ke
-0000e380: 795f 6e61 6d65 3a20 4f70 7469 6f6e 616c  y_name: Optional
-0000e390: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000e3a0: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
-0000e3b0: 7469 6f6e 5f64 6f63 6b65 725f 7265 706f  tion_docker_repo
-0000e3c0: 7369 746f 7279 3a20 4f70 7469 6f6e 616c  sitory: Optional
-0000e3d0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000e3e0: 2020 2020 2020 6d61 785f 6261 7463 6869        max_batchi
-0000e3f0: 6e67 5f72 6f77 733a 204f 7074 696f 6e61  ng_rows: Optiona
-0000e400: 6c5b 696e 745d 203d 2031 3030 302c 0a20  l[int] = 1000,. 
-0000e410: 2020 2020 2020 2063 6c6f 7564 5f66 756e         cloud_fun
-0000e420: 6374 696f 6e5f 7469 6d65 6f75 743a 204f  ction_timeout: O
-0000e430: 7074 696f 6e61 6c5b 696e 745d 203d 2036  ptional[int] = 6
-0000e440: 3030 2c0a 2020 2020 293a 0a20 2020 2020  00,.    ):.     
-0000e450: 2020 2022 2222 4465 636f 7261 746f 7220     """Decorator 
-0000e460: 746f 2074 7572 6e20 6120 7573 6572 2064  to turn a user d
-0000e470: 6566 696e 6564 2066 756e 6374 696f 6e20  efined function 
-0000e480: 696e 746f 2061 2042 6967 5175 6572 7920  into a BigQuery 
-0000e490: 7265 6d6f 7465 2066 756e 6374 696f 6e2e  remote function.
-0000e4a0: 2043 6865 636b 206f 7574 0a20 2020 2020   Check out.     
-0000e4b0: 2020 2074 6865 2063 6f64 6520 7361 6d70     the code samp
-0000e4c0: 6c65 7320 6174 3a20 6874 7470 733a 2f2f  les at: https://
-0000e4d0: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
-0000e4e0: 2f62 6967 7175 6572 792f 646f 6373 2f72  /bigquery/docs/r
-0000e4f0: 656d 6f74 652d 6675 6e63 7469 6f6e 7323  emote-functions#
-0000e500: 6269 6771 7565 7279 2d64 6174 6166 7261  bigquery-datafra
-0000e510: 6d65 732e 0a0a 2020 2020 2020 2020 2e2e  mes...        ..
-0000e520: 206e 6f74 653a 3a0a 2020 2020 2020 2020   note::.        
-0000e530: 2020 2020 506c 6561 7365 206d 616b 6520      Please make 
-0000e540: 7375 7265 2066 6f6c 6c6f 7769 6e67 2069  sure following i
-0000e550: 7320 7365 7475 7020 6265 666f 7265 2075  s setup before u
-0000e560: 7369 6e67 2074 6869 7320 4150 493a 0a0a  sing this API:..
-0000e570: 2020 2020 2020 2020 312e 2048 6176 6520          1. Have 
-0000e580: 7468 6520 6265 6c6f 7720 4150 4973 2065  the below APIs e
-0000e590: 6e61 626c 6564 2066 6f72 2079 6f75 7220  nabled for your 
-0000e5a0: 7072 6f6a 6563 743a 0a0a 2020 2020 2020  project:..      
-0000e5b0: 2020 2020 2020 2a20 4269 6751 7565 7279        * BigQuery
-0000e5c0: 2043 6f6e 6e65 6374 696f 6e20 4150 490a   Connection API.
-0000e5d0: 2020 2020 2020 2020 2020 2020 2a20 436c              * Cl
-0000e5e0: 6f75 6420 4675 6e63 7469 6f6e 7320 4150  oud Functions AP
-0000e5f0: 490a 2020 2020 2020 2020 2020 2020 2a20  I.            * 
-0000e600: 436c 6f75 6420 5275 6e20 4150 490a 2020  Cloud Run API.  
-0000e610: 2020 2020 2020 2020 2020 2a20 436c 6f75            * Clou
-0000e620: 6420 4275 696c 6420 4150 490a 2020 2020  d Build API.    
-0000e630: 2020 2020 2020 2020 2a20 4172 7469 6661          * Artifa
-0000e640: 6374 2052 6567 6973 7472 7920 4150 490a  ct Registry API.
-0000e650: 2020 2020 2020 2020 2020 2020 2a20 436c              * Cl
-0000e660: 6f75 6420 5265 736f 7572 6365 204d 616e  oud Resource Man
-0000e670: 6167 6572 2041 5049 0a0a 2020 2020 2020  ager API..      
-0000e680: 2020 2020 2054 6869 7320 6361 6e20 6265       This can be
-0000e690: 2064 6f6e 6520 6672 6f6d 2074 6865 2063   done from the c
-0000e6a0: 6c6f 7564 2063 6f6e 736f 6c65 2028 6368  loud console (ch
-0000e6b0: 616e 6765 2060 5052 4f4a 4543 545f 4944  ange `PROJECT_ID
-0000e6c0: 6020 746f 2079 6f75 7273 293a 0a20 2020  ` to yours):.   
-0000e6d0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-0000e6e0: 636f 6e73 6f6c 652e 636c 6f75 642e 676f  console.cloud.go
-0000e6f0: 6f67 6c65 2e63 6f6d 2f61 7069 732f 656e  ogle.com/apis/en
-0000e700: 6162 6c65 666c 6f77 3f61 7069 6964 3d62  ableflow?apiid=b
-0000e710: 6967 7175 6572 7963 6f6e 6e65 6374 696f  igqueryconnectio
-0000e720: 6e2e 676f 6f67 6c65 6170 6973 2e63 6f6d  n.googleapis.com
-0000e730: 2c63 6c6f 7564 6675 6e63 7469 6f6e 732e  ,cloudfunctions.
-0000e740: 676f 6f67 6c65 6170 6973 2e63 6f6d 2c72  googleapis.com,r
-0000e750: 756e 2e67 6f6f 676c 6561 7069 732e 636f  un.googleapis.co
-0000e760: 6d2c 636c 6f75 6462 7569 6c64 2e67 6f6f  m,cloudbuild.goo
-0000e770: 676c 6561 7069 732e 636f 6d2c 6172 7469  gleapis.com,arti
-0000e780: 6661 6374 7265 6769 7374 7279 2e67 6f6f  factregistry.goo
-0000e790: 676c 6561 7069 732e 636f 6d2c 636c 6f75  gleapis.com,clou
-0000e7a0: 6472 6573 6f75 7263 656d 616e 6167 6572  dresourcemanager
-0000e7b0: 2e67 6f6f 676c 6561 7069 732e 636f 6d26  .googleapis.com&
-0000e7c0: 7072 6f6a 6563 743d 5052 4f4a 4543 545f  project=PROJECT_
-0000e7d0: 4944 0a0a 2020 2020 2020 2020 2020 204f  ID..           O
-0000e7e0: 7220 6672 6f6d 2074 6865 2067 636c 6f75  r from the gclou
-0000e7f0: 6420 434c 493a 0a0a 2020 2020 2020 2020  d CLI:..        
-0000e800: 2020 2060 2420 6763 6c6f 7564 2073 6572     `$ gcloud ser
-0000e810: 7669 6365 7320 656e 6162 6c65 2062 6967  vices enable big
-0000e820: 7175 6572 7963 6f6e 6e65 6374 696f 6e2e  queryconnection.
-0000e830: 676f 6f67 6c65 6170 6973 2e63 6f6d 2063  googleapis.com c
-0000e840: 6c6f 7564 6675 6e63 7469 6f6e 732e 676f  loudfunctions.go
-0000e850: 6f67 6c65 6170 6973 2e63 6f6d 2072 756e  ogleapis.com run
-0000e860: 2e67 6f6f 676c 6561 7069 732e 636f 6d20  .googleapis.com 
-0000e870: 636c 6f75 6462 7569 6c64 2e67 6f6f 676c  cloudbuild.googl
-0000e880: 6561 7069 732e 636f 6d20 6172 7469 6661  eapis.com artifa
-0000e890: 6374 7265 6769 7374 7279 2e67 6f6f 676c  ctregistry.googl
-0000e8a0: 6561 7069 732e 636f 6d20 636c 6f75 6472  eapis.com cloudr
-0000e8b0: 6573 6f75 7263 656d 616e 6167 6572 2e67  esourcemanager.g
-0000e8c0: 6f6f 676c 6561 7069 732e 636f 6d60 0a0a  oogleapis.com`..
-0000e8d0: 2020 2020 2020 2020 322e 2048 6176 6520          2. Have 
-0000e8e0: 666f 6c6c 6f77 696e 6720 4941 4d20 726f  following IAM ro
-0000e8f0: 6c65 7320 656e 6162 6c65 6420 666f 7220  les enabled for 
-0000e900: 796f 753a 0a0a 2020 2020 2020 2020 2020  you:..          
-0000e910: 2020 2a20 4269 6751 7565 7279 2044 6174    * BigQuery Dat
-0000e920: 6120 4564 6974 6f72 2028 726f 6c65 732f  a Editor (roles/
-0000e930: 6269 6771 7565 7279 2e64 6174 6145 6469  bigquery.dataEdi
-0000e940: 746f 7229 0a20 2020 2020 2020 2020 2020  tor).           
-0000e950: 202a 2042 6967 5175 6572 7920 436f 6e6e   * BigQuery Conn
-0000e960: 6563 7469 6f6e 2041 646d 696e 2028 726f  ection Admin (ro
-0000e970: 6c65 732f 6269 6771 7565 7279 2e63 6f6e  les/bigquery.con
-0000e980: 6e65 6374 696f 6e41 646d 696e 290a 2020  nectionAdmin).  
-0000e990: 2020 2020 2020 2020 2020 2a20 436c 6f75            * Clou
-0000e9a0: 6420 4675 6e63 7469 6f6e 7320 4465 7665  d Functions Deve
-0000e9b0: 6c6f 7065 7220 2872 6f6c 6573 2f63 6c6f  loper (roles/clo
-0000e9c0: 7564 6675 6e63 7469 6f6e 732e 6465 7665  udfunctions.deve
-0000e9d0: 6c6f 7065 7229 0a20 2020 2020 2020 2020  loper).         
-0000e9e0: 2020 202a 2053 6572 7669 6365 2041 6363     * Service Acc
-0000e9f0: 6f75 6e74 2055 7365 7220 2872 6f6c 6573  ount User (roles
-0000ea00: 2f69 616d 2e73 6572 7669 6365 4163 636f  /iam.serviceAcco
-0000ea10: 756e 7455 7365 7229 206f 6e20 7468 6520  untUser) on the 
-0000ea20: 7365 7276 6963 6520 6163 636f 756e 7420  service account 
-0000ea30: 6050 524f 4a45 4354 5f4e 554d 4245 522d  `PROJECT_NUMBER-
-0000ea40: 636f 6d70 7574 6540 6465 7665 6c6f 7065  compute@develope
-0000ea50: 722e 6773 6572 7669 6365 6163 636f 756e  r.gserviceaccoun
-0000ea60: 742e 636f 6d60 0a20 2020 2020 2020 2020  t.com`.         
-0000ea70: 2020 202a 2053 746f 7261 6765 204f 626a     * Storage Obj
-0000ea80: 6563 7420 5669 6577 6572 2028 726f 6c65  ect Viewer (role
-0000ea90: 732f 7374 6f72 6167 652e 6f62 6a65 6374  s/storage.object
-0000eaa0: 5669 6577 6572 290a 2020 2020 2020 2020  Viewer).        
-0000eab0: 2020 2020 2a20 5072 6f6a 6563 7420 4941      * Project IA
-0000eac0: 4d20 4164 6d69 6e20 2872 6f6c 6573 2f72  M Admin (roles/r
-0000ead0: 6573 6f75 7263 656d 616e 6167 6572 2e70  esourcemanager.p
-0000eae0: 726f 6a65 6374 4961 6d41 646d 696e 2920  rojectIamAdmin) 
-0000eaf0: 284f 6e6c 7920 7265 7175 6972 6564 2069  (Only required i
-0000eb00: 6620 7468 6520 6269 6771 7565 7279 2063  f the bigquery c
-0000eb10: 6f6e 6e65 6374 696f 6e20 6265 696e 6720  onnection being 
-0000eb20: 7573 6564 2069 7320 6e6f 7420 7072 652d  used is not pre-
-0000eb30: 6372 6561 7465 6420 616e 6420 6973 2063  created and is c
-0000eb40: 7265 6174 6564 2064 796e 616d 6963 616c  reated dynamical
-0000eb50: 6c79 2077 6974 6820 7573 6572 2063 7265  ly with user cre
-0000eb60: 6465 6e74 6961 6c73 2e29 0a0a 2020 2020  dentials.)..    
-0000eb70: 2020 2020 332e 2045 6974 6865 7220 7468      3. Either th
-0000eb80: 6520 7573 6572 2068 6173 2073 6574 4961  e user has setIa
-0000eb90: 6d50 6f6c 6963 7920 7072 6976 696c 6567  mPolicy privileg
-0000eba0: 6520 6f6e 2074 6865 2070 726f 6a65 6374  e on the project
-0000ebb0: 2c20 6f72 2061 2042 6967 5175 6572 7920  , or a BigQuery 
-0000ebc0: 636f 6e6e 6563 7469 6f6e 2069 7320 7072  connection is pr
-0000ebd0: 652d 6372 6561 7465 6420 7769 7468 206e  e-created with n
-0000ebe0: 6563 6573 7361 7279 2049 414d 2072 6f6c  ecessary IAM rol
-0000ebf0: 6520 7365 743a 0a0a 2020 2020 2020 2020  e set:..        
-0000ec00: 2020 2020 312e 2054 6f20 6372 6561 7465      1. To create
-0000ec10: 2061 2063 6f6e 6e65 6374 696f 6e2c 2066   a connection, f
-0000ec20: 6f6c 6c6f 7720 6874 7470 733a 2f2f 636c  ollow https://cl
-0000ec30: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f62  oud.google.com/b
-0000ec40: 6967 7175 6572 792f 646f 6373 2f72 6566  igquery/docs/ref
-0000ec50: 6572 656e 6365 2f73 7461 6e64 6172 642d  erence/standard-
-0000ec60: 7371 6c2f 7265 6d6f 7465 2d66 756e 6374  sql/remote-funct
-0000ec70: 696f 6e73 2363 7265 6174 655f 615f 636f  ions#create_a_co
-0000ec80: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
-0000ec90: 2020 2020 2032 2e20 546f 2073 6574 2075       2. To set u
-0000eca0: 7020 4941 4d2c 2066 6f6c 6c6f 7720 6874  p IAM, follow ht
-0000ecb0: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-0000ecc0: 6c65 2e63 6f6d 2f62 6967 7175 6572 792f  le.com/bigquery/
-0000ecd0: 646f 6373 2f72 6566 6572 656e 6365 2f73  docs/reference/s
-0000ece0: 7461 6e64 6172 642d 7371 6c2f 7265 6d6f  tandard-sql/remo
-0000ecf0: 7465 2d66 756e 6374 696f 6e73 2367 7261  te-functions#gra
-0000ed00: 6e74 5f70 6572 6d69 7373 696f 6e5f 6f6e  nt_permission_on
-0000ed10: 5f66 756e 6374 696f 6e0a 0a20 2020 2020  _function..     
-0000ed20: 2020 2020 2020 2020 2020 416c 7465 726e            Altern
-0000ed30: 6174 6976 656c 792c 2074 6865 2049 414d  atively, the IAM
-0000ed40: 2063 6f75 6c64 2061 6c73 6f20 6265 2073   could also be s
-0000ed50: 6574 7570 2076 6961 2074 6865 2067 636c  etup via the gcl
-0000ed60: 6f75 6420 434c 493a 0a0a 2020 2020 2020  oud CLI:..      
-0000ed70: 2020 2020 2020 2020 2060 2420 6763 6c6f           `$ gclo
-0000ed80: 7564 2070 726f 6a65 6374 7320 6164 642d  ud projects add-
-0000ed90: 6961 6d2d 706f 6c69 6379 2d62 696e 6469  iam-policy-bindi
-0000eda0: 6e67 2050 524f 4a45 4354 5f49 4420 2d2d  ng PROJECT_ID --
-0000edb0: 6d65 6d62 6572 3d22 7365 7276 6963 6541  member="serviceA
-0000edc0: 6363 6f75 6e74 3a43 4f4e 4e45 4354 494f  ccount:CONNECTIO
-0000edd0: 4e5f 5345 5256 4943 455f 4143 434f 554e  N_SERVICE_ACCOUN
-0000ede0: 545f 4944 2220 2d2d 726f 6c65 3d22 726f  T_ID" --role="ro
-0000edf0: 6c65 732f 7275 6e2e 696e 766f 6b65 7222  les/run.invoker"
-0000ee00: 602e 0a0a 2020 2020 2020 2020 4172 6773  `...        Args
-0000ee10: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-0000ee20: 7075 745f 7479 7065 7320 2874 7970 6520  put_types (type 
-0000ee30: 6f72 2073 6571 7565 6e63 6528 7479 7065  or sequence(type
-0000ee40: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0000ee50: 2020 2020 496e 7075 7420 6461 7461 2074      Input data t
-0000ee60: 7970 652c 206f 7220 7365 7175 656e 6365  ype, or sequence
-0000ee70: 206f 6620 696e 7075 7420 6461 7461 2074   of input data t
-0000ee80: 7970 6573 2069 6e20 7468 6520 7573 6572  ypes in the user
-0000ee90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eea0: 2064 6566 696e 6564 2066 756e 6374 696f   defined functio
-0000eeb0: 6e2e 0a20 2020 2020 2020 2020 2020 206f  n..            o
-0000eec0: 7574 7075 745f 7479 7065 2028 7479 7065  utput_type (type
-0000eed0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000eee0: 2020 2044 6174 6120 7479 7065 206f 6620     Data type of 
-0000eef0: 7468 6520 6f75 7470 7574 2069 6e20 7468  the output in th
-0000ef00: 6520 7573 6572 2064 6566 696e 6564 2066  e user defined f
-0000ef10: 756e 6374 696f 6e2e 0a20 2020 2020 2020  unction..       
-0000ef20: 2020 2020 2064 6174 6173 6574 2028 7374       dataset (st
-0000ef30: 722c 204f 7074 696f 6e61 6c29 3a0a 2020  r, Optional):.  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 4461                Da
-0000ef50: 7461 7365 7420 696e 2077 6869 6368 2074  taset in which t
-0000ef60: 6f20 6372 6561 7465 2061 2042 6967 5175  o create a BigQu
-0000ef70: 6572 7920 7265 6d6f 7465 2066 756e 6374  ery remote funct
-0000ef80: 696f 6e2e 2049 7420 7368 6f75 6c64 2062  ion. It should b
-0000ef90: 6520 696e 0a20 2020 2020 2020 2020 2020  e in.           
-0000efa0: 2020 2020 2060 3c70 726f 6a65 6374 5f69       `<project_i
-0000efb0: 643e 2e3c 6461 7461 7365 745f 6e61 6d65  d>.<dataset_name
-0000efc0: 3e60 206f 7220 603c 6461 7461 7365 745f  >` or `<dataset_
-0000efd0: 6e61 6d65 3e60 2066 6f72 6d61 742e 2049  name>` format. I
-0000efe0: 6620 7468 6973 0a20 2020 2020 2020 2020  f this.         
-0000eff0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
-0000f000: 2069 7320 6e6f 7420 7072 6f76 6964 6564   is not provided
-0000f010: 2074 6865 6e20 7365 7373 696f 6e20 6461   then session da
-0000f020: 7461 7365 7420 6964 2069 7320 7573 6564  taset id is used
-0000f030: 2e0a 2020 2020 2020 2020 2020 2020 6269  ..            bi
-0000f040: 6771 7565 7279 5f63 6f6e 6e65 6374 696f  gquery_connectio
-0000f050: 6e20 2873 7472 2c20 4f70 7469 6f6e 616c  n (str, Optional
-0000f060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f070: 2020 204e 616d 6520 6f66 2074 6865 2042     Name of the B
-0000f080: 6967 5175 6572 7920 636f 6e6e 6563 7469  igQuery connecti
-0000f090: 6f6e 2e20 596f 7520 7368 6f75 6c64 2065  on. You should e
-0000f0a0: 6974 6865 7220 6861 7665 2074 6865 0a20  ither have the. 
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f0c0: 6f6e 6e65 6374 696f 6e20 616c 7265 6164  onnection alread
-0000f0d0: 7920 6372 6561 7465 6420 696e 2074 6865  y created in the
-0000f0e0: 2060 6c6f 6361 7469 6f6e 6020 796f 7520   `location` you 
-0000f0f0: 6861 7665 2063 686f 7365 6e2c 206f 720a  have chosen, or.
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 796f 7520 7368 6f75 6c64 2068 6176 6520  you should have 
-0000f120: 7468 6520 5072 6f6a 6563 7420 4941 4d20  the Project IAM 
-0000f130: 4164 6d69 6e20 726f 6c65 2074 6f20 656e  Admin role to en
-0000f140: 6162 6c65 2074 6865 2073 6572 7669 6365  able the service
-0000f150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f160: 2074 6f20 6372 6561 7465 2074 6865 2063   to create the c
-0000f170: 6f6e 6e65 6374 696f 6e20 666f 7220 796f  onnection for yo
-0000f180: 7520 6966 2079 6f75 206e 6565 6420 6974  u if you need it
-0000f190: 2e20 4966 2074 6869 7320 7061 7261 6d65  . If this parame
-0000f1a0: 7465 7220 6973 0a20 2020 2020 2020 2020  ter is.         
-0000f1b0: 2020 2020 2020 206e 6f74 2070 726f 7669         not provi
-0000f1c0: 6465 6420 7468 656e 2074 6865 2042 6967  ded then the Big
-0000f1d0: 5175 6572 7920 636f 6e6e 6563 7469 6f6e  Query connection
-0000f1e0: 2066 726f 6d20 7468 6520 7365 7373 696f   from the sessio
-0000f1f0: 6e20 6973 2075 7365 642e 0a20 2020 2020  n is used..     
-0000f200: 2020 2020 2020 2072 6575 7365 2028 626f         reuse (bo
-0000f210: 6f6c 2c20 4f70 7469 6f6e 616c 293a 0a20  ol, Optional):. 
-0000f220: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-0000f230: 6575 7365 2074 6865 2072 656d 6f74 6520  euse the remote 
-0000f240: 6675 6e63 7469 6f6e 2069 6620 616c 7265  function if alre
-0000f250: 6164 7920 6578 6973 7473 2e0a 2020 2020  ady exists..    
-0000f260: 2020 2020 2020 2020 2020 2020 6054 7275              `Tru
-0000f270: 6560 2062 7920 6465 6661 756c 742c 2077  e` by default, w
-0000f280: 6869 6368 2077 696c 6c20 7265 7375 6c74  hich will result
-0000f290: 2069 6e20 7265 7573 696e 6720 616e 2065   in reusing an e
-0000f2a0: 7869 7374 696e 6720 7265 6d6f 7465 0a20  xisting remote. 
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f2c0: 756e 6374 696f 6e20 616e 6420 636f 7272  unction and corr
-0000f2d0: 6573 706f 6e64 696e 6720 636c 6f75 6420  esponding cloud 
-0000f2e0: 6675 6e63 7469 6f6e 2028 6966 2061 6e79  function (if any
-0000f2f0: 2920 7468 6174 2077 6173 0a20 2020 2020  ) that was.     
-0000f300: 2020 2020 2020 2020 2020 2070 7265 7669             previ
-0000f310: 6f75 736c 7920 6372 6561 7465 6420 666f  ously created fo
-0000f320: 7220 7468 6520 7361 6d65 2075 6466 2e0a  r the same udf..
-0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f340: 5365 7474 696e 6720 6974 2074 6f20 6046  Setting it to `F
-0000f350: 616c 7365 6020 776f 756c 6420 666f 7263  alse` would forc
-0000f360: 6520 6372 6561 7469 6e67 2061 2075 6e69  e creating a uni
-0000f370: 7175 6520 7265 6d6f 7465 2066 756e 6374  que remote funct
-0000f380: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-0000f390: 2020 2020 2049 6620 7468 6520 7265 7175       If the requ
-0000f3a0: 6972 6564 2072 656d 6f74 6520 6675 6e63  ired remote func
-0000f3b0: 7469 6f6e 2064 6f65 7320 6e6f 7420 6578  tion does not ex
-0000f3c0: 6973 7420 7468 656e 2069 7420 776f 756c  ist then it woul
-0000f3d0: 6420 6265 0a20 2020 2020 2020 2020 2020  d be.           
-0000f3e0: 2020 2020 2063 7265 6174 6564 2069 7272       created irr
-0000f3f0: 6573 7065 6374 6976 6520 6f66 2074 6869  espective of thi
-0000f400: 7320 7061 7261 6d2e 0a20 2020 2020 2020  s param..       
-0000f410: 2020 2020 206e 616d 6520 2873 7472 2c20       name (str, 
-0000f420: 4f70 7469 6f6e 616c 293a 0a20 2020 2020  Optional):.     
-0000f430: 2020 2020 2020 2020 2020 2045 7870 6c69             Expli
-0000f440: 6369 7420 6e61 6d65 206f 6620 7468 6520  cit name of the 
-0000f450: 7065 7273 6973 7465 6420 4269 6751 7565  persisted BigQue
-0000f460: 7279 2072 656d 6f74 6520 6675 6e63 7469  ry remote functi
-0000f470: 6f6e 2e20 5573 6520 6974 2077 6974 680a  on. Use it with.
-0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 6361 7574 696f 6e2c 2062 6563 6175 7365  caution, because
-0000f4a0: 2074 776f 2075 7365 7273 2077 6f72 6b69   two users worki
-0000f4b0: 6e67 2069 6e20 7468 6520 7361 6d65 2070  ng in the same p
-0000f4c0: 726f 6a65 6374 2061 6e64 2064 6174 6173  roject and datas
-0000f4d0: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
-0000f4e0: 2020 2063 6f75 6c64 206f 7665 7277 7269     could overwri
-0000f4f0: 7465 2065 6163 6820 6f74 6865 7227 7320  te each other's 
-0000f500: 7265 6d6f 7465 2066 756e 6374 696f 6e73  remote functions
-0000f510: 2069 6620 7468 6579 2075 7365 2074 6865   if they use the
-0000f520: 2073 616d 650a 2020 2020 2020 2020 2020   same.          
-0000f530: 2020 2020 2020 7065 7273 6973 7465 6e74        persistent
-0000f540: 206e 616d 652e 0a20 2020 2020 2020 2020   name..         
-0000f550: 2020 2070 6163 6b61 6765 7320 2873 7472     packages (str
-0000f560: 5b5d 2c20 4f70 7469 6f6e 616c 293a 0a20  [], Optional):. 
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2045                 E
-0000f580: 7870 6c69 6369 7420 6e61 6d65 206f 6620  xplicit name of 
-0000f590: 7468 6520 6578 7465 726e 616c 2070 6163  the external pac
-0000f5a0: 6b61 6765 2064 6570 656e 6465 6e63 6965  kage dependencie
-0000f5b0: 732e 2045 6163 6820 6465 7065 6e64 656e  s. Each dependen
-0000f5c0: 6379 0a20 2020 2020 2020 2020 2020 2020  cy.             
-0000f5d0: 2020 2069 7320 6164 6465 6420 746f 2074     is added to t
-0000f5e0: 6865 2060 7265 7175 6972 656d 656e 7473  he `requirements
-0000f5f0: 2e74 7874 6020 6173 2069 732c 2061 6e64  .txt` as is, and
-0000f600: 2063 616e 2062 6520 6f66 2074 6865 2066   can be of the f
-0000f610: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
-0000f620: 2020 2020 7375 7070 6f72 7465 6420 696e      supported in
-0000f630: 2068 7474 7073 3a2f 2f70 6970 2e70 7970   https://pip.pyp
-0000f640: 612e 696f 2f65 6e2f 7374 6162 6c65 2f72  a.io/en/stable/r
-0000f650: 6566 6572 656e 6365 2f72 6571 7569 7265  eference/require
-0000f660: 6d65 6e74 732d 6669 6c65 2d66 6f72 6d61  ments-file-forma
-0000f670: 742f 2e0a 2020 2020 2020 2020 2020 2020  t/..            
-0000f680: 636c 6f75 645f 6675 6e63 7469 6f6e 5f73  cloud_function_s
-0000f690: 6572 7669 6365 5f61 6363 6f75 6e74 2028  ervice_account (
-0000f6a0: 7374 722c 204f 7074 696f 6e61 6c29 3a0a  str, Optional):.
-0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6c0: 5365 7276 6963 6520 6163 636f 756e 7420  Service account 
-0000f6d0: 746f 2075 7365 2066 6f72 2074 6865 2063  to use for the c
-0000f6e0: 6c6f 7564 2066 756e 6374 696f 6e73 2e20  loud functions. 
-0000f6f0: 4966 206e 6f74 2070 726f 7669 6465 640a  If not provided.
-0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f710: 7468 656e 2074 6865 2064 6566 6175 6c74  then the default
-0000f720: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-0000f730: 2077 6f75 6c64 2062 6520 7573 6564 2e20   would be used. 
-0000f740: 5365 650a 2020 2020 2020 2020 2020 2020  See.            
-0000f750: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
-0000f760: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
-0000f770: 6374 696f 6e73 2f64 6f63 732f 7365 6375  ctions/docs/secu
-0000f780: 7269 6e67 2f66 756e 6374 696f 6e2d 6964  ring/function-id
-0000f790: 656e 7469 7479 0a20 2020 2020 2020 2020  entity.         
-0000f7a0: 2020 2020 2020 2066 6f72 206d 6f72 6520         for more 
-0000f7b0: 6465 7461 696c 732e 2050 6c65 6173 6520  details. Please 
-0000f7c0: 6d61 6b65 2073 7572 6520 7468 6520 7365  make sure the se
-0000f7d0: 7276 6963 6520 6163 636f 756e 7420 6861  rvice account ha
-0000f7e0: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0000f7f0: 2020 2020 2020 6e65 6365 7373 6172 7920        necessary 
-0000f800: 4941 4d20 7065 726d 6973 7369 6f6e 7320  IAM permissions 
-0000f810: 636f 6e66 6967 7572 6564 2061 7320 6465  configured as de
-0000f820: 7363 7269 6265 6420 696e 0a20 2020 2020  scribed in.     
-0000f830: 2020 2020 2020 2020 2020 2068 7474 7073             https
-0000f840: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-0000f850: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
-0000f860: 6373 2f72 6566 6572 656e 6365 2f69 616d  cs/reference/iam
-0000f870: 2f72 6f6c 6573 2361 6464 6974 696f 6e61  /roles#additiona
-0000f880: 6c2d 636f 6e66 6967 7572 6174 696f 6e2e  l-configuration.
-0000f890: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
-0000f8a0: 7564 5f66 756e 6374 696f 6e5f 6b6d 735f  ud_function_kms_
-0000f8b0: 6b65 795f 6e61 6d65 2028 7374 722c 204f  key_name (str, O
-0000f8c0: 7074 696f 6e61 6c29 3a0a 2020 2020 2020  ptional):.      
-0000f8d0: 2020 2020 2020 2020 2020 4375 7374 6f6d            Custom
-0000f8e0: 6572 206d 616e 6167 6564 2065 6e63 7279  er managed encry
-0000f8f0: 7074 696f 6e20 6b65 7920 746f 2070 726f  ption key to pro
-0000f900: 7465 6374 2063 6c6f 7564 2066 756e 6374  tect cloud funct
-0000f910: 696f 6e73 2061 6e64 0a20 2020 2020 2020  ions and.       
-0000f920: 2020 2020 2020 2020 2072 656c 6174 6564           related
-0000f930: 2064 6174 6120 6174 2072 6573 742e 2054   data at rest. T
-0000f940: 6869 7320 6973 206f 6620 7468 6520 666f  his is of the fo
-0000f950: 726d 6174 0a20 2020 2020 2020 2020 2020  rmat.           
-0000f960: 2020 2020 2070 726f 6a65 6374 732f 5052       projects/PR
-0000f970: 4f4a 4543 545f 4944 2f6c 6f63 6174 696f  OJECT_ID/locatio
-0000f980: 6e73 2f4c 4f43 4154 494f 4e2f 6b65 7952  ns/LOCATION/keyR
-0000f990: 696e 6773 2f4b 4559 5249 4e47 2f63 7279  ings/KEYRING/cry
-0000f9a0: 7074 6f4b 6579 732f 4b45 592e 0a20 2020  ptoKeys/KEY..   
-0000f9b0: 2020 2020 2020 2020 2020 2020 2052 6561               Rea
-0000f9c0: 6420 6874 7470 733a 2f2f 636c 6f75 642e  d https://cloud.
-0000f9d0: 676f 6f67 6c65 2e63 6f6d 2f66 756e 6374  google.com/funct
-0000f9e0: 696f 6e73 2f64 6f63 732f 7365 6375 7269  ions/docs/securi
-0000f9f0: 6e67 2f63 6d65 6b20 666f 720a 2020 2020  ng/cmek for.    
-0000fa00: 2020 2020 2020 2020 2020 2020 6d6f 7265              more
-0000fa10: 2064 6574 6169 6c73 2069 6e63 6c75 6469   details includi
-0000fa20: 6e67 2067 7261 6e74 696e 6720 6e65 6365  ng granting nece
-0000fa30: 7373 6172 7920 7365 7276 6963 6520 6163  ssary service ac
-0000fa40: 636f 756e 7473 0a20 2020 2020 2020 2020  counts.         
-0000fa50: 2020 2020 2020 2061 6363 6573 7320 746f         access to
-0000fa60: 2074 6865 206b 6579 2e0a 2020 2020 2020   the key..      
-0000fa70: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
-0000fa80: 7469 6f6e 5f64 6f63 6b65 725f 7265 706f  tion_docker_repo
-0000fa90: 7369 746f 7279 2028 7374 722c 204f 7074  sitory (str, Opt
-0000faa0: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
-0000fab0: 2020 2020 2020 2020 446f 636b 6572 2072          Docker r
-0000fac0: 6570 6f73 6974 6f72 7920 6372 6561 7465  epository create
-0000fad0: 6420 7769 7468 2074 6865 2073 616d 6520  d with the same 
-0000fae0: 656e 6372 7970 7469 6f6e 206b 6579 2061  encryption key a
-0000faf0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000fb00: 2020 6063 6c6f 7564 5f66 756e 6374 696f    `cloud_functio
-0000fb10: 6e5f 6b6d 735f 6b65 795f 6e61 6d65 6020  n_kms_key_name` 
-0000fb20: 746f 2073 746f 7265 2065 6e63 7279 7074  to store encrypt
-0000fb30: 6564 2061 7274 6966 6163 7473 0a20 2020  ed artifacts.   
-0000fb40: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-0000fb50: 6174 6564 2074 6f20 7375 7070 6f72 7420  ated to support 
-0000fb60: 7468 6520 636c 6f75 6420 6675 6e63 7469  the cloud functi
-0000fb70: 6f6e 2e20 5468 6973 2069 7320 6f66 2074  on. This is of t
-0000fb80: 6865 2066 6f72 6d61 740a 2020 2020 2020  he format.      
-0000fb90: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
-0000fba0: 7473 2f50 524f 4a45 4354 5f49 442f 6c6f  ts/PROJECT_ID/lo
-0000fbb0: 6361 7469 6f6e 732f 4c4f 4341 5449 4f4e  cations/LOCATION
-0000fbc0: 2f72 6570 6f73 6974 6f72 6965 732f 5245  /repositories/RE
-0000fbd0: 504f 5349 544f 5259 5f4e 414d 452e 0a20  POSITORY_NAME.. 
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-0000fbf0: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
-0000fc00: 7365 650a 2020 2020 2020 2020 2020 2020  see.            
-0000fc10: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
-0000fc20: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
-0000fc30: 6374 696f 6e73 2f64 6f63 732f 7365 6375  ctions/docs/secu
-0000fc40: 7269 6e67 2f63 6d65 6b23 6265 666f 7265  ring/cmek#before
-0000fc50: 5f79 6f75 5f62 6567 696e 2e0a 2020 2020  _you_begin..    
-0000fc60: 2020 2020 2020 2020 6d61 785f 6261 7463          max_batc
-0000fc70: 6869 6e67 5f72 6f77 7320 2869 6e74 2c20  hing_rows (int, 
-0000fc80: 4f70 7469 6f6e 616c 293a 0a20 2020 2020  Optional):.     
-0000fc90: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-0000fca0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-0000fcb0: 2072 6f77 7320 746f 2062 6520 6261 7463   rows to be batc
-0000fcc0: 6865 6420 666f 7220 7072 6f63 6573 7369  hed for processi
-0000fcd0: 6e67 2069 6e20 7468 650a 2020 2020 2020  ng in the.      
-0000fce0: 2020 2020 2020 2020 2020 4251 2072 656d            BQ rem
-0000fcf0: 6f74 6520 6675 6e63 7469 6f6e 2e20 4465  ote function. De
-0000fd00: 6661 756c 7420 7661 6c75 6520 6973 2031  fault value is 1
-0000fd10: 3030 302e 2041 206c 6f77 6572 206e 756d  000. A lower num
-0000fd20: 6265 7220 6361 6e20 6265 0a20 2020 2020  ber can be.     
-0000fd30: 2020 2020 2020 2020 2020 2070 6173 7365             passe
-0000fd40: 6420 746f 2061 766f 6964 2074 696d 656f  d to avoid timeo
-0000fd50: 7574 7320 696e 2063 6173 6520 7468 6520  uts in case the 
-0000fd60: 7573 6572 2063 6f64 6520 6973 2074 6f6f  user code is too
-0000fd70: 2063 6f6d 706c 6578 2074 6f0a 2020 2020   complex to.    
-0000fd80: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-0000fd90: 6573 7320 6c61 7267 6520 6e75 6d62 6572  ess large number
-0000fda0: 206f 6620 726f 7773 2066 6173 7420 656e   of rows fast en
-0000fdb0: 6f75 6768 2e20 4120 6869 6768 6572 206e  ough. A higher n
-0000fdc0: 756d 6265 7220 6361 6e20 6265 0a20 2020  umber can be.   
-0000fdd0: 2020 2020 2020 2020 2020 2020 2075 7365               use
-0000fde0: 6420 746f 2069 6e63 7265 6173 6520 7468  d to increase th
-0000fdf0: 726f 7567 6870 7574 2069 6e20 6361 7365  roughput in case
-0000fe00: 2074 6865 2075 7365 7220 636f 6465 2069   the user code i
-0000fe10: 7320 6661 7374 2065 6e6f 7567 682e 0a20  s fast enough.. 
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-0000fe30: 4e6f 6e65 6020 6361 6e20 6265 2070 6173  None` can be pas
-0000fe40: 7365 6420 746f 206c 6574 2042 5120 7265  sed to let BQ re
-0000fe50: 6d6f 7465 2066 756e 6374 696f 6e73 2073  mote functions s
-0000fe60: 6572 7669 6365 2061 7070 6c79 0a20 2020  ervice apply.   
-0000fe70: 2020 2020 2020 2020 2020 2020 2064 6566               def
-0000fe80: 6175 6c74 2062 6174 6368 696e 672e 2053  ault batching. S
-0000fe90: 6565 2066 6f72 206d 6f72 6520 6465 7461  ee for more deta
-0000fea0: 696c 730a 2020 2020 2020 2020 2020 2020  ils.            
-0000feb0: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
-0000fec0: 642e 676f 6f67 6c65 2e63 6f6d 2f62 6967  d.google.com/big
-0000fed0: 7175 6572 792f 646f 6373 2f72 656d 6f74  query/docs/remot
-0000fee0: 652d 6675 6e63 7469 6f6e 7323 6c69 6d69  e-functions#limi
-0000fef0: 7469 6e67 5f6e 756d 6265 725f 6f66 5f72  ting_number_of_r
-0000ff00: 6f77 735f 696e 5f61 5f62 6174 6368 5f72  ows_in_a_batch_r
-0000ff10: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
-0000ff20: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-0000ff30: 6f6e 5f74 696d 656f 7574 2028 696e 742c  on_timeout (int,
-0000ff40: 204f 7074 696f 6e61 6c29 3a0a 2020 2020   Optional):.    
-0000ff50: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000ff60: 6d61 7869 6d75 6d20 616d 6f75 6e74 206f  maximum amount o
-0000ff70: 6620 7469 6d65 2028 696e 2073 6563 6f6e  f time (in secon
-0000ff80: 6473 2920 4269 6751 7565 7279 2073 686f  ds) BigQuery sho
-0000ff90: 756c 6420 7761 6974 2066 6f72 0a20 2020  uld wait for.   
-0000ffa0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-0000ffb0: 2063 6c6f 7564 2066 756e 6374 696f 6e20   cloud function 
-0000ffc0: 746f 2072 6574 7572 6e20 6120 7265 7370  to return a resp
-0000ffd0: 6f6e 7365 2e20 5365 6520 666f 7220 6d6f  onse. See for mo
-0000ffe0: 7265 2064 6574 6169 6c73 0a20 2020 2020  re details.     
-0000fff0: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00010000: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-00010010: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
-00010020: 6373 2f63 6f6e 6669 6775 7269 6e67 2f74  cs/configuring/t
-00010030: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
-00010040: 2020 2020 2020 2020 506c 6561 7365 206e          Please n
-00010050: 6f74 6520 7468 6174 2065 7665 6e20 7468  ote that even th
-00010060: 6f75 6768 2074 6865 2063 6c6f 7564 2066  ough the cloud f
-00010070: 756e 6374 696f 6e20 2832 6e64 2067 656e  unction (2nd gen
-00010080: 2920 6974 7365 6c66 0a20 2020 2020 2020  ) itself.       
-00010090: 2020 2020 2020 2020 2061 6c6c 6f77 7320           allows 
-000100a0: 7365 6574 696e 6720 7570 2074 6f20 3630  seeting up to 60
-000100b0: 206d 696e 7574 6573 206f 6620 7469 6d65   minutes of time
-000100c0: 6f75 742c 2042 6967 5175 6572 7920 7265  out, BigQuery re
-000100d0: 6d6f 7465 0a20 2020 2020 2020 2020 2020  mote.           
-000100e0: 2020 2020 2066 756e 6374 696f 6e20 6361       function ca
-000100f0: 6e20 7761 6974 206f 6e6c 7920 7570 2074  n wait only up t
-00010100: 6f20 3230 206d 696e 7574 6573 2c20 7365  o 20 minutes, se
-00010110: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
-00010120: 6c73 0a20 2020 2020 2020 2020 2020 2020  ls.             
-00010130: 2020 2068 7474 7073 3a2f 2f63 6c6f 7564     https://cloud
-00010140: 2e67 6f6f 676c 652e 636f 6d2f 6269 6771  .google.com/bigq
-00010150: 7565 7279 2f71 756f 7461 7323 7265 6d6f  uery/quotas#remo
-00010160: 7465 5f66 756e 6374 696f 6e5f 6c69 6d69  te_function_limi
-00010170: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00010180: 2020 2020 4279 2064 6566 6175 6c74 2042      By default B
-00010190: 6967 5175 6572 7920 4461 7461 4672 616d  igQuery DataFram
-000101a0: 6573 2075 7365 7320 6120 3130 206d 696e  es uses a 10 min
-000101b0: 7574 6520 7469 6d65 6f75 742e 2060 4e6f  ute timeout. `No
-000101c0: 6e65 600a 2020 2020 2020 2020 2020 2020  ne`.            
-000101d0: 2020 2020 6361 6e20 6265 2070 6173 7365      can be passe
-000101e0: 6420 746f 206c 6574 2074 6865 2063 6c6f  d to let the clo
-000101f0: 7564 2066 756e 6374 696f 6e73 2064 6566  ud functions def
-00010200: 6175 6c74 2074 696d 656f 7574 2074 616b  ault timeout tak
-00010210: 6520 6566 6665 6374 2e0a 2020 2020 2020  e effect..      
-00010220: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00010230: 2020 2020 2020 2063 616c 6c61 626c 653a         callable:
-00010240: 2041 2072 656d 6f74 6520 6675 6e63 7469   A remote functi
-00010250: 6f6e 206f 626a 6563 7420 706f 696e 7469  on object pointi
-00010260: 6e67 2074 6f20 7468 6520 636c 6f75 6420  ng to the cloud 
-00010270: 6173 7365 7473 2063 7265 6174 6564 0a20  assets created. 
-00010280: 2020 2020 2020 2020 2020 2069 6e20 7468             in th
-00010290: 6520 6261 636b 6772 6f75 6e64 2074 6f20  e background to 
-000102a0: 7375 7070 6f72 7420 7468 6520 7265 6d6f  support the remo
-000102b0: 7465 2065 7865 6375 7469 6f6e 2e20 5468  te execution. Th
-000102c0: 6520 636c 6f75 6420 6173 7365 7473 2063  e cloud assets c
-000102d0: 616e 2062 650a 2020 2020 2020 2020 2020  an be.          
-000102e0: 2020 6c6f 6361 7465 6420 7468 726f 7567    located throug
-000102f0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
-00010300: 7072 6f70 6572 7469 6573 2073 6574 2069  properties set i
-00010310: 6e20 7468 6520 6f62 6a65 6374 3a0a 0a20  n the object:.. 
-00010320: 2020 2020 2020 2020 2020 2060 6269 6766             `bigf
-00010330: 7261 6d65 735f 636c 6f75 645f 6675 6e63  rames_cloud_func
-00010340: 7469 6f6e 6020 2d20 5468 6520 676f 6f67  tion` - The goog
-00010350: 6c65 2063 6c6f 7564 2066 756e 6374 696f  le cloud functio
-00010360: 6e20 6465 706c 6f79 6564 2066 6f72 2074  n deployed for t
-00010370: 6865 2075 7365 7220 6465 6669 6e65 6420  he user defined 
-00010380: 636f 6465 2e0a 0a20 2020 2020 2020 2020  code...         
-00010390: 2020 2060 6269 6766 7261 6d65 735f 7265     `bigframes_re
-000103a0: 6d6f 7465 5f66 756e 6374 696f 6e60 202d  mote_function` -
-000103b0: 2054 6865 2062 6967 7175 6572 7920 7265   The bigquery re
-000103c0: 6d6f 7465 2066 756e 6374 696f 6e20 6361  mote function ca
-000103d0: 7061 626c 6520 6f66 2063 616c 6c69 6e67  pable of calling
-000103e0: 2069 6e74 6f20 6062 6967 6672 616d 6573   into `bigframes
-000103f0: 5f63 6c6f 7564 5f66 756e 6374 696f 6e60  _cloud_function`
-00010400: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00010410: 2020 2020 2020 7265 7475 726e 2062 6967        return big
-00010420: 6672 616d 6573 5f72 6628 0a20 2020 2020  frames_rf(.     
-00010430: 2020 2020 2020 2069 6e70 7574 5f74 7970         input_typ
-00010440: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00010450: 6f75 7470 7574 5f74 7970 652c 0a20 2020  output_type,.   
-00010460: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
-00010470: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
-00010480: 2020 2064 6174 6173 6574 3d64 6174 6173     dataset=datas
-00010490: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-000104a0: 6269 6771 7565 7279 5f63 6f6e 6e65 6374  bigquery_connect
-000104b0: 696f 6e3d 6269 6771 7565 7279 5f63 6f6e  ion=bigquery_con
-000104c0: 6e65 6374 696f 6e2c 0a20 2020 2020 2020  nection,.       
-000104d0: 2020 2020 2072 6575 7365 3d72 6575 7365       reuse=reuse
-000104e0: 2c0a 2020 2020 2020 2020 2020 2020 6e61  ,.            na
-000104f0: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
-00010500: 2020 2020 2070 6163 6b61 6765 733d 7061       packages=pa
-00010510: 636b 6167 6573 2c0a 2020 2020 2020 2020  ckages,.        
-00010520: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-00010530: 6f6e 5f73 6572 7669 6365 5f61 6363 6f75  on_service_accou
-00010540: 6e74 3d63 6c6f 7564 5f66 756e 6374 696f  nt=cloud_functio
-00010550: 6e5f 7365 7276 6963 655f 6163 636f 756e  n_service_accoun
-00010560: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
-00010570: 6c6f 7564 5f66 756e 6374 696f 6e5f 6b6d  loud_function_km
-00010580: 735f 6b65 795f 6e61 6d65 3d63 6c6f 7564  s_key_name=cloud
-00010590: 5f66 756e 6374 696f 6e5f 6b6d 735f 6b65  _function_kms_ke
-000105a0: 795f 6e61 6d65 2c0a 2020 2020 2020 2020  y_name,.        
-000105b0: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-000105c0: 6f6e 5f64 6f63 6b65 725f 7265 706f 7369  on_docker_reposi
-000105d0: 746f 7279 3d63 6c6f 7564 5f66 756e 6374  tory=cloud_funct
-000105e0: 696f 6e5f 646f 636b 6572 5f72 6570 6f73  ion_docker_repos
-000105f0: 6974 6f72 792c 0a20 2020 2020 2020 2020  itory,.         
-00010600: 2020 206d 6178 5f62 6174 6368 696e 675f     max_batching_
-00010610: 726f 7773 3d6d 6178 5f62 6174 6368 696e  rows=max_batchin
-00010620: 675f 726f 7773 2c0a 2020 2020 2020 2020  g_rows,.        
-00010630: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
-00010640: 6f6e 5f74 696d 656f 7574 3d63 6c6f 7564  on_timeout=cloud
-00010650: 5f66 756e 6374 696f 6e5f 7469 6d65 6f75  _function_timeou
-00010660: 742c 0a20 2020 2020 2020 2029 0a0a 2020  t,.        )..  
-00010670: 2020 6465 6620 7265 6164 5f67 6271 5f66    def read_gbq_f
-00010680: 756e 6374 696f 6e28 0a20 2020 2020 2020  unction(.       
-00010690: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
-000106a0: 756e 6374 696f 6e5f 6e61 6d65 3a20 7374  unction_name: st
-000106b0: 722c 0a20 2020 2029 3a0a 2020 2020 2020  r,.    ):.      
-000106c0: 2020 2222 224c 6f61 6473 2061 2042 6967    """Loads a Big
-000106d0: 5175 6572 7920 6675 6e63 7469 6f6e 2066  Query function f
-000106e0: 726f 6d20 4269 6751 7565 7279 2e0a 0a20  rom BigQuery... 
-000106f0: 2020 2020 2020 2054 6865 6e20 6974 2063         Then it c
-00010700: 616e 2062 6520 6170 706c 6965 6420 746f  an be applied to
-00010710: 2061 2044 6174 6146 7261 6d65 206f 7220   a DataFrame or 
-00010720: 5365 7269 6573 2e0a 0a20 2020 2020 2020  Series...       
-00010730: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
-00010740: 2020 2020 2020 2054 6865 2072 6574 7572         The retur
-00010750: 6e20 7479 7065 206f 6620 7468 6520 6675  n type of the fu
-00010760: 6e63 7469 6f6e 206d 7573 7420 6265 2065  nction must be e
-00010770: 7870 6c69 6369 746c 7920 7370 6563 6966  xplicitly specif
-00010780: 6965 6420 696e 2074 6865 0a20 2020 2020  ied in the.     
-00010790: 2020 2020 2020 2066 756e 6374 696f 6e27         function'
-000107a0: 7320 6f72 6967 696e 616c 2064 6566 696e  s original defin
-000107b0: 6974 696f 6e20 6576 656e 2069 6620 6e6f  ition even if no
-000107c0: 7420 6f74 6865 7277 6973 6520 7265 7175  t otherwise requ
-000107d0: 6972 6564 2e0a 0a20 2020 2020 2020 2042  ired...        B
-000107e0: 6967 5175 6572 7920 5574 696c 7320 7072  igQuery Utils pr
-000107f0: 6f76 6964 6573 206d 616e 7920 7075 626c  ovides many publ
-00010800: 6963 2066 756e 6374 696f 6e73 2075 6e64  ic functions und
-00010810: 6572 2074 6865 2060 6062 7175 7469 6c60  er the ``bqutil`
-00010820: 6020 7072 6f6a 6563 7420 6f6e 2047 6f6f  ` project on Goo
-00010830: 676c 6520 436c 6f75 6420 506c 6174 666f  gle Cloud Platfo
-00010840: 726d 2070 726f 6a65 6374 0a20 2020 2020  rm project.     
-00010850: 2020 2028 5365 653a 2068 7474 7073 3a2f     (See: https:/
-00010860: 2f67 6974 6875 622e 636f 6d2f 476f 6f67  /github.com/Goog
-00010870: 6c65 436c 6f75 6450 6c61 7466 6f72 6d2f  leCloudPlatform/
-00010880: 6269 6771 7565 7279 2d75 7469 6c73 2f74  bigquery-utils/t
-00010890: 7265 652f 6d61 7374 6572 2f75 6466 7323  ree/master/udfs#
-000108a0: 7573 696e 672d 7468 652d 7564 6673 292e  using-the-udfs).
-000108b0: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-000108c0: 2063 6865 636b 6f75 7420 436f 6d6d 756e   checkout Commun
-000108d0: 6974 7920 5544 4673 2074 6f20 7573 6520  ity UDFs to use 
-000108e0: 636f 6d6d 756e 6974 792d 636f 6e74 7269  community-contri
-000108f0: 6275 7465 6420 6675 6e63 7469 6f6e 732e  buted functions.
-00010900: 0a20 2020 2020 2020 2028 5365 653a 2068  .        (See: h
-00010910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00010920: 6d2f 476f 6f67 6c65 436c 6f75 6450 6c61  m/GoogleCloudPla
-00010930: 7466 6f72 6d2f 6269 6771 7565 7279 2d75  tform/bigquery-u
-00010940: 7469 6c73 2f74 7265 652f 6d61 7374 6572  tils/tree/master
-00010950: 2f75 6466 732f 636f 6d6d 756e 6974 7923  /udfs/community#
-00010960: 636f 6d6d 756e 6974 792d 7564 6673 292e  community-udfs).
-00010970: 0a0a 2020 2020 2020 2020 2a2a 4578 616d  ..        **Exam
-00010980: 706c 6573 3a2a 2a0a 0a20 2020 2020 2020  ples:**..       
-00010990: 2055 7365 2074 6865 2060 6063 775f 6c6f   Use the ``cw_lo
-000109a0: 7765 725f 6361 7365 5f61 7363 6969 5f6f  wer_case_ascii_o
-000109b0: 6e6c 7960 6020 6675 6e63 7469 6f6e 2066  nly`` function f
-000109c0: 726f 6d20 436f 6d6d 756e 6974 7920 5544  rom Community UD
-000109d0: 4673 2e0a 2020 2020 2020 2020 2868 7474  Fs..        (htt
-000109e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000109f0: 476f 6f67 6c65 436c 6f75 6450 6c61 7466  GoogleCloudPlatf
-00010a00: 6f72 6d2f 6269 6771 7565 7279 2d75 7469  orm/bigquery-uti
-00010a10: 6c73 2f62 6c6f 622f 6d61 7374 6572 2f75  ls/blob/master/u
-00010a20: 6466 732f 636f 6d6d 756e 6974 792f 6377  dfs/community/cw
-00010a30: 5f6c 6f77 6572 5f63 6173 655f 6173 6369  _lower_case_asci
-00010a40: 695f 6f6e 6c79 2e73 716c 7829 0a0a 2020  i_only.sqlx)..  
-00010a50: 2020 2020 2020 2020 2020 3e3e 3e20 696d            >>> im
-00010a60: 706f 7274 2062 6967 6672 616d 6573 2e70  port bigframes.p
-00010a70: 616e 6461 7320 6173 2062 7064 0a20 2020  andas as bpd.   
-00010a80: 2020 2020 2020 2020 203e 3e3e 2062 7064           >>> bpd
-00010a90: 2e6f 7074 696f 6e73 2e64 6973 706c 6179  .options.display
-00010aa0: 2e70 726f 6772 6573 735f 6261 7220 3d20  .progress_bar = 
-00010ab0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
-00010ac0: 2020 3e3e 3e20 6466 203d 2062 7064 2e44    >>> df = bpd.D
-00010ad0: 6174 6146 7261 6d65 287b 2769 6427 3a20  ataFrame({'id': 
-00010ae0: 5b31 2c20 322c 2033 5d2c 2027 6e61 6d65  [1, 2, 3], 'name
-00010af0: 273a 205b 2741 5552 c389 4c49 4527 2c20  ': ['AUR..LIE', 
-00010b00: 2743 c389 4c45 5354 494e 4527 2c20 2744  'C..LESTINE', 'D
-00010b10: 4150 484e c389 275d 7d29 0a20 2020 2020  APHN..']}).     
-00010b20: 2020 2020 2020 203e 3e3e 2064 660a 2020         >>> df.  
-00010b30: 2020 2020 2020 2020 2020 2020 2069 6420               id 
-00010b40: 2020 2020 2020 6e61 6d65 0a20 2020 2020        name.     
-00010b50: 2020 2020 2020 2030 2020 2031 2020 2020         0   1    
-00010b60: 4155 52c3 894c 4945 0a20 2020 2020 2020  AUR..LIE.       
-00010b70: 2020 2020 2031 2020 2032 2020 43c3 894c       1   2  C..L
-00010b80: 4553 5449 4e45 0a20 2020 2020 2020 2020  ESTINE.         
-00010b90: 2020 2032 2020 2033 2020 2020 2044 4150     2   3     DAP
-00010ba0: 484e c389 0a20 2020 2020 2020 2020 2020  HN...           
-00010bb0: 203c 424c 414e 4b4c 494e 453e 0a20 2020   <BLANKLINE>.   
-00010bc0: 2020 2020 2020 2020 205b 3320 726f 7773           [3 rows
-00010bd0: 2078 2032 2063 6f6c 756d 6e73 5d0a 0a20   x 2 columns].. 
-00010be0: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
-00010bf0: 756e 6320 3d20 6270 642e 7265 6164 5f67  unc = bpd.read_g
-00010c00: 6271 5f66 756e 6374 696f 6e28 2262 7175  bq_function("bqu
-00010c10: 7469 6c2e 666e 2e63 775f 6c6f 7765 725f  til.fn.cw_lower_
-00010c20: 6361 7365 5f61 7363 6969 5f6f 6e6c 7922  case_ascii_only"
-00010c30: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00010c40: 3e20 6466 3120 3d20 6466 2e61 7373 6967  > df1 = df.assig
-00010c50: 6e28 6e65 775f 6e61 6d65 3d64 665b 276e  n(new_name=df['n
-00010c60: 616d 6527 5d2e 6170 706c 7928 6675 6e63  ame'].apply(func
-00010c70: 2929 0a20 2020 2020 2020 2020 2020 203e  )).            >
-00010c80: 3e3e 2064 6631 0a20 2020 2020 2020 2020  >> df1.         
-00010c90: 2020 2020 2020 6964 2020 2020 2020 206e        id       n
-00010ca0: 616d 6520 2020 6e65 775f 6e61 6d65 0a20  ame   new_name. 
-00010cb0: 2020 2020 2020 2020 2020 2030 2020 2031             0   1
-00010cc0: 2020 2020 4155 52c3 894c 4945 2020 2020      AUR..LIE    
-00010cd0: 6175 72c3 896c 6965 0a20 2020 2020 2020  aur..lie.       
-00010ce0: 2020 2020 2031 2020 2032 2020 43c3 894c       1   2  C..L
-00010cf0: 4553 5449 4e45 2020 63c3 896c 6573 7469  ESTINE  c..lesti
-00010d00: 6e65 0a20 2020 2020 2020 2020 2020 2032  ne.            2
-00010d10: 2020 2033 2020 2020 2044 4150 484e c389     3     DAPHN..
-00010d20: 2020 2020 2064 6170 686e c389 0a20 2020       daphn...   
-00010d30: 2020 2020 2020 2020 203c 424c 414e 4b4c           <BLANKL
-00010d40: 494e 453e 0a20 2020 2020 2020 2020 2020  INE>.           
-00010d50: 205b 3320 726f 7773 2078 2033 2063 6f6c   [3 rows x 3 col
-00010d60: 756d 6e73 5d0a 0a20 2020 2020 2020 2041  umns]..        A
-00010d70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010d80: 2066 756e 6374 696f 6e5f 6e61 6d65 2028   function_name (
-00010d90: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00010da0: 2020 2020 2020 7468 6520 6675 6e63 7469        the functi
-00010db0: 6f6e 2773 206e 616d 6520 696e 2042 6967  on's name in Big
-00010dc0: 5175 6572 7920 696e 2074 6865 2066 6f72  Query in the for
-00010dd0: 6d61 740a 2020 2020 2020 2020 2020 2020  mat.            
-00010de0: 2020 2020 6070 726f 6a65 6374 5f69 642e      `project_id.
-00010df0: 6461 7461 7365 745f 6964 2e66 756e 6374  dataset_id.funct
-00010e00: 696f 6e5f 6e61 6d65 602c 206f 720a 2020  ion_name`, or.  
-00010e10: 2020 2020 2020 2020 2020 2020 2020 6064                `d
-00010e20: 6174 6173 6574 5f69 642e 6675 6e63 7469  ataset_id.functi
-00010e30: 6f6e 5f6e 616d 6560 2074 6f20 6c6f 6164  on_name` to load
-00010e40: 2066 726f 6d20 7468 6520 6465 6661 756c   from the defaul
-00010e50: 7420 7072 6f6a 6563 742c 206f 720a 2020  t project, or.  
-00010e60: 2020 2020 2020 2020 2020 2020 2020 6066                `f
-00010e70: 756e 6374 696f 6e5f 6e61 6d65 6020 746f  unction_name` to
-00010e80: 206c 6f61 6420 6672 6f6d 2074 6865 2064   load from the d
-00010e90: 6566 6175 6c74 2070 726f 6a65 6374 2061  efault project a
-00010ea0: 6e64 2074 6865 2064 6174 6173 6574 0a20  nd the dataset. 
-00010eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00010ec0: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
-00010ed0: 6865 2063 7572 7265 6e74 2073 6573 7369  he current sessi
-00010ee0: 6f6e 2e0a 0a20 2020 2020 2020 2052 6574  on...        Ret
-00010ef0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00010f00: 2020 6361 6c6c 6162 6c65 3a20 4120 6675    callable: A fu
-00010f10: 6e63 7469 6f6e 206f 626a 6563 7420 706f  nction object po
-00010f20: 696e 7469 6e67 2074 6f20 7468 6520 4269  inting to the Bi
-00010f30: 6751 7565 7279 2066 756e 6374 696f 6e20  gQuery function 
-00010f40: 7265 6164 0a20 2020 2020 2020 2020 2020  read.           
-00010f50: 2066 726f 6d20 4269 6751 7565 7279 2e0a   from BigQuery..
-00010f60: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00010f70: 206f 626a 6563 7420 6973 2073 696d 696c   object is simil
-00010f80: 6172 2074 6f20 7468 6520 6f6e 6520 6372  ar to the one cr
-00010f90: 6561 7465 6420 6279 2074 6865 2060 7265  eated by the `re
-00010fa0: 6d6f 7465 5f66 756e 6374 696f 6e60 0a20  mote_function`. 
-00010fb0: 2020 2020 2020 2020 2020 2064 6563 6f72             decor
-00010fc0: 6174 6f72 2c20 696e 636c 7564 696e 6720  ator, including 
-00010fd0: 7468 6520 6062 6967 6672 616d 6573 5f72  the `bigframes_r
-00010fe0: 656d 6f74 655f 6675 6e63 7469 6f6e 6020  emote_function` 
-00010ff0: 7072 6f70 6572 7479 2c20 6275 740a 2020  property, but.  
-00011000: 2020 2020 2020 2020 2020 6e6f 7420 696e            not in
-00011010: 636c 7564 696e 6720 7468 6520 6062 6967  cluding the `big
-00011020: 6672 616d 6573 5f63 6c6f 7564 5f66 756e  frames_cloud_fun
-00011030: 6374 696f 6e60 2070 726f 7065 7274 792e  ction` property.
-00011040: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00011050: 2020 2020 2020 7265 7475 726e 2062 6967        return big
-00011060: 6672 616d 6573 5f72 6766 280a 2020 2020  frames_rgf(.    
-00011070: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00011080: 5f6e 616d 653d 6675 6e63 7469 6f6e 5f6e  _name=function_n
-00011090: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000110a0: 2073 6573 7369 6f6e 3d73 656c 662c 0a20   session=self,. 
-000110b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-000110c0: 6620 5f70 7265 7061 7265 5f71 7565 7279  f _prepare_query
-000110d0: 5f6a 6f62 5f63 6f6e 6669 6728 0a20 2020  _job_config(.   
-000110e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000110f0: 2020 206a 6f62 5f63 6f6e 6669 673a 204f     job_config: O
-00011100: 7074 696f 6e61 6c5b 6269 6771 7565 7279  ptional[bigquery
-00011110: 2e51 7565 7279 4a6f 6243 6f6e 6669 675d  .QueryJobConfig]
-00011120: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
-00011130: 3e20 6269 6771 7565 7279 2e51 7565 7279  > bigquery.Query
-00011140: 4a6f 6243 6f6e 6669 673a 0a20 2020 2020  JobConfig:.     
-00011150: 2020 2069 6620 6a6f 625f 636f 6e66 6967     if job_config
-00011160: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00011170: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00011180: 203d 2062 6967 7175 6572 792e 5175 6572   = bigquery.Quer
-00011190: 794a 6f62 436f 6e66 6967 2829 0a20 2020  yJobConfig().   
-000111a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000111b0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-000111c0: 6120 636f 7079 2073 6f20 7468 6174 2077  a copy so that w
-000111d0: 6520 646f 6e27 7420 6d75 7461 7465 2074  e don't mutate t
-000111e0: 6865 206f 7269 6769 6e61 6c20 636f 6e66  he original conf
-000111f0: 6967 2070 6173 7365 640a 2020 2020 2020  ig passed.      
-00011200: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-00011210: 203d 2074 7970 696e 672e 6361 7374 280a   = typing.cast(.
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00011240: 6243 6f6e 6669 672c 0a20 2020 2020 2020  bConfig,.       
-00011250: 2020 2020 2020 2020 2062 6967 7175 6572           bigquer
-00011260: 792e 5175 6572 794a 6f62 436f 6e66 6967  y.QueryJobConfig
-00011270: 2e66 726f 6d5f 6170 695f 7265 7072 286a  .from_api_repr(j
-00011280: 6f62 5f63 6f6e 6669 672e 746f 5f61 7069  ob_config.to_api
-00011290: 5f72 6570 7228 2929 2c0a 2020 2020 2020  _repr()),.      
-000112a0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000112b0: 2069 6620 6269 6766 7261 6d65 732e 6f70   if bigframes.op
-000112c0: 7469 6f6e 732e 636f 6d70 7574 652e 6d61  tions.compute.ma
-000112d0: 7869 6d75 6d5f 6279 7465 735f 6269 6c6c  ximum_bytes_bill
-000112e0: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
-000112f0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-00011300: 636f 6e66 6967 2e6d 6178 696d 756d 5f62  config.maximum_b
-00011310: 7974 6573 5f62 696c 6c65 6420 3d20 280a  ytes_billed = (.
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 6269 6766 7261 6d65 732e 6f70 7469 6f6e  bigframes.option
-00011340: 732e 636f 6d70 7574 652e 6d61 7869 6d75  s.compute.maximu
-00011350: 6d5f 6279 7465 735f 6269 6c6c 6564 0a20  m_bytes_billed. 
-00011360: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00011370: 2020 2020 2020 6966 2073 656c 662e 5f62        if self._b
-00011380: 715f 6b6d 735f 6b65 795f 6e61 6d65 3a0a  q_kms_key_name:.
-00011390: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
-000113a0: 636f 6e66 6967 2e64 6573 7469 6e61 7469  config.destinati
-000113b0: 6f6e 5f65 6e63 7279 7074 696f 6e5f 636f  on_encryption_co
-000113c0: 6e66 6967 7572 6174 696f 6e20 3d20 280a  nfiguration = (.
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 6269 6771 7565 7279 2e45 6e63 7279 7074  bigquery.Encrypt
-000113f0: 696f 6e43 6f6e 6669 6775 7261 7469 6f6e  ionConfiguration
-00011400: 286b 6d73 5f6b 6579 5f6e 616d 653d 7365  (kms_key_name=se
-00011410: 6c66 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e  lf._bq_kms_key_n
-00011420: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00011430: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
-00011440: 726e 206a 6f62 5f63 6f6e 6669 670a 0a20  rn job_config.. 
-00011450: 2020 2064 6566 205f 7072 6570 6172 655f     def _prepare_
-00011460: 6c6f 6164 5f6a 6f62 5f63 6f6e 6669 6728  load_job_config(
-00011470: 7365 6c66 2920 2d3e 2062 6967 7175 6572  self) -> bigquer
-00011480: 792e 4c6f 6164 4a6f 6243 6f6e 6669 673a  y.LoadJobConfig:
-00011490: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-000114a0: 6520 6120 636f 7079 2073 6f20 7468 6174  e a copy so that
-000114b0: 2077 6520 646f 6e27 7420 6d75 7461 7465   we don't mutate
-000114c0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
-000114d0: 6e66 6967 2070 6173 7365 640a 2020 2020  nfig passed.    
-000114e0: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
-000114f0: 2062 6967 7175 6572 792e 4c6f 6164 4a6f   bigquery.LoadJo
-00011500: 6243 6f6e 6669 6728 290a 0a20 2020 2020  bConfig()..     
-00011510: 2020 2069 6620 7365 6c66 2e5f 6271 5f6b     if self._bq_k
-00011520: 6d73 5f6b 6579 5f6e 616d 653a 0a20 2020  ms_key_name:.   
-00011530: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
-00011540: 6669 672e 6465 7374 696e 6174 696f 6e5f  fig.destination_
-00011550: 656e 6372 7970 7469 6f6e 5f63 6f6e 6669  encryption_confi
-00011560: 6775 7261 7469 6f6e 203d 2028 0a20 2020  guration = (.   
-00011570: 2020 2020 2020 2020 2020 2020 2062 6967               big
-00011580: 7175 6572 792e 456e 6372 7970 7469 6f6e  query.Encryption
-00011590: 436f 6e66 6967 7572 6174 696f 6e28 6b6d  Configuration(km
-000115a0: 735f 6b65 795f 6e61 6d65 3d73 656c 662e  s_key_name=self.
-000115b0: 5f62 715f 6b6d 735f 6b65 795f 6e61 6d65  _bq_kms_key_name
-000115c0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-000115d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000115e0: 6a6f 625f 636f 6e66 6967 0a0a 2020 2020  job_config..    
-000115f0: 6465 6620 5f70 7265 7061 7265 5f63 6f70  def _prepare_cop
-00011600: 795f 6a6f 625f 636f 6e66 6967 2873 656c  y_job_config(sel
-00011610: 6629 202d 3e20 6269 6771 7565 7279 2e43  f) -> bigquery.C
-00011620: 6f70 794a 6f62 436f 6e66 6967 3a0a 2020  opyJobConfig:.  
-00011630: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-00011640: 2063 6f70 7920 736f 2074 6861 7420 7765   copy so that we
-00011650: 2064 6f6e 2774 206d 7574 6174 6520 7468   don't mutate th
-00011660: 6520 6f72 6967 696e 616c 2063 6f6e 6669  e original confi
-00011670: 6720 7061 7373 6564 0a20 2020 2020 2020  g passed.       
-00011680: 206a 6f62 5f63 6f6e 6669 6720 3d20 6269   job_config = bi
-00011690: 6771 7565 7279 2e43 6f70 794a 6f62 436f  gquery.CopyJobCo
-000116a0: 6e66 6967 2829 0a0a 2020 2020 2020 2020  nfig()..        
-000116b0: 6966 2073 656c 662e 5f62 715f 6b6d 735f  if self._bq_kms_
-000116c0: 6b65 795f 6e61 6d65 3a0a 2020 2020 2020  key_name:.      
-000116d0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
-000116e0: 2e64 6573 7469 6e61 7469 6f6e 5f65 6e63  .destination_enc
-000116f0: 7279 7074 696f 6e5f 636f 6e66 6967 7572  ryption_configur
-00011700: 6174 696f 6e20 3d20 280a 2020 2020 2020  ation = (.      
-00011710: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
-00011720: 7279 2e45 6e63 7279 7074 696f 6e43 6f6e  ry.EncryptionCon
-00011730: 6669 6775 7261 7469 6f6e 286b 6d73 5f6b  figuration(kms_k
-00011740: 6579 5f6e 616d 653d 7365 6c66 2e5f 6271  ey_name=self._bq
-00011750: 5f6b 6d73 5f6b 6579 5f6e 616d 6529 0a20  _kms_key_name). 
-00011760: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00011770: 2020 2020 2020 7265 7475 726e 206a 6f62        return job
-00011780: 5f63 6f6e 6669 670a 0a20 2020 2064 6566  _config..    def
-00011790: 205f 7374 6172 745f 7175 6572 7928 0a20   _start_query(. 
-000117a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000117b0: 2020 2020 2073 716c 3a20 7374 722c 0a20       sql: str,. 
-000117c0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
-000117d0: 673a 204f 7074 696f 6e61 6c5b 6269 6771  g: Optional[bigq
-000117e0: 7565 7279 2e6a 6f62 2e51 7565 7279 4a6f  uery.job.QueryJo
-000117f0: 6243 6f6e 6669 675d 203d 204e 6f6e 652c  bConfig] = None,
-00011800: 0a20 2020 2020 2020 206d 6178 5f72 6573  .        max_res
-00011810: 756c 7473 3a20 4f70 7469 6f6e 616c 5b69  ults: Optional[i
-00011820: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-00011830: 2020 2020 7469 6d65 6f75 743a 204f 7074      timeout: Opt
-00011840: 696f 6e61 6c5b 666c 6f61 745d 203d 204e  ional[float] = N
-00011850: 6f6e 652c 0a20 2020 2029 202d 3e20 5475  one,.    ) -> Tu
-00011860: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
-00011870: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
-00011880: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00011890: 625d 3a0a 2020 2020 2020 2020 2222 220a  b]:.        """.
-000118a0: 2020 2020 2020 2020 5374 6172 7473 2042          Starts B
-000118b0: 6967 5175 6572 7920 7175 6572 7920 6a6f  igQuery query jo
-000118c0: 6220 616e 6420 7761 6974 7320 666f 7220  b and waits for 
-000118d0: 7265 7375 6c74 732e 0a20 2020 2020 2020  results..       
-000118e0: 2022 2222 0a20 2020 2020 2020 206a 6f62   """.        job
-000118f0: 5f63 6f6e 6669 6720 3d20 7365 6c66 2e5f  _config = self._
-00011900: 7072 6570 6172 655f 7175 6572 795f 6a6f  prepare_query_jo
-00011910: 625f 636f 6e66 6967 286a 6f62 5f63 6f6e  b_config(job_con
-00011920: 6669 6729 0a20 2020 2020 2020 2072 6574  fig).        ret
-00011930: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
-00011940: 7373 696f 6e2e 5f69 6f2e 6269 6771 7565  ssion._io.bigque
-00011950: 7279 2e73 7461 7274 5f71 7565 7279 5f77  ry.start_query_w
-00011960: 6974 685f 636c 6965 6e74 280a 2020 2020  ith_client(.    
-00011970: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-00011980: 6c69 656e 742c 2073 716c 2c20 6a6f 625f  lient, sql, job_
-00011990: 636f 6e66 6967 2c20 6d61 785f 7265 7375  config, max_resu
-000119a0: 6c74 732c 2074 696d 656f 7574 0a20 2020  lts, timeout.   
-000119b0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-000119c0: 5f73 7461 7274 5f71 7565 7279 5f6d 6c5f  _start_query_ml_
-000119d0: 6464 6c28 0a20 2020 2020 2020 2073 656c  ddl(.        sel
-000119e0: 662c 0a20 2020 2020 2020 2073 716c 3a20  f,.        sql: 
-000119f0: 7374 722c 0a20 2020 2029 202d 3e20 5475  str,.    ) -> Tu
-00011a00: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
-00011a10: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
-00011a20: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-00011a30: 625d 3a0a 2020 2020 2020 2020 2222 220a  b]:.        """.
-00011a40: 2020 2020 2020 2020 5374 6172 7473 2042          Starts B
-00011a50: 6967 5175 6572 7920 4d4c 2044 444c 2071  igQuery ML DDL q
-00011a60: 7565 7279 206a 6f62 2028 4352 4541 5445  uery job (CREATE
-00011a70: 204d 4f44 454c 2f41 4c54 4552 204d 4f44   MODEL/ALTER MOD
-00011a80: 454c 2f2e 2e2e 2920 616e 640a 2020 2020  EL/...) and.    
-00011a90: 2020 2020 7761 6974 7320 666f 7220 7265      waits for re
-00011aa0: 7375 6c74 732e 0a20 2020 2020 2020 2022  sults..        "
-00011ab0: 2222 0a20 2020 2020 2020 206a 6f62 5f63  "".        job_c
-00011ac0: 6f6e 6669 6720 3d20 7365 6c66 2e5f 7072  onfig = self._pr
-00011ad0: 6570 6172 655f 7175 6572 795f 6a6f 625f  epare_query_job_
-00011ae0: 636f 6e66 6967 2829 0a0a 2020 2020 2020  config()..      
-00011af0: 2020 2320 4251 4d4c 2065 7870 6563 7473    # BQML expects
-00011b00: 206b 6d73 5f6b 6579 5f6e 616d 6520 7468   kms_key_name th
-00011b10: 726f 7567 6820 4f50 5449 4f4e 5320 616e  rough OPTIONS an
-00011b20: 6420 6e6f 7420 7468 726f 7567 6820 6a6f  d not through jo
-00011b30: 6220 636f 6e66 6967 2c0a 2020 2020 2020  b config,.      
-00011b40: 2020 2320 736f 2077 6520 6d75 7374 2072    # so we must r
-00011b50: 6573 6574 2061 6e79 2065 6e63 7279 7074  eset any encrypt
-00011b60: 696f 6e20 7365 7420 696e 2074 6865 206a  ion set in the j
-00011b70: 6f62 2063 6f6e 6669 670a 2020 2020 2020  ob config.      
-00011b80: 2020 2320 6874 7470 733a 2f2f 636c 6f75    # https://clou
-00011b90: 642e 676f 6f67 6c65 2e63 6f6d 2f62 6967  d.google.com/big
-00011ba0: 7175 6572 792f 646f 6373 2f63 7573 746f  query/docs/custo
-00011bb0: 6d65 722d 6d61 6e61 6765 642d 656e 6372  mer-managed-encr
-00011bc0: 7970 7469 6f6e 2365 6e63 7279 7074 2d6d  yption#encrypt-m
-00011bd0: 6f64 656c 0a20 2020 2020 2020 206a 6f62  odel.        job
-00011be0: 5f63 6f6e 6669 672e 6465 7374 696e 6174  _config.destinat
-00011bf0: 696f 6e5f 656e 6372 7970 7469 6f6e 5f63  ion_encryption_c
-00011c00: 6f6e 6669 6775 7261 7469 6f6e 203d 204e  onfiguration = N
-00011c10: 6f6e 650a 0a20 2020 2020 2020 2072 6574  one..        ret
-00011c20: 7572 6e20 6269 6766 7261 6d65 732e 7365  urn bigframes.se
-00011c30: 7373 696f 6e2e 5f69 6f2e 6269 6771 7565  ssion._io.bigque
-00011c40: 7279 2e73 7461 7274 5f71 7565 7279 5f77  ry.start_query_w
-00011c50: 6974 685f 636c 6965 6e74 280a 2020 2020  ith_client(.    
-00011c60: 2020 2020 2020 2020 7365 6c66 2e62 7163          self.bqc
-00011c70: 6c69 656e 742c 2073 716c 2c20 6a6f 625f  lient, sql, job_
-00011c80: 636f 6e66 6967 0a20 2020 2020 2020 2029  config.        )
-00011c90: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
-00011ca0: 5f77 6974 685f 636c 7573 7465 725f 636f  _with_cluster_co
-00011cb0: 6c73 280a 2020 2020 2020 2020 7365 6c66  ls(.        self
-00011cc0: 2c20 6172 7261 795f 7661 6c75 653a 2063  , array_value: c
-00011cd0: 6f72 652e 4172 7261 7956 616c 7565 2c20  ore.ArrayValue, 
-00011ce0: 636c 7573 7465 725f 636f 6c73 3a20 7479  cluster_cols: ty
-00011cf0: 7069 6e67 2e53 6571 7565 6e63 655b 7374  ping.Sequence[st
-00011d00: 725d 0a20 2020 2029 202d 3e20 636f 7265  r].    ) -> core
-00011d10: 2e41 7272 6179 5661 6c75 653a 0a20 2020  .ArrayValue:.   
-00011d20: 2020 2020 2022 2222 4578 6563 7574 6573       """Executes
-00011d30: 2074 6865 2071 7565 7279 2061 6e64 2075   the query and u
-00011d40: 7365 7320 7468 6520 7265 7375 6c74 696e  ses the resultin
-00011d50: 6720 7461 626c 6520 746f 2072 6577 7269  g table to rewri
-00011d60: 7465 2066 7574 7572 6520 6578 6563 7574  te future execut
-00011d70: 696f 6e73 2e22 2222 0a20 2020 2020 2020  ions.""".       
-00011d80: 2023 2054 4f44 4f3a 2055 7365 2074 6869   # TODO: Use thi
-00011d90: 7320 666f 7220 616c 6c20 6578 6563 7574  s for all execut
-00011da0: 696f 6e73 3f20 5072 6f62 6c65 6d20 6973  ions? Problem is
-00011db0: 2074 6861 7420 6361 6368 696e 6720 6d61   that caching ma
-00011dc0: 7465 7269 616c 697a 6573 2065 7874 7261  terializes extra
-00011dd0: 0a20 2020 2020 2020 2023 206f 7264 6572  .        # order
-00011de0: 696e 6720 636f 6c75 6d6e 730a 2020 2020  ing columns.    
-00011df0: 2020 2020 636f 6d70 696c 6564 5f76 616c      compiled_val
-00011e00: 7565 203d 2073 656c 662e 5f63 6f6d 7069  ue = self._compi
-00011e10: 6c65 5f6f 7264 6572 6564 2861 7272 6179  le_ordered(array
-00011e20: 5f76 616c 7565 290a 0a20 2020 2020 2020  _value)..       
-00011e30: 2069 6269 735f 6578 7072 203d 2063 6f6d   ibis_expr = com
-00011e40: 7069 6c65 645f 7661 6c75 652e 5f74 6f5f  piled_value._to_
-00011e50: 6962 6973 5f65 7870 7228 0a20 2020 2020  ibis_expr(.     
-00011e60: 2020 2020 2020 206f 7264 6572 696e 675f         ordering_
-00011e70: 6d6f 6465 3d22 756e 6f72 6465 7265 6422  mode="unordered"
-00011e80: 2c20 6578 706f 7365 5f68 6964 6465 6e5f  , expose_hidden_
-00011e90: 636f 6c73 3d54 7275 650a 2020 2020 2020  cols=True.      
-00011ea0: 2020 290a 2020 2020 2020 2020 746d 705f    ).        tmp_
-00011eb0: 7461 626c 6520 3d20 7365 6c66 2e5f 6962  table = self._ib
-00011ec0: 6973 5f74 6f5f 7465 6d70 5f74 6162 6c65  is_to_temp_table
-00011ed0: 280a 2020 2020 2020 2020 2020 2020 6962  (.            ib
-00011ee0: 6973 5f65 7870 722c 2063 6c75 7374 6572  is_expr, cluster
-00011ef0: 5f63 6f6c 733d 636c 7573 7465 725f 636f  _cols=cluster_co
-00011f00: 6c73 2c20 6170 695f 6e61 6d65 3d22 6361  ls, api_name="ca
-00011f10: 6368 6564 220a 2020 2020 2020 2020 290a  ched".        ).
-00011f20: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
-00011f30: 7072 6573 7369 6f6e 203d 2073 656c 662e  pression = self.
-00011f40: 6962 6973 5f63 6c69 656e 742e 7461 626c  ibis_client.tabl
-00011f50: 6528 0a20 2020 2020 2020 2020 2020 2074  e(.            t
-00011f60: 6d70 5f74 6162 6c65 2e74 6162 6c65 5f69  mp_table.table_i
-00011f70: 642c 0a20 2020 2020 2020 2020 2020 2073  d,.            s
-00011f80: 6368 656d 613d 746d 705f 7461 626c 652e  chema=tmp_table.
-00011f90: 6461 7461 7365 745f 6964 2c0a 2020 2020  dataset_id,.    
-00011fa0: 2020 2020 2020 2020 6461 7461 6261 7365          database
-00011fb0: 3d74 6d70 5f74 6162 6c65 2e70 726f 6a65  =tmp_table.proje
-00011fc0: 6374 2c0a 2020 2020 2020 2020 290a 2020  ct,.        ).  
-00011fd0: 2020 2020 2020 6e65 775f 636f 6c75 6d6e        new_column
-00011fe0: 7320 3d20 5b74 6162 6c65 5f65 7870 7265  s = [table_expre
-00011ff0: 7373 696f 6e5b 636f 6c75 6d6e 5d20 666f  ssion[column] fo
-00012000: 7220 636f 6c75 6d6e 2069 6e20 636f 6d70  r column in comp
-00012010: 696c 6564 5f76 616c 7565 2e63 6f6c 756d  iled_value.colum
-00012020: 6e5f 6964 735d 0a20 2020 2020 2020 206e  n_ids].        n
-00012030: 6577 5f68 6964 6465 6e5f 636f 6c75 6d6e  ew_hidden_column
-00012040: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-00012050: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
-00012060: 6f6e 5b63 6f6c 756d 6e5d 0a20 2020 2020  on[column].     
-00012070: 2020 2020 2020 2066 6f72 2063 6f6c 756d         for colum
-00012080: 6e20 696e 2063 6f6d 7069 6c65 645f 7661  n in compiled_va
-00012090: 6c75 652e 5f68 6964 6465 6e5f 6f72 6465  lue._hidden_orde
-000120a0: 7269 6e67 5f63 6f6c 756d 6e5f 6e61 6d65  ring_column_name
-000120b0: 730a 2020 2020 2020 2020 5d0a 2020 2020  s.        ].    
-000120c0: 2020 2020 2320 544f 444f 3a20 496e 7374      # TODO: Inst
-000120d0: 6561 642c 206b 6565 7020 7365 7373 696f  ead, keep sessio
-000120e0: 6e2d 7769 6465 206d 6170 206f 6620 6361  n-wide map of ca
-000120f0: 6368 6564 2072 6573 756c 7473 2061 6e64  ched results and
-00012100: 2061 7574 6f6d 6174 6963 616c 6c79 2072   automatically r
-00012110: 6575 7365 0a20 2020 2020 2020 2072 6574  euse.        ret
-00012120: 7572 6e20 636f 7265 2e41 7272 6179 5661  urn core.ArrayVa
-00012130: 6c75 652e 6672 6f6d 5f69 6269 7328 0a20  lue.from_ibis(. 
-00012140: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00012150: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00012160: 6c65 5f65 7870 7265 7373 696f 6e2c 0a20  le_expression,. 
-00012170: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00012180: 6e73 3d6e 6577 5f63 6f6c 756d 6e73 2c0a  ns=new_columns,.
-00012190: 2020 2020 2020 2020 2020 2020 6869 6464              hidd
-000121a0: 656e 5f6f 7264 6572 696e 675f 636f 6c75  en_ordering_colu
-000121b0: 6d6e 733d 6e65 775f 6869 6464 656e 5f63  mns=new_hidden_c
-000121c0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-000121d0: 2020 2020 6f72 6465 7269 6e67 3d63 6f6d      ordering=com
-000121e0: 7069 6c65 645f 7661 6c75 652e 5f6f 7264  piled_value._ord
-000121f0: 6572 696e 672c 0a20 2020 2020 2020 2029  ering,.        )
-00012200: 0a0a 2020 2020 6465 6620 5f63 6163 6865  ..    def _cache
-00012210: 5f77 6974 685f 6f66 6673 6574 7328 7365  _with_offsets(se
-00012220: 6c66 2c20 6172 7261 795f 7661 6c75 653a  lf, array_value:
-00012230: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
-00012240: 2920 2d3e 2063 6f72 652e 4172 7261 7956  ) -> core.ArrayV
-00012250: 616c 7565 3a0a 2020 2020 2020 2020 2222  alue:.        ""
-00012260: 2245 7865 6375 7465 7320 7468 6520 7175  "Executes the qu
-00012270: 6572 7920 616e 6420 7573 6573 2074 6865  ery and uses the
-00012280: 2072 6573 756c 7469 6e67 2074 6162 6c65   resulting table
-00012290: 2074 6f20 7265 7772 6974 6520 6675 7475   to rewrite futu
-000122a0: 7265 2065 7865 6375 7469 6f6e 732e 2222  re executions.""
-000122b0: 220a 2020 2020 2020 2020 2320 544f 444f  ".        # TODO
-000122c0: 3a20 5573 6520 7468 6973 2066 6f72 2061  : Use this for a
-000122d0: 6c6c 2065 7865 6375 7469 6f6e 733f 2050  ll executions? P
-000122e0: 726f 626c 656d 2069 7320 7468 6174 2063  roblem is that c
-000122f0: 6163 6869 6e67 206d 6174 6572 6961 6c69  aching materiali
-00012300: 7a65 7320 6578 7472 610a 2020 2020 2020  zes extra.      
-00012310: 2020 2320 6f72 6465 7269 6e67 2063 6f6c    # ordering col
-00012320: 756d 6e73 0a20 2020 2020 2020 2063 6f6d  umns.        com
-00012330: 7069 6c65 645f 7661 6c75 6520 3d20 7365  piled_value = se
-00012340: 6c66 2e5f 636f 6d70 696c 655f 6f72 6465  lf._compile_orde
-00012350: 7265 6428 6172 7261 795f 7661 6c75 6529  red(array_value)
-00012360: 0a0a 2020 2020 2020 2020 6962 6973 5f65  ..        ibis_e
-00012370: 7870 7220 3d20 636f 6d70 696c 6564 5f76  xpr = compiled_v
-00012380: 616c 7565 2e5f 746f 5f69 6269 735f 6578  alue._to_ibis_ex
-00012390: 7072 280a 2020 2020 2020 2020 2020 2020  pr(.            
-000123a0: 6f72 6465 7269 6e67 5f6d 6f64 653d 226f  ordering_mode="o
-000123b0: 6666 7365 745f 636f 6c22 2c20 6f72 6465  ffset_col", orde
-000123c0: 725f 636f 6c5f 6e61 6d65 3d22 6269 6766  r_col_name="bigf
-000123d0: 7261 6d65 735f 6f66 6673 6574 7322 0a20  rames_offsets". 
-000123e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000123f0: 2074 6d70 5f74 6162 6c65 203d 2073 656c   tmp_table = sel
-00012400: 662e 5f69 6269 735f 746f 5f74 656d 705f  f._ibis_to_temp_
-00012410: 7461 626c 6528 0a20 2020 2020 2020 2020  table(.         
-00012420: 2020 2069 6269 735f 6578 7072 2c20 636c     ibis_expr, cl
-00012430: 7573 7465 725f 636f 6c73 3d5b 2262 6967  uster_cols=["big
-00012440: 6672 616d 6573 5f6f 6666 7365 7473 225d  frames_offsets"]
-00012450: 2c20 6170 695f 6e61 6d65 3d22 6361 6368  , api_name="cach
-00012460: 6564 220a 2020 2020 2020 2020 290a 2020  ed".        ).  
-00012470: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
-00012480: 6573 7369 6f6e 203d 2073 656c 662e 6962  ession = self.ib
-00012490: 6973 5f63 6c69 656e 742e 7461 626c 6528  is_client.table(
-000124a0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-000124b0: 5f74 6162 6c65 2e74 6162 6c65 5f69 642c  _table.table_id,
-000124c0: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
-000124d0: 656d 613d 746d 705f 7461 626c 652e 6461  ema=tmp_table.da
-000124e0: 7461 7365 745f 6964 2c0a 2020 2020 2020  taset_id,.      
-000124f0: 2020 2020 2020 6461 7461 6261 7365 3d74        database=t
-00012500: 6d70 5f74 6162 6c65 2e70 726f 6a65 6374  mp_table.project
-00012510: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00012520: 2020 2020 6e65 775f 636f 6c75 6d6e 7320      new_columns 
-00012530: 3d20 5b74 6162 6c65 5f65 7870 7265 7373  = [table_express
-00012540: 696f 6e5b 636f 6c75 6d6e 5d20 666f 7220  ion[column] for 
-00012550: 636f 6c75 6d6e 2069 6e20 636f 6d70 696c  column in compil
-00012560: 6564 5f76 616c 7565 2e63 6f6c 756d 6e5f  ed_value.column_
-00012570: 6964 735d 0a20 2020 2020 2020 206e 6577  ids].        new
-00012580: 5f68 6964 6465 6e5f 636f 6c75 6d6e 7320  _hidden_columns 
-00012590: 3d20 5b74 6162 6c65 5f65 7870 7265 7373  = [table_express
-000125a0: 696f 6e5b 2262 6967 6672 616d 6573 5f6f  ion["bigframes_o
-000125b0: 6666 7365 7473 225d 5d0a 2020 2020 2020  ffsets"]].      
-000125c0: 2020 2320 544f 444f 3a20 496e 7374 6561    # TODO: Instea
-000125d0: 642c 206b 6565 7020 7365 7373 696f 6e2d  d, keep session-
-000125e0: 7769 6465 206d 6170 206f 6620 6361 6368  wide map of cach
-000125f0: 6564 2072 6573 756c 7473 2061 6e64 2061  ed results and a
-00012600: 7574 6f6d 6174 6963 616c 6c79 2072 6575  utomatically reu
-00012610: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
-00012620: 6e20 636f 7265 2e41 7272 6179 5661 6c75  n core.ArrayValu
-00012630: 652e 6672 6f6d 5f69 6269 7328 0a20 2020  e.from_ibis(.   
-00012640: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00012650: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-00012660: 5f65 7870 7265 7373 696f 6e2c 0a20 2020  _expression,.   
-00012670: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-00012680: 3d6e 6577 5f63 6f6c 756d 6e73 2c0a 2020  =new_columns,.  
-00012690: 2020 2020 2020 2020 2020 6869 6464 656e            hidden
-000126a0: 5f6f 7264 6572 696e 675f 636f 6c75 6d6e  _ordering_column
-000126b0: 733d 6e65 775f 6869 6464 656e 5f63 6f6c  s=new_hidden_col
-000126c0: 756d 6e73 2c0a 2020 2020 2020 2020 2020  umns,.          
-000126d0: 2020 6f72 6465 7269 6e67 3d6f 7264 6572    ordering=order
-000126e0: 2e45 7870 7265 7373 696f 6e4f 7264 6572  .ExpressionOrder
-000126f0: 696e 672e 6672 6f6d 5f6f 6666 7365 745f  ing.from_offset_
-00012700: 636f 6c28 2262 6967 6672 616d 6573 5f6f  col("bigframes_o
-00012710: 6666 7365 7473 2229 2c0a 2020 2020 2020  ffsets"),.      
-00012720: 2020 290a 0a20 2020 2064 6566 205f 7369    )..    def _si
-00012730: 6d70 6c69 6679 5f77 6974 685f 6361 6368  mplify_with_cach
-00012740: 696e 6728 7365 6c66 2c20 6172 7261 795f  ing(self, array_
-00012750: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
-00012760: 7956 616c 7565 2920 2d3e 2063 6f72 652e  yValue) -> core.
-00012770: 4172 7261 7956 616c 7565 3a0a 2020 2020  ArrayValue:.    
-00012780: 2020 2020 2222 2241 7474 656d 7074 7320      """Attempts 
-00012790: 746f 2068 616e 646c 6520 7468 6520 636f  to handle the co
-000127a0: 6d70 6c65 7869 7479 2062 7920 6361 6368  mplexity by cach
-000127b0: 696e 6720 6475 706c 6963 6174 6564 2073  ing duplicated s
-000127c0: 7562 7472 6565 7320 616e 6420 6272 6561  ubtrees and brea
-000127d0: 6b69 6e67 2074 6865 2071 7565 7279 2069  king the query i
-000127e0: 6e74 6f20 7069 6563 6573 2e22 2222 0a20  nto pieces.""". 
-000127f0: 2020 2020 2020 2069 6620 6e6f 7420 6269         if not bi
-00012800: 6766 7261 6d65 732e 6f70 7469 6f6e 732e  gframes.options.
-00012810: 636f 6d70 7574 652e 656e 6162 6c65 5f6d  compute.enable_m
-00012820: 756c 7469 5f71 7565 7279 5f65 7865 6375  ulti_query_execu
-00012830: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00012840: 2020 7265 7475 726e 2061 7272 6179 5f76    return array_v
-00012850: 616c 7565 0a20 2020 2020 2020 206e 6f64  alue.        nod
-00012860: 6520 3d20 6172 7261 795f 7661 6c75 652e  e = array_value.
-00012870: 6e6f 6465 0a20 2020 2020 2020 2069 6620  node.        if 
-00012880: 6e6f 6465 2e70 6c61 6e6e 696e 675f 636f  node.planning_co
-00012890: 6d70 6c65 7869 7479 203c 2051 5545 5259  mplexity < QUERY
-000128a0: 5f43 4f4d 504c 4558 4954 595f 4c49 4d49  _COMPLEXITY_LIMI
-000128b0: 543a 0a20 2020 2020 2020 2020 2020 2072  T:.            r
-000128c0: 6574 7572 6e20 6172 7261 795f 7661 6c75  eturn array_valu
-000128d0: 650a 0a20 2020 2020 2020 2066 6f72 205f  e..        for _
-000128e0: 2069 6e20 7261 6e67 6528 4d41 585f 5355   in range(MAX_SU
-000128f0: 4254 5245 455f 4641 4354 4f52 494e 4753  BTREE_FACTORINGS
-00012900: 293a 0a20 2020 2020 2020 2020 2020 2075  ):.            u
-00012910: 7064 6174 6564 203d 2073 656c 662e 5f63  pdated = self._c
-00012920: 6163 6865 5f6d 6f73 745f 636f 6d70 6c65  ache_most_comple
-00012930: 785f 7375 6274 7265 6528 6e6f 6465 290a  x_subtree(node).
-00012940: 2020 2020 2020 2020 2020 2020 6966 2075              if u
-00012950: 7064 6174 6564 2069 7320 4e6f 6e65 3a0a  pdated is None:.
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 7265 7475 726e 2063 6f72 652e 4172 7261  return core.Arra
-00012980: 7956 616c 7565 286e 6f64 6529 0a20 2020  yValue(node).   
-00012990: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000129a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000129b0: 6f64 6520 3d20 7570 6461 7465 640a 0a20  ode = updated.. 
-000129c0: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-000129d0: 7265 2e41 7272 6179 5661 6c75 6528 6e6f  re.ArrayValue(no
-000129e0: 6465 290a 0a20 2020 2064 6566 205f 6361  de)..    def _ca
-000129f0: 6368 655f 6d6f 7374 5f63 6f6d 706c 6578  che_most_complex
-00012a00: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
-00012a10: 2020 7365 6c66 2c20 6e6f 6465 3a20 6e6f    self, node: no
-00012a20: 6465 732e 4269 6746 7261 6d65 4e6f 6465  des.BigFrameNode
-00012a30: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
-00012a40: 616c 5b6e 6f64 6573 2e42 6967 4672 616d  al[nodes.BigFram
-00012a50: 654e 6f64 655d 3a0a 2020 2020 2020 2020  eNode]:.        
-00012a60: 2320 544f 444f 3a20 4966 2071 7565 7279  # TODO: If query
-00012a70: 2066 6169 6c73 2c20 7265 7472 7920 7769   fails, retry wi
-00012a80: 7468 206c 6f77 6572 2063 6f6d 706c 6578  th lower complex
-00012a90: 6974 7920 6c69 6d69 740a 2020 2020 2020  ity limit.      
-00012aa0: 2020 7661 6c69 645f 6361 6e64 6964 6174    valid_candidat
-00012ab0: 6573 203d 2074 7261 7665 7273 616c 732e  es = traversals.
-00012ac0: 636f 756e 745f 636f 6d70 6c65 785f 6e6f  count_complex_no
-00012ad0: 6465 7328 0a20 2020 2020 2020 2020 2020  des(.           
-00012ae0: 206e 6f64 652c 0a20 2020 2020 2020 2020   node,.         
-00012af0: 2020 206d 696e 5f63 6f6d 706c 6578 6974     min_complexit
-00012b00: 793d 2851 5545 5259 5f43 4f4d 504c 4558  y=(QUERY_COMPLEX
-00012b10: 4954 595f 4c49 4d49 5420 2f20 3530 3029  ITY_LIMIT / 500)
-00012b20: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-00012b30: 785f 636f 6d70 6c65 7869 7479 3d51 5545  x_complexity=QUE
-00012b40: 5259 5f43 4f4d 504c 4558 4954 595f 4c49  RY_COMPLEXITY_LI
-00012b50: 4d49 542c 0a20 2020 2020 2020 2029 2e69  MIT,.        ).i
-00012b60: 7465 6d73 2829 0a20 2020 2020 2020 2023  tems().        #
-00012b70: 2048 6575 7269 7374 6963 3a20 7375 6274   Heuristic: subt
-00012b80: 7265 655f 636f 6d70 6c65 6978 7479 202a  ree_compleixty *
-00012b90: 2028 636f 7069 6573 206f 6620 7375 6274   (copies of subt
-00012ba0: 7265 6529 5e32 0a20 2020 2020 2020 2062  ree)^2.        b
-00012bb0: 6573 745f 6361 6e64 6964 6174 6520 3d20  est_candidate = 
-00012bc0: 6d61 7828 0a20 2020 2020 2020 2020 2020  max(.           
-00012bd0: 2076 616c 6964 5f63 616e 6469 6461 7465   valid_candidate
-00012be0: 732c 0a20 2020 2020 2020 2020 2020 206b  s,.            k
-00012bf0: 6579 3d6c 616d 6264 6120 693a 2069 5b30  ey=lambda i: i[0
-00012c00: 5d2e 706c 616e 6e69 6e67 5f63 6f6d 706c  ].planning_compl
-00012c10: 6578 6974 7920 2b20 2869 5b31 5d20 2a2a  exity + (i[1] **
-00012c20: 2032 292c 0a20 2020 2020 2020 2020 2020   2),.           
-00012c30: 2064 6566 6175 6c74 3d4e 6f6e 652c 0a20   default=None,. 
-00012c40: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00012c50: 2020 6966 2062 6573 745f 6361 6e64 6964    if best_candid
-00012c60: 6174 6520 6973 204e 6f6e 653a 0a20 2020  ate is None:.   
-00012c70: 2020 2020 2020 2020 2023 204e 6f20 676f           # No go
-00012c80: 6f64 2073 7562 7472 6565 7320 746f 2063  od subtrees to c
-00012c90: 6163 6865 2c20 6a75 7374 2072 6574 7572  ache, just retur
-00012ca0: 6e20 6f72 6967 696e 616c 2074 7265 650a  n original tree.
-00012cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012cc0: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-00012cd0: 2023 2054 4f44 4f3a 2041 6464 2063 6c75   # TODO: Add clu
-00012ce0: 7374 6572 696e 6720 636f 6c75 6d6e 7320  stering columns 
-00012cf0: 6261 7365 6420 6f6e 2061 6363 6573 7320  based on access 
-00012d00: 7061 7474 6572 6e73 0a20 2020 2020 2020  patterns.       
-00012d10: 206d 6174 6572 6961 6c69 7a65 6420 3d20   materialized = 
-00012d20: 7365 6c66 2e5f 6361 6368 655f 7769 7468  self._cache_with
-00012d30: 5f63 6c75 7374 6572 5f63 6f6c 7328 0a20  _cluster_cols(. 
-00012d40: 2020 2020 2020 2020 2020 2063 6f72 652e             core.
-00012d50: 4172 7261 7956 616c 7565 2862 6573 745f  ArrayValue(best_
-00012d60: 6361 6e64 6964 6174 655b 305d 292c 205b  candidate[0]), [
-00012d70: 5d0a 2020 2020 2020 2020 292e 6e6f 6465  ].        ).node
-00012d80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00012d90: 2074 7261 7665 7273 616c 732e 7265 706c   traversals.repl
-00012da0: 6163 655f 6e6f 6465 7328 0a20 2020 2020  ace_nodes(.     
-00012db0: 2020 2020 2020 206e 6f64 652c 2074 6f5f         node, to_
-00012dc0: 7265 706c 6163 653d 6265 7374 5f63 616e  replace=best_can
-00012dd0: 6469 6461 7465 5b30 5d2c 2072 6570 6c61  didate[0], repla
-00012de0: 6365 6d65 6e65 743d 6d61 7465 7269 616c  cemenet=material
-00012df0: 697a 6564 0a20 2020 2020 2020 2029 0a0a  ized.        )..
-00012e00: 2020 2020 6465 6620 5f69 735f 7472 6976      def _is_triv
-00012e10: 6961 6c6c 795f 6578 6563 7574 6162 6c65  ially_executable
-00012e20: 2873 656c 662c 2061 7272 6179 5f76 616c  (self, array_val
-00012e30: 7565 3a20 636f 7265 2e41 7272 6179 5661  ue: core.ArrayVa
-00012e40: 6c75 6529 3a0a 2020 2020 2020 2020 2222  lue):.        ""
-00012e50: 220a 2020 2020 2020 2020 4361 6e20 7468  ".        Can th
-00012e60: 6520 626c 6f63 6b20 6265 2065 7661 6c75  e block be evalu
-00012e70: 6174 6564 2076 6572 7920 6368 6561 706c  ated very cheapl
-00012e80: 793f 0a20 2020 2020 2020 2049 6620 5472  y?.        If Tr
-00012e90: 7565 2c20 7468 6520 6172 7261 795f 7661  ue, the array_va
-00012ea0: 6c75 6520 7072 6f62 6162 6c79 2069 7320  lue probably is 
-00012eb0: 6e6f 7420 776f 7274 6820 6361 6368 696e  not worth cachin
-00012ec0: 672e 0a20 2020 2020 2020 2022 2222 0a20  g..        """. 
-00012ed0: 2020 2020 2020 2023 204f 6e63 6520 7265         # Once re
-00012ee0: 7772 6974 696e 6720 6973 2061 7661 696c  writing is avail
-00012ef0: 6162 6c65 2c20 7769 6c6c 2077 616e 7420  able, will want 
-00012f00: 746f 2072 6577 7269 7465 2062 6566 6f72  to rewrite befor
-00012f10: 650a 2020 2020 2020 2020 2320 6576 616c  e.        # eval
-00012f20: 7561 7469 6e67 2065 7865 6375 7469 6f6e  uating execution
-00012f30: 2063 6f73 742e 0a20 2020 2020 2020 2072   cost..        r
-00012f40: 6574 7572 6e20 7472 6176 6572 7361 6c73  eturn traversals
-00012f50: 2e69 735f 7472 6976 6961 6c6c 795f 6578  .is_trivially_ex
-00012f60: 6563 7574 6162 6c65 2861 7272 6179 5f76  ecutable(array_v
-00012f70: 616c 7565 2e6e 6f64 6529 0a0a 2020 2020  alue.node)..    
-00012f80: 6465 6620 5f65 7865 6375 7465 280a 2020  def _execute(.  
-00012f90: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00012fa0: 2020 2020 6172 7261 795f 7661 6c75 653a      array_value:
-00012fb0: 2063 6f72 652e 4172 7261 7956 616c 7565   core.ArrayValue
-00012fc0: 2c0a 2020 2020 2020 2020 6a6f 625f 636f  ,.        job_co
-00012fd0: 6e66 6967 3a20 4f70 7469 6f6e 616c 5b62  nfig: Optional[b
-00012fe0: 6967 7175 6572 792e 6a6f 622e 5175 6572  igquery.job.Quer
-00012ff0: 794a 6f62 436f 6e66 6967 5d20 3d20 4e6f  yJobConfig] = No
-00013000: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-00013010: 2020 2020 2020 2073 6f72 7465 643a 2062         sorted: b
-00013020: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-00013030: 2020 2020 6472 795f 7275 6e3d 4661 6c73      dry_run=Fals
-00013040: 652c 0a20 2020 2020 2020 2063 6f6c 5f69  e,.        col_i
-00013050: 645f 6f76 6572 7269 6465 733a 204d 6170  d_overrides: Map
-00013060: 7069 6e67 5b73 7472 2c20 7374 725d 203d  ping[str, str] =
-00013070: 207b 7d2c 0a20 2020 2029 202d 3e20 7475   {},.    ) -> tu
-00013080: 706c 655b 6269 6771 7565 7279 2e74 6162  ple[bigquery.tab
-00013090: 6c65 2e52 6f77 4974 6572 6174 6f72 2c20  le.RowIterator, 
-000130a0: 6269 6771 7565 7279 2e51 7565 7279 4a6f  bigquery.QueryJo
-000130b0: 625d 3a0a 2020 2020 2020 2020 7371 6c20  b]:.        sql 
-000130c0: 3d20 7365 6c66 2e5f 746f 5f73 716c 280a  = self._to_sql(.
-000130d0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
-000130e0: 795f 7661 6c75 652c 2073 6f72 7465 643d  y_value, sorted=
-000130f0: 736f 7274 6564 2c20 636f 6c5f 6964 5f6f  sorted, col_id_o
-00013100: 7665 7272 6964 6573 3d63 6f6c 5f69 645f  verrides=col_id_
-00013110: 6f76 6572 7269 6465 730a 2020 2020 2020  overrides.      
-00013120: 2020 2920 2023 2074 7970 653a 6967 6e6f    )  # type:igno
-00013130: 7265 0a20 2020 2020 2020 2069 6620 6a6f  re.        if jo
-00013140: 625f 636f 6e66 6967 2069 7320 4e6f 6e65  b_config is None
-00013150: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
-00013160: 625f 636f 6e66 6967 203d 2062 6967 7175  b_config = bigqu
-00013170: 6572 792e 5175 6572 794a 6f62 436f 6e66  ery.QueryJobConf
-00013180: 6967 2864 7279 5f72 756e 3d64 7279 5f72  ig(dry_run=dry_r
-00013190: 756e 290a 2020 2020 2020 2020 656c 7365  un).        else
-000131a0: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
-000131b0: 625f 636f 6e66 6967 2e64 7279 5f72 756e  b_config.dry_run
-000131c0: 203d 2064 7279 5f72 756e 0a20 2020 2020   = dry_run.     
-000131d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000131e0: 7374 6172 745f 7175 6572 7928 0a20 2020  start_query(.   
-000131f0: 2020 2020 2020 2020 2073 716c 3d73 716c           sql=sql
-00013200: 2c0a 2020 2020 2020 2020 2020 2020 6a6f  ,.            jo
-00013210: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
-00013220: 6669 672c 0a20 2020 2020 2020 2029 0a0a  fig,.        )..
-00013230: 2020 2020 6465 6620 5f70 6565 6b28 0a20      def _peek(. 
-00013240: 2020 2020 2020 2073 656c 662c 2061 7272         self, arr
-00013250: 6179 5f76 616c 7565 3a20 636f 7265 2e41  ay_value: core.A
-00013260: 7272 6179 5661 6c75 652c 206e 5f72 6f77  rrayValue, n_row
-00013270: 733a 2069 6e74 0a20 2020 2029 202d 3e20  s: int.    ) -> 
-00013280: 7475 706c 655b 6269 6771 7565 7279 2e74  tuple[bigquery.t
-00013290: 6162 6c65 2e52 6f77 4974 6572 6174 6f72  able.RowIterator
-000132a0: 2c20 6269 6771 7565 7279 2e51 7565 7279  , bigquery.Query
-000132b0: 4a6f 625d 3a0a 2020 2020 2020 2020 2222  Job]:.        ""
-000132c0: 2241 2027 7065 656b 2720 6566 6669 6369  "A 'peek' effici
-000132d0: 656e 746c 7920 6163 6365 7373 6573 2061  ently accesses a
-000132e0: 2073 6d61 6c6c 206e 756d 6265 7220 6f66   small number of
-000132f0: 2072 6f77 7320 696e 2074 6865 2064 6174   rows in the dat
-00013300: 6166 7261 6d65 2e22 2222 0a20 2020 2020  aframe.""".     
-00013310: 2020 2069 6620 6e6f 7420 7472 6565 5f70     if not tree_p
-00013320: 726f 7065 7274 6965 732e 7065 656b 6162  roperties.peekab
-00013330: 6c65 2861 7272 6179 5f76 616c 7565 2e6e  le(array_value.n
-00013340: 6f64 6529 3a0a 2020 2020 2020 2020 2020  ode):.          
-00013350: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00013360: 2250 6565 6b69 6e67 2074 6869 7320 7661  "Peeking this va
-00013370: 6c75 6520 6361 6e6e 6f74 2062 6520 646f  lue cannot be do
-00013380: 6e65 2065 6666 6963 6965 6e74 6c79 2e22  ne efficiently."
-00013390: 290a 2020 2020 2020 2020 7371 6c20 3d20  ).        sql = 
-000133a0: 7365 6c66 2e5f 636f 6d70 696c 655f 756e  self._compile_un
-000133b0: 6f72 6465 7265 6428 6172 7261 795f 7661  ordered(array_va
-000133c0: 6c75 6529 2e70 6565 6b5f 7371 6c28 6e5f  lue).peek_sql(n_
-000133d0: 726f 7773 290a 2020 2020 2020 2020 7265  rows).        re
-000133e0: 7475 726e 2073 656c 662e 5f73 7461 7274  turn self._start
-000133f0: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
-00013400: 2020 2020 7371 6c3d 7371 6c2c 0a20 2020      sql=sql,.   
-00013410: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00013420: 5f74 6f5f 7371 6c28 0a20 2020 2020 2020  _to_sql(.       
-00013430: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
-00013440: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
-00013450: 2e41 7272 6179 5661 6c75 652c 0a20 2020  .ArrayValue,.   
-00013460: 2020 2020 206f 6666 7365 745f 636f 6c75       offset_colu
-00013470: 6d6e 3a20 7479 7069 6e67 2e4f 7074 696f  mn: typing.Optio
-00013480: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00013490: 0a20 2020 2020 2020 2063 6f6c 5f69 645f  .        col_id_
-000134a0: 6f76 6572 7269 6465 733a 2074 7970 696e  overrides: typin
-000134b0: 672e 4d61 7070 696e 675b 7374 722c 2073  g.Mapping[str, s
-000134c0: 7472 5d20 3d20 7b7d 2c0a 2020 2020 2020  tr] = {},.      
-000134d0: 2020 736f 7274 6564 3a20 626f 6f6c 203d    sorted: bool =
-000134e0: 2046 616c 7365 2c0a 2020 2020 2920 2d3e   False,.    ) ->
-000134f0: 2073 7472 3a0a 2020 2020 2020 2020 6966   str:.        if
-00013500: 206f 6666 7365 745f 636f 6c75 6d6e 3a0a   offset_column:.
-00013510: 2020 2020 2020 2020 2020 2020 6172 7261              arra
-00013520: 795f 7661 6c75 6520 3d20 6172 7261 795f  y_value = array_
-00013530: 7661 6c75 652e 7072 6f6d 6f74 655f 6f66  value.promote_of
-00013540: 6673 6574 7328 6f66 6673 6574 5f63 6f6c  fsets(offset_col
-00013550: 756d 6e29 0a20 2020 2020 2020 2069 6620  umn).        if 
-00013560: 736f 7274 6564 3a0a 2020 2020 2020 2020  sorted:.        
-00013570: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00013580: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
-00013590: 2861 7272 6179 5f76 616c 7565 292e 746f  (array_value).to
-000135a0: 5f73 716c 280a 2020 2020 2020 2020 2020  _sql(.          
-000135b0: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
-000135c0: 7272 6964 6573 3d63 6f6c 5f69 645f 6f76  rrides=col_id_ov
-000135d0: 6572 7269 6465 732c 2073 6f72 7465 643d  errides, sorted=
-000135e0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-000135f0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00013600: 6e20 7365 6c66 2e5f 636f 6d70 696c 655f  n self._compile_
-00013610: 756e 6f72 6465 7265 6428 6172 7261 795f  unordered(array_
-00013620: 7661 6c75 6529 2e74 6f5f 7371 6c28 0a20  value).to_sql(. 
-00013630: 2020 2020 2020 2020 2020 2063 6f6c 5f69             col_i
-00013640: 645f 6f76 6572 7269 6465 733d 636f 6c5f  d_overrides=col_
-00013650: 6964 5f6f 7665 7272 6964 6573 0a20 2020  id_overrides.   
-00013660: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00013670: 5f63 6f6d 7069 6c65 5f6f 7264 6572 6564  _compile_ordered
-00013680: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00013690: 6172 7261 795f 7661 6c75 653a 2063 6f72  array_value: cor
-000136a0: 652e 4172 7261 7956 616c 7565 0a20 2020  e.ArrayValue.   
-000136b0: 2029 202d 3e20 6269 6766 7261 6d65 732e   ) -> bigframes.
-000136c0: 636f 7265 2e63 6f6d 7069 6c65 2e4f 7264  core.compile.Ord
-000136d0: 6572 6564 4952 3a0a 2020 2020 2020 2020  eredIR:.        
-000136e0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
-000136f0: 2e63 6f72 652e 636f 6d70 696c 652e 636f  .core.compile.co
-00013700: 6d70 696c 655f 6f72 6465 7265 645f 6972  mpile_ordered_ir
-00013710: 2861 7272 6179 5f76 616c 7565 2e6e 6f64  (array_value.nod
-00013720: 6529 0a0a 2020 2020 6465 6620 5f63 6f6d  e)..    def _com
-00013730: 7069 6c65 5f75 6e6f 7264 6572 6564 280a  pile_unordered(.
-00013740: 2020 2020 2020 2020 7365 6c66 2c20 6172          self, ar
-00013750: 7261 795f 7661 6c75 653a 2063 6f72 652e  ray_value: core.
-00013760: 4172 7261 7956 616c 7565 0a20 2020 2029  ArrayValue.    )
-00013770: 202d 3e20 6269 6766 7261 6d65 732e 636f   -> bigframes.co
-00013780: 7265 2e63 6f6d 7069 6c65 2e55 6e6f 7264  re.compile.Unord
-00013790: 6572 6564 4952 3a0a 2020 2020 2020 2020  eredIR:.        
-000137a0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
-000137b0: 2e63 6f72 652e 636f 6d70 696c 652e 636f  .core.compile.co
-000137c0: 6d70 696c 655f 756e 6f72 6465 7265 645f  mpile_unordered_
-000137d0: 6972 2861 7272 6179 5f76 616c 7565 2e6e  ir(array_value.n
-000137e0: 6f64 6529 0a0a 2020 2020 6465 6620 5f67  ode)..    def _g
-000137f0: 6574 5f74 6162 6c65 5f73 697a 6528 7365  et_table_size(se
-00013800: 6c66 2c20 6465 7374 696e 6174 696f 6e5f  lf, destination_
-00013810: 7461 626c 6529 3a0a 2020 2020 2020 2020  table):.        
-00013820: 7461 626c 6520 3d20 7365 6c66 2e62 7163  table = self.bqc
-00013830: 6c69 656e 742e 6765 745f 7461 626c 6528  lient.get_table(
-00013840: 6465 7374 696e 6174 696f 6e5f 7461 626c  destination_tabl
-00013850: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00013860: 6e20 7461 626c 652e 6e75 6d5f 6279 7465  n table.num_byte
-00013870: 730a 0a20 2020 2064 6566 205f 726f 7773  s..    def _rows
-00013880: 5f74 6f5f 6461 7461 6672 616d 6528 0a20  _to_dataframe(. 
-00013890: 2020 2020 2020 2073 656c 662c 2072 6f77         self, row
-000138a0: 5f69 7465 7261 746f 723a 2062 6967 7175  _iterator: bigqu
-000138b0: 6572 792e 7461 626c 652e 526f 7749 7465  ery.table.RowIte
-000138c0: 7261 746f 722c 2064 7479 7065 733a 2044  rator, dtypes: D
-000138d0: 6963 740a 2020 2020 2920 2d3e 2070 616e  ict.    ) -> pan
-000138e0: 6461 732e 4461 7461 4672 616d 653a 0a20  das.DataFrame:. 
-000138f0: 2020 2020 2020 2023 2043 616e 2069 676e         # Can ign
-00013900: 6f72 6520 696e 6665 7272 6564 2064 6174  ore inferred dat
-00013910: 6174 7970 6520 756e 7469 6c20 6474 7970  atype until dtyp
-00013920: 6520 656d 756c 6174 696f 6e20 6272 6561  e emulation brea
-00013930: 6b73 2031 3a31 206d 6170 7069 6e67 2062  ks 1:1 mapping b
-00013940: 6574 7765 656e 2042 5120 7479 7065 7320  etween BQ types 
-00013950: 616e 6420 6269 6766 7261 6d65 7320 7479  and bigframes ty
-00013960: 7065 730a 2020 2020 2020 2020 6474 7970  pes.        dtyp
-00013970: 6573 5f66 726f 6d5f 6271 203d 2062 6967  es_from_bq = big
-00013980: 6672 616d 6573 2e64 7479 7065 732e 6266  frames.dtypes.bf
-00013990: 5f74 7970 655f 6672 6f6d 5f74 7970 655f  _type_from_type_
-000139a0: 6b69 6e64 2872 6f77 5f69 7465 7261 746f  kind(row_iterato
-000139b0: 722e 7363 6865 6d61 290a 2020 2020 2020  r.schema).      
-000139c0: 2020 6172 726f 775f 7461 626c 6520 3d20    arrow_table = 
-000139d0: 726f 775f 6974 6572 6174 6f72 2e74 6f5f  row_iterator.to_
-000139e0: 6172 726f 7728 290a 2020 2020 2020 2020  arrow().        
-000139f0: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
-00013a00: 2e73 6573 7369 6f6e 2e5f 696f 2e70 616e  .session._io.pan
-00013a10: 6461 732e 6172 726f 775f 746f 5f70 616e  das.arrow_to_pan
-00013a20: 6461 7328 6172 726f 775f 7461 626c 652c  das(arrow_table,
-00013a30: 2064 7479 7065 735f 6672 6f6d 5f62 7129   dtypes_from_bq)
-00013a40: 0a0a 2020 2020 6465 6620 5f73 7461 7274  ..    def _start
-00013a50: 5f67 656e 6572 6963 5f6a 6f62 2873 656c  _generic_job(sel
-00013a60: 662c 206a 6f62 3a20 666f 726d 6174 7469  f, job: formatti
-00013a70: 6e67 5f68 656c 7065 7273 2e47 656e 6572  ng_helpers.Gener
-00013a80: 6963 4a6f 6229 3a0a 2020 2020 2020 2020  icJob):.        
-00013a90: 6966 2062 6967 6672 616d 6573 2e6f 7074  if bigframes.opt
-00013aa0: 696f 6e73 2e64 6973 706c 6179 2e70 726f  ions.display.pro
-00013ab0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00013ac0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013ad0: 2020 2066 6f72 6d61 7474 696e 675f 6865     formatting_he
-00013ae0: 6c70 6572 732e 7761 6974 5f66 6f72 5f6a  lpers.wait_for_j
-00013af0: 6f62 280a 2020 2020 2020 2020 2020 2020  ob(.            
-00013b00: 2020 2020 6a6f 622c 2062 6967 6672 616d      job, bigfram
-00013b10: 6573 2e6f 7074 696f 6e73 2e64 6973 706c  es.options.displ
-00013b20: 6179 2e70 726f 6772 6573 735f 6261 720a  ay.progress_bar.
-00013b30: 2020 2020 2020 2020 2020 2020 2920 2023              )  #
-00013b40: 2057 6169 7420 666f 7220 7468 6520 6a6f   Wait for the jo
-00013b50: 6220 746f 2063 6f6d 706c 6574 650a 2020  b to complete.  
-00013b60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013b70: 2020 2020 2020 2020 6a6f 622e 7265 7375          job.resu
-00013b80: 6c74 2829 0a0a 0a64 6566 2063 6f6e 6e65  lt()...def conne
-00013b90: 6374 2863 6f6e 7465 7874 3a20 4f70 7469  ct(context: Opti
-00013ba0: 6f6e 616c 5b62 6967 7175 6572 795f 6f70  onal[bigquery_op
-00013bb0: 7469 6f6e 732e 4269 6751 7565 7279 4f70  tions.BigQueryOp
-00013bc0: 7469 6f6e 735d 203d 204e 6f6e 6529 202d  tions] = None) -
-00013bd0: 3e20 5365 7373 696f 6e3a 0a20 2020 2072  > Session:.    r
-00013be0: 6574 7572 6e20 5365 7373 696f 6e28 636f  eturn Session(co
-00013bf0: 6e74 6578 7429 0a0a 0a64 6566 205f 6361  ntext)...def _ca
-00013c00: 6e5f 636c 7573 7465 725f 6271 2866 6965  n_cluster_bq(fie
-00013c10: 6c64 3a20 6269 6771 7565 7279 2e53 6368  ld: bigquery.Sch
-00013c20: 656d 6146 6965 6c64 293a 0a20 2020 2023  emaField):.    #
-00013c30: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
-00013c40: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
-00013c50: 7279 2f64 6f63 732f 636c 7573 7465 7265  ry/docs/clustere
-00013c60: 642d 7461 626c 6573 0a20 2020 2023 204e  d-tables.    # N
-00013c70: 6f74 6162 6c79 2c20 666c 6f61 7420 6973  otably, float is
-00013c80: 2065 7863 6c75 6465 640a 2020 2020 7479   excluded.    ty
-00013c90: 7065 5f20 3d20 6669 656c 642e 6669 656c  pe_ = field.fiel
-00013ca0: 645f 7479 7065 0a20 2020 2072 6574 7572  d_type.    retur
-00013cb0: 6e20 7479 7065 5f20 696e 2028 0a20 2020  n type_ in (.   
-00013cc0: 2020 2020 2022 494e 5445 4745 5222 2c0a       "INTEGER",.
-00013cd0: 2020 2020 2020 2020 2249 4e54 3634 222c          "INT64",
-00013ce0: 0a20 2020 2020 2020 2022 5354 5249 4e47  .        "STRING
-00013cf0: 222c 0a20 2020 2020 2020 2022 4e55 4d45  ",.        "NUME
-00013d00: 5249 4322 2c0a 2020 2020 2020 2020 2244  RIC",.        "D
-00013d10: 4543 494d 414c 222c 0a20 2020 2020 2020  ECIMAL",.       
-00013d20: 2022 4249 474e 554d 4552 4943 222c 0a20   "BIGNUMERIC",. 
-00013d30: 2020 2020 2020 2022 4249 4744 4543 494d         "BIGDECIM
-00013d40: 414c 222c 0a20 2020 2020 2020 2022 4441  AL",.        "DA
-00013d50: 5445 222c 0a20 2020 2020 2020 2022 4441  TE",.        "DA
-00013d60: 5445 5449 4d45 222c 0a20 2020 2020 2020  TETIME",.       
-00013d70: 2022 5449 4d45 5354 414d 5022 2c0a 2020   "TIMESTAMP",.  
-00013d80: 2020 2020 2020 2242 4f4f 4c22 2c0a 2020        "BOOL",.  
-00013d90: 2020 2020 2020 2242 4f4f 4c45 414e 222c        "BOOLEAN",
-00013da0: 0a20 2020 2029 0a0a 0a64 6566 205f 636f  .    )...def _co
-00013db0: 6e76 6572 745f 746f 5f6e 6f6e 6e75 6c6c  nvert_to_nonnull
-00013dc0: 5f73 7472 696e 6728 636f 6c75 6d6e 3a20  _string(column: 
-00013dd0: 6962 6973 5f74 7970 6573 2e43 6f6c 756d  ibis_types.Colum
-00013de0: 6e29 202d 3e20 6962 6973 5f74 7970 6573  n) -> ibis_types
-00013df0: 2e53 7472 696e 6756 616c 7565 3a0a 2020  .StringValue:.  
-00013e00: 2020 636f 6c5f 7479 7065 203d 2063 6f6c    col_type = col
-00013e10: 756d 6e2e 7479 7065 2829 0a20 2020 2069  umn.type().    i
-00013e20: 6620 280a 2020 2020 2020 2020 636f 6c5f  f (.        col_
-00013e30: 7479 7065 2e69 735f 6e75 6d65 7269 6328  type.is_numeric(
-00013e40: 290a 2020 2020 2020 2020 6f72 2063 6f6c  ).        or col
-00013e50: 5f74 7970 652e 6973 5f62 6f6f 6c65 616e  _type.is_boolean
-00013e60: 2829 0a20 2020 2020 2020 206f 7220 636f  ().        or co
-00013e70: 6c5f 7479 7065 2e69 735f 6269 6e61 7279  l_type.is_binary
-00013e80: 2829 0a20 2020 2020 2020 206f 7220 636f  ().        or co
-00013e90: 6c5f 7479 7065 2e69 735f 7465 6d70 6f72  l_type.is_tempor
-00013ea0: 616c 2829 0a20 2020 2029 3a0a 2020 2020  al().    ):.    
-00013eb0: 2020 2020 7265 7375 6c74 203d 2063 6f6c      result = col
-00013ec0: 756d 6e2e 6361 7374 2869 6269 735f 6474  umn.cast(ibis_dt
-00013ed0: 7970 6573 2e53 7472 696e 6728 6e75 6c6c  ypes.String(null
-00013ee0: 6162 6c65 3d54 7275 6529 290a 2020 2020  able=True)).    
-00013ef0: 656c 6966 2063 6f6c 5f74 7970 652e 6973  elif col_type.is
-00013f00: 5f67 656f 7370 6174 6961 6c28 293a 0a20  _geospatial():. 
-00013f10: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00013f20: 7479 7069 6e67 2e63 6173 7428 6962 6973  typing.cast(ibis
-00013f30: 5f74 7970 6573 2e47 656f 5370 6174 6961  _types.GeoSpatia
-00013f40: 6c43 6f6c 756d 6e2c 2063 6f6c 756d 6e29  lColumn, column)
-00013f50: 2e61 735f 7465 7874 2829 0a20 2020 2065  .as_text().    e
-00013f60: 6c69 6620 636f 6c5f 7479 7065 2e69 735f  lif col_type.is_
-00013f70: 7374 7269 6e67 2829 3a0a 2020 2020 2020  string():.      
-00013f80: 2020 7265 7375 6c74 203d 2063 6f6c 756d    result = colum
-00013f90: 6e0a 2020 2020 656c 7365 3a0a 2020 2020  n.    else:.    
-00013fa0: 2020 2020 2320 544f 5f4a 534f 4e5f 5354      # TO_JSON_ST
-00013fb0: 5249 4e47 2077 6f72 6b73 2077 6974 6820  RING works with 
-00013fc0: 616c 6c20 6461 7461 2074 7970 6573 2c20  all data types, 
-00013fd0: 6275 7420 6973 6e27 7420 7468 6520 6d6f  but isn't the mo
-00013fe0: 7374 2065 6666 6963 6965 6e74 0a20 2020  st efficient.   
-00013ff0: 2020 2020 2023 204e 6565 6465 6420 666f       # Needed fo
-00014000: 7220 4a53 4f4e 2c20 5354 5255 4354 2061  r JSON, STRUCT a
-00014010: 6e64 2041 5252 4159 2064 6174 6174 7970  nd ARRAY datatyp
-00014020: 6573 0a20 2020 2020 2020 2072 6573 756c  es.        resul
-00014030: 7420 3d20 7665 6e64 6f72 6564 5f69 6269  t = vendored_ibi
-00014040: 735f 6f70 732e 546f 4a73 6f6e 5374 7269  s_ops.ToJsonStri
-00014050: 6e67 2863 6f6c 756d 6e29 2e74 6f5f 6578  ng(column).to_ex
-00014060: 7072 2829 2020 2320 7479 7065 3a20 6967  pr()  # type: ig
-00014070: 6e6f 7265 0a20 2020 2023 2045 7363 6170  nore.    # Escap
-00014080: 6520 6261 636b 736c 6173 6865 7320 616e  e backslashes an
-00014090: 6420 7573 6520 6261 636b 736c 6173 6820  d use backslash 
-000140a0: 6173 2064 656c 696e 6561 746f 720a 2020  as delineator.  
-000140b0: 2020 6573 6361 7065 6420 3d20 7479 7069    escaped = typi
-000140c0: 6e67 2e63 6173 7428 6962 6973 5f74 7970  ng.cast(ibis_typ
-000140d0: 6573 2e53 7472 696e 6743 6f6c 756d 6e2c  es.StringColumn,
-000140e0: 2072 6573 756c 742e 6669 6c6c 6e61 2822   result.fillna("
-000140f0: 2229 292e 7265 706c 6163 6528 225c 5c22  ")).replace("\\"
-00014100: 2c20 225c 5c5c 5c22 2920 2023 2074 7970  , "\\\\")  # typ
-00014110: 653a 2069 676e 6f72 650a 2020 2020 7265  e: ignore.    re
-00014120: 7475 726e 2074 7970 696e 672e 6361 7374  turn typing.cast
-00014130: 2869 6269 735f 7479 7065 732e 5374 7269  (ibis_types.Stri
-00014140: 6e67 436f 6c75 6d6e 2c20 6962 6973 2e6c  ngColumn, ibis.l
-00014150: 6974 6572 616c 2822 5c5c 2229 292e 636f  iteral("\\")).co
-00014160: 6e63 6174 2865 7363 6170 6564 290a 0a0a  ncat(escaped)...
-00014170: 6465 6620 5f74 7261 6e73 666f 726d 5f72  def _transform_r
-00014180: 6561 645f 6762 715f 636f 6e66 6967 7572  ead_gbq_configur
-00014190: 6174 696f 6e28 636f 6e66 6967 7572 6174  ation(configurat
-000141a0: 696f 6e3a 204f 7074 696f 6e61 6c5b 6469  ion: Optional[di
-000141b0: 6374 5d29 202d 3e20 6469 6374 3a0a 2020  ct]) -> dict:.  
-000141c0: 2020 2222 220a 2020 2020 466f 7220 6261    """.    For ba
-000141d0: 636b 7761 7264 732d 636f 6d70 6174 6962  ckwards-compatib
-000141e0: 696c 6974 792c 2063 6f6e 7665 7274 2061  ility, convert a
-000141f0: 6e79 2070 7265 7669 6f75 736c 7920 636c  ny previously cl
-00014200: 6965 6e74 2d73 6964 6520 6f6e 6c79 0a20  ient-side only. 
-00014210: 2020 2070 6172 616d 6574 6572 7320 7375     parameters su
-00014220: 6368 2061 7320 7469 6d65 6f75 744d 7320  ch as timeoutMs 
-00014230: 746f 2074 6865 2070 726f 7065 7274 7920  to the property 
-00014240: 6e61 6d65 2065 7870 6563 7465 6420 6279  name expected by
-00014250: 2074 6865 2052 4553 5420 4150 492e 0a0a   the REST API...
-00014260: 2020 2020 4d61 6b65 7320 6120 636f 7079      Makes a copy
-00014270: 206f 6620 636f 6e66 6967 7572 6174 696f   of configuratio
-00014280: 6e20 6966 2063 6861 6e67 6573 2061 7265  n if changes are
-00014290: 206e 6565 6465 642e 0a20 2020 2022 2222   needed..    """
-000142a0: 0a0a 2020 2020 6966 2063 6f6e 6669 6775  ..    if configu
-000142b0: 7261 7469 6f6e 2069 7320 4e6f 6e65 3a0a  ration is None:.
-000142c0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-000142d0: 7d0a 0a20 2020 2074 696d 656f 7574 5f6d  }..    timeout_m
-000142e0: 7320 3d20 636f 6e66 6967 7572 6174 696f  s = configuratio
-000142f0: 6e2e 6765 7428 2271 7565 7279 222c 207b  n.get("query", {
-00014300: 7d29 2e67 6574 2822 7469 6d65 6f75 744d  }).get("timeoutM
-00014310: 7322 290a 2020 2020 6966 2074 696d 656f  s").    if timeo
-00014320: 7574 5f6d 7320 6973 206e 6f74 204e 6f6e  ut_ms is not Non
-00014330: 653a 0a20 2020 2020 2020 2023 2054 7261  e:.        # Tra
-00014340: 6e73 666f 726d 2074 696d 656f 7574 4d73  nsform timeoutMs
-00014350: 2074 6f20 616e 2061 6374 7561 6c20 7365   to an actual se
-00014360: 7276 6572 2d73 6964 6520 636f 6e66 6967  rver-side config
-00014370: 7572 6174 696f 6e2e 0a20 2020 2020 2020  uration..       
-00014380: 2023 2068 7474 7073 3a2f 2f67 6974 6875   # https://githu
-00014390: 622e 636f 6d2f 676f 6f67 6c65 6170 6973  b.com/googleapis
-000143a0: 2f70 7974 686f 6e2d 6269 6771 7565 7279  /python-bigquery
-000143b0: 2d70 616e 6461 732f 6973 7375 6573 2f34  -pandas/issues/4
-000143c0: 3739 0a20 2020 2020 2020 2063 6f6e 6669  79.        confi
-000143d0: 6775 7261 7469 6f6e 203d 2063 6f70 792e  guration = copy.
-000143e0: 6465 6570 636f 7079 2863 6f6e 6669 6775  deepcopy(configu
-000143f0: 7261 7469 6f6e 290a 2020 2020 2020 2020  ration).        
-00014400: 6465 6c20 636f 6e66 6967 7572 6174 696f  del configuratio
-00014410: 6e5b 2271 7565 7279 225d 5b22 7469 6d65  n["query"]["time
-00014420: 6f75 744d 7322 5d0a 2020 2020 2020 2020  outMs"].        
-00014430: 636f 6e66 6967 7572 6174 696f 6e5b 226a  configuration["j
-00014440: 6f62 5469 6d65 6f75 744d 7322 5d20 3d20  obTimeoutMs"] = 
-00014450: 7469 6d65 6f75 745f 6d73 0a0a 2020 2020  timeout_ms..    
-00014460: 7265 7475 726e 2063 6f6e 6669 6775 7261  return configura
-00014470: 7469 6f6e 0a                             tion.
+00002390: 6374 696f 6e63 6c69 656e 7428 7365 6c66  ctionclient(self
+000023a0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000023b0: 6e20 7365 6c66 2e5f 636c 6965 6e74 735f  n self._clients_
+000023c0: 7072 6f76 6964 6572 2e62 7163 6f6e 6e65  provider.bqconne
+000023d0: 6374 696f 6e63 6c69 656e 740a 0a20 2020  ctionclient..   
+000023e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+000023f0: 6566 2062 7173 746f 7261 6765 7265 6164  ef bqstorageread
+00002400: 636c 6965 6e74 2873 656c 6629 3a0a 2020  client(self):.  
+00002410: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002420: 662e 5f63 6c69 656e 7473 5f70 726f 7669  f._clients_provi
+00002430: 6465 722e 6271 7374 6f72 6167 6572 6561  der.bqstoragerea
+00002440: 6463 6c69 656e 740a 0a20 2020 2040 7072  dclient..    @pr
+00002450: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00002460: 6c6f 7564 6675 6e63 7469 6f6e 7363 6c69  loudfunctionscli
+00002470: 656e 7428 7365 6c66 293a 0a20 2020 2020  ent(self):.     
+00002480: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00002490: 636c 6965 6e74 735f 7072 6f76 6964 6572  clients_provider
+000024a0: 2e63 6c6f 7564 6675 6e63 7469 6f6e 7363  .cloudfunctionsc
+000024b0: 6c69 656e 740a 0a20 2020 2040 7072 6f70  lient..    @prop
+000024c0: 6572 7479 0a20 2020 2064 6566 2072 6573  erty.    def res
+000024d0: 6f75 7263 656d 616e 6167 6572 636c 6965  ourcemanagerclie
+000024e0: 6e74 2873 656c 6629 3a0a 2020 2020 2020  nt(self):.      
+000024f0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
+00002500: 6c69 656e 7473 5f70 726f 7669 6465 722e  lients_provider.
+00002510: 7265 736f 7572 6365 6d61 6e61 6765 7263  resourcemanagerc
+00002520: 6c69 656e 740a 0a20 2020 205f 6271 5f63  lient..    _bq_c
+00002530: 6f6e 6e65 6374 696f 6e5f 6d61 6e61 6765  onnection_manage
+00002540: 723a 204f 7074 696f 6e61 6c5b 6269 6766  r: Optional[bigf
+00002550: 7261 6d65 732e 636c 6965 6e74 732e 4271  rames.clients.Bq
+00002560: 436f 6e6e 6563 7469 6f6e 4d61 6e61 6765  ConnectionManage
+00002570: 725d 203d 204e 6f6e 650a 0a20 2020 2040  r] = None..    @
+00002580: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00002590: 2062 7163 6f6e 6e65 6374 696f 6e6d 616e   bqconnectionman
+000025a0: 6167 6572 2873 656c 6629 3a0a 2020 2020  ager(self):.    
+000025b0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+000025c0: 5f73 6b69 705f 6271 5f63 6f6e 6e65 6374  _skip_bq_connect
+000025d0: 696f 6e5f 6368 6563 6b20 616e 6420 6e6f  ion_check and no
+000025e0: 7420 7365 6c66 2e5f 6271 5f63 6f6e 6e65  t self._bq_conne
+000025f0: 6374 696f 6e5f 6d61 6e61 6765 723a 0a20  ction_manager:. 
+00002600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002610: 5f62 715f 636f 6e6e 6563 7469 6f6e 5f6d  _bq_connection_m
+00002620: 616e 6167 6572 203d 2062 6967 6672 616d  anager = bigfram
+00002630: 6573 2e63 6c69 656e 7473 2e42 7143 6f6e  es.clients.BqCon
+00002640: 6e65 6374 696f 6e4d 616e 6167 6572 280a  nectionManager(.
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 7365 6c66 2e62 7163 6f6e 6e65 6374 696f  self.bqconnectio
+00002670: 6e63 6c69 656e 742c 2073 656c 662e 7265  nclient, self.re
+00002680: 736f 7572 6365 6d61 6e61 6765 7263 6c69  sourcemanagercli
+00002690: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+000026a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000026b0: 2073 656c 662e 5f62 715f 636f 6e6e 6563   self._bq_connec
+000026c0: 7469 6f6e 5f6d 616e 6167 6572 0a0a 2020  tion_manager..  
+000026d0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000026e0: 6465 6620 7365 7373 696f 6e5f 6964 2873  def session_id(s
+000026f0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00002700: 7475 726e 2073 656c 662e 5f73 6573 7369  turn self._sessi
+00002710: 6f6e 5f69 640a 0a20 2020 2040 7072 6f70  on_id..    @prop
+00002720: 6572 7479 0a20 2020 2064 6566 205f 7072  erty.    def _pr
+00002730: 6f6a 6563 7428 7365 6c66 293a 0a20 2020  oject(self):.   
+00002740: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002750: 2e62 7163 6c69 656e 742e 7072 6f6a 6563  .bqclient.projec
+00002760: 740a 0a20 2020 2064 6566 205f 5f68 6173  t..    def __has
+00002770: 685f 5f28 7365 6c66 293a 0a20 2020 2020  h__(self):.     
+00002780: 2020 2023 2053 7461 626c 6520 6861 7368     # Stable hash
+00002790: 206e 6565 6465 6420 746f 2075 7365 2069   needed to use i
+000027a0: 6e20 6578 7072 6573 7369 6f6e 2074 7265  n expression tre
+000027b0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000027c0: 2068 6173 6828 7374 7228 7365 6c66 2e5f   hash(str(self._
+000027d0: 616e 6f6e 796d 6f75 735f 6461 7461 7365  anonymous_datase
+000027e0: 7429 290a 0a20 2020 2064 6566 2063 6c6f  t))..    def clo
+000027f0: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
+00002800: 2020 2222 2244 656c 6574 6520 7461 626c    """Delete tabl
+00002810: 6573 2074 6861 7420 7765 7265 2063 7265  es that were cre
+00002820: 6174 6564 2077 6974 6820 7468 6973 2073  ated with this s
+00002830: 6573 7369 6f6e 2773 2073 6573 7369 6f6e  ession's session
+00002840: 5f69 642e 2222 220a 2020 2020 2020 2020  _id.""".        
+00002850: 636c 6965 6e74 203d 2073 656c 662e 6271  client = self.bq
+00002860: 636c 6965 6e74 0a20 2020 2020 2020 2070  client.        p
+00002870: 726f 6a65 6374 5f69 6420 3d20 7365 6c66  roject_id = self
+00002880: 2e5f 616e 6f6e 796d 6f75 735f 6461 7461  ._anonymous_data
+00002890: 7365 742e 7072 6f6a 6563 740a 2020 2020  set.project.    
+000028a0: 2020 2020 6461 7461 7365 745f 6964 203d      dataset_id =
+000028b0: 2073 656c 662e 5f61 6e6f 6e79 6d6f 7573   self._anonymous
+000028c0: 5f64 6174 6173 6574 2e64 6174 6173 6574  _dataset.dataset
+000028d0: 5f69 640a 0a20 2020 2020 2020 2066 6f72  _id..        for
+000028e0: 2074 6162 6c65 5f69 6420 696e 2073 656c   table_id in sel
+000028f0: 662e 5f74 6162 6c65 5f69 6473 3a0a 2020  f._table_ids:.  
+00002900: 2020 2020 2020 2020 2020 6675 6c6c 5f69            full_i
+00002910: 6420 3d20 222e 222e 6a6f 696e 285b 7072  d = ".".join([pr
+00002920: 6f6a 6563 745f 6964 2c20 6461 7461 7365  oject_id, datase
+00002930: 745f 6964 2c20 7461 626c 655f 6964 5d29  t_id, table_id])
+00002940: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00002950: 656e 742e 6465 6c65 7465 5f74 6162 6c65  ent.delete_table
+00002960: 2866 756c 6c5f 6964 2c20 6e6f 745f 666f  (full_id, not_fo
+00002970: 756e 645f 6f6b 3d54 7275 6529 0a0a 2020  und_ok=True)..  
+00002980: 2020 6465 6620 7265 6164 5f67 6271 280a    def read_gbq(.
+00002990: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000029a0: 2020 2020 2020 7175 6572 795f 6f72 5f74        query_or_t
+000029b0: 6162 6c65 3a20 7374 722c 0a20 2020 2020  able: str,.     
+000029c0: 2020 202a 2c0a 2020 2020 2020 2020 696e     *,.        in
+000029d0: 6465 785f 636f 6c3a 2049 7465 7261 626c  dex_col: Iterabl
+000029e0: 655b 7374 725d 207c 2073 7472 207c 2062  e[str] | str | b
+000029f0: 6967 6672 616d 6573 2e65 6e75 6d73 2e44  igframes.enums.D
+00002a00: 6566 6175 6c74 496e 6465 784b 696e 6420  efaultIndexKind 
+00002a10: 3d20 2829 2c0a 2020 2020 2020 2020 636f  = (),.        co
+00002a20: 6c75 6d6e 733a 2049 7465 7261 626c 655b  lumns: Iterable[
+00002a30: 7374 725d 203d 2028 292c 0a20 2020 2020  str] = (),.     
+00002a40: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
+00002a50: 3a20 4f70 7469 6f6e 616c 5b44 6963 745d  : Optional[Dict]
+00002a60: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00002a70: 206d 6178 5f72 6573 756c 7473 3a20 4f70   max_results: Op
+00002a80: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00002a90: 6e65 2c0a 2020 2020 2020 2020 6669 6c74  ne,.        filt
+00002aa0: 6572 733a 2074 6869 7264 5f70 6172 7479  ers: third_party
+00002ab0: 5f70 616e 6461 735f 6762 712e 4669 6c74  _pandas_gbq.Filt
+00002ac0: 6572 7354 7970 6520 3d20 2829 2c0a 2020  ersType = (),.  
+00002ad0: 2020 2020 2020 7573 655f 6361 6368 653a        use_cache:
+00002ae0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+00002af0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00002b00: 636f 6c5f 6f72 6465 723a 2049 7465 7261  col_order: Itera
+00002b10: 626c 655b 7374 725d 203d 2028 292c 0a20  ble[str] = (),. 
+00002b20: 2020 2020 2020 2023 2041 6464 2061 2076         # Add a v
+00002b30: 6572 6966 7920 696e 6465 7820 6172 6775  erify index argu
+00002b40: 6d65 6e74 2074 6861 7420 6661 696c 7320  ment that fails 
+00002b50: 6966 2074 6865 2069 6e64 6578 2069 7320  if the index is 
+00002b60: 6e6f 7420 756e 6971 7565 2e0a 2020 2020  not unique..    
+00002b70: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
+00002b80: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+00002b90: 2020 2320 544f 444f 2862 2f32 3831 3537    # TODO(b/28157
+00002ba0: 3132 3134 293a 2047 656e 6572 6174 6520  1214): Generate 
+00002bb0: 7072 6f6d 7074 2074 6f20 7368 6f77 2074  prompt to show t
+00002bc0: 6865 2070 726f 6772 6573 7320 6f66 2072  he progress of r
+00002bd0: 6561 645f 6762 712e 0a20 2020 2020 2020  ead_gbq..       
+00002be0: 2069 6620 636f 6c75 6d6e 7320 616e 6420   if columns and 
+00002bf0: 636f 6c5f 6f72 6465 723a 0a20 2020 2020  col_order:.     
+00002c00: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00002c10: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+00002c20: 2020 2020 2020 2020 2022 4d75 7374 2073           "Must s
+00002c30: 7065 6369 6679 2065 6974 6865 7220 636f  pecify either co
+00002c40: 6c75 6d6e 7320 2870 7265 6665 7272 6564  lumns (preferred
+00002c50: 2920 6f72 2063 6f6c 5f6f 7264 6572 2c20  ) or col_order, 
+00002c60: 6e6f 7420 626f 7468 220a 2020 2020 2020  not both".      
+00002c70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002c80: 656c 6966 2063 6f6c 5f6f 7264 6572 3a0a  elif col_order:.
+00002c90: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00002ca0: 6d6e 7320 3d20 636f 6c5f 6f72 6465 720a  mns = col_order.
+00002cb0: 0a20 2020 2020 2020 2066 696c 7465 7273  .        filters
+00002cc0: 203d 206c 6973 7428 6669 6c74 6572 7329   = list(filters)
+00002cd0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00002ce0: 6669 6c74 6572 7329 2021 3d20 3020 6f72  filters) != 0 or
+00002cf0: 205f 6973 5f74 6162 6c65 5f77 6974 685f   _is_table_with_
+00002d00: 7769 6c64 6361 7264 5f73 7566 6669 7828  wildcard_suffix(
+00002d10: 7175 6572 795f 6f72 5f74 6162 6c65 293a  query_or_table):
+00002d20: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00002d30: 4f44 4f28 622f 3333 3831 3131 3334 3429  ODO(b/338111344)
+00002d40: 3a20 5468 6973 2061 7070 6561 7273 2074  : This appears t
+00002d50: 6f20 6265 206d 6973 7369 6e67 2069 6e64  o be missing ind
+00002d60: 6578 5f63 6f6c 732c 2077 6869 6368 0a20  ex_cols, which. 
+00002d70: 2020 2020 2020 2020 2020 2023 2061 7265             # are
+00002d80: 206e 6563 6573 7361 7279 2074 6f20 6265   necessary to be
+00002d90: 2073 656c 6563 7465 642e 0a20 2020 2020   selected..     
+00002da0: 2020 2020 2020 2023 2054 4f44 4f28 622f         # TODO(b/
+00002db0: 3333 3830 3339 3531 3729 3a20 416c 736f  338039517): Also
+00002dc0: 2c20 6e65 6564 2074 6f20 6163 636f 756e  , need to accoun
+00002dd0: 7420 666f 7220 7072 696d 6172 7920 6b65  t for primary ke
+00002de0: 7973 2e0a 2020 2020 2020 2020 2020 2020  ys..            
+00002df0: 7175 6572 795f 6f72 5f74 6162 6c65 203d  query_or_table =
+00002e00: 2073 656c 662e 5f74 6f5f 7175 6572 7928   self._to_query(
+00002e10: 7175 6572 795f 6f72 5f74 6162 6c65 2c20  query_or_table, 
+00002e20: 636f 6c75 6d6e 732c 2066 696c 7465 7273  columns, filters
+00002e30: 290a 0a20 2020 2020 2020 2069 6620 5f69  )..        if _i
+00002e40: 735f 7175 6572 7928 7175 6572 795f 6f72  s_query(query_or
+00002e50: 5f74 6162 6c65 293a 0a20 2020 2020 2020  _table):.       
+00002e60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002e70: 2e5f 7265 6164 5f67 6271 5f71 7565 7279  ._read_gbq_query
+00002e80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002e90: 2020 7175 6572 795f 6f72 5f74 6162 6c65    query_or_table
+00002ea0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002eb0: 2020 696e 6465 785f 636f 6c3d 696e 6465    index_col=inde
+00002ec0: 785f 636f 6c2c 0a20 2020 2020 2020 2020  x_col,.         
+00002ed0: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
+00002ee0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+00002ef0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00002f00: 6174 696f 6e3d 636f 6e66 6967 7572 6174  ation=configurat
+00002f10: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00002f20: 2020 2020 206d 6178 5f72 6573 756c 7473       max_results
+00002f30: 3d6d 6178 5f72 6573 756c 7473 2c0a 2020  =max_results,.  
+00002f40: 2020 2020 2020 2020 2020 2020 2020 6170                ap
+00002f50: 695f 6e61 6d65 3d22 7265 6164 5f67 6271  i_name="read_gbq
+00002f60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002f70: 2020 2075 7365 5f63 6163 6865 3d75 7365     use_cache=use
+00002f80: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
+00002f90: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00002fa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00002fb0: 6966 2063 6f6e 6669 6775 7261 7469 6f6e  if configuration
+00002fc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002fe0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003000: 2020 2020 2254 6865 2027 636f 6e66 6967      "The 'config
+00003010: 7572 6174 696f 6e27 2061 7267 756d 656e  uration' argumen
+00003020: 7420 6973 206e 6f74 2061 6c6c 6f77 6564  t is not allowed
+00003030: 2077 6865 6e20 220a 2020 2020 2020 2020   when ".        
+00003040: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
+00003050: 6563 746c 7920 7265 6164 696e 6720 6672  ectly reading fr
+00003060: 6f6d 2061 2074 6162 6c65 2e20 506c 6561  om a table. Plea
+00003070: 7365 2072 656d 6f76 6520 220a 2020 2020  se remove ".    
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2227 636f 6e66 6967 7572 6174 696f 6e27  "'configuration'
+000030a0: 206f 7220 7573 6520 6120 7175 6572 792e   or use a query.
+000030b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000030c0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+000030d0: 2072 6574 7572 6e20 7365 6c66 2e5f 7265   return self._re
+000030e0: 6164 5f67 6271 5f74 6162 6c65 280a 2020  ad_gbq_table(.  
+000030f0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+00003100: 6572 795f 6f72 5f74 6162 6c65 2c0a 2020  ery_or_table,.  
+00003110: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003120: 6465 785f 636f 6c3d 696e 6465 785f 636f  dex_col=index_co
+00003130: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00003140: 2020 2063 6f6c 756d 6e73 3d63 6f6c 756d     columns=colum
+00003150: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00003160: 2020 2020 6d61 785f 7265 7375 6c74 733d      max_results=
+00003170: 6d61 785f 7265 7375 6c74 732c 0a20 2020  max_results,.   
+00003180: 2020 2020 2020 2020 2020 2020 2061 7069               api
+00003190: 5f6e 616d 653d 2272 6561 645f 6762 7122  _name="read_gbq"
+000031a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000031b0: 2020 7573 655f 6361 6368 653d 7573 655f    use_cache=use_
+000031c0: 6361 6368 6520 6966 2075 7365 5f63 6163  cache if use_cac
+000031d0: 6865 2069 7320 6e6f 7420 4e6f 6e65 2065  he is not None e
+000031e0: 6c73 6520 5472 7565 2c0a 2020 2020 2020  lse True,.      
+000031f0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00003200: 205f 746f 5f71 7565 7279 280a 2020 2020   _to_query(.    
+00003210: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00003220: 2020 7175 6572 795f 6f72 5f74 6162 6c65    query_or_table
+00003230: 3a20 7374 722c 0a20 2020 2020 2020 2063  : str,.        c
+00003240: 6f6c 756d 6e73 3a20 4974 6572 6162 6c65  olumns: Iterable
+00003250: 5b73 7472 5d2c 0a20 2020 2020 2020 2066  [str],.        f
+00003260: 696c 7465 7273 3a20 7468 6972 645f 7061  ilters: third_pa
+00003270: 7274 795f 7061 6e64 6173 5f67 6271 2e46  rty_pandas_gbq.F
+00003280: 696c 7465 7273 5479 7065 2c0a 2020 2020  iltersType,.    
+00003290: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+000032a0: 2020 2222 2243 6f6d 7069 6c65 2071 7565    """Compile que
+000032b0: 7279 5f6f 725f 7461 626c 6520 7769 7468  ry_or_table with
+000032c0: 2063 6f6e 6469 7469 6f6e 7328 6669 6c74   conditions(filt
+000032d0: 6572 732c 2077 696c 6463 6172 6473 2920  ers, wildcards) 
+000032e0: 746f 2071 7565 7279 2e22 2222 0a20 2020  to query.""".   
+000032f0: 2020 2020 2066 696c 7465 7273 203d 206c       filters = l
+00003300: 6973 7428 6669 6c74 6572 7329 0a20 2020  ist(filters).   
+00003310: 2020 2020 2073 7562 5f71 7565 7279 203d       sub_query =
+00003320: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+00003330: 2228 7b71 7565 7279 5f6f 725f 7461 626c  "({query_or_tabl
+00003340: 657d 2922 0a20 2020 2020 2020 2020 2020  e})".           
+00003350: 2069 6620 5f69 735f 7175 6572 7928 7175   if _is_query(qu
+00003360: 6572 795f 6f72 5f74 6162 6c65 290a 2020  ery_or_table).  
+00003370: 2020 2020 2020 2020 2020 656c 7365 2066            else f
+00003380: 2260 7b71 7565 7279 5f6f 725f 7461 626c  "`{query_or_tabl
+00003390: 657d 6022 0a20 2020 2020 2020 2029 0a0a  e}`".        )..
+000033a0: 2020 2020 2020 2020 2320 544f 444f 2862          # TODO(b
+000033b0: 2f33 3338 3131 3133 3434 293a 2047 656e  /338111344): Gen
+000033c0: 6572 6174 6520 616e 2069 6e64 6578 2062  erate an index b
+000033d0: 6173 6564 206f 6e20 4465 6661 756c 7449  ased on DefaultI
+000033e0: 6e64 6578 4b69 6e64 2069 6620 7765 0a20  ndexKind if we. 
+000033f0: 2020 2020 2020 2023 2064 6f6e 2774 2068         # don't h
+00003400: 6176 6520 696e 6465 7820 636f 6c75 6d6e  ave index column
+00003410: 7320 7370 6563 6966 6965 642e 0a20 2020  s specified..   
+00003420: 2020 2020 2073 656c 6563 745f 636c 6175       select_clau
+00003430: 7365 203d 2022 5345 4c45 4354 2022 202b  se = "SELECT " +
+00003440: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+00003450: 2c20 222e 6a6f 696e 2866 2260 7b63 6f6c  , ".join(f"`{col
+00003460: 756d 6e7d 6022 2066 6f72 2063 6f6c 756d  umn}`" for colum
+00003470: 6e20 696e 2063 6f6c 756d 6e73 2920 6966  n in columns) if
+00003480: 2063 6f6c 756d 6e73 2065 6c73 6520 222a   columns else "*
+00003490: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
+000034a0: 2020 2020 2077 6865 7265 5f63 6c61 7573       where_claus
+000034b0: 6520 3d20 2222 0a20 2020 2020 2020 2069  e = "".        i
+000034c0: 6620 6669 6c74 6572 733a 0a20 2020 2020  f filters:.     
+000034d0: 2020 2020 2020 2076 616c 6964 5f6f 7065         valid_ope
+000034e0: 7261 746f 7273 3a20 4d61 7070 696e 675b  rators: Mapping[
+000034f0: 7468 6972 645f 7061 7274 795f 7061 6e64  third_party_pand
+00003500: 6173 5f67 6271 2e46 696c 7465 724f 7073  as_gbq.FilterOps
+00003510: 2c20 7374 725d 203d 207b 0a20 2020 2020  , str] = {.     
+00003520: 2020 2020 2020 2020 2020 2022 696e 223a             "in":
+00003530: 2022 494e 222c 0a20 2020 2020 2020 2020   "IN",.         
+00003540: 2020 2020 2020 2022 6e6f 7420 696e 223a         "not in":
+00003550: 2022 4e4f 5420 494e 222c 0a20 2020 2020   "NOT IN",.     
+00003560: 2020 2020 2020 2020 2020 2022 4c49 4b45             "LIKE
+00003570: 223a 2022 4c49 4b45 222c 0a20 2020 2020  ": "LIKE",.     
+00003580: 2020 2020 2020 2020 2020 2022 3d3d 223a             "==":
+00003590: 2022 3d22 2c0a 2020 2020 2020 2020 2020   "=",.          
+000035a0: 2020 2020 2020 223e 223a 2022 3e22 2c0a        ">": ">",.
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035c0: 223c 223a 2022 3c22 2c0a 2020 2020 2020  "<": "<",.      
+000035d0: 2020 2020 2020 2020 2020 223e 3d22 3a20            ">=": 
+000035e0: 223e 3d22 2c0a 2020 2020 2020 2020 2020  ">=",.          
+000035f0: 2020 2020 2020 223c 3d22 3a20 223c 3d22        "<=": "<="
+00003600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003610: 2020 2221 3d22 3a20 2221 3d22 2c0a 2020    "!=": "!=",.  
+00003620: 2020 2020 2020 2020 2020 7d0a 0a20 2020            }..   
+00003630: 2020 2020 2020 2020 2023 2049 6620 7369           # If si
+00003640: 6e67 6c65 206c 6179 6572 2066 696c 7465  ngle layer filte
+00003650: 722c 2061 6464 2061 6e6f 7468 6572 2070  r, add another p
+00003660: 7365 7564 6f20 6c61 7965 722e 2053 6f20  seudo layer. So 
+00003670: 7468 6520 7369 6e67 6c65 206c 6179 6572  the single layer
+00003680: 2072 6570 7265 7365 6e74 7320 2261 6e64   represents "and
+00003690: 2220 6c6f 6769 632e 0a20 2020 2020 2020  " logic..       
+000036a0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000036b0: 6365 2866 696c 7465 7273 5b30 5d2c 2074  ce(filters[0], t
+000036c0: 7570 6c65 2920 616e 6420 280a 2020 2020  uple) and (.    
+000036d0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+000036e0: 6669 6c74 6572 735b 305d 2920 3d3d 2030  filters[0]) == 0
+000036f0: 206f 7220 6e6f 7420 6973 696e 7374 616e   or not isinstan
+00003700: 6365 286c 6973 7428 6669 6c74 6572 735b  ce(list(filters[
+00003710: 305d 295b 305d 2c20 7475 706c 6529 0a20  0])[0], tuple). 
+00003720: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+00003730: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00003740: 6c74 6572 7320 3d20 7479 7069 6e67 2e63  lters = typing.c
+00003750: 6173 7428 7468 6972 645f 7061 7274 795f  ast(third_party_
+00003760: 7061 6e64 6173 5f67 6271 2e46 696c 7465  pandas_gbq.Filte
+00003770: 7273 5479 7065 2c20 5b66 696c 7465 7273  rsType, [filters
+00003780: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+00003790: 6f72 5f65 7870 7265 7373 696f 6e73 203d  or_expressions =
+000037a0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+000037b0: 666f 7220 6772 6f75 7020 696e 2066 696c  for group in fil
+000037c0: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+000037d0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+000037e0: 6e73 7461 6e63 6528 6772 6f75 702c 2049  nstance(group, I
+000037f0: 7465 7261 626c 6529 3a0a 2020 2020 2020  terable):.      
+00003800: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+00003810: 6f75 7020 3d20 5b67 726f 7570 5d0a 0a20  oup = [group].. 
+00003820: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003830: 6e64 5f65 7870 7265 7373 696f 6e73 203d  nd_expressions =
+00003840: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+00003850: 2020 2020 666f 7220 6669 6c74 6572 5f69      for filter_i
+00003860: 7465 6d20 696e 2067 726f 7570 3a0a 2020  tem in group:.  
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00003890: 6e63 6528 6669 6c74 6572 5f69 7465 6d2c  nce(filter_item,
+000038a0: 2074 7570 6c65 2920 6f72 2028 6c65 6e28   tuple) or (len(
+000038b0: 6669 6c74 6572 5f69 7465 6d29 2021 3d20  filter_item) != 
+000038c0: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
+000038d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000038e0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2020 2020 2020 6622 4669 6c74            f"Filt
+00003910: 6572 2063 6f6e 6469 7469 6f6e 2073 686f  er condition sho
+00003920: 756c 6420 6265 2061 2074 7570 6c65 206f  uld be a tuple o
+00003930: 6620 6c65 6e67 7468 2033 2c20 7b66 696c  f length 3, {fil
+00003940: 7465 725f 6974 656d 7d20 6973 206e 6f74  ter_item} is not
+00003950: 2076 616c 6964 2e22 0a20 2020 2020 2020   valid.".       
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00003980: 2020 2020 2020 2020 636f 6c75 6d6e 2c20          column, 
+00003990: 6f70 6572 6174 6f72 2c20 7661 6c75 6520  operator, value 
+000039a0: 3d20 6669 6c74 6572 5f69 7465 6d0a 0a20  = filter_item.. 
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039c0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+000039d0: 616e 6365 2863 6f6c 756d 6e2c 2073 7472  ance(column, str
+000039e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000039f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00003a00: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2020 2020 2020 2066 2243 6f6c 756d           f"Colum
+00003a30: 6e20 6e61 6d65 2073 686f 756c 6420 6265  n name should be
+00003a40: 2061 2073 7472 696e 672c 2062 7574 2072   a string, but r
+00003a50: 6563 6569 7665 6420 277b 636f 6c75 6d6e  eceived '{column
+00003a60: 7d27 206f 6620 7479 7065 207b 7479 7065  }' of type {type
+00003a70: 2863 6f6c 756d 6e29 2e5f 5f6e 616d 655f  (column).__name_
+00003a80: 5f7d 2e22 0a20 2020 2020 2020 2020 2020  _}.".           
+00003a90: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 2020 2020 6966 206f 7065 7261 746f 7220      if operator 
+00003ac0: 6e6f 7420 696e 2076 616c 6964 5f6f 7065  not in valid_ope
+00003ad0: 7261 746f 7273 3a0a 2020 2020 2020 2020  rators:.        
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00003b00: 2866 224f 7065 7261 746f 7220 7b6f 7065  (f"Operator {ope
+00003b10: 7261 746f 727d 2069 7320 6e6f 7420 7661  rator} is not va
+00003b20: 6c69 642e 2229 0a0a 2020 2020 2020 2020  lid.")..        
+00003b30: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
+00003b40: 6174 6f72 5f73 7472 203d 2076 616c 6964  ator_str = valid
+00003b50: 5f6f 7065 7261 746f 7273 5b6f 7065 7261  _operators[opera
+00003b60: 746f 725d 0a0a 2020 2020 2020 2020 2020  tor]..          
+00003b70: 2020 2020 2020 2020 2020 6966 206f 7065            if ope
+00003b80: 7261 746f 725f 7374 7220 696e 205b 2249  rator_str in ["I
+00003b90: 4e22 2c20 224e 4f54 2049 4e22 5d3a 0a20  N", "NOT IN"]:. 
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 2020 2020 2020 2076 616c 7565 5f6c 6973         value_lis
+00003bc0: 7420 3d20 222c 2022 2e6a 6f69 6e28 5b72  t = ", ".join([r
+00003bd0: 6570 7228 7629 2066 6f72 2076 2069 6e20  epr(v) for v in 
+00003be0: 7661 6c75 655d 290a 2020 2020 2020 2020  value]).        
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 6578 7072 6573 7369 6f6e 203d 2066 2260  expression = f"`
+00003c10: 7b63 6f6c 756d 6e7d 6020 7b6f 7065 7261  {column}` {opera
+00003c20: 746f 725f 7374 727d 2028 7b76 616c 7565  tor_str} ({value
+00003c30: 5f6c 6973 747d 2922 0a20 2020 2020 2020  _list})".       
+00003c40: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00003c50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00003c60: 2020 2020 2020 2020 2020 2065 7870 7265             expre
+00003c70: 7373 696f 6e20 3d20 6622 607b 636f 6c75  ssion = f"`{colu
+00003c80: 6d6e 7d60 207b 6f70 6572 6174 6f72 5f73  mn}` {operator_s
+00003c90: 7472 7d20 7b72 6570 7228 7661 6c75 6529  tr} {repr(value)
+00003ca0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00003cb0: 2020 2020 2020 2061 6e64 5f65 7870 7265         and_expre
+00003cc0: 7373 696f 6e73 2e61 7070 656e 6428 6578  ssions.append(ex
+00003cd0: 7072 6573 7369 6f6e 290a 0a20 2020 2020  pression)..     
+00003ce0: 2020 2020 2020 2020 2020 206f 725f 6578             or_ex
+00003cf0: 7072 6573 7369 6f6e 732e 6170 7065 6e64  pressions.append
+00003d00: 2822 2041 4e44 2022 2e6a 6f69 6e28 616e  (" AND ".join(an
+00003d10: 645f 6578 7072 6573 7369 6f6e 7329 290a  d_expressions)).
+00003d20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003d30: 6f72 5f65 7870 7265 7373 696f 6e73 3a0a  or_expressions:.
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 7768 6572 655f 636c 6175 7365 203d 2022  where_clause = "
+00003d60: 2057 4845 5245 2022 202b 2022 204f 5220   WHERE " + " OR 
+00003d70: 222e 6a6f 696e 286f 725f 6578 7072 6573  ".join(or_expres
+00003d80: 7369 6f6e 7329 0a0a 2020 2020 2020 2020  sions)..        
+00003d90: 6675 6c6c 5f71 7565 7279 203d 2066 227b  full_query = f"{
+00003da0: 7365 6c65 6374 5f63 6c61 7573 657d 2046  select_clause} F
+00003db0: 524f 4d20 7b73 7562 5f71 7565 7279 7d20  ROM {sub_query} 
+00003dc0: 4153 2073 7562 7b77 6865 7265 5f63 6c61  AS sub{where_cla
+00003dd0: 7573 657d 220a 2020 2020 2020 2020 7265  use}".        re
+00003de0: 7475 726e 2066 756c 6c5f 7175 6572 790a  turn full_query.
+00003df0: 0a20 2020 2064 6566 205f 7175 6572 795f  .    def _query_
+00003e00: 746f 5f64 6573 7469 6e61 7469 6f6e 280a  to_destination(.
+00003e10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00003e20: 2020 2020 2020 7175 6572 793a 2073 7472        query: str
+00003e30: 2c0a 2020 2020 2020 2020 696e 6465 785f  ,.        index_
+00003e40: 636f 6c73 3a20 4c69 7374 5b73 7472 5d2c  cols: List[str],
+00003e50: 0a20 2020 2020 2020 2061 7069 5f6e 616d  .        api_nam
+00003e60: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00003e70: 636f 6e66 6967 7572 6174 696f 6e3a 2064  configuration: d
+00003e80: 6963 7420 3d20 7b22 7175 6572 7922 3a20  ict = {"query": 
+00003e90: 7b22 7573 6551 7565 7279 4361 6368 6522  {"useQueryCache"
+00003ea0: 3a20 5472 7565 7d7d 2c0a 2020 2020 2020  : True}},.      
+00003eb0: 2020 646f 5f63 6c75 7374 6572 696e 673d    do_clustering=
+00003ec0: 5472 7565 2c0a 2020 2020 2920 2d3e 2054  True,.    ) -> T
+00003ed0: 7570 6c65 5b4f 7074 696f 6e61 6c5b 6269  uple[Optional[bi
+00003ee0: 6771 7565 7279 2e54 6162 6c65 5265 6665  gquery.TableRefe
+00003ef0: 7265 6e63 655d 2c20 6269 6771 7565 7279  rence], bigquery
+00003f00: 2e51 7565 7279 4a6f 625d 3a0a 2020 2020  .QueryJob]:.    
+00003f10: 2020 2020 2320 4966 2061 2064 7279 5f72      # If a dry_r
+00003f20: 756e 2069 6e64 6963 6174 6573 2074 6869  un indicates thi
+00003f30: 7320 6973 206e 6f74 2061 2071 7565 7279  s is not a query
+00003f40: 2074 7970 6520 6a6f 622c 2074 6865 6e20   type job, then 
+00003f50: 646f 6e27 740a 2020 2020 2020 2020 2320  don't.        # 
+00003f60: 626f 7468 6572 2074 7279 696e 6720 746f  bother trying to
+00003f70: 2064 6f20 6120 4352 4541 5445 2054 454d   do a CREATE TEM
+00003f80: 5020 5441 424c 4520 2e2e 2e20 4153 2053  P TABLE ... AS S
+00003f90: 454c 4543 5420 2e2e 2e20 7374 6174 656d  ELECT ... statem
+00003fa0: 656e 742e 0a20 2020 2020 2020 2064 7279  ent..        dry
+00003fb0: 5f72 756e 5f63 6f6e 6669 6720 3d20 6269  _run_config = bi
+00003fc0: 6771 7565 7279 2e51 7565 7279 4a6f 6243  gquery.QueryJobC
+00003fd0: 6f6e 6669 6728 290a 2020 2020 2020 2020  onfig().        
+00003fe0: 6472 795f 7275 6e5f 636f 6e66 6967 2e64  dry_run_config.d
+00003ff0: 7279 5f72 756e 203d 2054 7275 650a 2020  ry_run = True.  
+00004000: 2020 2020 2020 5f2c 2064 7279 5f72 756e        _, dry_run
+00004010: 5f6a 6f62 203d 2073 656c 662e 5f73 7461  _job = self._sta
+00004020: 7274 5f71 7565 7279 2871 7565 7279 2c20  rt_query(query, 
+00004030: 6a6f 625f 636f 6e66 6967 3d64 7279 5f72  job_config=dry_r
+00004040: 756e 5f63 6f6e 6669 6729 0a20 2020 2020  un_config).     
+00004050: 2020 2069 6620 6472 795f 7275 6e5f 6a6f     if dry_run_jo
+00004060: 622e 7374 6174 656d 656e 745f 7479 7065  b.statement_type
+00004070: 2021 3d20 2253 454c 4543 5422 3a0a 2020   != "SELECT":.  
+00004080: 2020 2020 2020 2020 2020 5f2c 2071 7565            _, que
+00004090: 7279 5f6a 6f62 203d 2073 656c 662e 5f73  ry_job = self._s
+000040a0: 7461 7274 5f71 7565 7279 2871 7565 7279  tart_query(query
+000040b0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000040c0: 7475 726e 2071 7565 7279 5f6a 6f62 2e64  turn query_job.d
+000040d0: 6573 7469 6e61 7469 6f6e 2c20 7175 6572  estination, quer
+000040e0: 795f 6a6f 620a 0a20 2020 2020 2020 2023  y_job..        #
+000040f0: 2043 7265 6174 6520 6120 7461 626c 6520   Create a table 
+00004100: 746f 2077 6f72 6b61 726f 756e 6420 4269  to workaround Bi
+00004110: 6751 7565 7279 2031 3020 4742 2071 7565  gQuery 10 GB que
+00004120: 7279 2072 6573 756c 7473 206c 696d 6974  ry results limit
+00004130: 2e20 5365 653a 0a20 2020 2020 2020 2023  . See:.        #
+00004140: 2069 6e74 6572 6e61 6c20 6973 7375 6520   internal issue 
+00004150: 3330 3330 3537 3333 362e 0a20 2020 2020  303057336..     
+00004160: 2020 2023 2053 696e 6365 2077 6520 6861     # Since we ha
+00004170: 7665 2061 2060 7374 6174 656d 656e 745f  ve a `statement_
+00004180: 7479 7065 203d 3d20 2753 454c 4543 5427  type == 'SELECT'
+00004190: 602c 2073 6368 656d 6120 7368 6f75 6c64  `, schema should
+000041a0: 2062 6520 706f 7075 6c61 7465 642e 0a20   be populated.. 
+000041b0: 2020 2020 2020 2073 6368 656d 6120 3d20         schema = 
+000041c0: 7479 7069 6e67 2e63 6173 7428 4974 6572  typing.cast(Iter
+000041d0: 6162 6c65 5b62 6967 7175 6572 792e 5363  able[bigquery.Sc
+000041e0: 6865 6d61 4669 656c 645d 2c20 6472 795f  hemaField], dry_
+000041f0: 7275 6e5f 6a6f 622e 7363 6865 6d61 290a  run_job.schema).
+00004200: 2020 2020 2020 2020 6966 2064 6f5f 636c          if do_cl
+00004210: 7573 7465 7269 6e67 3a0a 2020 2020 2020  ustering:.      
+00004220: 2020 2020 2020 636c 7573 7465 725f 636f        cluster_co
+00004230: 6c73 203d 205b 0a20 2020 2020 2020 2020  ls = [.         
+00004240: 2020 2020 2020 2069 7465 6d2e 6e61 6d65         item.name
+00004250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004260: 2066 6f72 2069 7465 6d20 696e 2073 6368   for item in sch
+00004270: 656d 610a 2020 2020 2020 2020 2020 2020  ema.            
+00004280: 2020 2020 6966 2028 6974 656d 2e6e 616d      if (item.nam
+00004290: 6520 696e 2069 6e64 6578 5f63 6f6c 7329  e in index_cols)
+000042a0: 2061 6e64 205f 6361 6e5f 636c 7573 7465   and _can_cluste
+000042b0: 725f 6271 2869 7465 6d29 0a20 2020 2020  r_bq(item).     
+000042c0: 2020 2020 2020 205d 5b3a 5f4d 4158 5f43         ][:_MAX_C
+000042d0: 4c55 5354 4552 5f43 4f4c 554d 4e53 5d0a  LUSTER_COLUMNS].
+000042e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000042f0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+00004300: 725f 636f 6c73 203d 205b 5d0a 2020 2020  r_cols = [].    
+00004310: 2020 2020 7465 6d70 5f74 6162 6c65 203d      temp_table =
+00004320: 2073 656c 662e 5f63 7265 6174 655f 656d   self._create_em
+00004330: 7074 795f 7465 6d70 5f74 6162 6c65 2873  pty_temp_table(s
+00004340: 6368 656d 612c 2063 6c75 7374 6572 5f63  chema, cluster_c
+00004350: 6f6c 7329 0a0a 2020 2020 2020 2020 7469  ols)..        ti
+00004360: 6d65 6f75 745f 6d73 203d 2063 6f6e 6669  meout_ms = confi
+00004370: 6775 7261 7469 6f6e 2e67 6574 2822 6a6f  guration.get("jo
+00004380: 6254 696d 656f 7574 4d73 2229 206f 7220  bTimeoutMs") or 
+00004390: 636f 6e66 6967 7572 6174 696f 6e5b 2271  configuration["q
+000043a0: 7565 7279 225d 2e67 6574 280a 2020 2020  uery"].get(.    
+000043b0: 2020 2020 2020 2020 2274 696d 656f 7574          "timeout
+000043c0: 4d73 220a 2020 2020 2020 2020 290a 0a20  Ms".        ).. 
+000043d0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+000043e0: 2074 696d 656f 7574 5f6d 7320 746f 2073   timeout_ms to s
+000043f0: 6563 6f6e 6473 2c20 656e 7375 7269 6e67  econds, ensuring
+00004400: 2061 206d 696e 696d 756d 206f 6620 302e   a minimum of 0.
+00004410: 3120 7365 636f 6e64 7320 746f 2061 766f  1 seconds to avo
+00004420: 6964 0a20 2020 2020 2020 2023 2074 6865  id.        # the
+00004430: 2070 726f 6772 616d 2067 6574 7469 6e67   program getting
+00004440: 2073 7475 636b 206f 6e20 746f 6f2d 7368   stuck on too-sh
+00004450: 6f72 7420 7469 6d65 6f75 7473 2e0a 2020  ort timeouts..  
+00004460: 2020 2020 2020 7469 6d65 6f75 7420 3d20        timeout = 
+00004470: 6d61 7828 696e 7428 7469 6d65 6f75 745f  max(int(timeout_
+00004480: 6d73 2920 2a20 3165 2d33 2c20 302e 3129  ms) * 1e-3, 0.1)
+00004490: 2069 6620 7469 6d65 6f75 745f 6d73 2065   if timeout_ms e
+000044a0: 6c73 6520 4e6f 6e65 0a0a 2020 2020 2020  lse None..      
+000044b0: 2020 6a6f 625f 636f 6e66 6967 203d 2074    job_config = t
+000044c0: 7970 696e 672e 6361 7374 280a 2020 2020  yping.cast(.    
+000044d0: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+000044e0: 2e51 7565 7279 4a6f 6243 6f6e 6669 672c  .QueryJobConfig,
+000044f0: 0a20 2020 2020 2020 2020 2020 2062 6967  .            big
+00004500: 7175 6572 792e 5175 6572 794a 6f62 436f  query.QueryJobCo
+00004510: 6e66 6967 2e66 726f 6d5f 6170 695f 7265  nfig.from_api_re
+00004520: 7072 2863 6f6e 6669 6775 7261 7469 6f6e  pr(configuration
+00004530: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
+00004540: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+00004550: 6c61 6265 6c73 5b22 6269 6766 7261 6d65  labels["bigframe
+00004560: 732d 6170 6922 5d20 3d20 6170 695f 6e61  s-api"] = api_na
+00004570: 6d65 0a20 2020 2020 2020 206a 6f62 5f63  me.        job_c
+00004580: 6f6e 6669 672e 6465 7374 696e 6174 696f  onfig.destinatio
+00004590: 6e20 3d20 7465 6d70 5f74 6162 6c65 0a0a  n = temp_table..
+000045a0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000045b0: 2020 2020 2020 2020 2023 2057 7269 7465           # Write
+000045c0: 2074 6f20 7465 6d70 2074 6162 6c65 2074   to temp table t
+000045d0: 6f20 776f 726b 6172 6f75 6e64 2042 6967  o workaround Big
+000045e0: 5175 6572 7920 3130 2047 4220 7175 6572  Query 10 GB quer
+000045f0: 7920 7265 7375 6c74 730a 2020 2020 2020  y results.      
+00004600: 2020 2020 2020 2320 6c69 6d69 742e 2053        # limit. S
+00004610: 6565 3a20 696e 7465 726e 616c 2069 7373  ee: internal iss
+00004620: 7565 2033 3033 3035 3733 3336 2e0a 2020  ue 303057336..  
+00004630: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+00004640: 6e66 6967 2e6c 6162 656c 735b 2265 7272  nfig.labels["err
+00004650: 6f72 5f63 6175 6768 7422 5d20 3d20 2274  or_caught"] = "t
+00004660: 7275 6522 0a20 2020 2020 2020 2020 2020  rue".           
+00004670: 205f 2c20 7175 6572 795f 6a6f 6220 3d20   _, query_job = 
+00004680: 7365 6c66 2e5f 7374 6172 745f 7175 6572  self._start_quer
+00004690: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+000046a0: 2020 2071 7565 7279 2c20 6a6f 625f 636f     query, job_co
+000046b0: 6e66 6967 3d6a 6f62 5f63 6f6e 6669 672c  nfig=job_config,
+000046c0: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+000046d0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000046e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000046f0: 6e20 7175 6572 795f 6a6f 622e 6465 7374  n query_job.dest
+00004700: 696e 6174 696f 6e2c 2071 7565 7279 5f6a  ination, query_j
+00004710: 6f62 0a20 2020 2020 2020 2065 7863 6570  ob.        excep
+00004720: 7420 676f 6f67 6c65 2e61 7069 5f63 6f72  t google.api_cor
+00004730: 652e 6578 6365 7074 696f 6e73 2e42 6164  e.exceptions.Bad
+00004740: 5265 7175 6573 743a 0a20 2020 2020 2020  Request:.       
+00004750: 2020 2020 2023 2053 6f6d 6520 5345 4c45       # Some SELE
+00004760: 4354 2073 7461 7465 6d65 6e74 7320 7374  CT statements st
+00004770: 696c 6c20 6172 656e 2774 2063 6f6d 7061  ill aren't compa
+00004780: 7469 626c 6520 7769 7468 2063 6c75 7374  tible with clust
+00004790: 6572 0a20 2020 2020 2020 2020 2020 2023  er.            #
+000047a0: 2074 6162 6c65 7320 6173 2074 6865 2064   tables as the d
+000047b0: 6573 7469 6e61 7469 6f6e 2e20 466f 7220  estination. For 
+000047c0: 6578 616d 706c 652c 2069 6620 7468 6520  example, if the 
+000047d0: 7175 6572 7920 6861 7320 610a 2020 2020  query has a.    
+000047e0: 2020 2020 2020 2020 2320 746f 702d 6c65          # top-le
+000047f0: 7665 6c20 4f52 4445 5220 4259 2c20 7468  vel ORDER BY, th
+00004800: 6973 2063 6f6e 666c 6963 7473 2077 6974  is conflicts wit
+00004810: 6820 6f75 7220 6162 696c 6974 7920 746f  h our ability to
+00004820: 2063 6c75 7374 6572 0a20 2020 2020 2020   cluster.       
+00004830: 2020 2020 2023 2074 6865 2074 6162 6c65       # the table
+00004840: 2062 7920 7468 6520 696e 6465 7820 636f   by the index co
+00004850: 6c75 6d6e 2873 292e 0a20 2020 2020 2020  lumn(s)..       
+00004860: 2020 2020 205f 2c20 7175 6572 795f 6a6f       _, query_jo
+00004870: 6220 3d20 7365 6c66 2e5f 7374 6172 745f  b = self._start_
+00004880: 7175 6572 7928 7175 6572 792c 2074 696d  query(query, tim
+00004890: 656f 7574 3d74 696d 656f 7574 290a 2020  eout=timeout).  
+000048a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000048b0: 2071 7565 7279 5f6a 6f62 2e64 6573 7469   query_job.desti
+000048c0: 6e61 7469 6f6e 2c20 7175 6572 795f 6a6f  nation, query_jo
+000048d0: 620a 0a20 2020 2064 6566 2072 6561 645f  b..    def read_
+000048e0: 6762 715f 7175 6572 7928 0a20 2020 2020  gbq_query(.     
+000048f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00004900: 2071 7565 7279 3a20 7374 722c 0a20 2020   query: str,.   
+00004910: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00004920: 696e 6465 785f 636f 6c3a 2049 7465 7261  index_col: Itera
+00004930: 626c 655b 7374 725d 207c 2073 7472 207c  ble[str] | str |
+00004940: 2062 6967 6672 616d 6573 2e65 6e75 6d73   bigframes.enums
+00004950: 2e44 6566 6175 6c74 496e 6465 784b 696e  .DefaultIndexKin
+00004960: 6420 3d20 2829 2c0a 2020 2020 2020 2020  d = (),.        
+00004970: 636f 6c75 6d6e 733a 2049 7465 7261 626c  columns: Iterabl
+00004980: 655b 7374 725d 203d 2028 292c 0a20 2020  e[str] = (),.   
+00004990: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+000049a0: 6f6e 3a20 4f70 7469 6f6e 616c 5b44 6963  on: Optional[Dic
+000049b0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+000049c0: 2020 206d 6178 5f72 6573 756c 7473 3a20     max_results: 
+000049d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000049e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7573  None,.        us
+000049f0: 655f 6361 6368 653a 204f 7074 696f 6e61  e_cache: Optiona
+00004a00: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
+00004a10: 2020 2020 2020 2020 636f 6c5f 6f72 6465          col_orde
+00004a20: 723a 2049 7465 7261 626c 655b 7374 725d  r: Iterable[str]
+00004a30: 203d 2028 292c 0a20 2020 2029 202d 3e20   = (),.    ) -> 
+00004a40: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+00004a50: 616d 653a 0a20 2020 2020 2020 2022 2222  ame:.        """
+00004a60: 5475 726e 2061 2053 514c 2071 7565 7279  Turn a SQL query
+00004a70: 2069 6e74 6f20 6120 4461 7461 4672 616d   into a DataFram
+00004a80: 652e 0a0a 2020 2020 2020 2020 4e6f 7465  e...        Note
+00004a90: 3a20 4265 6361 7573 6520 7468 6520 7265  : Because the re
+00004aa0: 7375 6c74 7320 6172 6520 7772 6974 7465  sults are writte
+00004ab0: 6e20 746f 2061 2074 656d 706f 7261 7279  n to a temporary
+00004ac0: 2074 6162 6c65 2c20 6f72 6465 7269 6e67   table, ordering
+00004ad0: 2062 790a 2020 2020 2020 2020 6060 4f52   by.        ``OR
+00004ae0: 4445 5220 4259 6060 2069 7320 6e6f 7420  DER BY`` is not 
+00004af0: 7072 6573 6572 7665 642e 2041 2075 6e69  preserved. A uni
+00004b00: 7175 6520 6069 6e64 6578 5f63 6f6c 6020  que `index_col` 
+00004b10: 6973 2072 6563 6f6d 6d65 6e64 6564 2e20  is recommended. 
+00004b20: 5573 650a 2020 2020 2020 2020 6060 726f  Use.        ``ro
+00004b30: 775f 6e75 6d62 6572 2829 206f 7665 7220  w_number() over 
+00004b40: 2829 6060 2069 6620 7468 6572 6520 6973  ()`` if there is
+00004b50: 206e 6f20 6e61 7475 7261 6c20 756e 6971   no natural uniq
+00004b60: 7565 2069 6e64 6578 206f 7220 796f 750a  ue index or you.
+00004b70: 2020 2020 2020 2020 7761 6e74 2074 6f20          want to 
+00004b80: 7072 6573 6572 7665 206f 7264 6572 696e  preserve orderin
+00004b90: 672e 0a0a 2020 2020 2020 2020 2a2a 4578  g...        **Ex
+00004ba0: 616d 706c 6573 3a2a 2a0a 0a20 2020 2020  amples:**..     
+00004bb0: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00004bc0: 7420 6269 6766 7261 6d65 732e 7061 6e64  t bigframes.pand
+00004bd0: 6173 2061 7320 6270 640a 2020 2020 2020  as as bpd.      
+00004be0: 2020 2020 2020 3e3e 3e20 6270 642e 6f70        >>> bpd.op
+00004bf0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
+00004c00: 6f67 7265 7373 5f62 6172 203d 204e 6f6e  ogress_bar = Non
+00004c10: 650a 0a20 2020 2020 2020 2053 696d 706c  e..        Simpl
+00004c20: 6520 7175 6572 7920 696e 7075 743a 0a0a  e query input:..
+00004c30: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00004c40: 6466 203d 2062 7064 2e72 6561 645f 6762  df = bpd.read_gb
+00004c50: 715f 7175 6572 7928 2727 270a 2020 2020  q_query('''.    
+00004c60: 2020 2020 2020 2020 2e2e 2e20 2020 2053          ...    S
+00004c70: 454c 4543 540a 2020 2020 2020 2020 2020  ELECT.          
+00004c80: 2020 2e2e 2e20 2020 2020 2020 7069 7463    ...       pitc
+00004c90: 6865 7246 6972 7374 4e61 6d65 2c0a 2020  herFirstName,.  
+00004ca0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004cb0: 2020 2020 7069 7463 6865 724c 6173 744e      pitcherLastN
+00004cc0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00004cd0: 202e 2e2e 2020 2020 2020 2070 6974 6368   ...       pitch
+00004ce0: 5370 6565 642c 0a20 2020 2020 2020 2020  Speed,.         
+00004cf0: 2020 202e 2e2e 2020 2020 4652 4f4d 2060     ...    FROM `
+00004d00: 6269 6771 7565 7279 2d70 7562 6c69 632d  bigquery-public-
+00004d10: 6461 7461 2e62 6173 6562 616c 6c2e 6761  data.baseball.ga
+00004d20: 6d65 735f 7769 6465 600a 2020 2020 2020  mes_wide`.      
+00004d30: 2020 2020 2020 2e2e 2e20 2727 2729 0a0a        ... ''')..
+00004d40: 2020 2020 2020 2020 5072 6573 6572 7665          Preserve
+00004d50: 206f 7264 6572 696e 6720 696e 2061 2071   ordering in a q
+00004d60: 7565 7279 2069 6e70 7574 2e0a 0a20 2020  uery input...   
+00004d70: 2020 2020 2020 2020 203e 3e3e 2064 6620           >>> df 
+00004d80: 3d20 6270 642e 7265 6164 5f67 6271 5f71  = bpd.read_gbq_q
+00004d90: 7565 7279 2827 2727 0a20 2020 2020 2020  uery('''.       
+00004da0: 2020 2020 202e 2e2e 2020 2020 5345 4c45       ...    SELE
+00004db0: 4354 0a20 2020 2020 2020 2020 2020 202e  CT.            .
+00004dc0: 2e2e 2020 2020 2020 202d 2d20 496e 7374  ..       -- Inst
+00004dd0: 6561 6420 6f66 2061 6e20 4f52 4445 5220  ead of an ORDER 
+00004de0: 4259 2063 6c61 7573 6520 6f6e 2074 6865  BY clause on the
+00004df0: 2071 7565 7279 2c20 7573 650a 2020 2020   query, use.    
+00004e00: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
+00004e10: 2020 2d2d 2052 4f57 5f4e 554d 4245 5228    -- ROW_NUMBER(
+00004e20: 2920 746f 2063 7265 6174 6520 616e 206f  ) to create an o
+00004e30: 7264 6572 6564 2044 6174 6146 7261 6d65  rdered DataFrame
+00004e40: 2e0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+00004e50: 2e20 2020 2020 2020 524f 575f 4e55 4d42  .       ROW_NUMB
+00004e60: 4552 2829 204f 5645 5220 284f 5244 4552  ER() OVER (ORDER
+00004e70: 2042 5920 4156 4728 7069 7463 6853 7065   BY AVG(pitchSpe
+00004e80: 6564 2920 4445 5343 290a 2020 2020 2020  ed) DESC).      
+00004e90: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
+00004ea0: 2020 4153 2072 6f77 696e 6465 782c 0a20    AS rowindex,. 
+00004eb0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+00004ec0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004ed0: 2020 2020 2070 6974 6368 6572 4669 7273       pitcherFirs
+00004ee0: 744e 616d 652c 0a20 2020 2020 2020 2020  tName,.         
+00004ef0: 2020 202e 2e2e 2020 2020 2020 2070 6974     ...       pit
+00004f00: 6368 6572 4c61 7374 4e61 6d65 2c0a 2020  cherLastName,.  
+00004f10: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004f20: 2020 2020 4156 4728 7069 7463 6853 7065      AVG(pitchSpe
+00004f30: 6564 2920 4153 2061 7665 7261 6765 5069  ed) AS averagePi
+00004f40: 7463 6853 7065 6564 0a20 2020 2020 2020  tchSpeed.       
+00004f50: 2020 2020 202e 2e2e 2020 2020 2046 524f       ...     FRO
+00004f60: 4d20 6062 6967 7175 6572 792d 7075 626c  M `bigquery-publ
+00004f70: 6963 2d64 6174 612e 6261 7365 6261 6c6c  ic-data.baseball
+00004f80: 2e67 616d 6573 5f77 6964 6560 0a20 2020  .games_wide`.   
+00004f90: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
+00004fa0: 2057 4845 5245 2079 6561 7220 3d20 3230   WHERE year = 20
+00004fb0: 3136 0a20 2020 2020 2020 2020 2020 202e  16.            .
+00004fc0: 2e2e 2020 2020 2047 524f 5550 2042 5920  ..     GROUP BY 
+00004fd0: 7069 7463 6865 7246 6972 7374 4e61 6d65  pitcherFirstName
+00004fe0: 2c20 7069 7463 6865 724c 6173 744e 616d  , pitcherLastNam
+00004ff0: 650a 2020 2020 2020 2020 2020 2020 2e2e  e.            ..
+00005000: 2e20 2727 272c 2069 6e64 6578 5f63 6f6c  . ''', index_col
+00005010: 3d22 726f 7769 6e64 6578 2229 0a20 2020  ="rowindex").   
+00005020: 2020 2020 2020 2020 203e 3e3e 2064 662e           >>> df.
+00005030: 6865 6164 2832 290a 2020 2020 2020 2020  head(2).        
+00005040: 2020 2020 2020 2020 2020 2020 2070 6974               pit
+00005050: 6368 6572 4669 7273 744e 616d 6520 7069  cherFirstName pi
+00005060: 7463 6865 724c 6173 744e 616d 6520 2061  tcherLastName  a
+00005070: 7665 7261 6765 5069 7463 6853 7065 6564  veragePitchSpeed
+00005080: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
+00005090: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
+000050a0: 2020 3120 2020 2020 2020 2020 2020 2020    1             
+000050b0: 2020 2041 6c62 6572 7469 6e20 2020 2020     Albertin     
+000050c0: 2020 2020 4368 6170 6d61 6e20 2020 2020      Chapman     
+000050d0: 2020 2020 2039 362e 3531 3431 3133 0a20       96.514113. 
+000050e0: 2020 2020 2020 2020 2020 2032 2020 2020             2    
+000050f0: 2020 2020 2020 2020 2020 2020 205a 6163               Zac
+00005100: 6861 7279 2020 2020 2020 2020 2042 7269  hary         Bri
+00005110: 7474 6f6e 2020 2020 2020 2020 2020 3934  tton          94
+00005120: 2e35 3931 3033 390a 2020 2020 2020 2020  .591039.        
+00005130: 2020 2020 3c42 4c41 4e4b 4c49 4e45 3e0a      <BLANKLINE>.
+00005140: 2020 2020 2020 2020 2020 2020 5b32 2072              [2 r
+00005150: 6f77 7320 7820 3320 636f 6c75 6d6e 735d  ows x 3 columns]
+00005160: 0a0a 2020 2020 2020 2020 5365 6520 616c  ..        See al
+00005170: 736f 3a20 3a6d 6574 683a 6053 6573 7369  so: :meth:`Sessi
+00005180: 6f6e 2e72 6561 645f 6762 7160 2e0a 2020  on.read_gbq`..  
+00005190: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000051a0: 2020 2320 4e4f 5445 3a20 5468 6973 206d    # NOTE: This m
+000051b0: 6574 686f 6420 646f 6573 6e27 7420 2879  ethod doesn't (y
+000051c0: 6574 2920 6578 6973 7420 696e 2070 616e  et) exist in pan
+000051d0: 6461 7320 6f72 2070 616e 6461 732d 6762  das or pandas-gb
+000051e0: 712c 2073 6f0a 2020 2020 2020 2020 2320  q, so.        # 
+000051f0: 7468 6573 6520 646f 6373 7472 696e 6773  these docstrings
+00005200: 2061 7265 2069 6e6c 696e 652e 0a20 2020   are inline..   
+00005210: 2020 2020 2069 6620 636f 6c75 6d6e 7320       if columns 
+00005220: 616e 6420 636f 6c5f 6f72 6465 723a 0a20  and col_order:. 
+00005230: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00005240: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+00005250: 2020 2020 2020 2020 2020 2020 2022 4d75               "Mu
+00005260: 7374 2073 7065 6369 6679 2065 6974 6865  st specify eithe
+00005270: 7220 636f 6c75 6d6e 7320 2870 7265 6665  r columns (prefe
+00005280: 7272 6564 2920 6f72 2063 6f6c 5f6f 7264  rred) or col_ord
+00005290: 6572 2c20 6e6f 7420 626f 7468 220a 2020  er, not both".  
+000052a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000052b0: 2020 2020 656c 6966 2063 6f6c 5f6f 7264      elif col_ord
+000052c0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000052d0: 636f 6c75 6d6e 7320 3d20 636f 6c5f 6f72  columns = col_or
+000052e0: 6465 720a 0a20 2020 2020 2020 2072 6574  der..        ret
+000052f0: 7572 6e20 7365 6c66 2e5f 7265 6164 5f67  urn self._read_g
+00005300: 6271 5f71 7565 7279 280a 2020 2020 2020  bq_query(.      
+00005310: 2020 2020 2020 7175 6572 793d 7175 6572        query=quer
+00005320: 792c 0a20 2020 2020 2020 2020 2020 2069  y,.            i
+00005330: 6e64 6578 5f63 6f6c 3d69 6e64 6578 5f63  ndex_col=index_c
+00005340: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+00005350: 636f 6c75 6d6e 733d 636f 6c75 6d6e 732c  columns=columns,
+00005360: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00005370: 6669 6775 7261 7469 6f6e 3d63 6f6e 6669  figuration=confi
+00005380: 6775 7261 7469 6f6e 2c0a 2020 2020 2020  guration,.      
+00005390: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
+000053a0: 733d 6d61 785f 7265 7375 6c74 732c 0a20  s=max_results,. 
+000053b0: 2020 2020 2020 2020 2020 2061 7069 5f6e             api_n
+000053c0: 616d 653d 2272 6561 645f 6762 715f 7175  ame="read_gbq_qu
+000053d0: 6572 7922 2c0a 2020 2020 2020 2020 2020  ery",.          
+000053e0: 2020 7573 655f 6361 6368 653d 7573 655f    use_cache=use_
+000053f0: 6361 6368 652c 0a20 2020 2020 2020 2029  cache,.        )
+00005400: 0a0a 2020 2020 6465 6620 5f72 6561 645f  ..    def _read_
+00005410: 6762 715f 7175 6572 7928 0a20 2020 2020  gbq_query(.     
+00005420: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00005430: 2071 7565 7279 3a20 7374 722c 0a20 2020   query: str,.   
+00005440: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00005450: 696e 6465 785f 636f 6c3a 2049 7465 7261  index_col: Itera
+00005460: 626c 655b 7374 725d 207c 2073 7472 207c  ble[str] | str |
+00005470: 2062 6967 6672 616d 6573 2e65 6e75 6d73   bigframes.enums
+00005480: 2e44 6566 6175 6c74 496e 6465 784b 696e  .DefaultIndexKin
+00005490: 6420 3d20 2829 2c0a 2020 2020 2020 2020  d = (),.        
+000054a0: 636f 6c75 6d6e 733a 2049 7465 7261 626c  columns: Iterabl
+000054b0: 655b 7374 725d 203d 2028 292c 0a20 2020  e[str] = (),.   
+000054c0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+000054d0: 6f6e 3a20 4f70 7469 6f6e 616c 5b44 6963  on: Optional[Dic
+000054e0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+000054f0: 2020 206d 6178 5f72 6573 756c 7473 3a20     max_results: 
+00005500: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00005510: 4e6f 6e65 2c0a 2020 2020 2020 2020 6170  None,.        ap
+00005520: 695f 6e61 6d65 3a20 7374 7220 3d20 2272  i_name: str = "r
+00005530: 6561 645f 6762 715f 7175 6572 7922 2c0a  ead_gbq_query",.
+00005540: 2020 2020 2020 2020 7573 655f 6361 6368          use_cach
+00005550: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+00005560: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
+00005570: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
+00005580: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+00005590: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+000055a0: 2e64 6174 6166 7261 6d65 2061 7320 6461  .dataframe as da
+000055b0: 7461 6672 616d 650a 0a20 2020 2020 2020  taframe..       
+000055c0: 2063 6f6e 6669 6775 7261 7469 6f6e 203d   configuration =
+000055d0: 205f 7472 616e 7366 6f72 6d5f 7265 6164   _transform_read
+000055e0: 5f67 6271 5f63 6f6e 6669 6775 7261 7469  _gbq_configurati
+000055f0: 6f6e 2863 6f6e 6669 6775 7261 7469 6f6e  on(configuration
+00005600: 290a 0a20 2020 2020 2020 2069 6620 2271  )..        if "q
+00005610: 7565 7279 2220 6e6f 7420 696e 2063 6f6e  uery" not in con
+00005620: 6669 6775 7261 7469 6f6e 3a0a 2020 2020  figuration:.    
+00005630: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00005640: 6174 696f 6e5b 2271 7565 7279 225d 203d  ation["query"] =
+00005650: 207b 7d0a 0a20 2020 2020 2020 2069 6620   {}..        if 
+00005660: 2271 7565 7279 2220 696e 2063 6f6e 6669  "query" in confi
+00005670: 6775 7261 7469 6f6e 5b22 7175 6572 7922  guration["query"
+00005680: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
+00005690: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000056a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000056b0: 2022 5468 6520 7175 6572 7920 7374 6174   "The query stat
+000056c0: 656d 656e 7420 6d75 7374 206e 6f74 2062  ement must not b
+000056d0: 6520 696e 636c 7564 6564 2069 6e20 7468  e included in th
+000056e0: 6520 222c 0a20 2020 2020 2020 2020 2020  e ",.           
+000056f0: 2020 2020 2022 2763 6f6e 6669 6775 7261       "'configura
+00005700: 7469 6f6e 2720 6265 6361 7573 6520 6974  tion' because it
+00005710: 2069 7320 616c 7265 6164 7920 7072 6f76   is already prov
+00005720: 6964 6564 2061 7322 2c0a 2020 2020 2020  ided as",.      
+00005730: 2020 2020 2020 2020 2020 2220 6120 7365            " a se
+00005740: 7061 7261 7465 2070 6172 616d 6574 6572  parate parameter
+00005750: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00005760: 290a 0a20 2020 2020 2020 2069 6620 2275  )..        if "u
+00005770: 7365 5175 6572 7943 6163 6865 2220 696e  seQueryCache" in
+00005780: 2063 6f6e 6669 6775 7261 7469 6f6e 5b22   configuration["
+00005790: 7175 6572 7922 5d3a 0a20 2020 2020 2020  query"]:.       
+000057a0: 2020 2020 2069 6620 7573 655f 6361 6368       if use_cach
+000057b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000057d0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000057e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057f0: 2020 2020 2022 2775 7365 5175 6572 7943       "'useQueryC
+00005800: 6163 6865 2720 696e 2027 636f 6e66 6967  ache' in 'config
+00005810: 7572 6174 696f 6e27 2063 6f6e 666c 6963  uration' conflic
+00005820: 7473 2077 6974 6822 0a20 2020 2020 2020  ts with".       
+00005830: 2020 2020 2020 2020 2020 2020 2022 2027               " '
+00005840: 7573 655f 6361 6368 6527 2070 6172 616d  use_cache' param
+00005850: 6574 6572 2e20 506c 6561 7365 2073 7065  eter. Please spe
+00005860: 6369 6679 206f 6e6c 7920 6f6e 652e 220a  cify only one.".
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00005890: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+000058a0: 6967 7572 6174 696f 6e5b 2271 7565 7279  iguration["query
+000058b0: 225d 5b22 7573 6551 7565 7279 4361 6368  "]["useQueryCach
+000058c0: 6522 5d20 3d20 280a 2020 2020 2020 2020  e"] = (.        
+000058d0: 2020 2020 2020 2020 5472 7565 2069 6620          True if 
+000058e0: 7573 655f 6361 6368 6520 6973 204e 6f6e  use_cache is Non
+000058f0: 6520 656c 7365 2075 7365 5f63 6163 6865  e else use_cache
+00005900: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00005910: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00005920: 7461 6e63 6528 696e 6465 785f 636f 6c2c  tance(index_col,
+00005930: 2062 6967 6672 616d 6573 2e65 6e75 6d73   bigframes.enums
+00005940: 2e44 6566 6175 6c74 496e 6465 784b 696e  .DefaultIndexKin
+00005950: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+00005960: 696e 6465 785f 636f 6c73 203d 205b 5d0a  index_cols = [].
+00005970: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00005980: 6e73 7461 6e63 6528 696e 6465 785f 636f  nstance(index_co
+00005990: 6c2c 2073 7472 293a 0a20 2020 2020 2020  l, str):.       
+000059a0: 2020 2020 2069 6e64 6578 5f63 6f6c 7320       index_cols 
+000059b0: 3d20 5b69 6e64 6578 5f63 6f6c 5d0a 2020  = [index_col].  
+000059c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000059d0: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+000059e0: 6c73 203d 206c 6973 7428 696e 6465 785f  ls = list(index_
+000059f0: 636f 6c29 0a0a 2020 2020 2020 2020 6465  col)..        de
+00005a00: 7374 696e 6174 696f 6e2c 2071 7565 7279  stination, query
+00005a10: 5f6a 6f62 203d 2073 656c 662e 5f71 7565  _job = self._que
+00005a20: 7279 5f74 6f5f 6465 7374 696e 6174 696f  ry_to_destinatio
+00005a30: 6e28 0a20 2020 2020 2020 2020 2020 2071  n(.            q
+00005a40: 7565 7279 2c0a 2020 2020 2020 2020 2020  uery,.          
+00005a50: 2020 696e 6465 785f 636f 6c73 2c0a 2020    index_cols,.  
+00005a60: 2020 2020 2020 2020 2020 6170 695f 6e61            api_na
+00005a70: 6d65 3d61 7069 5f6e 616d 652c 0a20 2020  me=api_name,.   
+00005a80: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
+00005a90: 7261 7469 6f6e 3d63 6f6e 6669 6775 7261  ration=configura
+00005aa0: 7469 6f6e 2c0a 2020 2020 2020 2020 290a  tion,.        ).
+00005ab0: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
+00005ac0: 6572 6520 7761 7320 6e6f 2064 6573 7469  ere was no desti
+00005ad0: 6e61 7469 6f6e 2074 6162 6c65 2c20 7468  nation table, th
+00005ae0: 6174 206d 6561 6e73 2074 6865 2071 7565  at means the que
+00005af0: 7279 206d 7573 7420 6861 7665 0a20 2020  ry must have.   
+00005b00: 2020 2020 2023 2062 6565 6e20 4444 4c20       # been DDL 
+00005b10: 6f72 2044 4d4c 2e20 5265 7475 726e 2073  or DML. Return s
+00005b20: 6f6d 6520 6a6f 6220 6d65 7461 6461 7461  ome job metadata
+00005b30: 2c20 696e 7374 6561 642e 0a20 2020 2020  , instead..     
+00005b40: 2020 2069 6620 6e6f 7420 6465 7374 696e     if not destin
+00005b50: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+00005b60: 2020 2072 6574 7572 6e20 6461 7461 6672     return datafr
+00005b70: 616d 652e 4461 7461 4672 616d 6528 0a20  ame.DataFrame(. 
+00005b80: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005b90: 6174 613d 7061 6e64 6173 2e44 6174 6146  ata=pandas.DataF
+00005ba0: 7261 6d65 280a 2020 2020 2020 2020 2020  rame(.          
+00005bb0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2020 2020 2273 7461 7465 6d65 6e74 5f74      "statement_t
+00005be0: 7970 6522 3a20 5b0a 2020 2020 2020 2020  ype": [.        
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c00: 2020 2020 7175 6572 795f 6a6f 622e 7374      query_job.st
+00005c10: 6174 656d 656e 745f 7479 7065 2069 6620  atement_type if 
+00005c20: 7175 6572 795f 6a6f 6220 656c 7365 2022  query_job else "
+00005c30: 756e 6b6e 6f77 6e22 0a20 2020 2020 2020  unknown".       
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00005c60: 2020 2020 2020 2020 2020 2020 226a 6f62              "job
+00005c70: 5f69 6422 3a20 5b71 7565 7279 5f6a 6f62  _id": [query_job
+00005c80: 2e6a 6f62 5f69 6420 6966 2071 7565 7279  .job_id if query
+00005c90: 5f6a 6f62 2065 6c73 6520 2275 6e6b 6e6f  _job else "unkno
+00005ca0: 776e 225d 2c0a 2020 2020 2020 2020 2020  wn"],.          
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00005cc0: 6f63 6174 696f 6e22 3a20 5b71 7565 7279  ocation": [query
+00005cd0: 5f6a 6f62 2e6c 6f63 6174 696f 6e20 6966  _job.location if
+00005ce0: 2071 7565 7279 5f6a 6f62 2065 6c73 6520   query_job else 
+00005cf0: 2275 6e6b 6e6f 776e 225d 2c0a 2020 2020  "unknown"],.    
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00005d20: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00005d30: 2020 2020 2073 6573 7369 6f6e 3d73 656c       session=sel
+00005d40: 662c 0a20 2020 2020 2020 2020 2020 2029  f,.            )
+00005d50: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005d60: 2073 656c 662e 7265 6164 5f67 6271 5f74   self.read_gbq_t
+00005d70: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00005d80: 2020 6622 7b64 6573 7469 6e61 7469 6f6e    f"{destination
+00005d90: 2e70 726f 6a65 6374 7d2e 7b64 6573 7469  .project}.{desti
+00005da0: 6e61 7469 6f6e 2e64 6174 6173 6574 5f69  nation.dataset_i
+00005db0: 647d 2e7b 6465 7374 696e 6174 696f 6e2e  d}.{destination.
+00005dc0: 7461 626c 655f 6964 7d22 2c0a 2020 2020  table_id}",.    
+00005dd0: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+00005de0: 6c3d 696e 6465 785f 636f 6c2c 0a20 2020  l=index_col,.   
+00005df0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00005e00: 3d63 6f6c 756d 6e73 2c0a 2020 2020 2020  =columns,.      
+00005e10: 2020 2020 2020 6d61 785f 7265 7375 6c74        max_result
+00005e20: 733d 6d61 785f 7265 7375 6c74 732c 0a20  s=max_results,. 
+00005e30: 2020 2020 2020 2020 2020 2075 7365 5f63             use_c
+00005e40: 6163 6865 3d63 6f6e 6669 6775 7261 7469  ache=configurati
+00005e50: 6f6e 5b22 7175 6572 7922 5d5b 2275 7365  on["query"]["use
+00005e60: 5175 6572 7943 6163 6865 225d 2c0a 2020  QueryCache"],.  
+00005e70: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00005e80: 2072 6561 645f 6762 715f 7461 626c 6528   read_gbq_table(
+00005e90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00005ea0: 2020 2020 2020 2071 7565 7279 3a20 7374         query: st
+00005eb0: 722c 0a20 2020 2020 2020 202a 2c0a 2020  r,.        *,.  
+00005ec0: 2020 2020 2020 696e 6465 785f 636f 6c3a        index_col:
+00005ed0: 2049 7465 7261 626c 655b 7374 725d 207c   Iterable[str] |
+00005ee0: 2073 7472 207c 2062 6967 6672 616d 6573   str | bigframes
+00005ef0: 2e65 6e75 6d73 2e44 6566 6175 6c74 496e  .enums.DefaultIn
+00005f00: 6465 784b 696e 6420 3d20 2829 2c0a 2020  dexKind = (),.  
+00005f10: 2020 2020 2020 636f 6c75 6d6e 733a 2049        columns: I
+00005f20: 7465 7261 626c 655b 7374 725d 203d 2028  terable[str] = (
+00005f30: 292c 0a20 2020 2020 2020 206d 6178 5f72  ),.        max_r
+00005f40: 6573 756c 7473 3a20 4f70 7469 6f6e 616c  esults: Optional
+00005f50: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+00005f60: 2020 2020 2020 6669 6c74 6572 733a 2074        filters: t
+00005f70: 6869 7264 5f70 6172 7479 5f70 616e 6461  hird_party_panda
+00005f80: 735f 6762 712e 4669 6c74 6572 7354 7970  s_gbq.FiltersTyp
+00005f90: 6520 3d20 2829 2c0a 2020 2020 2020 2020  e = (),.        
+00005fa0: 7573 655f 6361 6368 653a 2062 6f6f 6c20  use_cache: bool 
+00005fb0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00005fc0: 636f 6c5f 6f72 6465 723a 2049 7465 7261  col_order: Itera
+00005fd0: 626c 655b 7374 725d 203d 2028 292c 0a20  ble[str] = (),. 
+00005fe0: 2020 2029 202d 3e20 6461 7461 6672 616d     ) -> datafram
+00005ff0: 652e 4461 7461 4672 616d 653a 0a20 2020  e.DataFrame:.   
+00006000: 2020 2020 2022 2222 5475 726e 2061 2042       """Turn a B
+00006010: 6967 5175 6572 7920 7461 626c 6520 696e  igQuery table in
+00006020: 746f 2061 2044 6174 6146 7261 6d65 2e0a  to a DataFrame..
+00006030: 0a20 2020 2020 2020 202a 2a45 7861 6d70  .        **Examp
+00006040: 6c65 733a 2a2a 0a0a 2020 2020 2020 2020  les:**..        
+00006050: 2020 2020 3e3e 3e20 696d 706f 7274 2062      >>> import b
+00006060: 6967 6672 616d 6573 2e70 616e 6461 7320  igframes.pandas 
+00006070: 6173 2062 7064 0a20 2020 2020 2020 2020  as bpd.         
+00006080: 2020 203e 3e3e 2062 7064 2e6f 7074 696f     >>> bpd.optio
+00006090: 6e73 2e64 6973 706c 6179 2e70 726f 6772  ns.display.progr
+000060a0: 6573 735f 6261 7220 3d20 4e6f 6e65 0a0a  ess_bar = None..
+000060b0: 2020 2020 2020 2020 5265 6164 2061 2077          Read a w
+000060c0: 686f 6c65 2074 6162 6c65 2c20 7769 7468  hole table, with
+000060d0: 2061 7262 6974 7261 7279 206f 7264 6572   arbitrary order
+000060e0: 696e 6720 6f72 206f 7264 6572 696e 6720  ing or ordering 
+000060f0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00006100: 2074 6865 2070 7269 6d61 7279 206b 6579   the primary key
+00006110: 2873 292e 0a0a 2020 2020 2020 2020 2020  (s)...          
+00006120: 2020 3e3e 3e20 6466 203d 2062 7064 2e72    >>> df = bpd.r
+00006130: 6561 645f 6762 715f 7461 626c 6528 2262  ead_gbq_table("b
+00006140: 6967 7175 6572 792d 7075 626c 6963 2d64  igquery-public-d
+00006150: 6174 612e 6d6c 5f64 6174 6173 6574 732e  ata.ml_datasets.
+00006160: 7065 6e67 7569 6e73 2229 0a0a 2020 2020  penguins")..    
+00006170: 2020 2020 5365 6520 616c 736f 3a20 3a6d      See also: :m
+00006180: 6574 683a 6053 6573 7369 6f6e 2e72 6561  eth:`Session.rea
+00006190: 645f 6762 7160 2e0a 2020 2020 2020 2020  d_gbq`..        
+000061a0: 2222 220a 2020 2020 2020 2020 2320 4e4f  """.        # NO
+000061b0: 5445 3a20 5468 6973 206d 6574 686f 6420  TE: This method 
+000061c0: 646f 6573 6e27 7420 2879 6574 2920 6578  doesn't (yet) ex
+000061d0: 6973 7420 696e 2070 616e 6461 7320 6f72  ist in pandas or
+000061e0: 2070 616e 6461 732d 6762 712c 2073 6f0a   pandas-gbq, so.
+000061f0: 2020 2020 2020 2020 2320 7468 6573 6520          # these 
+00006200: 646f 6373 7472 696e 6773 2061 7265 2069  docstrings are i
+00006210: 6e6c 696e 652e 0a20 2020 2020 2020 2069  nline..        i
+00006220: 6620 636f 6c75 6d6e 7320 616e 6420 636f  f columns and co
+00006230: 6c5f 6f72 6465 723a 0a20 2020 2020 2020  l_order:.       
+00006240: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00006250: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00006260: 2020 2020 2020 2022 4d75 7374 2073 7065         "Must spe
+00006270: 6369 6679 2065 6974 6865 7220 636f 6c75  cify either colu
+00006280: 6d6e 7320 2870 7265 6665 7272 6564 2920  mns (preferred) 
+00006290: 6f72 2063 6f6c 5f6f 7264 6572 2c20 6e6f  or col_order, no
+000062a0: 7420 626f 7468 220a 2020 2020 2020 2020  t both".        
+000062b0: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+000062c0: 6966 2063 6f6c 5f6f 7264 6572 3a0a 2020  if col_order:.  
+000062d0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+000062e0: 7320 3d20 636f 6c5f 6f72 6465 720a 0a20  s = col_order.. 
+000062f0: 2020 2020 2020 2066 696c 7465 7273 203d         filters =
+00006300: 206c 6973 7428 6669 6c74 6572 7329 0a20   list(filters). 
+00006310: 2020 2020 2020 2069 6620 6c65 6e28 6669         if len(fi
+00006320: 6c74 6572 7329 2021 3d20 3020 6f72 205f  lters) != 0 or _
+00006330: 6973 5f74 6162 6c65 5f77 6974 685f 7769  is_table_with_wi
+00006340: 6c64 6361 7264 5f73 7566 6669 7828 7175  ldcard_suffix(qu
+00006350: 6572 7929 3a0a 2020 2020 2020 2020 2020  ery):.          
+00006360: 2020 7175 6572 7920 3d20 7365 6c66 2e5f    query = self._
+00006370: 746f 5f71 7565 7279 2871 7565 7279 2c20  to_query(query, 
+00006380: 636f 6c75 6d6e 732c 2066 696c 7465 7273  columns, filters
+00006390: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000063a0: 6574 7572 6e20 7365 6c66 2e5f 7265 6164  eturn self._read
+000063b0: 5f67 6271 5f71 7565 7279 280a 2020 2020  _gbq_query(.    
+000063c0: 2020 2020 2020 2020 2020 2020 7175 6572              quer
+000063d0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+000063e0: 2020 2069 6e64 6578 5f63 6f6c 3d69 6e64     index_col=ind
+000063f0: 6578 5f63 6f6c 2c0a 2020 2020 2020 2020  ex_col,.        
+00006400: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
+00006410: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
+00006420: 2020 2020 2020 2020 206d 6178 5f72 6573           max_res
+00006430: 756c 7473 3d6d 6178 5f72 6573 756c 7473  ults=max_results
+00006440: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006450: 2020 6170 695f 6e61 6d65 3d22 7265 6164    api_name="read
+00006460: 5f67 6271 5f74 6162 6c65 222c 0a20 2020  _gbq_table",.   
+00006470: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00006480: 5f63 6163 6865 3d75 7365 5f63 6163 6865  _cache=use_cache
+00006490: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+000064a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000064b0: 7365 6c66 2e5f 7265 6164 5f67 6271 5f74  self._read_gbq_t
+000064c0: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+000064d0: 2020 7175 6572 793d 7175 6572 792c 0a20    query=query,. 
+000064e0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+000064f0: 5f63 6f6c 3d69 6e64 6578 5f63 6f6c 2c0a  _col=index_col,.
+00006500: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00006510: 6d6e 733d 636f 6c75 6d6e 732c 0a20 2020  mns=columns,.   
+00006520: 2020 2020 2020 2020 206d 6178 5f72 6573           max_res
+00006530: 756c 7473 3d6d 6178 5f72 6573 756c 7473  ults=max_results
+00006540: 2c0a 2020 2020 2020 2020 2020 2020 6170  ,.            ap
+00006550: 695f 6e61 6d65 3d22 7265 6164 5f67 6271  i_name="read_gbq
+00006560: 5f74 6162 6c65 222c 0a20 2020 2020 2020  _table",.       
+00006570: 2020 2020 2075 7365 5f63 6163 6865 3d75       use_cache=u
+00006580: 7365 5f63 6163 6865 2c0a 2020 2020 2020  se_cache,.      
+00006590: 2020 290a 0a20 2020 2064 6566 205f 7265    )..    def _re
+000065a0: 6164 5f67 6271 5f74 6162 6c65 280a 2020  ad_gbq_table(.  
+000065b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000065c0: 2020 2020 7175 6572 793a 2073 7472 2c0a      query: str,.
+000065d0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000065e0: 2020 2069 6e64 6578 5f63 6f6c 3a20 4974     index_col: It
+000065f0: 6572 6162 6c65 5b73 7472 5d20 7c20 7374  erable[str] | st
+00006600: 7220 7c20 6269 6766 7261 6d65 732e 656e  r | bigframes.en
+00006610: 756d 732e 4465 6661 756c 7449 6e64 6578  ums.DefaultIndex
+00006620: 4b69 6e64 203d 2028 292c 0a20 2020 2020  Kind = (),.     
+00006630: 2020 2063 6f6c 756d 6e73 3a20 4974 6572     columns: Iter
+00006640: 6162 6c65 5b73 7472 5d20 3d20 2829 2c0a  able[str] = (),.
+00006650: 2020 2020 2020 2020 6d61 785f 7265 7375          max_resu
+00006660: 6c74 733a 204f 7074 696f 6e61 6c5b 696e  lts: Optional[in
+00006670: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+00006680: 2020 2061 7069 5f6e 616d 653a 2073 7472     api_name: str
+00006690: 2c0a 2020 2020 2020 2020 7573 655f 6361  ,.        use_ca
+000066a0: 6368 653a 2062 6f6f 6c20 3d20 5472 7565  che: bool = True
+000066b0: 2c0a 2020 2020 2920 2d3e 2064 6174 6166  ,.    ) -> dataf
+000066c0: 7261 6d65 2e44 6174 6146 7261 6d65 3a0a  rame.DataFrame:.
+000066d0: 2020 2020 2020 2020 696d 706f 7274 2062          import b
+000066e0: 6967 6672 616d 6573 2e64 6174 6166 7261  igframes.datafra
+000066f0: 6d65 2061 7320 6461 7461 6672 616d 650a  me as dataframe.
+00006700: 0a20 2020 2020 2020 2023 202d 2d2d 2d2d  .        # -----
+00006710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00006730: 2020 2020 2023 2056 616c 6964 6174 6520       # Validate 
+00006740: 616e 6420 7472 616e 7366 6f72 6d20 7061  and transform pa
+00006750: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00006760: 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   # -------------
+00006770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006780: 2d2d 2d2d 0a0a 2020 2020 2020 2020 6966  ----..        if
+00006790: 206d 6178 5f72 6573 756c 7473 2061 6e64   max_results and
+000067a0: 206d 6178 5f72 6573 756c 7473 203c 3d20   max_results <= 
+000067b0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+000067c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+000067d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000067e0: 2066 2260 6d61 785f 7265 7375 6c74 7360   f"`max_results`
+000067f0: 2073 686f 756c 6420 6265 2061 2070 6f73   should be a pos
+00006800: 6974 6976 6520 6e75 6d62 6572 2c20 676f  itive number, go
+00006810: 7420 7b6d 6178 5f72 6573 756c 7473 7d2e  t {max_results}.
+00006820: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00006830: 0a20 2020 2020 2020 2074 6162 6c65 5f72  .        table_r
+00006840: 6566 203d 2062 6967 7175 6572 792e 7461  ef = bigquery.ta
+00006850: 626c 652e 5461 626c 6552 6566 6572 656e  ble.TableReferen
+00006860: 6365 2e66 726f 6d5f 7374 7269 6e67 280a  ce.from_string(.
+00006870: 2020 2020 2020 2020 2020 2020 7175 6572              quer
+00006880: 792c 2064 6566 6175 6c74 5f70 726f 6a65  y, default_proje
+00006890: 6374 3d73 656c 662e 6271 636c 6965 6e74  ct=self.bqclient
+000068a0: 2e70 726f 6a65 6374 0a20 2020 2020 2020  .project.       
+000068b0: 2029 0a0a 2020 2020 2020 2020 2320 2d2d   )..        # --
+000068c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000068d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000068e0: 2020 2020 2020 2020 2320 4665 7463 6820          # Fetch 
+000068f0: 7461 626c 6520 6d65 7461 6461 7461 2061  table metadata a
+00006900: 6e64 2076 616c 6964 6174 650a 2020 2020  nd validate.    
+00006910: 2020 2020 2320 2d2d 2d2d 2d2d 2d2d 2d2d      # ----------
+00006920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006930: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020 2020  -------..       
+00006940: 2028 7469 6d65 5f74 7261 7665 6c5f 7469   (time_travel_ti
+00006950: 6d65 7374 616d 702c 2074 6162 6c65 2c29  mestamp, table,)
+00006960: 203d 2062 665f 7265 6164 5f67 6271 5f74   = bf_read_gbq_t
+00006970: 6162 6c65 2e67 6574 5f74 6162 6c65 5f6d  able.get_table_m
+00006980: 6574 6164 6174 6128 0a20 2020 2020 2020  etadata(.       
+00006990: 2020 2020 2073 656c 662e 6271 636c 6965       self.bqclie
+000069a0: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+000069b0: 7461 626c 655f 7265 663d 7461 626c 655f  table_ref=table_
+000069c0: 7265 662c 0a20 2020 2020 2020 2020 2020  ref,.           
+000069d0: 2061 7069 5f6e 616d 653d 6170 695f 6e61   api_name=api_na
+000069e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000069f0: 6361 6368 653d 7365 6c66 2e5f 6466 5f73  cache=self._df_s
+00006a00: 6e61 7073 686f 742c 0a20 2020 2020 2020  napshot,.       
+00006a10: 2020 2020 2075 7365 5f63 6163 6865 3d75       use_cache=u
+00006a20: 7365 5f63 6163 6865 2c0a 2020 2020 2020  se_cache,.      
+00006a30: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00006a40: 7461 626c 652e 6c6f 6361 7469 6f6e 2e63  table.location.c
+00006a50: 6173 6566 6f6c 6428 2920 213d 2073 656c  asefold() != sel
+00006a60: 662e 5f6c 6f63 6174 696f 6e2e 6361 7365  f._location.case
+00006a70: 666f 6c64 2829 3a0a 2020 2020 2020 2020  fold():.        
+00006a80: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00006a90: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00006aa0: 2020 2020 2020 6622 4375 7272 656e 7420        f"Current 
+00006ab0: 7365 7373 696f 6e20 6973 2069 6e20 7b73  session is in {s
+00006ac0: 656c 662e 5f6c 6f63 6174 696f 6e7d 2062  elf._location} b
+00006ad0: 7574 2064 6174 6173 6574 2027 7b74 6162  ut dataset '{tab
+00006ae0: 6c65 2e70 726f 6a65 6374 7d2e 7b74 6162  le.project}.{tab
+00006af0: 6c65 2e64 6174 6173 6574 5f69 647d 2720  le.dataset_id}' 
+00006b00: 6973 206c 6f63 6174 6564 2069 6e20 7b74  is located in {t
+00006b10: 6162 6c65 2e6c 6f63 6174 696f 6e7d 220a  able.location}".
+00006b20: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00006b30: 2020 2020 2020 2023 202d 2d2d 2d2d 2d2d         # -------
+00006b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b60: 2d2d 0a20 2020 2020 2020 2023 2043 7265  --.        # Cre
+00006b70: 6174 6520 4962 6973 2074 6162 6c65 2065  ate Ibis table e
+00006b80: 7870 7265 7373 696f 6e20 616e 6420 7661  xpression and va
+00006b90: 6c69 6461 7465 0a20 2020 2020 2020 2023  lidate.        #
+00006ba0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00006bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
+00006bd0: 2020 2020 2320 5573 6520 6120 7469 6d65      # Use a time
+00006be0: 2074 7261 7665 6c20 746f 206d 616b 6520   travel to make 
+00006bf0: 7375 7265 2074 6865 2044 6174 6146 7261  sure the DataFra
+00006c00: 6d65 2069 7320 6465 7465 726d 696e 6973  me is determinis
+00006c10: 7469 632c 2065 7665 6e0a 2020 2020 2020  tic, even.      
+00006c20: 2020 2320 6966 2074 6865 2075 6e64 6572    # if the under
+00006c30: 6c79 696e 6720 7461 626c 6520 6368 616e  lying table chan
+00006c40: 6765 732e 0a20 2020 2020 2020 2074 6162  ges..        tab
+00006c50: 6c65 5f65 7870 7265 7373 696f 6e20 3d20  le_expression = 
+00006c60: 6266 5f72 6561 645f 6762 715f 7461 626c  bf_read_gbq_tabl
+00006c70: 652e 6765 745f 6962 6973 5f74 696d 655f  e.get_ibis_time_
+00006c80: 7472 6176 656c 5f74 6162 6c65 280a 2020  travel_table(.  
+00006c90: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00006ca0: 6269 735f 636c 6965 6e74 2c0a 2020 2020  bis_client,.    
+00006cb0: 2020 2020 2020 2020 7461 626c 655f 7265          table_re
+00006cc0: 662c 0a20 2020 2020 2020 2020 2020 2074  f,.            t
+00006cd0: 696d 655f 7472 6176 656c 5f74 696d 6573  ime_travel_times
+00006ce0: 7461 6d70 2c0a 2020 2020 2020 2020 290a  tamp,.        ).
+00006cf0: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
+00006d00: 2069 6e20 636f 6c75 6d6e 733a 0a20 2020   in columns:.   
+00006d10: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+00006d20: 6e6f 7420 696e 2074 6162 6c65 5f65 7870  not in table_exp
+00006d30: 7265 7373 696f 6e2e 636f 6c75 6d6e 733a  ression.columns:
+00006d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d50: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00006d60: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00006d70: 2020 2020 2020 2066 2243 6f6c 756d 6e20         f"Column 
+00006d80: 277b 6b65 797d 2720 6f66 2060 636f 6c75  '{key}' of `colu
+00006d90: 6d6e 7360 206e 6f74 2066 6f75 6e64 2069  mns` not found i
+00006da0: 6e20 7468 6973 2074 6162 6c65 2e22 0a20  n this table.". 
+00006db0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00006dc0: 0a0a 2020 2020 2020 2020 2320 2d2d 2d2d  ..        # ----
+00006dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006df0: 2d2d 2d0a 2020 2020 2020 2020 2320 4372  ---.        # Cr
+00006e00: 6561 7465 2061 206e 6f6e 2d64 6566 6175  eate a non-defau
+00006e10: 6c74 2069 6e64 6578 2061 6e64 2076 616c  lt index and val
+00006e20: 6964 6174 650a 2020 2020 2020 2020 2320  idate.        # 
+00006e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006e50: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020 2020  -------..       
+00006e60: 2023 2054 4f44 4f28 622f 3333 3739 3235   # TODO(b/337925
+00006e70: 3134 3229 3a20 4d6f 7665 2069 6e64 6578  142): Move index
+00006e80: 5f63 6f6c 7320 6372 6561 7469 6f6e 2074  _cols creation t
+00006e90: 6f20 6265 666f 7265 2077 6520 6372 6561  o before we crea
+00006ea0: 7465 2074 6865 0a20 2020 2020 2020 2023  te the.        #
+00006eb0: 2049 6269 7320 7461 626c 6520 6578 7072   Ibis table expr
+00006ec0: 6573 7369 6f6e 2073 6f20 7765 2064 6f6e  ession so we don
+00006ed0: 2774 2068 6176 6520 6120 2253 454c 4543  't have a "SELEC
+00006ee0: 5420 2a22 2073 7562 7175 6572 7920 696e  T *" subquery in
+00006ef0: 2074 6865 0a20 2020 2020 2020 2023 2071   the.        # q
+00006f00: 7565 7279 2074 6861 7420 6368 6563 6b73  uery that checks
+00006f10: 2066 6f72 2069 6e64 6578 2075 6e69 7175   for index uniqu
+00006f20: 656e 6573 732e 0a0a 2020 2020 2020 2020  eness...        
+00006f30: 696e 6465 785f 636f 6c73 2c20 6973 5f69  index_cols, is_i
+00006f40: 6e64 6578 5f75 6e69 7175 6520 3d20 6266  ndex_unique = bf
+00006f50: 5f72 6561 645f 6762 715f 7461 626c 652e  _read_gbq_table.
+00006f60: 6765 745f 696e 6465 785f 636f 6c73 5f61  get_index_cols_a
+00006f70: 6e64 5f75 6e69 7175 656e 6573 7328 0a20  nd_uniqueness(. 
+00006f80: 2020 2020 2020 2020 2020 2062 7163 6c69             bqcli
+00006f90: 656e 743d 7365 6c66 2e62 7163 6c69 656e  ent=self.bqclien
+00006fa0: 742c 0a20 2020 2020 2020 2020 2020 2069  t,.            i
+00006fb0: 6269 735f 636c 6965 6e74 3d73 656c 662e  bis_client=self.
+00006fc0: 6962 6973 5f63 6c69 656e 742c 0a20 2020  ibis_client,.   
+00006fd0: 2020 2020 2020 2020 2074 6162 6c65 3d74           table=t
+00006fe0: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
+00006ff0: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
+00007000: 6f6e 3d74 6162 6c65 5f65 7870 7265 7373  on=table_express
+00007010: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00007020: 2069 6e64 6578 5f63 6f6c 3d69 6e64 6578   index_col=index
+00007030: 5f63 6f6c 2c0a 2020 2020 2020 2020 2020  _col,.          
+00007040: 2020 6170 695f 6e61 6d65 3d61 7069 5f6e    api_name=api_n
+00007050: 616d 652c 0a20 2020 2020 2020 2029 0a0a  ame,.        )..
+00007060: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
+00007070: 696e 2069 6e64 6578 5f63 6f6c 733a 0a20  in index_cols:. 
+00007080: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+00007090: 7920 6e6f 7420 696e 2074 6162 6c65 5f65  y not in table_e
+000070a0: 7870 7265 7373 696f 6e2e 636f 6c75 6d6e  xpression.column
+000070b0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000070c0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000070d0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+000070e0: 2020 2020 2020 2020 2066 2243 6f6c 756d           f"Colum
+000070f0: 6e20 607b 6b65 797d 6020 6f66 2060 696e  n `{key}` of `in
+00007100: 6465 785f 636f 6c60 206e 6f74 2066 6f75  dex_col` not fou
+00007110: 6e64 2069 6e20 7468 6973 2074 6162 6c65  nd in this table
+00007120: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00007130: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+00007140: 544f 444f 2862 2f33 3337 3932 3531 3432  TODO(b/337925142
+00007150: 293a 2057 6520 7368 6f75 6c64 2070 7573  ): We should pus
+00007160: 6820 646f 776e 2063 6f6c 756d 6e20 6669  h down column fi
+00007170: 6c74 6572 7320 7768 656e 2077 6520 6765  lters when we ge
+00007180: 7420 7468 6520 7469 6d65 0a20 2020 2020  t the time.     
+00007190: 2020 2023 2074 7261 7665 6c20 7461 626c     # travel tabl
+000071a0: 6520 746f 2061 766f 6964 2022 5345 4c45  e to avoid "SELE
+000071b0: 4354 202a 2220 7375 6271 7565 7269 6573  CT *" subqueries
+000071c0: 2e0a 2020 2020 2020 2020 6966 2063 6f6c  ..        if col
+000071d0: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
+000071e0: 2020 7461 626c 655f 6578 7072 6573 7369    table_expressi
+000071f0: 6f6e 203d 2074 6162 6c65 5f65 7870 7265  on = table_expre
+00007200: 7373 696f 6e2e 7365 6c65 6374 285b 2a69  ssion.select([*i
+00007210: 6e64 6578 5f63 6f6c 732c 202a 636f 6c75  ndex_cols, *colu
+00007220: 6d6e 735d 290a 0a20 2020 2020 2020 2023  mns])..        #
+00007230: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00007240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00007250: 2020 2020 2020 2320 4372 6561 7465 206f        # Create o
+00007260: 7264 6572 696e 6720 616e 6420 7661 6c69  rdering and vali
+00007270: 6461 7465 0a20 2020 2020 2020 2023 202d  date.        # -
+00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
+000072a0: 2020 2020 2069 6620 6973 5f69 6e64 6578       if is_index
+000072b0: 5f75 6e69 7175 653a 0a20 2020 2020 2020  _unique:.       
+000072c0: 2020 2020 2061 7272 6179 5f76 616c 7565       array_value
+000072d0: 203d 2062 665f 7265 6164 5f67 6271 5f74   = bf_read_gbq_t
+000072e0: 6162 6c65 2e74 6f5f 6172 7261 795f 7661  able.to_array_va
+000072f0: 6c75 655f 7769 7468 5f74 6f74 616c 5f6f  lue_with_total_o
+00007300: 7264 6572 696e 6728 0a20 2020 2020 2020  rdering(.       
+00007310: 2020 2020 2020 2020 2073 6573 7369 6f6e           session
+00007320: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
+00007330: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
+00007340: 7265 7373 696f 6e3d 7461 626c 655f 6578  ression=table_ex
+00007350: 7072 6573 7369 6f6e 2c0a 2020 2020 2020  pression,.      
+00007360: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
+00007370: 6f72 6465 7269 6e67 5f63 6f6c 733d 696e  ordering_cols=in
+00007380: 6465 785f 636f 6c73 2c0a 2020 2020 2020  dex_cols,.      
+00007390: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000073a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000073b0: 2020 2320 4e6f 7465 3a20 4576 656e 2074    # Note: Even t
+000073c0: 686f 7567 6820 7765 2772 6520 6164 6469  hough we're addi
+000073d0: 6e67 2061 2064 6566 6175 6c74 206f 7264  ng a default ord
+000073e0: 6572 696e 6720 6865 7265 2c20 7468 6174  ering here, that
+000073f0: 2773 0a20 2020 2020 2020 2020 2020 2023  's.            #
+00007400: 206a 7573 7420 736f 2077 6520 6861 7665   just so we have
+00007410: 2061 2064 6574 6572 6d69 6e69 7374 6963   a deterministic
+00007420: 2074 6f74 616c 206f 7264 6572 696e 672e   total ordering.
+00007430: 2049 6620 7468 6520 7573 6572 0a20 2020   If the user.   
+00007440: 2020 2020 2020 2020 2023 2073 7065 6369           # speci
+00007450: 6669 6564 2061 206e 6f6e 2d75 6e69 7175  fied a non-uniqu
+00007460: 6520 696e 6465 782c 2077 6520 7374 696c  e index, we stil
+00007470: 6c20 736f 7274 2062 7920 7468 6174 206c  l sort by that l
+00007480: 6174 6572 2e0a 2020 2020 2020 2020 2020  ater..          
+00007490: 2020 6172 7261 795f 7661 6c75 6520 3d20    array_value = 
+000074a0: 6266 5f72 6561 645f 6762 715f 7461 626c  bf_read_gbq_tabl
+000074b0: 652e 746f 5f61 7272 6179 5f76 616c 7565  e.to_array_value
+000074c0: 5f77 6974 685f 6465 6661 756c 745f 6f72  _with_default_or
+000074d0: 6465 7269 6e67 280a 2020 2020 2020 2020  dering(.        
+000074e0: 2020 2020 2020 2020 7365 7373 696f 6e3d          session=
+000074f0: 7365 6c66 2c20 7461 626c 653d 7461 626c  self, table=tabl
+00007500: 655f 6578 7072 6573 7369 6f6e 2c20 7461  e_expression, ta
+00007510: 626c 655f 726f 7773 3d74 6162 6c65 2e6e  ble_rows=table.n
+00007520: 756d 5f72 6f77 730a 2020 2020 2020 2020  um_rows.        
+00007530: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00007540: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00007550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007570: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
+00007580: 4372 6561 7465 2042 6c6f 636b 2026 2064  Create Block & d
+00007590: 6566 6175 6c74 2069 6e64 6578 2069 6620  efault index if 
+000075a0: 6c65 6e28 696e 6465 785f 636f 6c73 2920  len(index_cols) 
+000075b0: 3d3d 2030 0a20 2020 2020 2020 2023 202d  == 0.        # -
+000075c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000075d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000075e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000075f0: 2d2d 2d0a 0a20 2020 2020 2020 2076 616c  ---..        val
+00007600: 7565 5f63 6f6c 756d 6e73 203d 205b 636f  ue_columns = [co
+00007610: 6c20 666f 7220 636f 6c20 696e 2061 7272  l for col in arr
+00007620: 6179 5f76 616c 7565 2e63 6f6c 756d 6e5f  ay_value.column_
+00007630: 6964 7320 6966 2063 6f6c 206e 6f74 2069  ids if col not i
+00007640: 6e20 696e 6465 785f 636f 6c73 5d0a 2020  n index_cols].  
+00007650: 2020 2020 2020 626c 6f63 6b20 3d20 626c        block = bl
+00007660: 6f63 6b73 2e42 6c6f 636b 280a 2020 2020  ocks.Block(.    
+00007670: 2020 2020 2020 2020 6172 7261 795f 7661          array_va
+00007680: 6c75 652c 0a20 2020 2020 2020 2020 2020  lue,.           
+00007690: 2069 6e64 6578 5f63 6f6c 756d 6e73 3d69   index_columns=i
+000076a0: 6e64 6578 5f63 6f6c 732c 0a20 2020 2020  ndex_cols,.     
+000076b0: 2020 2020 2020 2063 6f6c 756d 6e5f 6c61         column_la
+000076c0: 6265 6c73 3d76 616c 7565 5f63 6f6c 756d  bels=value_colum
+000076d0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+000076e0: 696e 6465 785f 6c61 6265 6c73 3d69 6e64  index_labels=ind
+000076f0: 6578 5f63 6f6c 732c 0a20 2020 2020 2020  ex_cols,.       
+00007700: 2029 0a20 2020 2020 2020 2069 6620 6d61   ).        if ma
+00007710: 785f 7265 7375 6c74 733a 0a20 2020 2020  x_results:.     
+00007720: 2020 2020 2020 2062 6c6f 636b 203d 2062         block = b
+00007730: 6c6f 636b 2e73 6c69 6365 2873 746f 703d  lock.slice(stop=
+00007740: 6d61 785f 7265 7375 6c74 7329 0a20 2020  max_results).   
+00007750: 2020 2020 2064 6620 3d20 6461 7461 6672       df = datafr
+00007760: 616d 652e 4461 7461 4672 616d 6528 626c  ame.DataFrame(bl
+00007770: 6f63 6b29 0a0a 2020 2020 2020 2020 2320  ock)..        # 
+00007780: 4966 2075 7365 7220 7072 6f76 6964 6564  If user provided
+00007790: 2069 6e64 6578 2063 6f6c 756d 6e73 2c20   index columns, 
+000077a0: 7368 6f75 6c64 2073 6f72 7420 6f76 6572  should sort over
+000077b0: 2069 740a 2020 2020 2020 2020 6966 206c   it.        if l
+000077c0: 656e 2869 6e64 6578 5f63 6f6c 7329 203e  en(index_cols) >
+000077d0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+000077e0: 6466 2e73 6f72 745f 696e 6465 7828 290a  df.sort_index().
+000077f0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00007800: 660a 0a20 2020 2064 6566 205f 7265 6164  f..    def _read
+00007810: 5f62 6967 7175 6572 795f 6c6f 6164 5f6a  _bigquery_load_j
+00007820: 6f62 280a 2020 2020 2020 2020 7365 6c66  ob(.        self
+00007830: 2c0a 2020 2020 2020 2020 6669 6c65 7061  ,.        filepa
+00007840: 7468 5f6f 725f 6275 6666 6572 3a20 7374  th_or_buffer: st
+00007850: 7220 7c20 494f 5b22 6279 7465 7322 5d2c  r | IO["bytes"],
+00007860: 0a20 2020 2020 2020 2074 6162 6c65 3a20  .        table: 
+00007870: 556e 696f 6e5b 6269 6771 7565 7279 2e54  Union[bigquery.T
+00007880: 6162 6c65 2c20 6269 6771 7565 7279 2e54  able, bigquery.T
+00007890: 6162 6c65 5265 6665 7265 6e63 655d 2c0a  ableReference],.
+000078a0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000078b0: 2020 206a 6f62 5f63 6f6e 6669 673a 2062     job_config: b
+000078c0: 6967 7175 6572 792e 4c6f 6164 4a6f 6243  igquery.LoadJobC
+000078d0: 6f6e 6669 672c 0a20 2020 2020 2020 2069  onfig,.        i
+000078e0: 6e64 6578 5f63 6f6c 3a20 4974 6572 6162  ndex_col: Iterab
+000078f0: 6c65 5b73 7472 5d20 7c20 7374 7220 7c20  le[str] | str | 
+00007900: 6269 6766 7261 6d65 732e 656e 756d 732e  bigframes.enums.
+00007910: 4465 6661 756c 7449 6e64 6578 4b69 6e64  DefaultIndexKind
+00007920: 203d 2028 292c 0a20 2020 2020 2020 2063   = (),.        c
+00007930: 6f6c 756d 6e73 3a20 4974 6572 6162 6c65  olumns: Iterable
+00007940: 5b73 7472 5d20 3d20 2829 2c0a 2020 2020  [str] = (),.    
+00007950: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
+00007960: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+00007970: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00007980: 696e 6465 785f 636f 6c2c 2062 6967 6672  index_col, bigfr
+00007990: 616d 6573 2e65 6e75 6d73 2e44 6566 6175  ames.enums.Defau
+000079a0: 6c74 496e 6465 784b 696e 6429 3a0a 2020  ltIndexKind):.  
+000079b0: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+000079c0: 636f 6c73 203d 205b 5d0a 2020 2020 2020  cols = [].      
+000079d0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000079e0: 6528 696e 6465 785f 636f 6c2c 2073 7472  e(index_col, str
+000079f0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00007a00: 6e64 6578 5f63 6f6c 7320 3d20 5b69 6e64  ndex_cols = [ind
+00007a10: 6578 5f63 6f6c 5d0a 2020 2020 2020 2020  ex_col].        
+00007a20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007a30: 2020 696e 6465 785f 636f 6c73 203d 206c    index_cols = l
+00007a40: 6973 7428 696e 6465 785f 636f 6c29 0a0a  ist(index_col)..
+00007a50: 2020 2020 2020 2020 6966 206e 6f74 206a          if not j
+00007a60: 6f62 5f63 6f6e 6669 672e 636c 7573 7465  ob_config.cluste
+00007a70: 7269 6e67 5f66 6965 6c64 7320 616e 6420  ring_fields and 
+00007a80: 696e 6465 785f 636f 6c73 3a0a 2020 2020  index_cols:.    
+00007a90: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+00007aa0: 6967 2e63 6c75 7374 6572 696e 675f 6669  ig.clustering_fi
+00007ab0: 656c 6473 203d 2069 6e64 6578 5f63 6f6c  elds = index_col
+00007ac0: 735b 3a5f 4d41 585f 434c 5553 5445 525f  s[:_MAX_CLUSTER_
+00007ad0: 434f 4c55 4d4e 535d 0a0a 2020 2020 2020  COLUMNS]..      
+00007ae0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00007af0: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+00007b00: 6572 2c20 7374 7229 3a0a 2020 2020 2020  er, str):.      
+00007b10: 2020 2020 2020 6966 2066 696c 6570 6174        if filepat
+00007b20: 685f 6f72 5f62 7566 6665 722e 7374 6172  h_or_buffer.star
+00007b30: 7473 7769 7468 2822 6773 3a2f 2f22 293a  tswith("gs://"):
+00007b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b50: 206c 6f61 645f 6a6f 6220 3d20 7365 6c66   load_job = self
+00007b60: 2e62 7163 6c69 656e 742e 6c6f 6164 5f74  .bqclient.load_t
+00007b70: 6162 6c65 5f66 726f 6d5f 7572 6928 0a20  able_from_uri(. 
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2020 2066 696c 6570 6174 685f 6f72 5f62     filepath_or_b
+00007ba0: 7566 6665 722c 2074 6162 6c65 2c20 6a6f  uffer, table, jo
+00007bb0: 625f 636f 6e66 6967 3d6a 6f62 5f63 6f6e  b_config=job_con
+00007bc0: 6669 670a 2020 2020 2020 2020 2020 2020  fig.            
+00007bd0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00007be0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007bf0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00007c00: 6e28 6669 6c65 7061 7468 5f6f 725f 6275  n(filepath_or_bu
+00007c10: 6666 6572 2c20 2272 6222 2920 6173 2073  ffer, "rb") as s
+00007c20: 6f75 7263 655f 6669 6c65 3a0a 2020 2020  ource_file:.    
+00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 6c6f 6164 5f6a 6f62 203d 2073 656c 662e  load_job = self.
+00007c50: 6271 636c 6965 6e74 2e6c 6f61 645f 7461  bqclient.load_ta
+00007c60: 626c 655f 6672 6f6d 5f66 696c 6528 0a20  ble_from_file(. 
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2073 6f75 7263 655f 6669         source_fi
+00007c90: 6c65 2c20 7461 626c 652c 206a 6f62 5f63  le, table, job_c
+00007ca0: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
+00007cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007cc0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00007cd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007ce0: 206c 6f61 645f 6a6f 6220 3d20 7365 6c66   load_job = self
+00007cf0: 2e62 7163 6c69 656e 742e 6c6f 6164 5f74  .bqclient.load_t
+00007d00: 6162 6c65 5f66 726f 6d5f 6669 6c65 280a  able_from_file(.
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 6669 6c65 7061 7468 5f6f 725f 6275 6666  filepath_or_buff
+00007d30: 6572 2c20 7461 626c 652c 206a 6f62 5f63  er, table, job_c
+00007d40: 6f6e 6669 673d 6a6f 625f 636f 6e66 6967  onfig=job_config
+00007d50: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00007d60: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
+00007d70: 6172 745f 6765 6e65 7269 635f 6a6f 6228  art_generic_job(
+00007d80: 6c6f 6164 5f6a 6f62 290a 2020 2020 2020  load_job).      
+00007d90: 2020 7461 626c 655f 6964 203d 2066 227b    table_id = f"{
+00007da0: 7461 626c 652e 7072 6f6a 6563 747d 2e7b  table.project}.{
+00007db0: 7461 626c 652e 6461 7461 7365 745f 6964  table.dataset_id
+00007dc0: 7d2e 7b74 6162 6c65 2e74 6162 6c65 5f69  }.{table.table_i
+00007dd0: 647d 220a 0a20 2020 2020 2020 2023 2055  d}"..        # U
+00007de0: 7064 6174 6520 7468 6520 7461 626c 6520  pdate the table 
+00007df0: 6578 7069 7261 7469 6f6e 2073 6f20 7765  expiration so we
+00007e00: 2061 7265 6e27 7420 6c69 6d69 7465 6420   aren't limited 
+00007e10: 746f 2074 6865 2064 6566 6175 6c74 2032  to the default 2
+00007e20: 340a 2020 2020 2020 2020 2320 686f 7572  4.        # hour
+00007e30: 7320 6f66 2074 6865 2061 6e6f 6e79 6d6f  s of the anonymo
+00007e40: 7573 2064 6174 6173 6574 2e0a 2020 2020  us dataset..    
+00007e50: 2020 2020 7461 626c 655f 6578 7069 7261      table_expira
+00007e60: 7469 6f6e 203d 2062 6967 7175 6572 792e  tion = bigquery.
+00007e70: 5461 626c 6528 7461 626c 655f 6964 290a  Table(table_id).
+00007e80: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
+00007e90: 7069 7261 7469 6f6e 2e65 7870 6972 6573  piration.expires
+00007ea0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00007eb0: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+00007ec0: 6d65 2e6e 6f77 2864 6174 6574 696d 652e  me.now(datetime.
+00007ed0: 7469 6d65 7a6f 6e65 2e75 7463 2920 2b20  timezone.utc) + 
+00007ee0: 636f 6e73 7461 6e74 732e 4445 4641 554c  constants.DEFAUL
+00007ef0: 545f 4558 5049 5241 5449 4f4e 0a20 2020  T_EXPIRATION.   
+00007f00: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00007f10: 656c 662e 6271 636c 6965 6e74 2e75 7064  elf.bqclient.upd
+00007f20: 6174 655f 7461 626c 6528 7461 626c 655f  ate_table(table_
+00007f30: 6578 7069 7261 7469 6f6e 2c20 5b22 6578  expiration, ["ex
+00007f40: 7069 7265 7322 5d29 0a0a 2020 2020 2020  pires"])..      
+00007f50: 2020 2320 5468 6520 4269 6751 7565 7279    # The BigQuery
+00007f60: 2052 4553 5420 4150 4920 666f 7220 7461   REST API for ta
+00007f70: 626c 6573 2e67 6574 2064 6f65 736e 2774  bles.get doesn't
+00007f80: 2074 616b 6520 6120 7365 7373 696f 6e20   take a session 
+00007f90: 4944 2c20 736f 2077 650a 2020 2020 2020  ID, so we.      
+00007fa0: 2020 2320 6361 6e27 7420 6765 7420 7468    # can't get th
+00007fb0: 6520 7363 6865 6d61 2066 6f72 2061 2074  e schema for a t
+00007fc0: 656d 7020 7461 626c 6520 7468 6174 2077  emp table that w
+00007fd0: 6179 2e0a 2020 2020 2020 2020 7265 7475  ay..        retu
+00007fe0: 726e 2073 656c 662e 7265 6164 5f67 6271  rn self.read_gbq
+00007ff0: 5f74 6162 6c65 280a 2020 2020 2020 2020  _table(.        
+00008000: 2020 2020 7461 626c 655f 6964 2c0a 2020      table_id,.  
+00008010: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+00008020: 636f 6c3d 696e 6465 785f 636f 6c2c 0a20  col=index_col,. 
+00008030: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+00008040: 6e73 3d63 6f6c 756d 6e73 2c0a 2020 2020  ns=columns,.    
+00008050: 2020 2020 290a 0a20 2020 2064 6566 2072      )..    def r
+00008060: 6561 645f 6762 715f 6d6f 6465 6c28 7365  ead_gbq_model(se
+00008070: 6c66 2c20 6d6f 6465 6c5f 6e61 6d65 3a20  lf, model_name: 
+00008080: 7374 7229 3a0a 2020 2020 2020 2020 2222  str):.        ""
+00008090: 224c 6f61 6473 2061 2042 6967 5175 6572  "Loads a BigQuer
+000080a0: 7920 4d4c 206d 6f64 656c 2066 726f 6d20  y ML model from 
+000080b0: 4269 6751 7565 7279 2e0a 0a20 2020 2020  BigQuery...     
+000080c0: 2020 202a 2a45 7861 6d70 6c65 733a 2a2a     **Examples:**
+000080d0: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+000080e0: 3e20 696d 706f 7274 2062 6967 6672 616d  > import bigfram
+000080f0: 6573 2e70 616e 6461 7320 6173 2062 7064  es.pandas as bpd
+00008100: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00008110: 2062 7064 2e6f 7074 696f 6e73 2e64 6973   bpd.options.dis
+00008120: 706c 6179 2e70 726f 6772 6573 735f 6261  play.progress_ba
+00008130: 7220 3d20 4e6f 6e65 0a0a 2020 2020 2020  r = None..      
+00008140: 2020 5265 6164 2061 6e20 6578 6973 7469    Read an existi
+00008150: 6e67 2042 6967 5175 6572 7920 4d4c 206d  ng BigQuery ML m
+00008160: 6f64 656c 2e0a 0a20 2020 2020 2020 2020  odel...         
+00008170: 2020 203e 3e3e 206d 6f64 656c 5f6e 616d     >>> model_nam
+00008180: 6520 3d20 2262 6967 6672 616d 6573 2d64  e = "bigframes-d
+00008190: 6576 2e62 716d 6c5f 7475 746f 7269 616c  ev.bqml_tutorial
+000081a0: 2e70 656e 6775 696e 735f 6d6f 6465 6c22  .penguins_model"
+000081b0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000081c0: 206d 6f64 656c 203d 2062 7064 2e72 6561   model = bpd.rea
+000081d0: 645f 6762 715f 6d6f 6465 6c28 6d6f 6465  d_gbq_model(mode
+000081e0: 6c5f 6e61 6d65 290a 0a20 2020 2020 2020  l_name)..       
+000081f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00008200: 2020 206d 6f64 656c 5f6e 616d 6520 2873     model_name (s
+00008210: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00008220: 2020 2020 2074 6865 206d 6f64 656c 2773       the model's
+00008230: 206e 616d 6520 696e 2042 6967 5175 6572   name in BigQuer
+00008240: 7920 696e 2074 6865 2066 6f72 6d61 740a  y in the format.
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 6070 726f 6a65 6374 5f69 642e 6461 7461  `project_id.data
+00008270: 7365 745f 6964 2e6d 6f64 656c 5f69 6460  set_id.model_id`
+00008280: 2c20 6f72 206a 7573 7420 6064 6174 6173  , or just `datas
+00008290: 6574 5f69 642e 6d6f 6465 6c5f 6964 600a  et_id.model_id`.
+000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082b0: 746f 206c 6f61 6420 6672 6f6d 2074 6865  to load from the
+000082c0: 2064 6566 6175 6c74 2070 726f 6a65 6374   default project
+000082d0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000082e0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000082f0: 4120 6269 6766 7261 6d65 732e 6d6c 204d  A bigframes.ml M
+00008300: 6f64 656c 2c20 5472 616e 7366 6f72 6d65  odel, Transforme
+00008310: 7220 6f72 2050 6970 656c 696e 6520 7772  r or Pipeline wr
+00008320: 6170 7069 6e67 2074 6865 206d 6f64 656c  apping the model
+00008330: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00008340: 2020 2020 2020 696d 706f 7274 2062 6967        import big
+00008350: 6672 616d 6573 2e6d 6c2e 6c6f 6164 6572  frames.ml.loader
+00008360: 0a0a 2020 2020 2020 2020 6d6f 6465 6c5f  ..        model_
+00008370: 7265 6620 3d20 6269 6771 7565 7279 2e4d  ref = bigquery.M
+00008380: 6f64 656c 5265 6665 7265 6e63 652e 6672  odelReference.fr
+00008390: 6f6d 5f73 7472 696e 6728 0a20 2020 2020  om_string(.     
+000083a0: 2020 2020 2020 206d 6f64 656c 5f6e 616d         model_nam
+000083b0: 652c 2064 6566 6175 6c74 5f70 726f 6a65  e, default_proje
+000083c0: 6374 3d73 656c 662e 6271 636c 6965 6e74  ct=self.bqclient
+000083d0: 2e70 726f 6a65 6374 0a20 2020 2020 2020  .project.       
+000083e0: 2029 0a20 2020 2020 2020 206d 6f64 656c   ).        model
+000083f0: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
+00008400: 2e67 6574 5f6d 6f64 656c 286d 6f64 656c  .get_model(model
+00008410: 5f72 6566 290a 2020 2020 2020 2020 7265  _ref).        re
+00008420: 7475 726e 2062 6967 6672 616d 6573 2e6d  turn bigframes.m
+00008430: 6c2e 6c6f 6164 6572 2e66 726f 6d5f 6271  l.loader.from_bq
+00008440: 2873 656c 662c 206d 6f64 656c 290a 0a20  (self, model).. 
+00008450: 2020 2040 7479 7069 6e67 2e6f 7665 726c     @typing.overl
+00008460: 6f61 640a 2020 2020 6465 6620 7265 6164  oad.    def read
+00008470: 5f70 616e 6461 7328 0a20 2020 2020 2020  _pandas(.       
+00008480: 2073 656c 662c 2070 616e 6461 735f 6461   self, pandas_da
+00008490: 7461 6672 616d 653a 2070 616e 6461 732e  taframe: pandas.
+000084a0: 496e 6465 780a 2020 2020 2920 2d3e 2062  Index.    ) -> b
+000084b0: 6967 6672 616d 6573 2e63 6f72 652e 696e  igframes.core.in
+000084c0: 6465 7865 732e 496e 6465 783a 0a20 2020  dexes.Index:.   
+000084d0: 2020 2020 202e 2e2e 0a0a 2020 2020 4074       .....    @t
+000084e0: 7970 696e 672e 6f76 6572 6c6f 6164 0a20  yping.overload. 
+000084f0: 2020 2064 6566 2072 6561 645f 7061 6e64     def read_pand
+00008500: 6173 2873 656c 662c 2070 616e 6461 735f  as(self, pandas_
+00008510: 6461 7461 6672 616d 653a 2070 616e 6461  dataframe: panda
+00008520: 732e 5365 7269 6573 2920 2d3e 2062 6967  s.Series) -> big
+00008530: 6672 616d 6573 2e73 6572 6965 732e 5365  frames.series.Se
+00008540: 7269 6573 3a0a 2020 2020 2020 2020 2e2e  ries:.        ..
+00008550: 2e0a 0a20 2020 2040 7479 7069 6e67 2e6f  ...    @typing.o
+00008560: 7665 726c 6f61 640a 2020 2020 6465 6620  verload.    def 
+00008570: 7265 6164 5f70 616e 6461 7328 7365 6c66  read_pandas(self
+00008580: 2c20 7061 6e64 6173 5f64 6174 6166 7261  , pandas_datafra
+00008590: 6d65 3a20 7061 6e64 6173 2e44 6174 6146  me: pandas.DataF
+000085a0: 7261 6d65 2920 2d3e 2064 6174 6166 7261  rame) -> datafra
+000085b0: 6d65 2e44 6174 6146 7261 6d65 3a0a 2020  me.DataFrame:.  
+000085c0: 2020 2020 2020 2e2e 2e0a 0a20 2020 2064        .....    d
+000085d0: 6566 2072 6561 645f 7061 6e64 6173 280a  ef read_pandas(.
+000085e0: 2020 2020 2020 2020 7365 6c66 2c20 7061          self, pa
+000085f0: 6e64 6173 5f64 6174 6166 7261 6d65 3a20  ndas_dataframe: 
+00008600: 556e 696f 6e5b 7061 6e64 6173 2e44 6174  Union[pandas.Dat
+00008610: 6146 7261 6d65 2c20 7061 6e64 6173 2e53  aFrame, pandas.S
+00008620: 6572 6965 732c 2070 616e 6461 732e 496e  eries, pandas.In
+00008630: 6465 785d 0a20 2020 2029 3a0a 2020 2020  dex].    ):.    
+00008640: 2020 2020 2222 224c 6f61 6473 2044 6174      """Loads Dat
+00008650: 6146 7261 6d65 2066 726f 6d20 6120 7061  aFrame from a pa
+00008660: 6e64 6173 2044 6174 6146 7261 6d65 2e0a  ndas DataFrame..
+00008670: 0a20 2020 2020 2020 2054 6865 2070 616e  .        The pan
+00008680: 6461 7320 4461 7461 4672 616d 6520 7769  das DataFrame wi
+00008690: 6c6c 2062 6520 7065 7273 6973 7465 6420  ll be persisted 
+000086a0: 6173 2061 2074 656d 706f 7261 7279 2042  as a temporary B
+000086b0: 6967 5175 6572 7920 7461 626c 652c 2077  igQuery table, w
+000086c0: 6869 6368 2063 616e 2062 650a 2020 2020  hich can be.    
+000086d0: 2020 2020 6175 746f 6d61 7469 6361 6c6c      automaticall
+000086e0: 7920 7265 6379 636c 6564 2061 6674 6572  y recycled after
+000086f0: 2074 6865 2053 6573 7369 6f6e 2069 7320   the Session is 
+00008700: 636c 6f73 6564 2e0a 0a20 2020 2020 2020  closed...       
+00008710: 202a 2a45 7861 6d70 6c65 733a 2a2a 0a0a   **Examples:**..
+00008720: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00008730: 696d 706f 7274 2062 6967 6672 616d 6573  import bigframes
+00008740: 2e70 616e 6461 7320 6173 2062 7064 0a20  .pandas as bpd. 
+00008750: 2020 2020 2020 2020 2020 203e 3e3e 2069             >>> i
+00008760: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+00008770: 7064 0a20 2020 2020 2020 2020 2020 203e  pd.            >
+00008780: 3e3e 2062 7064 2e6f 7074 696f 6e73 2e64  >> bpd.options.d
+00008790: 6973 706c 6179 2e70 726f 6772 6573 735f  isplay.progress_
+000087a0: 6261 7220 3d20 4e6f 6e65 0a0a 2020 2020  bar = None..    
+000087b0: 2020 2020 2020 2020 3e3e 3e20 6420 3d20          >>> d = 
+000087c0: 7b27 636f 6c31 273a 205b 312c 2032 5d2c  {'col1': [1, 2],
+000087d0: 2027 636f 6c32 273a 205b 332c 2034 5d7d   'col2': [3, 4]}
+000087e0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000087f0: 2070 616e 6461 735f 6466 203d 2070 642e   pandas_df = pd.
+00008800: 4461 7461 4672 616d 6528 6461 7461 3d64  DataFrame(data=d
+00008810: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00008820: 3e20 6466 203d 2062 7064 2e72 6561 645f  > df = bpd.read_
+00008830: 7061 6e64 6173 2870 616e 6461 735f 6466  pandas(pandas_df
+00008840: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00008850: 3e20 6466 0a20 2020 2020 2020 2020 2020  > df.           
+00008860: 2020 2020 636f 6c31 2020 636f 6c32 0a20      col1  col2. 
+00008870: 2020 2020 2020 2020 2020 2030 2020 2020             0    
+00008880: 2031 2020 2020 2033 0a20 2020 2020 2020   1     3.       
+00008890: 2020 2020 2031 2020 2020 2032 2020 2020       1     2    
+000088a0: 2034 0a20 2020 2020 2020 2020 2020 203c   4.            <
+000088b0: 424c 414e 4b4c 494e 453e 0a20 2020 2020  BLANKLINE>.     
+000088c0: 2020 2020 2020 205b 3220 726f 7773 2078         [2 rows x
+000088d0: 2032 2063 6f6c 756d 6e73 5d0a 0a20 2020   2 columns]..   
+000088e0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000088f0: 2020 2020 2020 2070 616e 6461 735f 6461         pandas_da
+00008900: 7461 6672 616d 6520 2870 616e 6461 732e  taframe (pandas.
+00008910: 4461 7461 4672 616d 652c 2070 616e 6461  DataFrame, panda
+00008920: 732e 5365 7269 6573 2c20 6f72 2070 616e  s.Series, or pan
+00008930: 6461 732e 496e 6465 7829 3a0a 2020 2020  das.Index):.    
+00008940: 2020 2020 2020 2020 2020 2020 6120 7061              a pa
+00008950: 6e64 6173 2044 6174 6146 7261 6d65 2f53  ndas DataFrame/S
+00008960: 6572 6965 732f 496e 6465 7820 6f62 6a65  eries/Index obje
+00008970: 6374 2074 6f20 6265 206c 6f61 6465 642e  ct to be loaded.
+00008980: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00008990: 733a 0a20 2020 2020 2020 2020 2020 2041  s:.            A
+000089a0: 6e20 6571 7569 7661 6c65 6e74 2062 6967  n equivalent big
+000089b0: 6672 616d 6573 2e70 616e 6461 732e 2844  frames.pandas.(D
+000089c0: 6174 6146 7261 6d65 2f53 6572 6965 732f  ataFrame/Series/
+000089d0: 496e 6465 7829 206f 626a 6563 740a 2020  Index) object.  
+000089e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000089f0: 2020 696d 706f 7274 2062 6967 6672 616d    import bigfram
+00008a00: 6573 2e73 6572 6965 7320 6173 2073 6572  es.series as ser
+00008a10: 6965 730a 0a20 2020 2020 2020 2023 2054  ies..        # T
+00008a20: 7279 2074 6f20 6861 6e64 6c65 206e 6f6e  ry to handle non
+00008a30: 2d64 6174 6166 7261 6d65 2070 616e 6461  -dataframe panda
+00008a40: 7320 6f62 6a65 6374 7320 6173 2077 656c  s objects as wel
+00008a50: 6c0a 2020 2020 2020 2020 6966 2069 7369  l.        if isi
+00008a60: 6e73 7461 6e63 6528 7061 6e64 6173 5f64  nstance(pandas_d
+00008a70: 6174 6166 7261 6d65 2c20 7061 6e64 6173  ataframe, pandas
+00008a80: 2e53 6572 6965 7329 3a0a 2020 2020 2020  .Series):.      
+00008a90: 2020 2020 2020 6266 5f64 6620 3d20 7365        bf_df = se
+00008aa0: 6c66 2e5f 7265 6164 5f70 616e 6461 7328  lf._read_pandas(
+00008ab0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00008ac0: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
+00008ad0: 6529 2c20 2272 6561 645f 7061 6e64 6173  e), "read_pandas
+00008ae0: 2229 0a20 2020 2020 2020 2020 2020 2062  ").            b
+00008af0: 665f 7365 7269 6573 203d 2074 7970 696e  f_series = typin
+00008b00: 672e 6361 7374 2873 6572 6965 732e 5365  g.cast(series.Se
+00008b10: 7269 6573 2c20 6266 5f64 665b 6266 5f64  ries, bf_df[bf_d
+00008b20: 662e 636f 6c75 6d6e 735b 305d 5d29 0a20  f.columns[0]]). 
+00008b30: 2020 2020 2020 2020 2020 2023 2077 7261             # wra
+00008b40: 7070 696e 6720 696e 746f 2064 6620 6361  pping into df ca
+00008b50: 6e20 7365 7420 6e61 6d65 2074 6f20 3020  n set name to 0 
+00008b60: 736f 2072 6573 6574 2074 6f20 6f72 6967  so reset to orig
+00008b70: 696e 616c 206f 626a 6563 7420 6e61 6d65  inal object name
+00008b80: 0a20 2020 2020 2020 2020 2020 2062 665f  .            bf_
+00008b90: 7365 7269 6573 2e6e 616d 6520 3d20 7061  series.name = pa
+00008ba0: 6e64 6173 5f64 6174 6166 7261 6d65 2e6e  ndas_dataframe.n
+00008bb0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00008bc0: 7265 7475 726e 2062 665f 7365 7269 6573  return bf_series
+00008bd0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00008be0: 7374 616e 6365 2870 616e 6461 735f 6461  stance(pandas_da
+00008bf0: 7461 6672 616d 652c 2070 616e 6461 732e  taframe, pandas.
+00008c00: 496e 6465 7829 3a0a 2020 2020 2020 2020  Index):.        
+00008c10: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00008c20: 5f72 6561 645f 7061 6e64 6173 280a 2020  _read_pandas(.  
+00008c30: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00008c40: 6e64 6173 2e44 6174 6146 7261 6d65 2869  ndas.DataFrame(i
+00008c50: 6e64 6578 3d70 616e 6461 735f 6461 7461  ndex=pandas_data
+00008c60: 6672 616d 6529 2c20 2272 6561 645f 7061  frame), "read_pa
+00008c70: 6e64 6173 220a 2020 2020 2020 2020 2020  ndas".          
+00008c80: 2020 292e 696e 6465 780a 2020 2020 2020    ).index.      
+00008c90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00008ca0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+00008cb0: 2c20 7061 6e64 6173 2e44 6174 6146 7261  , pandas.DataFra
+00008cc0: 6d65 293a 0a20 2020 2020 2020 2020 2020  me):.           
+00008cd0: 2072 6574 7572 6e20 7365 6c66 2e5f 7265   return self._re
+00008ce0: 6164 5f70 616e 6461 7328 7061 6e64 6173  ad_pandas(pandas
+00008cf0: 5f64 6174 6166 7261 6d65 2c20 2272 6561  _dataframe, "rea
+00008d00: 645f 7061 6e64 6173 2229 0a20 2020 2020  d_pandas").     
+00008d10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008d20: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00008d30: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00008d40: 2020 2020 2020 2066 2272 6561 645f 7061         f"read_pa
+00008d50: 6e64 6173 2829 2065 7870 6563 7473 2061  ndas() expects a
+00008d60: 2070 616e 6461 732e 4461 7461 4672 616d   pandas.DataFram
+00008d70: 652c 2062 7574 2067 6f74 2061 207b 7479  e, but got a {ty
+00008d80: 7065 2870 616e 6461 735f 6461 7461 6672  pe(pandas_datafr
+00008d90: 616d 6529 7d22 0a20 2020 2020 2020 2020  ame)}".         
+00008da0: 2020 2029 0a0a 2020 2020 6465 6620 5f72     )..    def _r
+00008db0: 6561 645f 7061 6e64 6173 280a 2020 2020  ead_pandas(.    
+00008dc0: 2020 2020 7365 6c66 2c20 7061 6e64 6173      self, pandas
+00008dd0: 5f64 6174 6166 7261 6d65 3a20 7061 6e64  _dataframe: pand
+00008de0: 6173 2e44 6174 6146 7261 6d65 2c20 6170  as.DataFrame, ap
+00008df0: 695f 6e61 6d65 3a20 7374 720a 2020 2020  i_name: str.    
+00008e00: 2920 2d3e 2064 6174 6166 7261 6d65 2e44  ) -> dataframe.D
+00008e10: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+00008e20: 2020 696d 706f 7274 2062 6967 6672 616d    import bigfram
+00008e30: 6573 2e64 6174 6166 7261 6d65 2061 7320  es.dataframe as 
+00008e40: 6461 7461 6672 616d 650a 0a20 2020 2020  dataframe..     
+00008e50: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00008e60: 2870 616e 6461 735f 6461 7461 6672 616d  (pandas_datafram
+00008e70: 652c 2064 6174 6166 7261 6d65 2e44 6174  e, dataframe.Dat
+00008e80: 6146 7261 6d65 293a 0a20 2020 2020 2020  aFrame):.       
+00008e90: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00008ea0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00008eb0: 2020 2020 2020 2022 7265 6164 5f70 616e         "read_pan
+00008ec0: 6461 7328 2920 6578 7065 6374 7320 6120  das() expects a 
+00008ed0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00008ee0: 2c20 6275 7420 676f 7420 6120 220a 2020  , but got a ".  
+00008ef0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00008f00: 6967 6672 616d 6573 2e70 616e 6461 732e  igframes.pandas.
+00008f10: 4461 7461 4672 616d 652e 220a 2020 2020  DataFrame.".    
+00008f20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00008f30: 2020 2069 6e6c 696e 655f 6466 203d 2073     inline_df = s
+00008f40: 656c 662e 5f72 6561 645f 7061 6e64 6173  elf._read_pandas
+00008f50: 5f69 6e6c 696e 6528 7061 6e64 6173 5f64  _inline(pandas_d
+00008f60: 6174 6166 7261 6d65 290a 2020 2020 2020  ataframe).      
+00008f70: 2020 6966 2069 6e6c 696e 655f 6466 2069    if inline_df i
+00008f80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008f90: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00008fa0: 6e6c 696e 655f 6466 0a20 2020 2020 2020  nline_df.       
+00008fb0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00008fc0: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
+00008fd0: 6561 645f 7061 6e64 6173 5f6c 6f61 645f  ead_pandas_load_
+00008fe0: 6a6f 6228 7061 6e64 6173 5f64 6174 6166  job(pandas_dataf
+00008ff0: 7261 6d65 2c20 6170 695f 6e61 6d65 290a  rame, api_name).
+00009000: 2020 2020 2020 2020 6578 6365 7074 2070          except p
+00009010: 612e 4172 726f 7749 6e76 616c 6964 2061  a.ArrowInvalid a
+00009020: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00009030: 2072 6169 7365 2070 612e 4172 726f 7749   raise pa.ArrowI
+00009040: 6e76 616c 6964 280a 2020 2020 2020 2020  nvalid(.        
+00009050: 2020 2020 2020 2020 6622 436f 756c 6420          f"Could 
+00009060: 6e6f 7420 636f 6e76 6572 7420 7769 7468  not convert with
+00009070: 2061 2042 6967 5175 6572 7920 7479 7065   a BigQuery type
+00009080: 3a20 607b 657d 602e 2022 0a20 2020 2020  : `{e}`. ".     
+00009090: 2020 2020 2020 2029 2066 726f 6d20 650a         ) from e.
+000090a0: 0a20 2020 2064 6566 205f 7265 6164 5f70  .    def _read_p
+000090b0: 616e 6461 735f 696e 6c69 6e65 280a 2020  andas_inline(.  
+000090c0: 2020 2020 2020 7365 6c66 2c20 7061 6e64        self, pand
+000090d0: 6173 5f64 6174 6166 7261 6d65 3a20 7061  as_dataframe: pa
+000090e0: 6e64 6173 2e44 6174 6146 7261 6d65 0a20  ndas.DataFrame. 
+000090f0: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
+00009100: 5b64 6174 6166 7261 6d65 2e44 6174 6146  [dataframe.DataF
+00009110: 7261 6d65 5d3a 0a20 2020 2020 2020 2069  rame]:.        i
+00009120: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+00009130: 6461 7461 6672 616d 6520 6173 2064 6174  dataframe as dat
+00009140: 6166 7261 6d65 0a0a 2020 2020 2020 2020  aframe..        
+00009150: 6966 2070 616e 6461 735f 6461 7461 6672  if pandas_datafr
+00009160: 616d 652e 6d65 6d6f 7279 5f75 7361 6765  ame.memory_usage
+00009170: 2864 6565 703d 5472 7565 292e 7375 6d28  (deep=True).sum(
+00009180: 2920 3e20 4d41 585f 494e 4c49 4e45 5f44  ) > MAX_INLINE_D
+00009190: 465f 4259 5445 533a 0a20 2020 2020 2020  F_BYTES:.       
+000091a0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000091b0: 0a0a 2020 2020 2020 2020 7472 793a 0a20  ..        try:. 
+000091c0: 2020 2020 2020 2020 2020 2069 6e6c 696e             inlin
+000091d0: 655f 6466 203d 2064 6174 6166 7261 6d65  e_df = dataframe
+000091e0: 2e44 6174 6146 7261 6d65 280a 2020 2020  .DataFrame(.    
+000091f0: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
+00009200: 6b73 2e42 6c6f 636b 2e66 726f 6d5f 6c6f  ks.Block.from_lo
+00009210: 6361 6c28 7061 6e64 6173 5f64 6174 6166  cal(pandas_dataf
+00009220: 7261 6d65 2c20 7365 6c66 290a 2020 2020  rame, self).    
+00009230: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009240: 2020 6578 6365 7074 2070 612e 4172 726f    except pa.Arro
+00009250: 7749 6e76 616c 6964 2061 7320 653a 0a20  wInvalid as e:. 
+00009260: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00009270: 2070 612e 4172 726f 7749 6e76 616c 6964   pa.ArrowInvalid
+00009280: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009290: 2020 6622 436f 756c 6420 6e6f 7420 636f    f"Could not co
+000092a0: 6e76 6572 7420 7769 7468 2061 2042 6967  nvert with a Big
+000092b0: 5175 6572 7920 7479 7065 3a20 607b 657d  Query type: `{e}
+000092c0: 602e 2022 0a20 2020 2020 2020 2020 2020  `. ".           
+000092d0: 2029 2066 726f 6d20 650a 2020 2020 2020   ) from e.      
+000092e0: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+000092f0: 726f 723a 2020 2320 5468 726f 776e 2062  ror:  # Thrown b
+00009300: 7920 6962 6973 2066 6f72 2073 6f6d 6520  y ibis for some 
+00009310: 756e 6861 6e64 6c65 6420 7479 7065 730a  unhandled types.
+00009320: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009330: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00009340: 6578 6365 7074 2070 612e 4172 726f 7754  except pa.ArrowT
+00009350: 7970 6545 7272 6f72 3a20 2023 2054 6872  ypeError:  # Thr
+00009360: 6f77 6e20 6279 2061 7272 6f77 2066 6f72  own by arrow for
+00009370: 2074 7970 6573 2077 6974 686f 7574 206d   types without m
+00009380: 6170 7069 6e67 2028 6765 6f29 2e0a 2020  apping (geo)..  
+00009390: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000093a0: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
+000093b0: 6e6c 696e 655f 7479 7065 7320 3d20 696e  nline_types = in
+000093c0: 6c69 6e65 5f64 662e 5f62 6c6f 636b 2e65  line_df._block.e
+000093d0: 7870 722e 7363 6865 6d61 2e64 7479 7065  xpr.schema.dtype
+000093e0: 730a 2020 2020 2020 2020 2320 4962 6973  s.        # Ibis
+000093f0: 2068 6173 2070 726f 626c 656d 7320 6573   has problems es
+00009400: 6361 7069 6e67 2062 7974 6573 206c 6974  caping bytes lit
+00009410: 6572 616c 732c 2077 6869 6368 2077 696c  erals, which wil
+00009420: 6c20 6361 7573 6520 7379 6e74 6178 2065  l cause syntax e
+00009430: 7272 6f72 7320 7365 7276 6572 2d73 6964  rrors server-sid
+00009440: 652e 0a20 2020 2020 2020 2069 6620 616c  e..        if al
+00009450: 6c28 6474 7970 6520 696e 2049 4e4c 494e  l(dtype in INLIN
+00009460: 4142 4c45 5f44 5459 5045 5320 666f 7220  ABLE_DTYPES for 
+00009470: 6474 7970 6520 696e 2069 6e6c 696e 655f  dtype in inline_
+00009480: 7479 7065 7329 3a0a 2020 2020 2020 2020  types):.        
+00009490: 2020 2020 7265 7475 726e 2069 6e6c 696e      return inlin
+000094a0: 655f 6466 0a20 2020 2020 2020 2072 6574  e_df.        ret
+000094b0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
+000094c0: 6620 5f72 6561 645f 7061 6e64 6173 5f6c  f _read_pandas_l
+000094d0: 6f61 645f 6a6f 6228 0a20 2020 2020 2020  oad_job(.       
+000094e0: 2073 656c 662c 2070 616e 6461 735f 6461   self, pandas_da
+000094f0: 7461 6672 616d 653a 2070 616e 6461 732e  taframe: pandas.
+00009500: 4461 7461 4672 616d 652c 2061 7069 5f6e  DataFrame, api_n
+00009510: 616d 653a 2073 7472 0a20 2020 2029 202d  ame: str.    ) -
+00009520: 3e20 6461 7461 6672 616d 652e 4461 7461  > dataframe.Data
+00009530: 4672 616d 653a 0a20 2020 2020 2020 2069  Frame:.        i
+00009540: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+00009550: 6461 7461 6672 616d 6520 6173 2064 6174  dataframe as dat
+00009560: 6166 7261 6d65 0a0a 2020 2020 2020 2020  aframe..        
+00009570: 636f 6c5f 696e 6465 7820 3d20 7061 6e64  col_index = pand
+00009580: 6173 5f64 6174 6166 7261 6d65 2e63 6f6c  as_dataframe.col
+00009590: 756d 6e73 2e63 6f70 7928 290a 2020 2020  umns.copy().    
+000095a0: 2020 2020 636f 6c5f 6c61 6265 6c73 2c20      col_labels, 
+000095b0: 6964 785f 6c61 6265 6c73 203d 2028 0a20  idx_labels = (. 
+000095c0: 2020 2020 2020 2020 2020 2063 6f6c 5f69             col_i
+000095d0: 6e64 6578 2e74 6f5f 6c69 7374 2829 2c0a  ndex.to_list(),.
+000095e0: 2020 2020 2020 2020 2020 2020 7061 6e64              pand
+000095f0: 6173 5f64 6174 6166 7261 6d65 2e69 6e64  as_dataframe.ind
+00009600: 6578 2e6e 616d 6573 2c0a 2020 2020 2020  ex.names,.      
+00009610: 2020 290a 2020 2020 2020 2020 6e65 775f    ).        new_
+00009620: 636f 6c5f 6964 732c 206e 6577 5f69 6478  col_ids, new_idx
+00009630: 5f69 6473 203d 2075 7469 6c73 2e67 6574  _ids = utils.get
+00009640: 5f73 7461 6e64 6172 6469 7a65 645f 6964  _standardized_id
+00009650: 7328 0a20 2020 2020 2020 2020 2020 2063  s(.            c
+00009660: 6f6c 5f6c 6162 656c 732c 0a20 2020 2020  ol_labels,.     
+00009670: 2020 2020 2020 2069 6478 5f6c 6162 656c         idx_label
+00009680: 732c 0a20 2020 2020 2020 2020 2020 2023  s,.            #
+00009690: 204c 6f61 6469 6e67 2070 6172 7175 6574   Loading parquet
+000096a0: 2066 696c 6573 2069 6e74 6f20 4269 6751   files into BigQ
+000096b0: 7565 7279 2077 6974 6820 7370 6563 6961  uery with specia
+000096c0: 6c20 636f 6c75 6d6e 206e 616d 6573 0a20  l column names. 
+000096d0: 2020 2020 2020 2020 2020 2023 2069 7320             # is 
+000096e0: 6f6e 6c79 2073 7570 706f 7274 6564 2075  only supported u
+000096f0: 6e64 6572 2061 6e20 616c 6c6f 776c 6973  nder an allowlis
+00009700: 742e 0a20 2020 2020 2020 2020 2020 2073  t..            s
+00009710: 7472 6963 743d 5472 7565 2c0a 2020 2020  trict=True,.    
+00009720: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00009730: 2041 6464 206f 7264 6572 2063 6f6c 756d   Add order colum
+00009740: 6e20 746f 2070 616e 6461 7320 4461 7461  n to pandas Data
+00009750: 4672 616d 6520 746f 2070 7265 7365 7276  Frame to preserv
+00009760: 6520 6f72 6465 7220 696e 2042 6967 5175  e order in BigQu
+00009770: 6572 790a 2020 2020 2020 2020 6f72 6465  ery.        orde
+00009780: 7269 6e67 5f63 6f6c 203d 2022 726f 7769  ring_col = "rowi
+00009790: 6422 0a20 2020 2020 2020 2063 6f6c 756d  d".        colum
+000097a0: 6e73 203d 2066 726f 7a65 6e73 6574 2863  ns = frozenset(c
+000097b0: 6f6c 5f6c 6162 656c 7320 2b20 6964 785f  ol_labels + idx_
+000097c0: 6c61 6265 6c73 290a 2020 2020 2020 2020  labels).        
+000097d0: 7375 6666 6978 203d 2032 0a20 2020 2020  suffix = 2.     
+000097e0: 2020 2077 6869 6c65 206f 7264 6572 696e     while orderin
+000097f0: 675f 636f 6c20 696e 2063 6f6c 756d 6e73  g_col in columns
+00009800: 3a0a 2020 2020 2020 2020 2020 2020 6f72  :.            or
+00009810: 6465 7269 6e67 5f63 6f6c 203d 2066 2272  dering_col = f"r
+00009820: 6f77 6964 5f7b 7375 6666 6978 7d22 0a20  owid_{suffix}". 
+00009830: 2020 2020 2020 2020 2020 2073 7566 6669             suffi
+00009840: 7820 2b3d 2031 0a0a 2020 2020 2020 2020  x += 1..        
+00009850: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+00009860: 5f63 6f70 7920 3d20 7061 6e64 6173 5f64  _copy = pandas_d
+00009870: 6174 6166 7261 6d65 2e63 6f70 7928 290a  ataframe.copy().
+00009880: 2020 2020 2020 2020 7061 6e64 6173 5f64          pandas_d
+00009890: 6174 6166 7261 6d65 5f63 6f70 792e 696e  ataframe_copy.in
+000098a0: 6465 782e 6e61 6d65 7320 3d20 6e65 775f  dex.names = new_
+000098b0: 6964 785f 6964 730a 2020 2020 2020 2020  idx_ids.        
+000098c0: 7061 6e64 6173 5f64 6174 6166 7261 6d65  pandas_dataframe
+000098d0: 5f63 6f70 792e 636f 6c75 6d6e 7320 3d20  _copy.columns = 
+000098e0: 7061 6e64 6173 2e49 6e64 6578 286e 6577  pandas.Index(new
+000098f0: 5f63 6f6c 5f69 6473 290a 2020 2020 2020  _col_ids).      
+00009900: 2020 7061 6e64 6173 5f64 6174 6166 7261    pandas_datafra
+00009910: 6d65 5f63 6f70 795b 6f72 6465 7269 6e67  me_copy[ordering
+00009920: 5f63 6f6c 5d20 3d20 6e70 2e61 7261 6e67  _col] = np.arang
+00009930: 6528 7061 6e64 6173 5f64 6174 6166 7261  e(pandas_datafra
+00009940: 6d65 5f63 6f70 792e 7368 6170 655b 305d  me_copy.shape[0]
+00009950: 290a 0a20 2020 2020 2020 206a 6f62 5f63  )..        job_c
+00009960: 6f6e 6669 6720 3d20 7365 6c66 2e5f 7072  onfig = self._pr
+00009970: 6570 6172 655f 6c6f 6164 5f6a 6f62 5f63  epare_load_job_c
+00009980: 6f6e 6669 6728 290a 0a20 2020 2020 2020  onfig()..       
+00009990: 2023 2053 7065 6369 6679 2074 6865 2064   # Specify the d
+000099a0: 6174 6574 696d 6520 6474 7970 6573 2c20  atetime dtypes, 
+000099b0: 7768 6963 6820 6973 2061 7574 6f2d 6465  which is auto-de
+000099c0: 7465 6374 6564 2061 7320 7469 6d65 7374  tected as timest
+000099d0: 616d 7020 7479 7065 732e 0a20 2020 2020  amp types..     
+000099e0: 2020 2073 6368 656d 613a 206c 6973 745b     schema: list[
+000099f0: 6269 6771 7565 7279 2e53 6368 656d 6146  bigquery.SchemaF
+00009a00: 6965 6c64 5d20 3d20 5b5d 0a20 2020 2020  ield] = [].     
+00009a10: 2020 2066 6f72 2063 6f6c 756d 6e2c 2064     for column, d
+00009a20: 7479 7065 2069 6e20 7a69 7028 6e65 775f  type in zip(new_
+00009a30: 636f 6c5f 6964 732c 2070 616e 6461 735f  col_ids, pandas_
+00009a40: 6461 7461 6672 616d 652e 6474 7970 6573  dataframe.dtypes
+00009a50: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00009a60: 6620 6474 7970 6520 3d3d 2022 7469 6d65  f dtype == "time
+00009a70: 7374 616d 705b 7573 5d5b 7079 6172 726f  stamp[us][pyarro
+00009a80: 775d 223a 0a20 2020 2020 2020 2020 2020  w]":.           
+00009a90: 2020 2020 2073 6368 656d 612e 6170 7065       schema.appe
+00009aa0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+00009ab0: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+00009ac0: 2e53 6368 656d 6146 6965 6c64 2863 6f6c  .SchemaField(col
+00009ad0: 756d 6e2c 2062 6967 7175 6572 792e 656e  umn, bigquery.en
+00009ae0: 756d 732e 5371 6c54 7970 654e 616d 6573  ums.SqlTypeNames
+00009af0: 2e44 4154 4554 494d 4529 0a20 2020 2020  .DATETIME).     
+00009b00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00009b10: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+00009b20: 7363 6865 6d61 203d 2073 6368 656d 610a  schema = schema.
+00009b30: 0a20 2020 2020 2020 2023 2043 6c75 7374  .        # Clust
+00009b40: 6572 696e 6720 7072 6f62 6162 6c79 206e  ering probably n
+00009b50: 6f74 206e 6565 6465 6420 616e 7977 6179  ot needed anyway
+00009b60: 7320 6173 2070 616e 6461 7320 7461 626c  s as pandas tabl
+00009b70: 6573 2061 7265 2073 6d61 6c6c 0a20 2020  es are small.   
+00009b80: 2020 2020 2063 6c75 7374 6572 5f63 6f6c       cluster_col
+00009b90: 7320 3d20 5b6f 7264 6572 696e 675f 636f  s = [ordering_co
+00009ba0: 6c5d 0a20 2020 2020 2020 206a 6f62 5f63  l].        job_c
+00009bb0: 6f6e 6669 672e 636c 7573 7465 7269 6e67  onfig.clustering
+00009bc0: 5f66 6965 6c64 7320 3d20 636c 7573 7465  _fields = cluste
+00009bd0: 725f 636f 6c73 0a0a 2020 2020 2020 2020  r_cols..        
+00009be0: 6a6f 625f 636f 6e66 6967 2e6c 6162 656c  job_config.label
+00009bf0: 7320 3d20 7b22 6269 6766 7261 6d65 732d  s = {"bigframes-
+00009c00: 6170 6922 3a20 6170 695f 6e61 6d65 7d0a  api": api_name}.
+00009c10: 0a20 2020 2020 2020 206c 6f61 645f 7461  .        load_ta
+00009c20: 626c 655f 6465 7374 696e 6174 696f 6e20  ble_destination 
+00009c30: 3d20 7365 6c66 2e5f 7261 6e64 6f6d 5f74  = self._random_t
+00009c40: 6162 6c65 2829 0a20 2020 2020 2020 206c  able().        l
+00009c50: 6f61 645f 6a6f 6220 3d20 7365 6c66 2e62  oad_job = self.b
+00009c60: 7163 6c69 656e 742e 6c6f 6164 5f74 6162  qclient.load_tab
+00009c70: 6c65 5f66 726f 6d5f 6461 7461 6672 616d  le_from_datafram
+00009c80: 6528 0a20 2020 2020 2020 2020 2020 2070  e(.            p
+00009c90: 616e 6461 735f 6461 7461 6672 616d 655f  andas_dataframe_
+00009ca0: 636f 7079 2c0a 2020 2020 2020 2020 2020  copy,.          
+00009cb0: 2020 6c6f 6164 5f74 6162 6c65 5f64 6573    load_table_des
+00009cc0: 7469 6e61 7469 6f6e 2c0a 2020 2020 2020  tination,.      
+00009cd0: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+00009ce0: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
+00009cf0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00009d00: 656c 662e 5f73 7461 7274 5f67 656e 6572  elf._start_gener
+00009d10: 6963 5f6a 6f62 286c 6f61 645f 6a6f 6229  ic_job(load_job)
+00009d20: 0a0a 2020 2020 2020 2020 6f72 6465 7269  ..        orderi
+00009d30: 6e67 203d 206f 7264 6572 2e45 7870 7265  ng = order.Expre
+00009d40: 7373 696f 6e4f 7264 6572 696e 6728 0a20  ssionOrdering(. 
+00009d50: 2020 2020 2020 2020 2020 206f 7264 6572             order
+00009d60: 696e 675f 7661 6c75 655f 636f 6c75 6d6e  ing_value_column
+00009d70: 733d 7475 706c 6528 5b6f 7264 6572 2e61  s=tuple([order.a
+00009d80: 7363 656e 6469 6e67 5f6f 7665 7228 6f72  scending_over(or
+00009d90: 6465 7269 6e67 5f63 6f6c 295d 292c 0a20  dering_col)]),. 
+00009da0: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00009db0: 5f6f 7264 6572 696e 675f 636f 6c75 6d6e  _ordering_column
+00009dc0: 733d 6672 6f7a 656e 7365 7428 5b6f 7264  s=frozenset([ord
+00009dd0: 6572 696e 675f 636f 6c5d 292c 0a20 2020  ering_col]),.   
+00009de0: 2020 2020 2020 2020 2069 6e74 6567 6572           integer
+00009df0: 5f65 6e63 6f64 696e 673d 496e 7465 6765  _encoding=Intege
+00009e00: 7245 6e63 6f64 696e 6728 5472 7565 2c20  rEncoding(True, 
+00009e10: 6973 5f73 6571 7565 6e74 6961 6c3d 5472  is_sequential=Tr
+00009e20: 7565 292c 0a20 2020 2020 2020 2029 0a20  ue),.        ). 
+00009e30: 2020 2020 2020 2074 6162 6c65 5f65 7870         table_exp
+00009e40: 7265 7373 696f 6e20 3d20 7365 6c66 2e69  ression = self.i
+00009e50: 6269 735f 636c 6965 6e74 2e74 6162 6c65  bis_client.table
+00009e60: 2820 2023 2074 7970 653a 2069 676e 6f72  (  # type: ignor
+00009e70: 650a 2020 2020 2020 2020 2020 2020 6c6f  e.            lo
+00009e80: 6164 5f74 6162 6c65 5f64 6573 7469 6e61  ad_table_destina
+00009e90: 7469 6f6e 2e74 6162 6c65 5f69 642c 0a20  tion.table_id,. 
+00009ea0: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00009eb0: 613d 6c6f 6164 5f74 6162 6c65 5f64 6573  a=load_table_des
+00009ec0: 7469 6e61 7469 6f6e 2e64 6174 6173 6574  tination.dataset
+00009ed0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00009ee0: 2064 6174 6162 6173 653d 6c6f 6164 5f74   database=load_t
+00009ef0: 6162 6c65 5f64 6573 7469 6e61 7469 6f6e  able_destination
+00009f00: 2e70 726f 6a65 6374 2c0a 2020 2020 2020  .project,.      
+00009f10: 2020 290a 0a20 2020 2020 2020 2023 2062    )..        # b
+00009f20: 2f32 3937 3539 3031 3738 2050 6f74 656e  /297590178 Poten
+00009f30: 7469 616c 6c79 2061 2062 7567 2069 6e20  tially a bug in 
+00009f40: 6271 636c 6965 6e74 2e6c 6f61 645f 7461  bqclient.load_ta
+00009f50: 626c 655f 6672 6f6d 5f64 6174 6166 7261  ble_from_datafra
+00009f60: 6d65 2829 2c20 7468 6174 206f 6e6c 7920  me(), that only 
+00009f70: 7768 656e 2074 6865 2044 4620 6973 2065  when the DF is e
+00009f80: 6d70 7479 2c20 7468 6520 696e 6465 7820  mpty, the index 
+00009f90: 636f 6c75 6d6e 7320 6469 7361 7070 6561  columns disappea
+00009fa0: 7220 696e 2074 6162 6c65 5f65 7870 7265  r in table_expre
+00009fb0: 7373 696f 6e2e 0a20 2020 2020 2020 2069  ssion..        i
+00009fc0: 6620 616e 7928 0a20 2020 2020 2020 2020  f any(.         
+00009fd0: 2020 205b 6e65 775f 6964 785f 6964 206e     [new_idx_id n
+00009fe0: 6f74 2069 6e20 7461 626c 655f 6578 7072  ot in table_expr
+00009ff0: 6573 7369 6f6e 2e63 6f6c 756d 6e73 2066  ession.columns f
+0000a000: 6f72 206e 6577 5f69 6478 5f69 6420 696e  or new_idx_id in
+0000a010: 206e 6577 5f69 6478 5f69 6473 5d0a 2020   new_idx_ids].  
+0000a020: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000a030: 2020 2020 206e 6577 5f69 6478 5f69 6473       new_idx_ids
+0000a040: 2c20 6964 785f 6c61 6265 6c73 203d 205b  , idx_labels = [
+0000a050: 5d2c 205b 5d0a 0a20 2020 2020 2020 2063  ], []..        c
+0000a060: 6f6c 756d 6e5f 7661 6c75 6573 203d 205b  olumn_values = [
+0000a070: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+0000a080: 6c65 5f65 7870 7265 7373 696f 6e5b 636f  le_expression[co
+0000a090: 6c5d 0a20 2020 2020 2020 2020 2020 2066  l].            f
+0000a0a0: 6f72 2063 6f6c 2069 6e20 7461 626c 655f  or col in table_
+0000a0b0: 6578 7072 6573 7369 6f6e 2e63 6f6c 756d  expression.colum
+0000a0c0: 6e73 0a20 2020 2020 2020 2020 2020 2069  ns.            i
+0000a0d0: 6620 636f 6c20 213d 206f 7264 6572 696e  f col != orderin
+0000a0e0: 675f 636f 6c0a 2020 2020 2020 2020 5d0a  g_col.        ].
+0000a0f0: 2020 2020 2020 2020 6172 7261 795f 7661          array_va
+0000a100: 6c75 6520 3d20 636f 7265 2e41 7272 6179  lue = core.Array
+0000a110: 5661 6c75 652e 6672 6f6d 5f69 6269 7328  Value.from_ibis(
+0000a120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a130: 662c 0a20 2020 2020 2020 2020 2020 2074  f,.            t
+0000a140: 6162 6c65 5f65 7870 7265 7373 696f 6e2c  able_expression,
+0000a150: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+0000a160: 756d 6e73 3d63 6f6c 756d 6e5f 7661 6c75  umns=column_valu
+0000a170: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0000a180: 6869 6464 656e 5f6f 7264 6572 696e 675f  hidden_ordering_
+0000a190: 636f 6c75 6d6e 733d 5b74 6162 6c65 5f65  columns=[table_e
+0000a1a0: 7870 7265 7373 696f 6e5b 6f72 6465 7269  xpression[orderi
+0000a1b0: 6e67 5f63 6f6c 5d5d 2c0a 2020 2020 2020  ng_col]],.      
+0000a1c0: 2020 2020 2020 6f72 6465 7269 6e67 3d6f        ordering=o
+0000a1d0: 7264 6572 696e 672c 0a20 2020 2020 2020  rdering,.       
+0000a1e0: 2029 0a0a 2020 2020 2020 2020 626c 6f63   )..        bloc
+0000a1f0: 6b20 3d20 626c 6f63 6b73 2e42 6c6f 636b  k = blocks.Block
+0000a200: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
+0000a210: 7261 795f 7661 6c75 652c 0a20 2020 2020  ray_value,.     
+0000a220: 2020 2020 2020 2069 6e64 6578 5f63 6f6c         index_col
+0000a230: 756d 6e73 3d6e 6577 5f69 6478 5f69 6473  umns=new_idx_ids
+0000a240: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+0000a250: 6c75 6d6e 5f6c 6162 656c 733d 636f 6c5f  lumn_labels=col_
+0000a260: 696e 6465 782c 0a20 2020 2020 2020 2020  index,.         
+0000a270: 2020 2069 6e64 6578 5f6c 6162 656c 733d     index_labels=
+0000a280: 6964 785f 6c61 6265 6c73 2c0a 2020 2020  idx_labels,.    
+0000a290: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0000a2a0: 7475 726e 2064 6174 6166 7261 6d65 2e44  turn dataframe.D
+0000a2b0: 6174 6146 7261 6d65 2862 6c6f 636b 290a  ataFrame(block).
+0000a2c0: 0a20 2020 2064 6566 2072 6561 645f 6373  .    def read_cs
+0000a2d0: 7628 0a20 2020 2020 2020 2073 656c 662c  v(.        self,
+0000a2e0: 0a20 2020 2020 2020 2066 696c 6570 6174  .        filepat
+0000a2f0: 685f 6f72 5f62 7566 6665 723a 2073 7472  h_or_buffer: str
+0000a300: 207c 2049 4f5b 2262 7974 6573 225d 2c0a   | IO["bytes"],.
+0000a310: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000a320: 2020 2073 6570 3a20 4f70 7469 6f6e 616c     sep: Optional
+0000a330: 5b73 7472 5d20 3d20 222c 222c 0a20 2020  [str] = ",",.   
+0000a340: 2020 2020 2068 6561 6465 723a 204f 7074       header: Opt
+0000a350: 696f 6e61 6c5b 696e 745d 203d 2030 2c0a  ional[int] = 0,.
+0000a360: 2020 2020 2020 2020 6e61 6d65 733a 204f          names: O
+0000a370: 7074 696f 6e61 6c5b 0a20 2020 2020 2020  ptional[.       
+0000a380: 2020 2020 2055 6e69 6f6e 5b4d 7574 6162       Union[Mutab
+0000a390: 6c65 5365 7175 656e 6365 5b41 6e79 5d2c  leSequence[Any],
+0000a3a0: 206e 702e 6e64 6172 7261 795b 416e 792c   np.ndarray[Any,
+0000a3b0: 2041 6e79 5d2c 2054 7570 6c65 5b41 6e79   Any], Tuple[Any
+0000a3c0: 2c20 2e2e 2e5d 2c20 7261 6e67 655d 0a20  , ...], range]. 
+0000a3d0: 2020 2020 2020 205d 203d 204e 6f6e 652c         ] = None,
+0000a3e0: 0a20 2020 2020 2020 2069 6e64 6578 5f63  .        index_c
+0000a3f0: 6f6c 3a20 4f70 7469 6f6e 616c 5b0a 2020  ol: Optional[.  
+0000a400: 2020 2020 2020 2020 2020 556e 696f 6e5b            Union[
+0000a410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a420: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
+0000a430: 2020 2020 2020 7374 722c 0a20 2020 2020        str,.     
+0000a440: 2020 2020 2020 2020 2020 2053 6571 7565             Seque
+0000a450: 6e63 655b 556e 696f 6e5b 7374 722c 2069  nce[Union[str, i
+0000a460: 6e74 5d5d 2c0a 2020 2020 2020 2020 2020  nt]],.          
+0000a470: 2020 2020 2020 6269 6766 7261 6d65 732e        bigframes.
+0000a480: 656e 756d 732e 4465 6661 756c 7449 6e64  enums.DefaultInd
+0000a490: 6578 4b69 6e64 2c0a 2020 2020 2020 2020  exKind,.        
+0000a4a0: 2020 2020 2020 2020 4c69 7465 7261 6c5b          Literal[
+0000a4b0: 4661 6c73 655d 2c0a 2020 2020 2020 2020  False],.        
+0000a4c0: 2020 2020 5d0a 2020 2020 2020 2020 5d20      ].        ] 
+0000a4d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000a4e0: 7573 6563 6f6c 733a 204f 7074 696f 6e61  usecols: Optiona
+0000a4f0: 6c5b 0a20 2020 2020 2020 2020 2020 2055  l[.            U
+0000a500: 6e69 6f6e 5b0a 2020 2020 2020 2020 2020  nion[.          
+0000a510: 2020 2020 2020 4d75 7461 626c 6553 6571        MutableSeq
+0000a520: 7565 6e63 655b 7374 725d 2c0a 2020 2020  uence[str],.    
+0000a530: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+0000a540: 655b 7374 722c 202e 2e2e 5d2c 0a20 2020  e[str, ...],.   
+0000a550: 2020 2020 2020 2020 2020 2020 2053 6571               Seq
+0000a560: 7565 6e63 655b 696e 745d 2c0a 2020 2020  uence[int],.    
+0000a570: 2020 2020 2020 2020 2020 2020 7061 6e64              pand
+0000a580: 6173 2e53 6572 6965 732c 0a20 2020 2020  as.Series,.     
+0000a590: 2020 2020 2020 2020 2020 2070 616e 6461             panda
+0000a5a0: 732e 496e 6465 782c 0a20 2020 2020 2020  s.Index,.       
+0000a5b0: 2020 2020 2020 2020 206e 702e 6e64 6172           np.ndar
+0000a5c0: 7261 795b 416e 792c 2041 6e79 5d2c 0a20  ray[Any, Any],. 
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+0000a5e0: 616c 6c61 626c 655b 5b41 6e79 5d2c 2062  allable[[Any], b
+0000a5f0: 6f6f 6c5d 2c0a 2020 2020 2020 2020 2020  ool],.          
+0000a600: 2020 5d0a 2020 2020 2020 2020 5d20 3d20    ].        ] = 
+0000a610: 4e6f 6e65 2c0a 2020 2020 2020 2020 6474  None,.        dt
+0000a620: 7970 653a 204f 7074 696f 6e61 6c5b 4469  ype: Optional[Di
+0000a630: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
+0000a640: 2020 2020 656e 6769 6e65 3a20 4f70 7469      engine: Opti
+0000a650: 6f6e 616c 5b0a 2020 2020 2020 2020 2020  onal[.          
+0000a660: 2020 4c69 7465 7261 6c5b 2263 222c 2022    Literal["c", "
+0000a670: 7079 7468 6f6e 222c 2022 7079 6172 726f  python", "pyarro
+0000a680: 7722 2c20 2270 7974 686f 6e2d 6677 6622  w", "python-fwf"
+0000a690: 2c20 2262 6967 7175 6572 7922 5d0a 2020  , "bigquery"].  
+0000a6a0: 2020 2020 2020 5d20 3d20 4e6f 6e65 2c0a        ] = None,.
+0000a6b0: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
+0000a6c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000a6d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000a6e0: 2a2a 6b77 6172 6773 2c0a 2020 2020 2920  **kwargs,.    ) 
+0000a6f0: 2d3e 2064 6174 6166 7261 6d65 2e44 6174  -> dataframe.Dat
+0000a700: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+0000a710: 7461 626c 6520 3d20 7365 6c66 2e5f 7261  table = self._ra
+0000a720: 6e64 6f6d 5f74 6162 6c65 2829 0a0a 2020  ndom_table()..  
+0000a730: 2020 2020 2020 6966 2065 6e67 696e 6520        if engine 
+0000a740: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+0000a750: 656e 6769 6e65 203d 3d20 2262 6967 7175  engine == "bigqu
+0000a760: 6572 7922 3a0a 2020 2020 2020 2020 2020  ery":.          
+0000a770: 2020 6966 2061 6e79 2870 6172 616d 2069    if any(param i
+0000a780: 7320 6e6f 7420 4e6f 6e65 2066 6f72 2070  s not None for p
+0000a790: 6172 616d 2069 6e20 2864 7479 7065 2c20  aram in (dtype, 
+0000a7a0: 6e61 6d65 7329 293a 0a20 2020 2020 2020  names)):.       
+0000a7b0: 2020 2020 2020 2020 206e 6f74 5f73 7570           not_sup
+0000a7c0: 706f 7274 6564 203d 2028 2264 7479 7065  ported = ("dtype
+0000a7d0: 222c 2022 6e61 6d65 7322 290a 2020 2020  ", "names").    
+0000a7e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000a7f0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000a800: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000a810: 2020 2020 2020 2020 2020 2066 2242 6967             f"Big
+0000a820: 5175 6572 7920 656e 6769 6e65 2064 6f65  Query engine doe
+0000a830: 7320 6e6f 7420 7375 7070 6f72 7420 7468  s not support th
+0000a840: 6573 6520 6172 6775 6d65 6e74 733a 207b  ese arguments: {
+0000a850: 6e6f 745f 7375 7070 6f72 7465 647d 2e20  not_supported}. 
+0000a860: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000a870: 2020 2020 2020 6622 7b63 6f6e 7374 616e        f"{constan
+0000a880: 7473 2e46 4545 4442 4143 4b5f 4c49 4e4b  ts.FEEDBACK_LINK
+0000a890: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000a8a0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0000a8b0: 2020 2320 544f 444f 2862 2f33 3338 3038    # TODO(b/33808
+0000a8c0: 3936 3539 293a 204c 6f6f 6b73 206c 696b  9659): Looks lik
+0000a8d0: 6520 7765 2063 616e 2072 656c 6178 2074  e we can relax t
+0000a8e0: 6869 7320 3120 636f 6c75 6d6e 0a20 2020  his 1 column.   
+0000a8f0: 2020 2020 2020 2020 2023 2072 6573 7472           # restr
+0000a900: 6963 7469 6f6e 2069 6620 7765 2063 6865  iction if we che
+0000a910: 636b 2074 6865 2063 6f6e 7465 6e74 7320  ck the contents 
+0000a920: 6f66 2061 6e20 6974 6572 6162 6c65 2061  of an iterable a
+0000a930: 7265 2073 7472 696e 6773 0a20 2020 2020  re strings.     
+0000a940: 2020 2020 2020 2023 206e 6f74 2069 6e74         # not int
+0000a950: 6567 6572 732e 0a20 2020 2020 2020 2020  egers..         
+0000a960: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+0000a970: 2020 2020 2020 2020 2320 456d 7074 7920          # Empty 
+0000a980: 7475 706c 6573 2c20 4e6f 6e65 2c20 616e  tuples, None, an
+0000a990: 6420 4661 6c73 6520 6172 6520 616c 6c6f  d False are allo
+0000a9a0: 7765 6420 616e 6420 6661 6c73 6579 2e0a  wed and falsey..
+0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9c0: 696e 6465 785f 636f 6c0a 2020 2020 2020  index_col.      
+0000a9d0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0000a9e0: 7420 6973 696e 7374 616e 6365 2869 6e64  t isinstance(ind
+0000a9f0: 6578 5f63 6f6c 2c20 6269 6766 7261 6d65  ex_col, bigframe
+0000aa00: 732e 656e 756d 732e 4465 6661 756c 7449  s.enums.DefaultI
+0000aa10: 6e64 6578 4b69 6e64 290a 2020 2020 2020  ndexKind).      
+0000aa20: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0000aa30: 7420 6973 696e 7374 616e 6365 2869 6e64  t isinstance(ind
+0000aa40: 6578 5f63 6f6c 2c20 7374 7229 0a20 2020  ex_col, str).   
+0000aa50: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000aa60: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000aa70: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000aa80: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000aa90: 2020 2020 2020 2020 2020 2022 4269 6751             "BigQ
+0000aaa0: 7565 7279 2065 6e67 696e 6520 6f6e 6c79  uery engine only
+0000aab0: 2073 7570 706f 7274 7320 6120 7369 6e67   supports a sing
+0000aac0: 6c65 2063 6f6c 756d 6e20 6e61 6d65 2066  le column name f
+0000aad0: 6f72 2060 696e 6465 785f 636f 6c60 2c20  or `index_col`, 
+0000aae0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000aaf0: 2020 2020 2020 6622 676f 743a 207b 7265        f"got: {re
+0000ab00: 7072 2869 6e64 6578 5f63 6f6c 297d 2e20  pr(index_col)}. 
+0000ab10: 7b63 6f6e 7374 616e 7473 2e46 4545 4442  {constants.FEEDB
+0000ab20: 4143 4b5f 4c49 4e4b 7d22 0a20 2020 2020  ACK_LINK}".     
+0000ab30: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000ab40: 2020 2020 2020 2020 2020 2320 4e6f 6e65            # None
+0000ab50: 2061 6e64 2046 616c 7365 2063 616e 6e6f   and False canno
+0000ab60: 7420 6265 2070 6173 7365 6420 746f 2072  t be passed to r
+0000ab70: 6561 645f 6762 712e 0a20 2020 2020 2020  ead_gbq..       
+0000ab80: 2020 2020 2023 2054 4f44 4f28 622f 3333       # TODO(b/33
+0000ab90: 3834 3030 3133 3329 3a20 5768 656e 2069  8400133): When i
+0000aba0: 6e64 6578 5f63 6f6c 2069 7320 4e6f 6e65  ndex_col is None
+0000abb0: 2c20 7765 2073 686f 756c 6420 6265 2075  , we should be u
+0000abc0: 7369 6e67 2074 6865 0a20 2020 2020 2020  sing the.       
+0000abd0: 2020 2020 2023 2066 6972 7374 2063 6f6c       # first col
+0000abe0: 756d 6e20 6f66 2074 6865 2043 5356 2061  umn of the CSV a
+0000abf0: 7320 7468 6520 696e 6465 7820 746f 2062  s the index to b
+0000ac00: 6520 636f 6d70 6174 6962 6c65 2077 6974  e compatible wit
+0000ac10: 6820 7468 650a 2020 2020 2020 2020 2020  h the.          
+0000ac20: 2020 2320 7061 6e64 6173 2065 6e67 696e    # pandas engin
+0000ac30: 652e 2041 6363 6f72 6469 6e67 2074 6f20  e. According to 
+0000ac40: 7468 6520 7061 6e64 6173 2064 6f63 732c  the pandas docs,
+0000ac50: 206f 6e6c 7920 2246 616c 7365 220a 2020   only "False".  
+0000ac60: 2020 2020 2020 2020 2020 2320 696e 6469            # indi
+0000ac70: 6361 7465 7320 6120 6465 6661 756c 7420  cates a default 
+0000ac80: 7365 7175 656e 7469 616c 2069 6e64 6578  sequential index
+0000ac90: 2e0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000aca0: 206e 6f74 2069 6e64 6578 5f63 6f6c 3a0a   not index_col:.
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 696e 6465 785f 636f 6c20 3d20 2829 0a0a  index_col = ()..
+0000acd0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000ace0: 785f 636f 6c20 3d20 7479 7069 6e67 2e63  x_col = typing.c
+0000acf0: 6173 7428 0a20 2020 2020 2020 2020 2020  ast(.           
+0000ad00: 2020 2020 2055 6e69 6f6e 5b0a 2020 2020       Union[.    
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad20: 5365 7175 656e 6365 5b73 7472 5d2c 2020  Sequence[str],  
+0000ad30: 2320 4661 6c73 6579 2076 616c 7565 730a  # Falsey values.
+0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad50: 2020 2020 6269 6766 7261 6d65 732e 656e      bigframes.en
+0000ad60: 756d 732e 4465 6661 756c 7449 6e64 6578  ums.DefaultIndex
+0000ad70: 4b69 6e64 2c0a 2020 2020 2020 2020 2020  Kind,.          
+0000ad80: 2020 2020 2020 2020 2020 7374 722c 0a20            str,. 
+0000ad90: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000ada0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000adb0: 2020 696e 6465 785f 636f 6c2c 0a20 2020    index_col,.   
+0000adc0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000add0: 2020 2020 2020 2020 2320 7573 6563 6f6c          # usecol
+0000ade0: 7320 7368 6f75 6c64 206f 6e6c 7920 6265  s should only be
+0000adf0: 2061 6e20 6974 6572 6162 6c65 206f 6620   an iterable of 
+0000ae00: 7374 7269 6e67 7320 2863 6f6c 756d 6e20  strings (column 
+0000ae10: 6e61 6d65 7329 2066 6f72 2075 7365 2061  names) for use a
+0000ae20: 7320 636f 6c75 6d6e 7320 696e 2072 6561  s columns in rea
+0000ae30: 645f 6762 712e 0a20 2020 2020 2020 2020  d_gbq..         
+0000ae40: 2020 2063 6f6c 756d 6e73 3a20 5475 706c     columns: Tupl
+0000ae50: 655b 416e 792c 202e 2e2e 5d20 3d20 7475  e[Any, ...] = tu
+0000ae60: 706c 6528 290a 2020 2020 2020 2020 2020  ple().          
+0000ae70: 2020 6966 2075 7365 636f 6c73 2069 7320    if usecols is 
+0000ae80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ae90: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000aea0: 6e73 7461 6e63 6528 7573 6563 6f6c 732c  nstance(usecols,
+0000aeb0: 2049 7465 7261 626c 6529 2061 6e64 2061   Iterable) and a
+0000aec0: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
+0000aed0: 2020 2020 2020 2020 6973 696e 7374 616e          isinstan
+0000aee0: 6365 2863 6f6c 2c20 7374 7229 2066 6f72  ce(col, str) for
+0000aef0: 2063 6f6c 2069 6e20 7573 6563 6f6c 730a   col in usecols.
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000af20: 2020 2020 2020 2063 6f6c 756d 6e73 203d         columns =
+0000af30: 2074 7570 6c65 2863 6f6c 2066 6f72 2063   tuple(col for c
+0000af40: 6f6c 2069 6e20 7573 6563 6f6c 7329 0a20  ol in usecols). 
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000af60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000af70: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+0000af80: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+0000af90: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000afa0: 2020 2020 2020 2020 2020 2020 2242 6967              "Big
+0000afb0: 5175 6572 7920 656e 6769 6e65 206f 6e6c  Query engine onl
+0000afc0: 7920 7375 7070 6f72 7473 2061 6e20 6974  y supports an it
+0000afd0: 6572 6162 6c65 206f 6620 7374 7269 6e67  erable of string
+0000afe0: 7320 666f 7220 6075 7365 636f 6c73 602e  s for `usecols`.
+0000aff0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000b000: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
+0000b010: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
+0000b020: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
+0000b030: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000b040: 2020 2020 2020 2020 2020 2069 6620 656e             if en
+0000b050: 636f 6469 6e67 2069 7320 6e6f 7420 4e6f  coding is not No
+0000b060: 6e65 2061 6e64 2065 6e63 6f64 696e 6720  ne and encoding 
+0000b070: 6e6f 7420 696e 205f 5641 4c49 445f 454e  not in _VALID_EN
+0000b080: 434f 4449 4e47 533a 0a20 2020 2020 2020  CODINGS:.       
+0000b090: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
+0000b0a0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+0000b0b0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000b0c0: 2020 2020 2020 2020 6622 4269 6751 7565          f"BigQue
+0000b0d0: 7279 2065 6e67 696e 6520 6f6e 6c79 2073  ry engine only s
+0000b0e0: 7570 706f 7274 7320 7468 6520 666f 6c6c  upports the foll
+0000b0f0: 6f77 696e 6720 656e 636f 6469 6e67 733a  owing encodings:
+0000b100: 207b 5f56 414c 4944 5f45 4e43 4f44 494e   {_VALID_ENCODIN
+0000b110: 4753 7d2e 2022 0a20 2020 2020 2020 2020  GS}. ".         
+0000b120: 2020 2020 2020 2020 2020 2066 227b 636f             f"{co
+0000b130: 6e73 7461 6e74 732e 4645 4544 4241 434b  nstants.FEEDBACK
+0000b140: 5f4c 494e 4b7d 220a 2020 2020 2020 2020  _LINK}".        
+0000b150: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000b160: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+0000b170: 6720 3d20 7365 6c66 2e5f 7072 6570 6172  g = self._prepar
+0000b180: 655f 6c6f 6164 5f6a 6f62 5f63 6f6e 6669  e_load_job_confi
+0000b190: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+0000b1a0: 6a6f 625f 636f 6e66 6967 2e63 7265 6174  job_config.creat
+0000b1b0: 655f 6469 7370 6f73 6974 696f 6e20 3d20  e_disposition = 
+0000b1c0: 6269 6771 7565 7279 2e43 7265 6174 6544  bigquery.CreateD
+0000b1d0: 6973 706f 7369 7469 6f6e 2e43 5245 4154  isposition.CREAT
+0000b1e0: 455f 4946 5f4e 4545 4445 440a 2020 2020  E_IF_NEEDED.    
+0000b1f0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000b200: 6967 2e73 6f75 7263 655f 666f 726d 6174  ig.source_format
+0000b210: 203d 2062 6967 7175 6572 792e 536f 7572   = bigquery.Sour
+0000b220: 6365 466f 726d 6174 2e43 5356 0a20 2020  ceFormat.CSV.   
+0000b230: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000b240: 6669 672e 7772 6974 655f 6469 7370 6f73  fig.write_dispos
+0000b250: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
+0000b260: 2e57 7269 7465 4469 7370 6f73 6974 696f  .WriteDispositio
+0000b270: 6e2e 5752 4954 455f 454d 5054 590a 2020  n.WRITE_EMPTY.  
+0000b280: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+0000b290: 6e66 6967 2e61 7574 6f64 6574 6563 7420  nfig.autodetect 
+0000b2a0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+0000b2b0: 2020 206a 6f62 5f63 6f6e 6669 672e 6669     job_config.fi
+0000b2c0: 656c 645f 6465 6c69 6d69 7465 7220 3d20  eld_delimiter = 
+0000b2d0: 7365 700a 2020 2020 2020 2020 2020 2020  sep.            
+0000b2e0: 6a6f 625f 636f 6e66 6967 2e65 6e63 6f64  job_config.encod
+0000b2f0: 696e 6720 3d20 656e 636f 6469 6e67 0a20  ing = encoding. 
+0000b300: 2020 2020 2020 2020 2020 206a 6f62 5f63             job_c
+0000b310: 6f6e 6669 672e 6c61 6265 6c73 203d 207b  onfig.labels = {
+0000b320: 2262 6967 6672 616d 6573 2d61 7069 223a  "bigframes-api":
+0000b330: 2022 7265 6164 5f63 7376 227d 0a0a 2020   "read_csv"}..  
+0000b340: 2020 2020 2020 2020 2020 2320 5765 2077            # We w
+0000b350: 616e 7420 746f 206d 6174 6368 2070 616e  ant to match pan
+0000b360: 6461 7320 6265 6861 7669 6f72 2e20 4966  das behavior. If
+0000b370: 2068 6561 6465 7220 6973 2030 2c20 6e6f   header is 0, no
+0000b380: 2072 6f77 7320 7368 6f75 6c64 2062 6520   rows should be 
+0000b390: 736b 6970 7065 642c 2073 6f20 7765 0a20  skipped, so we. 
+0000b3a0: 2020 2020 2020 2020 2020 2023 2064 6f20             # do 
+0000b3b0: 6e6f 7420 6e65 6564 2074 6f20 7365 7420  not need to set 
+0000b3c0: 6073 6b69 705f 6c65 6164 696e 675f 726f  `skip_leading_ro
+0000b3d0: 7773 602e 2049 6620 6865 6164 6572 2069  ws`. If header i
+0000b3e0: 7320 4e6f 6e65 2c20 7468 656e 2074 6865  s None, then the
+0000b3f0: 7265 2069 7320 6e6f 2068 6561 6465 722e  re is no header.
+0000b400: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
+0000b410: 6574 7469 6e67 2073 6b69 705f 6c65 6164  etting skip_lead
+0000b420: 696e 675f 726f 7773 2074 6f20 3020 646f  ing_rows to 0 do
+0000b430: 6573 2074 6861 742e 2049 6620 6865 6164  es that. If head
+0000b440: 6572 3d4e 2061 6e64 204e 3e30 2c20 7765  er=N and N>0, we
+0000b450: 2077 616e 7420 746f 2073 6b69 7020 4e20   want to skip N 
+0000b460: 726f 7773 2e0a 2020 2020 2020 2020 2020  rows..          
+0000b470: 2020 6966 2068 6561 6465 7220 6973 204e    if header is N
+0000b480: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b490: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+0000b4a0: 736b 6970 5f6c 6561 6469 6e67 5f72 6f77  skip_leading_row
+0000b4b0: 7320 3d20 300a 2020 2020 2020 2020 2020  s = 0.          
+0000b4c0: 2020 656c 6966 2068 6561 6465 7220 3e20    elif header > 
+0000b4d0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000b4e0: 2020 206a 6f62 5f63 6f6e 6669 672e 736b     job_config.sk
+0000b4f0: 6970 5f6c 6561 6469 6e67 5f72 6f77 7320  ip_leading_rows 
+0000b500: 3d20 6865 6164 6572 0a0a 2020 2020 2020  = header..      
+0000b510: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000b520: 662e 5f72 6561 645f 6269 6771 7565 7279  f._read_bigquery
+0000b530: 5f6c 6f61 645f 6a6f 6228 0a20 2020 2020  _load_job(.     
+0000b540: 2020 2020 2020 2020 2020 2066 696c 6570             filep
+0000b550: 6174 685f 6f72 5f62 7566 6665 722c 0a20  ath_or_buffer,. 
+0000b560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000b570: 6162 6c65 2c0a 2020 2020 2020 2020 2020  able,.          
+0000b580: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+0000b590: 3d6a 6f62 5f63 6f6e 6669 672c 0a20 2020  =job_config,.   
+0000b5a0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000b5b0: 6578 5f63 6f6c 3d69 6e64 6578 5f63 6f6c  ex_col=index_col
+0000b5c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b5d0: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
+0000b5e0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0000b5f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000b600: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000b610: 696e 7374 616e 6365 2869 6e64 6578 5f63  instance(index_c
+0000b620: 6f6c 2c20 6269 6766 7261 6d65 732e 656e  ol, bigframes.en
+0000b630: 756d 732e 4465 6661 756c 7449 6e64 6578  ums.DefaultIndex
+0000b640: 4b69 6e64 293a 0a20 2020 2020 2020 2020  Kind):.         
+0000b650: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+0000b660: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+0000b670: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000b680: 2020 2020 2020 6622 5769 7468 2069 6e64        f"With ind
+0000b690: 6578 5f63 6f6c 3d7b 7265 7072 2869 6e64  ex_col={repr(ind
+0000b6a0: 6578 5f63 6f6c 297d 2c20 6f6e 6c79 2065  ex_col)}, only e
+0000b6b0: 6e67 696e 653d 2762 6967 7175 6572 7927  ngine='bigquery'
+0000b6c0: 2069 7320 7375 7070 6f72 7465 642e 2022   is supported. "
+0000b6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6e0: 2020 2020 2066 227b 636f 6e73 7461 6e74       f"{constant
+0000b6f0: 732e 4645 4544 4241 434b 5f4c 494e 4b7d  s.FEEDBACK_LINK}
+0000b700: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000b710: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000b720: 6966 2061 6e79 2861 7267 2069 6e20 6b77  if any(arg in kw
+0000b730: 6172 6773 2066 6f72 2061 7267 2069 6e20  args for arg in 
+0000b740: 2822 6368 756e 6b73 697a 6522 2c20 2269  ("chunksize", "i
+0000b750: 7465 7261 746f 7222 2929 3a0a 2020 2020  terator")):.    
+0000b760: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000b770: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+0000b780: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000b790: 2020 2020 2020 2020 2020 2022 2763 6875             "'chu
+0000b7a0: 6e6b 7369 7a65 2720 616e 6420 2769 7465  nksize' and 'ite
+0000b7b0: 7261 746f 7227 2061 7267 756d 656e 7473  rator' arguments
+0000b7c0: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
+0000b7d0: 6564 2e20 220a 2020 2020 2020 2020 2020  ed. ".          
+0000b7e0: 2020 2020 2020 2020 2020 6622 7b63 6f6e            f"{con
+0000b7f0: 7374 616e 7473 2e46 4545 4442 4143 4b5f  stants.FEEDBACK_
+0000b800: 4c49 4e4b 7d22 0a20 2020 2020 2020 2020  LINK}".         
+0000b810: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000b820: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000b830: 6e63 6528 6669 6c65 7061 7468 5f6f 725f  nce(filepath_or_
+0000b840: 6275 6666 6572 2c20 7374 7229 3a0a 2020  buffer, str):.  
+0000b850: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b860: 6c66 2e5f 6368 6563 6b5f 6669 6c65 5f73  lf._check_file_s
+0000b870: 697a 6528 6669 6c65 7061 7468 5f6f 725f  ize(filepath_or_
+0000b880: 6275 6666 6572 290a 2020 2020 2020 2020  buffer).        
+0000b890: 2020 2020 7061 6e64 6173 5f64 6620 3d20      pandas_df = 
+0000b8a0: 7061 6e64 6173 2e72 6561 645f 6373 7628  pandas.read_csv(
+0000b8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b8c0: 2066 696c 6570 6174 685f 6f72 5f62 7566   filepath_or_buf
+0000b8d0: 6665 722c 0a20 2020 2020 2020 2020 2020  fer,.           
+0000b8e0: 2020 2020 2073 6570 3d73 6570 2c0a 2020       sep=sep,.  
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 6865                he
+0000b900: 6164 6572 3d68 6561 6465 722c 0a20 2020  ader=header,.   
+0000b910: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0000b920: 6573 3d6e 616d 6573 2c0a 2020 2020 2020  es=names,.      
+0000b930: 2020 2020 2020 2020 2020 696e 6465 785f            index_
+0000b940: 636f 6c3d 696e 6465 785f 636f 6c2c 0a20  col=index_col,. 
+0000b950: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0000b960: 7365 636f 6c73 3d75 7365 636f 6c73 2c20  secols=usecols, 
+0000b970: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
+0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b990: 6474 7970 653d 6474 7970 652c 0a20 2020  dtype=dtype,.   
+0000b9a0: 2020 2020 2020 2020 2020 2020 2065 6e67               eng
+0000b9b0: 696e 653d 656e 6769 6e65 2c0a 2020 2020  ine=engine,.    
+0000b9c0: 2020 2020 2020 2020 2020 2020 656e 636f              enco
+0000b9d0: 6469 6e67 3d65 6e63 6f64 696e 672c 0a20  ding=encoding,. 
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000b9f0: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
+0000ba00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000ba10: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000ba20: 7265 6164 5f70 616e 6461 7328 7061 6e64  read_pandas(pand
+0000ba30: 6173 5f64 662c 2022 7265 6164 5f63 7376  as_df, "read_csv
+0000ba40: 2229 2020 2320 7479 7065 3a20 6967 6e6f  ")  # type: igno
+0000ba50: 7265 0a0a 2020 2020 6465 6620 7265 6164  re..    def read
+0000ba60: 5f70 6963 6b6c 6528 0a20 2020 2020 2020  _pickle(.       
+0000ba70: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+0000ba80: 696c 6570 6174 685f 6f72 5f62 7566 6665  ilepath_or_buffe
+0000ba90: 723a 2046 696c 6550 6174 6820 7c20 5265  r: FilePath | Re
+0000baa0: 6164 5069 636b 6c65 4275 6666 6572 2c0a  adPickleBuffer,.
+0000bab0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
+0000bac0: 696f 6e3a 2043 6f6d 7072 6573 7369 6f6e  ion: Compression
+0000bad0: 4f70 7469 6f6e 7320 3d20 2269 6e66 6572  Options = "infer
+0000bae0: 222c 0a20 2020 2020 2020 2073 746f 7261  ",.        stora
+0000baf0: 6765 5f6f 7074 696f 6e73 3a20 5374 6f72  ge_options: Stor
+0000bb00: 6167 654f 7074 696f 6e73 203d 204e 6f6e  ageOptions = Non
+0000bb10: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+0000bb20: 2020 7061 6e64 6173 5f6f 626a 203d 2070    pandas_obj = p
+0000bb30: 616e 6461 732e 7265 6164 5f70 6963 6b6c  andas.read_pickl
+0000bb40: 6528 0a20 2020 2020 2020 2020 2020 2066  e(.            f
+0000bb50: 696c 6570 6174 685f 6f72 5f62 7566 6665  ilepath_or_buffe
+0000bb60: 722c 0a20 2020 2020 2020 2020 2020 2063  r,.            c
+0000bb70: 6f6d 7072 6573 7369 6f6e 3d63 6f6d 7072  ompression=compr
+0000bb80: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
+0000bb90: 2020 2020 7374 6f72 6167 655f 6f70 7469      storage_opti
+0000bba0: 6f6e 733d 7374 6f72 6167 655f 6f70 7469  ons=storage_opti
+0000bbb0: 6f6e 732c 0a20 2020 2020 2020 2029 0a0a  ons,.        )..
+0000bbc0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000bbd0: 7461 6e63 6528 7061 6e64 6173 5f6f 626a  tance(pandas_obj
+0000bbe0: 2c20 7061 6e64 6173 2e53 6572 6965 7329  , pandas.Series)
+0000bbf0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000bc00: 2070 616e 6461 735f 6f62 6a2e 6e61 6d65   pandas_obj.name
+0000bc10: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000bc20: 2020 2020 2020 2020 2020 7061 6e64 6173            pandas
+0000bc30: 5f6f 626a 2e6e 616d 6520 3d20 2230 220a  _obj.name = "0".
+0000bc40: 2020 2020 2020 2020 2020 2020 6269 6766              bigf
+0000bc50: 7261 6d65 735f 6466 203d 2073 656c 662e  rames_df = self.
+0000bc60: 5f72 6561 645f 7061 6e64 6173 2870 616e  _read_pandas(pan
+0000bc70: 6461 735f 6f62 6a2e 746f 5f66 7261 6d65  das_obj.to_frame
+0000bc80: 2829 2c20 2272 6561 645f 7069 636b 6c65  (), "read_pickle
+0000bc90: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+0000bca0: 6574 7572 6e20 6269 6766 7261 6d65 735f  eturn bigframes_
+0000bcb0: 6466 5b62 6967 6672 616d 6573 5f64 662e  df[bigframes_df.
+0000bcc0: 636f 6c75 6d6e 735b 305d 5d0a 2020 2020  columns[0]].    
+0000bcd0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000bce0: 5f72 6561 645f 7061 6e64 6173 2870 616e  _read_pandas(pan
+0000bcf0: 6461 735f 6f62 6a2c 2022 7265 6164 5f70  das_obj, "read_p
+0000bd00: 6963 6b6c 6522 290a 0a20 2020 2064 6566  ickle")..    def
+0000bd10: 2072 6561 645f 7061 7271 7565 7428 0a20   read_parquet(. 
+0000bd20: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000bd30: 2020 2020 2070 6174 683a 2073 7472 207c       path: str |
+0000bd40: 2049 4f5b 2262 7974 6573 225d 2c0a 2020   IO["bytes"],.  
+0000bd50: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+0000bd60: 2065 6e67 696e 653a 2073 7472 203d 2022   engine: str = "
+0000bd70: 6175 746f 222c 0a20 2020 2029 202d 3e20  auto",.    ) -> 
+0000bd80: 6461 7461 6672 616d 652e 4461 7461 4672  dataframe.DataFr
+0000bd90: 616d 653a 0a20 2020 2020 2020 2074 6162  ame:.        tab
+0000bda0: 6c65 203d 2073 656c 662e 5f72 616e 646f  le = self._rando
+0000bdb0: 6d5f 7461 626c 6528 290a 0a20 2020 2020  m_table()..     
+0000bdc0: 2020 2069 6620 656e 6769 6e65 203d 3d20     if engine == 
+0000bdd0: 2262 6967 7175 6572 7922 3a0a 2020 2020  "bigquery":.    
+0000bde0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+0000bdf0: 6967 203d 2073 656c 662e 5f70 7265 7061  ig = self._prepa
+0000be00: 7265 5f6c 6f61 645f 6a6f 625f 636f 6e66  re_load_job_conf
+0000be10: 6967 2829 0a20 2020 2020 2020 2020 2020  ig().           
+0000be20: 206a 6f62 5f63 6f6e 6669 672e 6372 6561   job_config.crea
+0000be30: 7465 5f64 6973 706f 7369 7469 6f6e 203d  te_disposition =
+0000be40: 2062 6967 7175 6572 792e 4372 6561 7465   bigquery.Create
+0000be50: 4469 7370 6f73 6974 696f 6e2e 4352 4541  Disposition.CREA
+0000be60: 5445 5f49 465f 4e45 4544 4544 0a20 2020  TE_IF_NEEDED.   
+0000be70: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000be80: 6669 672e 736f 7572 6365 5f66 6f72 6d61  fig.source_forma
+0000be90: 7420 3d20 6269 6771 7565 7279 2e53 6f75  t = bigquery.Sou
+0000bea0: 7263 6546 6f72 6d61 742e 5041 5251 5545  rceFormat.PARQUE
+0000beb0: 540a 2020 2020 2020 2020 2020 2020 6a6f  T.            jo
+0000bec0: 625f 636f 6e66 6967 2e77 7269 7465 5f64  b_config.write_d
+0000bed0: 6973 706f 7369 7469 6f6e 203d 2062 6967  isposition = big
+0000bee0: 7175 6572 792e 5772 6974 6544 6973 706f  query.WriteDispo
+0000bef0: 7369 7469 6f6e 2e57 5249 5445 5f45 4d50  sition.WRITE_EMP
+0000bf00: 5459 0a20 2020 2020 2020 2020 2020 206a  TY.            j
+0000bf10: 6f62 5f63 6f6e 6669 672e 6c61 6265 6c73  ob_config.labels
+0000bf20: 203d 207b 2262 6967 6672 616d 6573 2d61   = {"bigframes-a
+0000bf30: 7069 223a 2022 7265 6164 5f70 6172 7175  pi": "read_parqu
+0000bf40: 6574 227d 0a0a 2020 2020 2020 2020 2020  et"}..          
+0000bf50: 2020 7265 7475 726e 2073 656c 662e 5f72    return self._r
+0000bf60: 6561 645f 6269 6771 7565 7279 5f6c 6f61  ead_bigquery_loa
+0000bf70: 645f 6a6f 6228 7061 7468 2c20 7461 626c  d_job(path, tabl
+0000bf80: 652c 206a 6f62 5f63 6f6e 6669 673d 6a6f  e, job_config=jo
+0000bf90: 625f 636f 6e66 6967 290a 2020 2020 2020  b_config).      
+0000bfa0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000bfb0: 2020 2020 7265 6164 5f70 6172 7175 6574      read_parquet
+0000bfc0: 5f6b 7761 7267 733a 2044 6963 745b 7374  _kwargs: Dict[st
+0000bfd0: 722c 2041 6e79 5d20 3d20 7b7d 0a20 2020  r, Any] = {}.   
+0000bfe0: 2020 2020 2020 2020 2069 6620 7061 6e64           if pand
+0000bff0: 6173 2e5f 5f76 6572 7369 6f6e 5f5f 2e73  as.__version__.s
+0000c000: 7461 7274 7377 6974 6828 2231 2e22 293a  tartswith("1."):
+0000c010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c020: 2072 6561 645f 7061 7271 7565 745f 6b77   read_parquet_kw
+0000c030: 6172 6773 5b22 7573 655f 6e75 6c6c 6162  args["use_nullab
+0000c040: 6c65 5f64 7479 7065 7322 5d20 3d20 5472  le_dtypes"] = Tr
+0000c050: 7565 0a20 2020 2020 2020 2020 2020 2065  ue.            e
+0000c060: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000c070: 2020 2020 2072 6561 645f 7061 7271 7565       read_parque
+0000c080: 745f 6b77 6172 6773 5b22 6474 7970 655f  t_kwargs["dtype_
+0000c090: 6261 636b 656e 6422 5d20 3d20 2270 7961  backend"] = "pya
+0000c0a0: 7272 6f77 220a 0a20 2020 2020 2020 2020  rrow"..         
+0000c0b0: 2020 2070 616e 6461 735f 6f62 6a20 3d20     pandas_obj = 
+0000c0c0: 7061 6e64 6173 2e72 6561 645f 7061 7271  pandas.read_parq
+0000c0d0: 7565 7428 0a20 2020 2020 2020 2020 2020  uet(.           
+0000c0e0: 2020 2020 2070 6174 682c 0a20 2020 2020       path,.     
+0000c0f0: 2020 2020 2020 2020 2020 2065 6e67 696e             engin
+0000c100: 653d 656e 6769 6e65 2c20 2023 2074 7970  e=engine,  # typ
+0000c110: 653a 2069 676e 6f72 650a 2020 2020 2020  e: ignore.      
+0000c120: 2020 2020 2020 2020 2020 2a2a 7265 6164            **read
+0000c130: 5f70 6172 7175 6574 5f6b 7761 7267 732c  _parquet_kwargs,
+0000c140: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000c150: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c160: 6e20 7365 6c66 2e5f 7265 6164 5f70 616e  n self._read_pan
+0000c170: 6461 7328 7061 6e64 6173 5f6f 626a 2c20  das(pandas_obj, 
+0000c180: 2272 6561 645f 7061 7271 7565 7422 290a  "read_parquet").
+0000c190: 0a20 2020 2064 6566 2072 6561 645f 6a73  .    def read_js
+0000c1a0: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
+0000c1b0: 2c0a 2020 2020 2020 2020 7061 7468 5f6f  ,.        path_o
+0000c1c0: 725f 6275 663a 2073 7472 207c 2049 4f5b  r_buf: str | IO[
+0000c1d0: 2262 7974 6573 225d 2c0a 2020 2020 2020  "bytes"],.      
+0000c1e0: 2020 2a2c 0a20 2020 2020 2020 206f 7269    *,.        ori
+0000c1f0: 656e 743a 204c 6974 6572 616c 5b0a 2020  ent: Literal[.  
+0000c200: 2020 2020 2020 2020 2020 2273 706c 6974            "split
+0000c210: 222c 2022 7265 636f 7264 7322 2c20 2269  ", "records", "i
+0000c220: 6e64 6578 222c 2022 636f 6c75 6d6e 7322  ndex", "columns"
+0000c230: 2c20 2276 616c 7565 7322 2c20 2274 6162  , "values", "tab
+0000c240: 6c65 220a 2020 2020 2020 2020 5d20 3d20  le".        ] = 
+0000c250: 2263 6f6c 756d 6e73 222c 0a20 2020 2020  "columns",.     
+0000c260: 2020 2064 7479 7065 3a20 4f70 7469 6f6e     dtype: Option
+0000c270: 616c 5b44 6963 745d 203d 204e 6f6e 652c  al[Dict] = None,
+0000c280: 0a20 2020 2020 2020 2065 6e63 6f64 696e  .        encodin
+0000c290: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
+0000c2a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000c2b0: 206c 696e 6573 3a20 626f 6f6c 203d 2046   lines: bool = F
+0000c2c0: 616c 7365 2c0a 2020 2020 2020 2020 656e  alse,.        en
+0000c2d0: 6769 6e65 3a20 4c69 7465 7261 6c5b 2275  gine: Literal["u
+0000c2e0: 6a73 6f6e 222c 2022 7079 6172 726f 7722  json", "pyarrow"
+0000c2f0: 2c20 2262 6967 7175 6572 7922 5d20 3d20  , "bigquery"] = 
+0000c300: 2275 6a73 6f6e 222c 0a20 2020 2020 2020  "ujson",.       
+0000c310: 202a 2a6b 7761 7267 732c 0a20 2020 2029   **kwargs,.    )
+0000c320: 202d 3e20 6461 7461 6672 616d 652e 4461   -> dataframe.Da
+0000c330: 7461 4672 616d 653a 0a20 2020 2020 2020  taFrame:.       
+0000c340: 2074 6162 6c65 203d 2073 656c 662e 5f72   table = self._r
+0000c350: 616e 646f 6d5f 7461 626c 6528 290a 0a20  andom_table().. 
+0000c360: 2020 2020 2020 2069 6620 656e 6769 6e65         if engine
+0000c370: 203d 3d20 2262 6967 7175 6572 7922 3a0a   == "bigquery":.
+0000c380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c390: 6474 7970 6520 6973 206e 6f74 204e 6f6e  dtype is not Non
+0000c3a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c3b0: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+0000c3c0: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2020 2242 6967 5175 6572 7920 656e 6769    "BigQuery engi
+0000c3f0: 6e65 2064 6f65 7320 6e6f 7420 7375 7070  ne does not supp
+0000c400: 6f72 7420 7468 6520 6474 7970 6520 6172  ort the dtype ar
+0000c410: 6775 6d65 6e74 732e 220a 2020 2020 2020  guments.".      
+0000c420: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000c430: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000c440: 6c69 6e65 733a 0a20 2020 2020 2020 2020  lines:.         
+0000c450: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+0000c460: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+0000c470: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c480: 2020 2020 2020 224f 6e6c 7920 6e65 776c        "Only newl
+0000c490: 696e 6520 6465 6c69 6d69 7465 6420 4a53  ine delimited JS
+0000c4a0: 4f4e 2066 6f72 6d61 7420 6973 2073 7570  ON format is sup
+0000c4b0: 706f 7274 6564 2e22 0a20 2020 2020 2020  ported.".       
+0000c4c0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000c4d0: 2020 2020 2020 2020 6966 2065 6e63 6f64          if encod
+0000c4e0: 696e 6720 6973 206e 6f74 204e 6f6e 6520  ing is not None 
+0000c4f0: 616e 6420 656e 636f 6469 6e67 206e 6f74  and encoding not
+0000c500: 2069 6e20 5f56 414c 4944 5f45 4e43 4f44   in _VALID_ENCOD
+0000c510: 494e 4753 3a0a 2020 2020 2020 2020 2020  INGS:.          
+0000c520: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+0000c530: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+0000c540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c550: 2020 2020 2066 2242 6967 5175 6572 7920       f"BigQuery 
+0000c560: 656e 6769 6e65 206f 6e6c 7920 7375 7070  engine only supp
+0000c570: 6f72 7473 2074 6865 2066 6f6c 6c6f 7769  orts the followi
+0000c580: 6e67 2065 6e63 6f64 696e 6773 3a20 7b5f  ng encodings: {_
+0000c590: 5641 4c49 445f 454e 434f 4449 4e47 537d  VALID_ENCODINGS}
+0000c5a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000c5b0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+0000c5c0: 2069 6620 6c69 6e65 7320 616e 6420 6f72   if lines and or
+0000c5d0: 6965 6e74 2021 3d20 2272 6563 6f72 6473  ient != "records
+0000c5e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000c5f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000c600: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000c610: 2020 2020 2020 2020 2022 276c 696e 6573           "'lines
+0000c620: 2720 6b65 7977 6f72 6420 6973 206f 6e6c  ' keyword is onl
+0000c630: 7920 7661 6c69 6420 7768 656e 2027 6f72  y valid when 'or
+0000c640: 6965 6e74 2720 6973 2027 7265 636f 7264  ient' is 'record
+0000c650: 7327 2e22 0a20 2020 2020 2020 2020 2020  s'.".           
+0000c660: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000c670: 2020 2020 6a6f 625f 636f 6e66 6967 203d      job_config =
+0000c680: 2073 656c 662e 5f70 7265 7061 7265 5f6c   self._prepare_l
+0000c690: 6f61 645f 6a6f 625f 636f 6e66 6967 2829  oad_job_config()
+0000c6a0: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+0000c6b0: 5f63 6f6e 6669 672e 6372 6561 7465 5f64  _config.create_d
+0000c6c0: 6973 706f 7369 7469 6f6e 203d 2062 6967  isposition = big
+0000c6d0: 7175 6572 792e 4372 6561 7465 4469 7370  query.CreateDisp
+0000c6e0: 6f73 6974 696f 6e2e 4352 4541 5445 5f49  osition.CREATE_I
+0000c6f0: 465f 4e45 4544 4544 0a20 2020 2020 2020  F_NEEDED.       
+0000c700: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+0000c710: 736f 7572 6365 5f66 6f72 6d61 7420 3d20  source_format = 
+0000c720: 6269 6771 7565 7279 2e53 6f75 7263 6546  bigquery.SourceF
+0000c730: 6f72 6d61 742e 4e45 574c 494e 455f 4445  ormat.NEWLINE_DE
+0000c740: 4c49 4d49 5445 445f 4a53 4f4e 0a20 2020  LIMITED_JSON.   
+0000c750: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+0000c760: 6669 672e 7772 6974 655f 6469 7370 6f73  fig.write_dispos
+0000c770: 6974 696f 6e20 3d20 6269 6771 7565 7279  ition = bigquery
+0000c780: 2e57 7269 7465 4469 7370 6f73 6974 696f  .WriteDispositio
+0000c790: 6e2e 5752 4954 455f 454d 5054 590a 2020  n.WRITE_EMPTY.  
+0000c7a0: 2020 2020 2020 2020 2020 6a6f 625f 636f            job_co
+0000c7b0: 6e66 6967 2e61 7574 6f64 6574 6563 7420  nfig.autodetect 
+0000c7c0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+0000c7d0: 2020 206a 6f62 5f63 6f6e 6669 672e 656e     job_config.en
+0000c7e0: 636f 6469 6e67 203d 2065 6e63 6f64 696e  coding = encodin
+0000c7f0: 670a 2020 2020 2020 2020 2020 2020 6a6f  g.            jo
+0000c800: 625f 636f 6e66 6967 2e6c 6162 656c 7320  b_config.labels 
+0000c810: 3d20 7b22 6269 6766 7261 6d65 732d 6170  = {"bigframes-ap
+0000c820: 6922 3a20 2272 6561 645f 6a73 6f6e 227d  i": "read_json"}
+0000c830: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000c840: 7475 726e 2073 656c 662e 5f72 6561 645f  turn self._read_
+0000c850: 6269 6771 7565 7279 5f6c 6f61 645f 6a6f  bigquery_load_jo
+0000c860: 6228 0a20 2020 2020 2020 2020 2020 2020  b(.             
+0000c870: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
+0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 7461 626c 652c 0a20 2020 2020 2020 2020  table,.         
+0000c8a0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+0000c8b0: 673d 6a6f 625f 636f 6e66 6967 2c0a 2020  g=job_config,.  
+0000c8c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000c8d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c8e0: 2020 2020 2020 6966 2061 6e79 2861 7267        if any(arg
+0000c8f0: 2069 6e20 6b77 6172 6773 2066 6f72 2061   in kwargs for a
+0000c900: 7267 2069 6e20 2822 6368 756e 6b73 697a  rg in ("chunksiz
+0000c910: 6522 2c20 2269 7465 7261 746f 7222 2929  e", "iterator"))
+0000c920: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c930: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000c940: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2022 2763 6875 6e6b 7369 7a65 2720 616e   "'chunksize' an
+0000c970: 6420 2769 7465 7261 746f 7227 2061 7267  d 'iterator' arg
+0000c980: 756d 656e 7473 2061 7265 206e 6f74 2073  uments are not s
+0000c990: 7570 706f 7274 6564 2e22 0a20 2020 2020  upported.".     
+0000c9a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000c9b0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000c9c0: 6e73 7461 6e63 6528 7061 7468 5f6f 725f  nstance(path_or_
+0000c9d0: 6275 662c 2073 7472 293a 0a20 2020 2020  buf, str):.     
+0000c9e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c9f0: 5f63 6865 636b 5f66 696c 655f 7369 7a65  _check_file_size
+0000ca00: 2870 6174 685f 6f72 5f62 7566 290a 0a20  (path_or_buf).. 
+0000ca10: 2020 2020 2020 2020 2020 2069 6620 656e             if en
+0000ca20: 6769 6e65 203d 3d20 2275 6a73 6f6e 223a  gine == "ujson":
+0000ca30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca40: 2070 616e 6461 735f 6466 203d 2070 616e   pandas_df = pan
+0000ca50: 6461 732e 7265 6164 5f6a 736f 6e28 2020  das.read_json(  
+0000ca60: 2320 7479 7065 3a20 6967 6e6f 7265 0a20  # type: ignore. 
+0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 2020 2070 6174 685f 6f72 5f62 7566 2c0a     path_or_buf,.
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 2020 2020 6f72 6965 6e74 3d6f 7269 656e      orient=orien
+0000cab0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0000cac0: 2020 2020 2020 2064 7479 7065 3d64 7479         dtype=dty
+0000cad0: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0000cae0: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
+0000caf0: 3d65 6e63 6f64 696e 672c 0a20 2020 2020  =encoding,.     
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000cb10: 696e 6573 3d6c 696e 6573 2c0a 2020 2020  ines=lines,.    
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 2a2a 6b77 6172 6773 2c0a 2020 2020 2020  **kwargs,.      
+0000cb40: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000cb50: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000cb70: 616e 6461 735f 6466 203d 2070 616e 6461  andas_df = panda
+0000cb80: 732e 7265 6164 5f6a 736f 6e28 2020 2320  s.read_json(  # 
+0000cb90: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2070 6174 685f 6f72 5f62 7566 2c0a 2020   path_or_buf,.  
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 2020 6f72 6965 6e74 3d6f 7269 656e 742c    orient=orient,
+0000cbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cbf0: 2020 2020 2064 7479 7065 3d64 7479 7065       dtype=dtype
+0000cc00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cc10: 2020 2020 2020 656e 636f 6469 6e67 3d65        encoding=e
+0000cc20: 6e63 6f64 696e 672c 0a20 2020 2020 2020  ncoding,.       
+0000cc30: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+0000cc40: 6573 3d6c 696e 6573 2c0a 2020 2020 2020  es=lines,.      
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 656e                en
+0000cc60: 6769 6e65 3d65 6e67 696e 652c 0a20 2020  gine=engine,.   
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 202a 2a6b 7761 7267 732c 0a20 2020 2020   **kwargs,.     
+0000cc90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000cca0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000ccb0: 7365 6c66 2e5f 7265 6164 5f70 616e 6461  self._read_panda
+0000ccc0: 7328 7061 6e64 6173 5f64 662c 2022 7265  s(pandas_df, "re
+0000ccd0: 6164 5f6a 736f 6e22 290a 0a20 2020 2064  ad_json")..    d
+0000cce0: 6566 205f 6368 6563 6b5f 6669 6c65 5f73  ef _check_file_s
+0000ccf0: 697a 6528 7365 6c66 2c20 6669 6c65 7061  ize(self, filepa
+0000cd00: 7468 3a20 7374 7229 3a0a 2020 2020 2020  th: str):.      
+0000cd10: 2020 6d61 785f 7369 7a65 203d 2031 3032    max_size = 102
+0000cd20: 3420 2a20 3130 3234 202a 2031 3032 3420  4 * 1024 * 1024 
+0000cd30: 2023 2031 2047 4220 696e 2062 7974 6573   # 1 GB in bytes
+0000cd40: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
+0000cd50: 7061 7468 2e73 7461 7274 7377 6974 6828  path.startswith(
+0000cd60: 2267 733a 2f2f 2229 3a20 2023 2047 4353  "gs://"):  # GCS
+0000cd70: 2066 696c 6520 7061 7468 0a20 2020 2020   file path.     
+0000cd80: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+0000cd90: 7374 6f72 6167 652e 436c 6965 6e74 2829  storage.Client()
+0000cda0: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
+0000cdb0: 6b65 745f 6e61 6d65 2c20 626c 6f62 5f6e  ket_name, blob_n
+0000cdc0: 616d 6520 3d20 6669 6c65 7061 7468 2e73  ame = filepath.s
+0000cdd0: 706c 6974 2822 2f22 2c20 3329 5b32 3a5d  plit("/", 3)[2:]
+0000cde0: 0a20 2020 2020 2020 2020 2020 2062 7563  .            buc
+0000cdf0: 6b65 7420 3d20 636c 6965 6e74 2e62 7563  ket = client.buc
+0000ce00: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+0000ce10: 0a20 2020 2020 2020 2020 2020 2062 6c6f  .            blo
+0000ce20: 6220 3d20 6275 636b 6574 2e62 6c6f 6228  b = bucket.blob(
+0000ce30: 626c 6f62 5f6e 616d 6529 0a20 2020 2020  blob_name).     
+0000ce40: 2020 2020 2020 2062 6c6f 622e 7265 6c6f         blob.relo
+0000ce50: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+0000ce60: 2066 696c 655f 7369 7a65 203d 2062 6c6f   file_size = blo
+0000ce70: 622e 7369 7a65 0a20 2020 2020 2020 2065  b.size.        e
+0000ce80: 6c73 653a 2020 2320 6c6f 6361 6c20 6669  lse:  # local fi
+0000ce90: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
+0000cea0: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
+0000ceb0: 6f73 2e70 6174 682e 6765 7473 697a 6528  os.path.getsize(
+0000cec0: 6669 6c65 7061 7468 290a 0a20 2020 2020  filepath)..     
+0000ced0: 2020 2069 6620 6669 6c65 5f73 697a 6520     if file_size 
+0000cee0: 3e20 6d61 785f 7369 7a65 3a0a 2020 2020  > max_size:.    
+0000cef0: 2020 2020 2020 2020 2320 436f 6e76 6572          # Conver
+0000cf00: 7420 746f 2047 420a 2020 2020 2020 2020  t to GB.        
+0000cf10: 2020 2020 6669 6c65 5f73 697a 6520 3d20      file_size = 
+0000cf20: 726f 756e 6428 6669 6c65 5f73 697a 6520  round(file_size 
+0000cf30: 2f20 2831 3032 342a 2a33 292c 2031 290a  / (1024**3), 1).
+0000cf40: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000cf50: 7369 7a65 203d 2069 6e74 286d 6178 5f73  size = int(max_s
+0000cf60: 697a 6520 2f20 3130 3234 2a2a 3329 0a20  ize / 1024**3). 
+0000cf70: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000cf80: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
+0000cf90: 2020 2020 2020 2020 2020 2066 2246 696c             f"Fil
+0000cfa0: 6520 7369 7a65 207b 6669 6c65 5f73 697a  e size {file_siz
+0000cfb0: 657d 4742 2065 7863 6565 6473 207b 6d61  e}GB exceeds {ma
+0000cfc0: 785f 7369 7a65 7d47 422e 2022 0a20 2020  x_size}GB. ".   
+0000cfd0: 2020 2020 2020 2020 2020 2020 2022 4974               "It
+0000cfe0: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
+0000cff0: 746f 2075 7365 2065 6e67 696e 653d 2762  to use engine='b
+0000d000: 6967 7175 6572 7927 2022 0a20 2020 2020  igquery' ".     
+0000d010: 2020 2020 2020 2020 2020 2022 666f 7220             "for 
+0000d020: 6c61 7267 6520 6669 6c65 7320 746f 2061  large files to a
+0000d030: 766f 6964 206c 6f61 6469 6e67 2074 6865  void loading the
+0000d040: 2066 696c 6520 696e 746f 206c 6f63 616c   file into local
+0000d050: 206d 656d 6f72 792e 220a 2020 2020 2020   memory.".      
+0000d060: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000d070: 205f 6372 6561 7465 5f65 6d70 7479 5f74   _create_empty_t
+0000d080: 656d 705f 7461 626c 6528 0a20 2020 2020  emp_table(.     
+0000d090: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d0a0: 2073 6368 656d 613a 2049 7465 7261 626c   schema: Iterabl
+0000d0b0: 655b 6269 6771 7565 7279 2e53 6368 656d  e[bigquery.Schem
+0000d0c0: 6146 6965 6c64 5d2c 0a20 2020 2020 2020  aField],.       
+0000d0d0: 2063 6c75 7374 6572 5f63 6f6c 733a 204c   cluster_cols: L
+0000d0e0: 6973 745b 7374 725d 2c0a 2020 2020 2920  ist[str],.    ) 
+0000d0f0: 2d3e 2062 6967 7175 6572 792e 5461 626c  -> bigquery.Tabl
+0000d100: 6552 6566 6572 656e 6365 3a0a 2020 2020  eReference:.    
+0000d110: 2020 2020 2320 4361 6e27 7420 7365 7420      # Can't set 
+0000d120: 6120 7461 626c 6520 696e 205f 5345 5353  a table in _SESS
+0000d130: 494f 4e20 6173 2064 6573 7469 6e61 7469  ION as destinati
+0000d140: 6f6e 2076 6961 2071 7565 7279 206a 6f62  on via query job
+0000d150: 2041 5049 2c20 736f 2077 650a 2020 2020   API, so we.    
+0000d160: 2020 2020 2320 7275 6e20 4444 4c2c 2069      # run DDL, i
+0000d170: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
+0000d180: 6578 7069 7261 7469 6f6e 203d 2028 0a20  expiration = (. 
+0000d190: 2020 2020 2020 2020 2020 2064 6174 6574             datet
+0000d1a0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+0000d1b0: 2864 6174 6574 696d 652e 7469 6d65 7a6f  (datetime.timezo
+0000d1c0: 6e65 2e75 7463 2920 2b20 636f 6e73 7461  ne.utc) + consta
+0000d1d0: 6e74 732e 4445 4641 554c 545f 4558 5049  nts.DEFAULT_EXPI
+0000d1e0: 5241 5449 4f4e 0a20 2020 2020 2020 2029  RATION.        )
+0000d1f0: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
+0000d200: 3d20 6269 6766 7261 6d65 735f 696f 2e63  = bigframes_io.c
+0000d210: 7265 6174 655f 7465 6d70 5f74 6162 6c65  reate_temp_table
+0000d220: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000d230: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000d240: 6578 7069 7261 7469 6f6e 2c0a 2020 2020  expiration,.    
+0000d250: 2020 2020 2020 2020 7363 6865 6d61 3d73          schema=s
+0000d260: 6368 656d 612c 0a20 2020 2020 2020 2020  chema,.         
+0000d270: 2020 2063 6c75 7374 6572 5f63 6f6c 756d     cluster_colum
+0000d280: 6e73 3d63 6c75 7374 6572 5f63 6f6c 732c  ns=cluster_cols,
+0000d290: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000d2a0: 2020 2072 6574 7572 6e20 6269 6771 7565     return bigque
+0000d2b0: 7279 2e54 6162 6c65 5265 6665 7265 6e63  ry.TableReferenc
+0000d2c0: 652e 6672 6f6d 5f73 7472 696e 6728 7461  e.from_string(ta
+0000d2d0: 626c 6529 0a0a 2020 2020 6465 6620 5f69  ble)..    def _i
+0000d2e0: 6269 735f 746f 5f74 656d 705f 7461 626c  bis_to_temp_tabl
+0000d2f0: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
+0000d300: 0a20 2020 2020 2020 2074 6162 6c65 3a20  .        table: 
+0000d310: 6962 6973 5f74 7970 6573 2e54 6162 6c65  ibis_types.Table
+0000d320: 2c0a 2020 2020 2020 2020 636c 7573 7465  ,.        cluste
+0000d330: 725f 636f 6c73 3a20 4974 6572 6162 6c65  r_cols: Iterable
+0000d340: 5b73 7472 5d2c 0a20 2020 2020 2020 2061  [str],.        a
+0000d350: 7069 5f6e 616d 653a 2073 7472 2c0a 2020  pi_name: str,.  
+0000d360: 2020 2920 2d3e 2062 6967 7175 6572 792e    ) -> bigquery.
+0000d370: 5461 626c 6552 6566 6572 656e 6365 3a0a  TableReference:.
+0000d380: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+0000d390: 696f 6e2c 205f 203d 2073 656c 662e 5f71  ion, _ = self._q
+0000d3a0: 7565 7279 5f74 6f5f 6465 7374 696e 6174  uery_to_destinat
+0000d3b0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000d3c0: 2073 656c 662e 6962 6973 5f63 6c69 656e   self.ibis_clien
+0000d3d0: 742e 636f 6d70 696c 6528 7461 626c 6529  t.compile(table)
+0000d3e0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+0000d3f0: 6465 785f 636f 6c73 3d6c 6973 7428 636c  dex_cols=list(cl
+0000d400: 7573 7465 725f 636f 6c73 292c 0a20 2020  uster_cols),.   
+0000d410: 2020 2020 2020 2020 2061 7069 5f6e 616d           api_nam
+0000d420: 653d 6170 695f 6e61 6d65 2c0a 2020 2020  e=api_name,.    
+0000d430: 2020 2020 290a 2020 2020 2020 2020 2320      ).        # 
+0000d440: 5468 6572 6520 7368 6f75 6c64 2061 6c77  There should alw
+0000d450: 6179 7320 6265 2061 2064 6573 7469 6e61  ays be a destina
+0000d460: 7469 6f6e 2074 6162 6c65 2066 6f72 2074  tion table for t
+0000d470: 6869 7320 7175 6572 7920 7479 7065 2e0a  his query type..
+0000d480: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+0000d490: 7970 696e 672e 6361 7374 2862 6967 7175  yping.cast(bigqu
+0000d4a0: 6572 792e 5461 626c 6552 6566 6572 656e  ery.TableReferen
+0000d4b0: 6365 2c20 6465 7374 696e 6174 696f 6e29  ce, destination)
+0000d4c0: 0a0a 2020 2020 6465 6620 7265 6d6f 7465  ..    def remote
+0000d4d0: 5f66 756e 6374 696f 6e28 0a20 2020 2020  _function(.     
+0000d4e0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d4f0: 2069 6e70 7574 5f74 7970 6573 3a20 556e   input_types: Un
+0000d500: 696f 6e5b 7479 7065 2c20 5365 7175 656e  ion[type, Sequen
+0000d510: 6365 5b74 7970 655d 5d2c 0a20 2020 2020  ce[type]],.     
+0000d520: 2020 206f 7574 7075 745f 7479 7065 3a20     output_type: 
+0000d530: 7479 7065 2c0a 2020 2020 2020 2020 6461  type,.        da
+0000d540: 7461 7365 743a 204f 7074 696f 6e61 6c5b  taset: Optional[
+0000d550: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000d560: 2020 2020 2062 6967 7175 6572 795f 636f       bigquery_co
+0000d570: 6e6e 6563 7469 6f6e 3a20 4f70 7469 6f6e  nnection: Option
+0000d580: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000d590: 2020 2020 2020 2020 7265 7573 653a 2062          reuse: b
+0000d5a0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+0000d5b0: 2020 2020 6e61 6d65 3a20 4f70 7469 6f6e      name: Option
+0000d5c0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000d5d0: 2020 2020 2020 2020 7061 636b 6167 6573          packages
+0000d5e0: 3a20 4f70 7469 6f6e 616c 5b53 6571 7565  : Optional[Seque
+0000d5f0: 6e63 655b 7374 725d 5d20 3d20 4e6f 6e65  nce[str]] = None
+0000d600: 2c0a 2020 2020 2020 2020 636c 6f75 645f  ,.        cloud_
+0000d610: 6675 6e63 7469 6f6e 5f73 6572 7669 6365  function_service
+0000d620: 5f61 6363 6f75 6e74 3a20 4f70 7469 6f6e  _account: Option
+0000d630: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000d640: 2020 2020 2020 2020 636c 6f75 645f 6675          cloud_fu
+0000d650: 6e63 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e  nction_kms_key_n
+0000d660: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
+0000d670: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000d680: 2020 2063 6c6f 7564 5f66 756e 6374 696f     cloud_functio
+0000d690: 6e5f 646f 636b 6572 5f72 6570 6f73 6974  n_docker_reposit
+0000d6a0: 6f72 793a 204f 7074 696f 6e61 6c5b 7374  ory: Optional[st
+0000d6b0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000d6c0: 2020 206d 6178 5f62 6174 6368 696e 675f     max_batching_
+0000d6d0: 726f 7773 3a20 4f70 7469 6f6e 616c 5b69  rows: Optional[i
+0000d6e0: 6e74 5d20 3d20 3130 3030 2c0a 2020 2020  nt] = 1000,.    
+0000d6f0: 2020 2020 636c 6f75 645f 6675 6e63 7469      cloud_functi
+0000d700: 6f6e 5f74 696d 656f 7574 3a20 4f70 7469  on_timeout: Opti
+0000d710: 6f6e 616c 5b69 6e74 5d20 3d20 3630 302c  onal[int] = 600,
+0000d720: 0a20 2020 2020 2020 2063 6c6f 7564 5f66  .        cloud_f
+0000d730: 756e 6374 696f 6e5f 6d61 785f 696e 7374  unction_max_inst
+0000d740: 616e 6365 733a 204f 7074 696f 6e61 6c5b  ances: Optional[
+0000d750: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+0000d760: 2029 3a0a 2020 2020 2020 2020 2222 2244   ):.        """D
+0000d770: 6563 6f72 6174 6f72 2074 6f20 7475 726e  ecorator to turn
+0000d780: 2061 2075 7365 7220 6465 6669 6e65 6420   a user defined 
+0000d790: 6675 6e63 7469 6f6e 2069 6e74 6f20 6120  function into a 
+0000d7a0: 4269 6751 7565 7279 2072 656d 6f74 6520  BigQuery remote 
+0000d7b0: 6675 6e63 7469 6f6e 2e20 4368 6563 6b20  function. Check 
+0000d7c0: 6f75 740a 2020 2020 2020 2020 7468 6520  out.        the 
+0000d7d0: 636f 6465 2073 616d 706c 6573 2061 743a  code samples at:
+0000d7e0: 2068 7474 7073 3a2f 2f63 6c6f 7564 2e67   https://cloud.g
+0000d7f0: 6f6f 676c 652e 636f 6d2f 6269 6771 7565  oogle.com/bigque
+0000d800: 7279 2f64 6f63 732f 7265 6d6f 7465 2d66  ry/docs/remote-f
+0000d810: 756e 6374 696f 6e73 2362 6967 7175 6572  unctions#bigquer
+0000d820: 792d 6461 7461 6672 616d 6573 2e0a 0a20  y-dataframes... 
+0000d830: 2020 2020 2020 202e 2e20 6e6f 7465 3a3a         .. note::
+0000d840: 0a20 2020 2020 2020 2020 2020 2050 6c65  .            Ple
+0000d850: 6173 6520 6d61 6b65 2073 7572 6520 666f  ase make sure fo
+0000d860: 6c6c 6f77 696e 6720 6973 2073 6574 7570  llowing is setup
+0000d870: 2062 6566 6f72 6520 7573 696e 6720 7468   before using th
+0000d880: 6973 2041 5049 3a0a 0a20 2020 2020 2020  is API:..       
+0000d890: 2031 2e20 4861 7665 2074 6865 2062 656c   1. Have the bel
+0000d8a0: 6f77 2041 5049 7320 656e 6162 6c65 6420  ow APIs enabled 
+0000d8b0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+0000d8c0: 3a0a 0a20 2020 2020 2020 2020 2020 202a  :..            *
+0000d8d0: 2042 6967 5175 6572 7920 436f 6e6e 6563   BigQuery Connec
+0000d8e0: 7469 6f6e 2041 5049 0a20 2020 2020 2020  tion API.       
+0000d8f0: 2020 2020 202a 2043 6c6f 7564 2046 756e       * Cloud Fun
+0000d900: 6374 696f 6e73 2041 5049 0a20 2020 2020  ctions API.     
+0000d910: 2020 2020 2020 202a 2043 6c6f 7564 2052         * Cloud R
+0000d920: 756e 2041 5049 0a20 2020 2020 2020 2020  un API.         
+0000d930: 2020 202a 2043 6c6f 7564 2042 7569 6c64     * Cloud Build
+0000d940: 2041 5049 0a20 2020 2020 2020 2020 2020   API.           
+0000d950: 202a 2041 7274 6966 6163 7420 5265 6769   * Artifact Regi
+0000d960: 7374 7279 2041 5049 0a20 2020 2020 2020  stry API.       
+0000d970: 2020 2020 202a 2043 6c6f 7564 2052 6573       * Cloud Res
+0000d980: 6f75 7263 6520 4d61 6e61 6765 7220 4150  ource Manager AP
+0000d990: 490a 0a20 2020 2020 2020 2020 2020 5468  I..           Th
+0000d9a0: 6973 2063 616e 2062 6520 646f 6e65 2066  is can be done f
+0000d9b0: 726f 6d20 7468 6520 636c 6f75 6420 636f  rom the cloud co
+0000d9c0: 6e73 6f6c 6520 2863 6861 6e67 6520 6050  nsole (change `P
+0000d9d0: 524f 4a45 4354 5f49 4460 2074 6f20 796f  ROJECT_ID` to yo
+0000d9e0: 7572 7329 3a0a 2020 2020 2020 2020 2020  urs):.          
+0000d9f0: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
+0000da00: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
+0000da10: 6d2f 6170 6973 2f65 6e61 626c 6566 6c6f  m/apis/enableflo
+0000da20: 773f 6170 6969 643d 6269 6771 7565 7279  w?apiid=bigquery
+0000da30: 636f 6e6e 6563 7469 6f6e 2e67 6f6f 676c  connection.googl
+0000da40: 6561 7069 732e 636f 6d2c 636c 6f75 6466  eapis.com,cloudf
+0000da50: 756e 6374 696f 6e73 2e67 6f6f 676c 6561  unctions.googlea
+0000da60: 7069 732e 636f 6d2c 7275 6e2e 676f 6f67  pis.com,run.goog
+0000da70: 6c65 6170 6973 2e63 6f6d 2c63 6c6f 7564  leapis.com,cloud
+0000da80: 6275 696c 642e 676f 6f67 6c65 6170 6973  build.googleapis
+0000da90: 2e63 6f6d 2c61 7274 6966 6163 7472 6567  .com,artifactreg
+0000daa0: 6973 7472 792e 676f 6f67 6c65 6170 6973  istry.googleapis
+0000dab0: 2e63 6f6d 2c63 6c6f 7564 7265 736f 7572  .com,cloudresour
+0000dac0: 6365 6d61 6e61 6765 722e 676f 6f67 6c65  cemanager.google
+0000dad0: 6170 6973 2e63 6f6d 2670 726f 6a65 6374  apis.com&project
+0000dae0: 3d50 524f 4a45 4354 5f49 440a 0a20 2020  =PROJECT_ID..   
+0000daf0: 2020 2020 2020 2020 4f72 2066 726f 6d20          Or from 
+0000db00: 7468 6520 6763 6c6f 7564 2043 4c49 3a0a  the gcloud CLI:.
+0000db10: 0a20 2020 2020 2020 2020 2020 6024 2067  .           `$ g
+0000db20: 636c 6f75 6420 7365 7276 6963 6573 2065  cloud services e
+0000db30: 6e61 626c 6520 6269 6771 7565 7279 636f  nable bigqueryco
+0000db40: 6e6e 6563 7469 6f6e 2e67 6f6f 676c 6561  nnection.googlea
+0000db50: 7069 732e 636f 6d20 636c 6f75 6466 756e  pis.com cloudfun
+0000db60: 6374 696f 6e73 2e67 6f6f 676c 6561 7069  ctions.googleapi
+0000db70: 732e 636f 6d20 7275 6e2e 676f 6f67 6c65  s.com run.google
+0000db80: 6170 6973 2e63 6f6d 2063 6c6f 7564 6275  apis.com cloudbu
+0000db90: 696c 642e 676f 6f67 6c65 6170 6973 2e63  ild.googleapis.c
+0000dba0: 6f6d 2061 7274 6966 6163 7472 6567 6973  om artifactregis
+0000dbb0: 7472 792e 676f 6f67 6c65 6170 6973 2e63  try.googleapis.c
+0000dbc0: 6f6d 2063 6c6f 7564 7265 736f 7572 6365  om cloudresource
+0000dbd0: 6d61 6e61 6765 722e 676f 6f67 6c65 6170  manager.googleap
+0000dbe0: 6973 2e63 6f6d 600a 0a20 2020 2020 2020  is.com`..       
+0000dbf0: 2032 2e20 4861 7665 2066 6f6c 6c6f 7769   2. Have followi
+0000dc00: 6e67 2049 414d 2072 6f6c 6573 2065 6e61  ng IAM roles ena
+0000dc10: 626c 6564 2066 6f72 2079 6f75 3a0a 0a20  bled for you:.. 
+0000dc20: 2020 2020 2020 2020 2020 202a 2042 6967             * Big
+0000dc30: 5175 6572 7920 4461 7461 2045 6469 746f  Query Data Edito
+0000dc40: 7220 2872 6f6c 6573 2f62 6967 7175 6572  r (roles/bigquer
+0000dc50: 792e 6461 7461 4564 6974 6f72 290a 2020  y.dataEditor).  
+0000dc60: 2020 2020 2020 2020 2020 2a20 4269 6751            * BigQ
+0000dc70: 7565 7279 2043 6f6e 6e65 6374 696f 6e20  uery Connection 
+0000dc80: 4164 6d69 6e20 2872 6f6c 6573 2f62 6967  Admin (roles/big
+0000dc90: 7175 6572 792e 636f 6e6e 6563 7469 6f6e  query.connection
+0000dca0: 4164 6d69 6e29 0a20 2020 2020 2020 2020  Admin).         
+0000dcb0: 2020 202a 2043 6c6f 7564 2046 756e 6374     * Cloud Funct
+0000dcc0: 696f 6e73 2044 6576 656c 6f70 6572 2028  ions Developer (
+0000dcd0: 726f 6c65 732f 636c 6f75 6466 756e 6374  roles/cloudfunct
+0000dce0: 696f 6e73 2e64 6576 656c 6f70 6572 290a  ions.developer).
+0000dcf0: 2020 2020 2020 2020 2020 2020 2a20 5365              * Se
+0000dd00: 7276 6963 6520 4163 636f 756e 7420 5573  rvice Account Us
+0000dd10: 6572 2028 726f 6c65 732f 6961 6d2e 7365  er (roles/iam.se
+0000dd20: 7276 6963 6541 6363 6f75 6e74 5573 6572  rviceAccountUser
+0000dd30: 2920 6f6e 2074 6865 2073 6572 7669 6365  ) on the service
+0000dd40: 2061 6363 6f75 6e74 2060 5052 4f4a 4543   account `PROJEC
+0000dd50: 545f 4e55 4d42 4552 2d63 6f6d 7075 7465  T_NUMBER-compute
+0000dd60: 4064 6576 656c 6f70 6572 2e67 7365 7276  @developer.gserv
+0000dd70: 6963 6561 6363 6f75 6e74 2e63 6f6d 600a  iceaccount.com`.
+0000dd80: 2020 2020 2020 2020 2020 2020 2a20 5374              * St
+0000dd90: 6f72 6167 6520 4f62 6a65 6374 2056 6965  orage Object Vie
+0000dda0: 7765 7220 2872 6f6c 6573 2f73 746f 7261  wer (roles/stora
+0000ddb0: 6765 2e6f 626a 6563 7456 6965 7765 7229  ge.objectViewer)
+0000ddc0: 0a20 2020 2020 2020 2020 2020 202a 2050  .            * P
+0000ddd0: 726f 6a65 6374 2049 414d 2041 646d 696e  roject IAM Admin
+0000dde0: 2028 726f 6c65 732f 7265 736f 7572 6365   (roles/resource
+0000ddf0: 6d61 6e61 6765 722e 7072 6f6a 6563 7449  manager.projectI
+0000de00: 616d 4164 6d69 6e29 2028 4f6e 6c79 2072  amAdmin) (Only r
+0000de10: 6571 7569 7265 6420 6966 2074 6865 2062  equired if the b
+0000de20: 6967 7175 6572 7920 636f 6e6e 6563 7469  igquery connecti
+0000de30: 6f6e 2062 6569 6e67 2075 7365 6420 6973  on being used is
+0000de40: 206e 6f74 2070 7265 2d63 7265 6174 6564   not pre-created
+0000de50: 2061 6e64 2069 7320 6372 6561 7465 6420   and is created 
+0000de60: 6479 6e61 6d69 6361 6c6c 7920 7769 7468  dynamically with
+0000de70: 2075 7365 7220 6372 6564 656e 7469 616c   user credential
+0000de80: 732e 290a 0a20 2020 2020 2020 2033 2e20  s.)..        3. 
+0000de90: 4569 7468 6572 2074 6865 2075 7365 7220  Either the user 
+0000dea0: 6861 7320 7365 7449 616d 506f 6c69 6379  has setIamPolicy
+0000deb0: 2070 7269 7669 6c65 6765 206f 6e20 7468   privilege on th
+0000dec0: 6520 7072 6f6a 6563 742c 206f 7220 6120  e project, or a 
+0000ded0: 4269 6751 7565 7279 2063 6f6e 6e65 6374  BigQuery connect
+0000dee0: 696f 6e20 6973 2070 7265 2d63 7265 6174  ion is pre-creat
+0000def0: 6564 2077 6974 6820 6e65 6365 7373 6172  ed with necessar
+0000df00: 7920 4941 4d20 726f 6c65 2073 6574 3a0a  y IAM role set:.
+0000df10: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
+0000df20: 546f 2063 7265 6174 6520 6120 636f 6e6e  To create a conn
+0000df30: 6563 7469 6f6e 2c20 666f 6c6c 6f77 2068  ection, follow h
+0000df40: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
+0000df50: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
+0000df60: 2f64 6f63 732f 7265 6665 7265 6e63 652f  /docs/reference/
+0000df70: 7374 616e 6461 7264 2d73 716c 2f72 656d  standard-sql/rem
+0000df80: 6f74 652d 6675 6e63 7469 6f6e 7323 6372  ote-functions#cr
+0000df90: 6561 7465 5f61 5f63 6f6e 6e65 6374 696f  eate_a_connectio
+0000dfa0: 6e0a 2020 2020 2020 2020 2020 2020 322e  n.            2.
+0000dfb0: 2054 6f20 7365 7420 7570 2049 414d 2c20   To set up IAM, 
+0000dfc0: 666f 6c6c 6f77 2068 7474 7073 3a2f 2f63  follow https://c
+0000dfd0: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
+0000dfe0: 6269 6771 7565 7279 2f64 6f63 732f 7265  bigquery/docs/re
+0000dff0: 6665 7265 6e63 652f 7374 616e 6461 7264  ference/standard
+0000e000: 2d73 716c 2f72 656d 6f74 652d 6675 6e63  -sql/remote-func
+0000e010: 7469 6f6e 7323 6772 616e 745f 7065 726d  tions#grant_perm
+0000e020: 6973 7369 6f6e 5f6f 6e5f 6675 6e63 7469  ission_on_functi
+0000e030: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+0000e040: 2020 2041 6c74 6572 6e61 7469 7665 6c79     Alternatively
+0000e050: 2c20 7468 6520 4941 4d20 636f 756c 6420  , the IAM could 
+0000e060: 616c 736f 2062 6520 7365 7475 7020 7669  also be setup vi
+0000e070: 6120 7468 6520 6763 6c6f 7564 2043 4c49  a the gcloud CLI
+0000e080: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e090: 2020 6024 2067 636c 6f75 6420 7072 6f6a    `$ gcloud proj
+0000e0a0: 6563 7473 2061 6464 2d69 616d 2d70 6f6c  ects add-iam-pol
+0000e0b0: 6963 792d 6269 6e64 696e 6720 5052 4f4a  icy-binding PROJ
+0000e0c0: 4543 545f 4944 202d 2d6d 656d 6265 723d  ECT_ID --member=
+0000e0d0: 2273 6572 7669 6365 4163 636f 756e 743a  "serviceAccount:
+0000e0e0: 434f 4e4e 4543 5449 4f4e 5f53 4552 5649  CONNECTION_SERVI
+0000e0f0: 4345 5f41 4343 4f55 4e54 5f49 4422 202d  CE_ACCOUNT_ID" -
+0000e100: 2d72 6f6c 653d 2272 6f6c 6573 2f72 756e  -role="roles/run
+0000e110: 2e69 6e76 6f6b 6572 2260 2e0a 0a20 2020  .invoker"`...   
+0000e120: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000e130: 2020 2020 2020 2069 6e70 7574 5f74 7970         input_typ
+0000e140: 6573 2028 7479 7065 206f 7220 7365 7175  es (type or sequ
+0000e150: 656e 6365 2874 7970 6529 293a 0a20 2020  ence(type)):.   
+0000e160: 2020 2020 2020 2020 2020 2020 2049 6e70               Inp
+0000e170: 7574 2064 6174 6120 7479 7065 2c20 6f72  ut data type, or
+0000e180: 2073 6571 7565 6e63 6520 6f66 2069 6e70   sequence of inp
+0000e190: 7574 2064 6174 6120 7479 7065 7320 696e  ut data types in
+0000e1a0: 2074 6865 2075 7365 720a 2020 2020 2020   the user.      
+0000e1b0: 2020 2020 2020 2020 2020 6465 6669 6e65            define
+0000e1c0: 6420 6675 6e63 7469 6f6e 2e0a 2020 2020  d function..    
+0000e1d0: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
+0000e1e0: 7970 6520 2874 7970 6529 3a0a 2020 2020  ype (type):.    
+0000e1f0: 2020 2020 2020 2020 2020 2020 4461 7461              Data
+0000e200: 2074 7970 6520 6f66 2074 6865 206f 7574   type of the out
+0000e210: 7075 7420 696e 2074 6865 2075 7365 7220  put in the user 
+0000e220: 6465 6669 6e65 6420 6675 6e63 7469 6f6e  defined function
+0000e230: 2e0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+0000e240: 7461 7365 7420 2873 7472 2c20 4f70 7469  taset (str, Opti
+0000e250: 6f6e 616c 293a 0a20 2020 2020 2020 2020  onal):.         
+0000e260: 2020 2020 2020 2044 6174 6173 6574 2069         Dataset i
+0000e270: 6e20 7768 6963 6820 746f 2063 7265 6174  n which to creat
+0000e280: 6520 6120 4269 6751 7565 7279 2072 656d  e a BigQuery rem
+0000e290: 6f74 6520 6675 6e63 7469 6f6e 2e20 4974  ote function. It
+0000e2a0: 2073 686f 756c 6420 6265 2069 6e0a 2020   should be in.  
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 603c                `<
+0000e2c0: 7072 6f6a 6563 745f 6964 3e2e 3c64 6174  project_id>.<dat
+0000e2d0: 6173 6574 5f6e 616d 653e 6020 6f72 2060  aset_name>` or `
+0000e2e0: 3c64 6174 6173 6574 5f6e 616d 653e 6020  <dataset_name>` 
+0000e2f0: 666f 726d 6174 2e20 4966 2074 6869 730a  format. If this.
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 7061 7261 6d65 7465 7220 6973 206e 6f74  parameter is not
+0000e320: 2070 726f 7669 6465 6420 7468 656e 2073   provided then s
+0000e330: 6573 7369 6f6e 2064 6174 6173 6574 2069  ession dataset i
+0000e340: 6420 6973 2075 7365 642e 0a20 2020 2020  d is used..     
+0000e350: 2020 2020 2020 2062 6967 7175 6572 795f         bigquery_
+0000e360: 636f 6e6e 6563 7469 6f6e 2028 7374 722c  connection (str,
+0000e370: 204f 7074 696f 6e61 6c29 3a0a 2020 2020   Optional):.    
+0000e380: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
+0000e390: 206f 6620 7468 6520 4269 6751 7565 7279   of the BigQuery
+0000e3a0: 2063 6f6e 6e65 6374 696f 6e2e 2059 6f75   connection. You
+0000e3b0: 2073 686f 756c 6420 6569 7468 6572 2068   should either h
+0000e3c0: 6176 6520 7468 650a 2020 2020 2020 2020  ave the.        
+0000e3d0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+0000e3e0: 6f6e 2061 6c72 6561 6479 2063 7265 6174  on already creat
+0000e3f0: 6564 2069 6e20 7468 6520 606c 6f63 6174  ed in the `locat
+0000e400: 696f 6e60 2079 6f75 2068 6176 6520 6368  ion` you have ch
+0000e410: 6f73 656e 2c20 6f72 0a20 2020 2020 2020  osen, or.       
+0000e420: 2020 2020 2020 2020 2079 6f75 2073 686f           you sho
+0000e430: 756c 6420 6861 7665 2074 6865 2050 726f  uld have the Pro
+0000e440: 6a65 6374 2049 414d 2041 646d 696e 2072  ject IAM Admin r
+0000e450: 6f6c 6520 746f 2065 6e61 626c 6520 7468  ole to enable th
+0000e460: 6520 7365 7276 6963 650a 2020 2020 2020  e service.      
+0000e470: 2020 2020 2020 2020 2020 746f 2063 7265            to cre
+0000e480: 6174 6520 7468 6520 636f 6e6e 6563 7469  ate the connecti
+0000e490: 6f6e 2066 6f72 2079 6f75 2069 6620 796f  on for you if yo
+0000e4a0: 7520 6e65 6564 2069 742e 2049 6620 7468  u need it. If th
+0000e4b0: 6973 2070 6172 616d 6574 6572 2069 730a  is parameter is.
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 6e6f 7420 7072 6f76 6964 6564 2074 6865  not provided the
+0000e4e0: 6e20 7468 6520 4269 6751 7565 7279 2063  n the BigQuery c
+0000e4f0: 6f6e 6e65 6374 696f 6e20 6672 6f6d 2074  onnection from t
+0000e500: 6865 2073 6573 7369 6f6e 2069 7320 7573  he session is us
+0000e510: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000e520: 7265 7573 6520 2862 6f6f 6c2c 204f 7074  reuse (bool, Opt
+0000e530: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
+0000e540: 2020 2020 2020 2020 5265 7573 6520 7468          Reuse th
+0000e550: 6520 7265 6d6f 7465 2066 756e 6374 696f  e remote functio
+0000e560: 6e20 6966 2061 6c72 6561 6479 2065 7869  n if already exi
+0000e570: 7374 732e 0a20 2020 2020 2020 2020 2020  sts..           
+0000e580: 2020 2020 2060 5472 7565 6020 6279 2064       `True` by d
+0000e590: 6566 6175 6c74 2c20 7768 6963 6820 7769  efault, which wi
+0000e5a0: 6c6c 2072 6573 756c 7420 696e 2072 6575  ll result in reu
+0000e5b0: 7369 6e67 2061 6e20 6578 6973 7469 6e67  sing an existing
+0000e5c0: 2072 656d 6f74 650a 2020 2020 2020 2020   remote.        
+0000e5d0: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+0000e5e0: 2061 6e64 2063 6f72 7265 7370 6f6e 6469   and correspondi
+0000e5f0: 6e67 2063 6c6f 7564 2066 756e 6374 696f  ng cloud functio
+0000e600: 6e20 2869 6620 616e 7929 2074 6861 7420  n (if any) that 
+0000e610: 7761 730a 2020 2020 2020 2020 2020 2020  was.            
+0000e620: 2020 2020 7072 6576 696f 7573 6c79 2063      previously c
+0000e630: 7265 6174 6564 2066 6f72 2074 6865 2073  reated for the s
+0000e640: 616d 6520 7564 662e 0a20 2020 2020 2020  ame udf..       
+0000e650: 2020 2020 2020 2020 2053 6574 7469 6e67           Setting
+0000e660: 2069 7420 746f 2060 4661 6c73 6560 2077   it to `False` w
+0000e670: 6f75 6c64 2066 6f72 6365 2063 7265 6174  ould force creat
+0000e680: 696e 6720 6120 756e 6971 7565 2072 656d  ing a unique rem
+0000e690: 6f74 6520 6675 6e63 7469 6f6e 2e0a 2020  ote function..  
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+0000e6b0: 2074 6865 2072 6571 7569 7265 6420 7265   the required re
+0000e6c0: 6d6f 7465 2066 756e 6374 696f 6e20 646f  mote function do
+0000e6d0: 6573 206e 6f74 2065 7869 7374 2074 6865  es not exist the
+0000e6e0: 6e20 6974 2077 6f75 6c64 2062 650a 2020  n it would be.  
+0000e6f0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+0000e700: 6561 7465 6420 6972 7265 7370 6563 7469  eated irrespecti
+0000e710: 7665 206f 6620 7468 6973 2070 6172 616d  ve of this param
+0000e720: 2e0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+0000e730: 6d65 2028 7374 722c 204f 7074 696f 6e61  me (str, Optiona
+0000e740: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+0000e750: 2020 2020 4578 706c 6963 6974 206e 616d      Explicit nam
+0000e760: 6520 6f66 2074 6865 2070 6572 7369 7374  e of the persist
+0000e770: 6564 2042 6967 5175 6572 7920 7265 6d6f  ed BigQuery remo
+0000e780: 7465 2066 756e 6374 696f 6e2e 2055 7365  te function. Use
+0000e790: 2069 7420 7769 7468 0a20 2020 2020 2020   it with.       
+0000e7a0: 2020 2020 2020 2020 2063 6175 7469 6f6e           caution
+0000e7b0: 2c20 6265 6361 7573 6520 7477 6f20 7573  , because two us
+0000e7c0: 6572 7320 776f 726b 696e 6720 696e 2074  ers working in t
+0000e7d0: 6865 2073 616d 6520 7072 6f6a 6563 7420  he same project 
+0000e7e0: 616e 6420 6461 7461 7365 740a 2020 2020  and dataset.    
+0000e7f0: 2020 2020 2020 2020 2020 2020 636f 756c              coul
+0000e800: 6420 6f76 6572 7772 6974 6520 6561 6368  d overwrite each
+0000e810: 206f 7468 6572 2773 2072 656d 6f74 6520   other's remote 
+0000e820: 6675 6e63 7469 6f6e 7320 6966 2074 6865  functions if the
+0000e830: 7920 7573 6520 7468 6520 7361 6d65 0a20  y use the same. 
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e850: 6572 7369 7374 656e 7420 6e61 6d65 2e0a  ersistent name..
+0000e860: 2020 2020 2020 2020 2020 2020 7061 636b              pack
+0000e870: 6167 6573 2028 7374 725b 5d2c 204f 7074  ages (str[], Opt
+0000e880: 696f 6e61 6c29 3a0a 2020 2020 2020 2020  ional):.        
+0000e890: 2020 2020 2020 2020 4578 706c 6963 6974          Explicit
+0000e8a0: 206e 616d 6520 6f66 2074 6865 2065 7874   name of the ext
+0000e8b0: 6572 6e61 6c20 7061 636b 6167 6520 6465  ernal package de
+0000e8c0: 7065 6e64 656e 6369 6573 2e20 4561 6368  pendencies. Each
+0000e8d0: 2064 6570 656e 6465 6e63 790a 2020 2020   dependency.    
+0000e8e0: 2020 2020 2020 2020 2020 2020 6973 2061              is a
+0000e8f0: 6464 6564 2074 6f20 7468 6520 6072 6571  dded to the `req
+0000e900: 7569 7265 6d65 6e74 732e 7478 7460 2061  uirements.txt` a
+0000e910: 7320 6973 2c20 616e 6420 6361 6e20 6265  s is, and can be
+0000e920: 206f 6620 7468 6520 666f 726d 0a20 2020   of the form.   
+0000e930: 2020 2020 2020 2020 2020 2020 2073 7570               sup
+0000e940: 706f 7274 6564 2069 6e20 6874 7470 733a  ported in https:
+0000e950: 2f2f 7069 702e 7079 7061 2e69 6f2f 656e  //pip.pypa.io/en
+0000e960: 2f73 7461 626c 652f 7265 6665 7265 6e63  /stable/referenc
+0000e970: 652f 7265 7175 6972 656d 656e 7473 2d66  e/requirements-f
+0000e980: 696c 652d 666f 726d 6174 2f2e 0a20 2020  ile-format/..   
+0000e990: 2020 2020 2020 2020 2063 6c6f 7564 5f66           cloud_f
+0000e9a0: 756e 6374 696f 6e5f 7365 7276 6963 655f  unction_service_
+0000e9b0: 6163 636f 756e 7420 2873 7472 2c20 4f70  account (str, Op
+0000e9c0: 7469 6f6e 616c 293a 0a20 2020 2020 2020  tional):.       
+0000e9d0: 2020 2020 2020 2020 2053 6572 7669 6365           Service
+0000e9e0: 2061 6363 6f75 6e74 2074 6f20 7573 6520   account to use 
+0000e9f0: 666f 7220 7468 6520 636c 6f75 6420 6675  for the cloud fu
+0000ea00: 6e63 7469 6f6e 732e 2049 6620 6e6f 7420  nctions. If not 
+0000ea10: 7072 6f76 6964 6564 0a20 2020 2020 2020  provided.       
+0000ea20: 2020 2020 2020 2020 2074 6865 6e20 7468           then th
+0000ea30: 6520 6465 6661 756c 7420 7365 7276 6963  e default servic
+0000ea40: 6520 6163 636f 756e 7420 776f 756c 6420  e account would 
+0000ea50: 6265 2075 7365 642e 2053 6565 0a20 2020  be used. See.   
+0000ea60: 2020 2020 2020 2020 2020 2020 2068 7474               htt
+0000ea70: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
+0000ea80: 652e 636f 6d2f 6675 6e63 7469 6f6e 732f  e.com/functions/
+0000ea90: 646f 6373 2f73 6563 7572 696e 672f 6675  docs/securing/fu
+0000eaa0: 6e63 7469 6f6e 2d69 6465 6e74 6974 790a  nction-identity.
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
+0000ead0: 2e20 506c 6561 7365 206d 616b 6520 7375  . Please make su
+0000eae0: 7265 2074 6865 2073 6572 7669 6365 2061  re the service a
+0000eaf0: 6363 6f75 6e74 2068 6173 2074 6865 0a20  ccount has the. 
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000eb10: 6563 6573 7361 7279 2049 414d 2070 6572  ecessary IAM per
+0000eb20: 6d69 7373 696f 6e73 2063 6f6e 6669 6775  missions configu
+0000eb30: 7265 6420 6173 2064 6573 6372 6962 6564  red as described
+0000eb40: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+0000eb50: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
+0000eb60: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
+0000eb70: 6374 696f 6e73 2f64 6f63 732f 7265 6665  ctions/docs/refe
+0000eb80: 7265 6e63 652f 6961 6d2f 726f 6c65 7323  rence/iam/roles#
+0000eb90: 6164 6469 7469 6f6e 616c 2d63 6f6e 6669  additional-confi
+0000eba0: 6775 7261 7469 6f6e 2e0a 2020 2020 2020  guration..      
+0000ebb0: 2020 2020 2020 636c 6f75 645f 6675 6e63        cloud_func
+0000ebc0: 7469 6f6e 5f6b 6d73 5f6b 6579 5f6e 616d  tion_kms_key_nam
+0000ebd0: 6520 2873 7472 2c20 4f70 7469 6f6e 616c  e (str, Optional
+0000ebe0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ebf0: 2020 2043 7573 746f 6d65 7220 6d61 6e61     Customer mana
+0000ec00: 6765 6420 656e 6372 7970 7469 6f6e 206b  ged encryption k
+0000ec10: 6579 2074 6f20 7072 6f74 6563 7420 636c  ey to protect cl
+0000ec20: 6f75 6420 6675 6e63 7469 6f6e 7320 616e  oud functions an
+0000ec30: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000ec40: 2020 7265 6c61 7465 6420 6461 7461 2061    related data a
+0000ec50: 7420 7265 7374 2e20 5468 6973 2069 7320  t rest. This is 
+0000ec60: 6f66 2074 6865 2066 6f72 6d61 740a 2020  of the format.  
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000ec80: 6f6a 6563 7473 2f50 524f 4a45 4354 5f49  ojects/PROJECT_I
+0000ec90: 442f 6c6f 6361 7469 6f6e 732f 4c4f 4341  D/locations/LOCA
+0000eca0: 5449 4f4e 2f6b 6579 5269 6e67 732f 4b45  TION/keyRings/KE
+0000ecb0: 5952 494e 472f 6372 7970 746f 4b65 7973  YRING/cryptoKeys
+0000ecc0: 2f4b 4559 2e0a 2020 2020 2020 2020 2020  /KEY..          
+0000ecd0: 2020 2020 2020 5265 6164 2068 7474 7073        Read https
+0000ece0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+0000ecf0: 636f 6d2f 6675 6e63 7469 6f6e 732f 646f  com/functions/do
+0000ed00: 6373 2f73 6563 7572 696e 672f 636d 656b  cs/securing/cmek
+0000ed10: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
+0000ed20: 2020 2020 206d 6f72 6520 6465 7461 696c       more detail
+0000ed30: 7320 696e 636c 7564 696e 6720 6772 616e  s including gran
+0000ed40: 7469 6e67 206e 6563 6573 7361 7279 2073  ting necessary s
+0000ed50: 6572 7669 6365 2061 6363 6f75 6e74 730a  ervice accounts.
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed70: 6163 6365 7373 2074 6f20 7468 6520 6b65  access to the ke
+0000ed80: 792e 0a20 2020 2020 2020 2020 2020 2063  y..            c
+0000ed90: 6c6f 7564 5f66 756e 6374 696f 6e5f 646f  loud_function_do
+0000eda0: 636b 6572 5f72 6570 6f73 6974 6f72 7920  cker_repository 
+0000edb0: 2873 7472 2c20 4f70 7469 6f6e 616c 293a  (str, Optional):
+0000edc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edd0: 2044 6f63 6b65 7220 7265 706f 7369 746f   Docker reposito
+0000ede0: 7279 2063 7265 6174 6564 2077 6974 6820  ry created with 
+0000edf0: 7468 6520 7361 6d65 2065 6e63 7279 7074  the same encrypt
+0000ee00: 696f 6e20 6b65 7920 6173 0a20 2020 2020  ion key as.     
+0000ee10: 2020 2020 2020 2020 2020 2060 636c 6f75             `clou
+0000ee20: 645f 6675 6e63 7469 6f6e 5f6b 6d73 5f6b  d_function_kms_k
+0000ee30: 6579 5f6e 616d 6560 2074 6f20 7374 6f72  ey_name` to stor
+0000ee40: 6520 656e 6372 7970 7465 6420 6172 7469  e encrypted arti
+0000ee50: 6661 6374 730a 2020 2020 2020 2020 2020  facts.          
+0000ee60: 2020 2020 2020 6372 6561 7465 6420 746f        created to
+0000ee70: 2073 7570 706f 7274 2074 6865 2063 6c6f   support the clo
+0000ee80: 7564 2066 756e 6374 696f 6e2e 2054 6869  ud function. Thi
+0000ee90: 7320 6973 206f 6620 7468 6520 666f 726d  s is of the form
+0000eea0: 6174 0a20 2020 2020 2020 2020 2020 2020  at.             
+0000eeb0: 2020 2070 726f 6a65 6374 732f 5052 4f4a     projects/PROJ
+0000eec0: 4543 545f 4944 2f6c 6f63 6174 696f 6e73  ECT_ID/locations
+0000eed0: 2f4c 4f43 4154 494f 4e2f 7265 706f 7369  /LOCATION/reposi
+0000eee0: 746f 7269 6573 2f52 4550 4f53 4954 4f52  tories/REPOSITOR
+0000eef0: 595f 4e41 4d45 2e0a 2020 2020 2020 2020  Y_NAME..        
+0000ef00: 2020 2020 2020 2020 466f 7220 6d6f 7265          For more
+0000ef10: 2064 6574 6169 6c73 2073 6565 0a20 2020   details see.   
+0000ef20: 2020 2020 2020 2020 2020 2020 2068 7474               htt
+0000ef30: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
+0000ef40: 652e 636f 6d2f 6675 6e63 7469 6f6e 732f  e.com/functions/
+0000ef50: 646f 6373 2f73 6563 7572 696e 672f 636d  docs/securing/cm
+0000ef60: 656b 2362 6566 6f72 655f 796f 755f 6265  ek#before_you_be
+0000ef70: 6769 6e2e 0a20 2020 2020 2020 2020 2020  gin..           
+0000ef80: 206d 6178 5f62 6174 6368 696e 675f 726f   max_batching_ro
+0000ef90: 7773 2028 696e 742c 204f 7074 696f 6e61  ws (int, Optiona
+0000efa0: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
+0000efb0: 2020 2020 5468 6520 6d61 7869 6d75 6d20      The maximum 
+0000efc0: 6e75 6d62 6572 206f 6620 726f 7773 2074  number of rows t
+0000efd0: 6f20 6265 2062 6174 6368 6564 2066 6f72  o be batched for
+0000efe0: 2070 726f 6365 7373 696e 6720 696e 2074   processing in t
+0000eff0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+0000f000: 2020 2042 5120 7265 6d6f 7465 2066 756e     BQ remote fun
+0000f010: 6374 696f 6e2e 2044 6566 6175 6c74 2076  ction. Default v
+0000f020: 616c 7565 2069 7320 3130 3030 2e20 4120  alue is 1000. A 
+0000f030: 6c6f 7765 7220 6e75 6d62 6572 2063 616e  lower number can
+0000f040: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+0000f050: 2020 2020 7061 7373 6564 2074 6f20 6176      passed to av
+0000f060: 6f69 6420 7469 6d65 6f75 7473 2069 6e20  oid timeouts in 
+0000f070: 6361 7365 2074 6865 2075 7365 7220 636f  case the user co
+0000f080: 6465 2069 7320 746f 6f20 636f 6d70 6c65  de is too comple
+0000f090: 7820 746f 0a20 2020 2020 2020 2020 2020  x to.           
+0000f0a0: 2020 2020 2070 726f 6365 7373 206c 6172       process lar
+0000f0b0: 6765 206e 756d 6265 7220 6f66 2072 6f77  ge number of row
+0000f0c0: 7320 6661 7374 2065 6e6f 7567 682e 2041  s fast enough. A
+0000f0d0: 2068 6967 6865 7220 6e75 6d62 6572 2063   higher number c
+0000f0e0: 616e 2062 650a 2020 2020 2020 2020 2020  an be.          
+0000f0f0: 2020 2020 2020 7573 6564 2074 6f20 696e        used to in
+0000f100: 6372 6561 7365 2074 6872 6f75 6768 7075  crease throughpu
+0000f110: 7420 696e 2063 6173 6520 7468 6520 7573  t in case the us
+0000f120: 6572 2063 6f64 6520 6973 2066 6173 7420  er code is fast 
+0000f130: 656e 6f75 6768 2e0a 2020 2020 2020 2020  enough..        
+0000f140: 2020 2020 2020 2020 604e 6f6e 6560 2063          `None` c
+0000f150: 616e 2062 6520 7061 7373 6564 2074 6f20  an be passed to 
+0000f160: 6c65 7420 4251 2072 656d 6f74 6520 6675  let BQ remote fu
+0000f170: 6e63 7469 6f6e 7320 7365 7276 6963 6520  nctions service 
+0000f180: 6170 706c 790a 2020 2020 2020 2020 2020  apply.          
+0000f190: 2020 2020 2020 6465 6661 756c 7420 6261        default ba
+0000f1a0: 7463 6869 6e67 2e20 5365 6520 666f 7220  tching. See for 
+0000f1b0: 6d6f 7265 2064 6574 6169 6c73 0a20 2020  more details.   
+0000f1c0: 2020 2020 2020 2020 2020 2020 2068 7474               htt
+0000f1d0: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
+0000f1e0: 652e 636f 6d2f 6269 6771 7565 7279 2f64  e.com/bigquery/d
+0000f1f0: 6f63 732f 7265 6d6f 7465 2d66 756e 6374  ocs/remote-funct
+0000f200: 696f 6e73 236c 696d 6974 696e 675f 6e75  ions#limiting_nu
+0000f210: 6d62 6572 5f6f 665f 726f 7773 5f69 6e5f  mber_of_rows_in_
+0000f220: 615f 6261 7463 685f 7265 7175 6573 742e  a_batch_request.
+0000f230: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+0000f240: 7564 5f66 756e 6374 696f 6e5f 7469 6d65  ud_function_time
+0000f250: 6f75 7420 2869 6e74 2c20 4f70 7469 6f6e  out (int, Option
+0000f260: 616c 293a 0a20 2020 2020 2020 2020 2020  al):.           
+0000f270: 2020 2020 2054 6865 206d 6178 696d 756d       The maximum
+0000f280: 2061 6d6f 756e 7420 6f66 2074 696d 6520   amount of time 
+0000f290: 2869 6e20 7365 636f 6e64 7329 2042 6967  (in seconds) Big
+0000f2a0: 5175 6572 7920 7368 6f75 6c64 2077 6169  Query should wai
+0000f2b0: 7420 666f 720a 2020 2020 2020 2020 2020  t for.          
+0000f2c0: 2020 2020 2020 7468 6520 636c 6f75 6420        the cloud 
+0000f2d0: 6675 6e63 7469 6f6e 2074 6f20 7265 7475  function to retu
+0000f2e0: 726e 2061 2072 6573 706f 6e73 652e 2053  rn a response. S
+0000f2f0: 6565 2066 6f72 206d 6f72 6520 6465 7461  ee for more deta
+0000f300: 696c 730a 2020 2020 2020 2020 2020 2020  ils.            
+0000f310: 2020 2020 6874 7470 733a 2f2f 636c 6f75      https://clou
+0000f320: 642e 676f 6f67 6c65 2e63 6f6d 2f66 756e  d.google.com/fun
+0000f330: 6374 696f 6e73 2f64 6f63 732f 636f 6e66  ctions/docs/conf
+0000f340: 6967 7572 696e 672f 7469 6d65 6f75 742e  iguring/timeout.
+0000f350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f360: 2050 6c65 6173 6520 6e6f 7465 2074 6861   Please note tha
+0000f370: 7420 6576 656e 2074 686f 7567 6820 7468  t even though th
+0000f380: 6520 636c 6f75 6420 6675 6e63 7469 6f6e  e cloud function
+0000f390: 2028 326e 6420 6765 6e29 2069 7473 656c   (2nd gen) itsel
+0000f3a0: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
+0000f3b0: 2020 616c 6c6f 7773 2073 6565 7469 6e67    allows seeting
+0000f3c0: 2075 7020 746f 2036 3020 6d69 6e75 7465   up to 60 minute
+0000f3d0: 7320 6f66 2074 696d 656f 7574 2c20 4269  s of timeout, Bi
+0000f3e0: 6751 7565 7279 2072 656d 6f74 650a 2020  gQuery remote.  
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000f400: 6e63 7469 6f6e 2063 616e 2077 6169 7420  nction can wait 
+0000f410: 6f6e 6c79 2075 7020 746f 2032 3020 6d69  only up to 20 mi
+0000f420: 6e75 7465 732c 2073 6565 2066 6f72 206d  nutes, see for m
+0000f430: 6f72 6520 6465 7461 696c 730a 2020 2020  ore details.    
+0000f440: 2020 2020 2020 2020 2020 2020 6874 7470              http
+0000f450: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+0000f460: 2e63 6f6d 2f62 6967 7175 6572 792f 7175  .com/bigquery/qu
+0000f470: 6f74 6173 2372 656d 6f74 655f 6675 6e63  otas#remote_func
+0000f480: 7469 6f6e 5f6c 696d 6974 732e 0a20 2020  tion_limits..   
+0000f490: 2020 2020 2020 2020 2020 2020 2042 7920               By 
+0000f4a0: 6465 6661 756c 7420 4269 6751 7565 7279  default BigQuery
+0000f4b0: 2044 6174 6146 7261 6d65 7320 7573 6573   DataFrames uses
+0000f4c0: 2061 2031 3020 6d69 6e75 7465 2074 696d   a 10 minute tim
+0000f4d0: 656f 7574 2e20 604e 6f6e 6560 0a20 2020  eout. `None`.   
+0000f4e0: 2020 2020 2020 2020 2020 2020 2063 616e               can
+0000f4f0: 2062 6520 7061 7373 6564 2074 6f20 6c65   be passed to le
+0000f500: 7420 7468 6520 636c 6f75 6420 6675 6e63  t the cloud func
+0000f510: 7469 6f6e 7320 6465 6661 756c 7420 7469  tions default ti
+0000f520: 6d65 6f75 7420 7461 6b65 2065 6666 6563  meout take effec
+0000f530: 742e 0a20 2020 2020 2020 2020 2020 2063  t..            c
+0000f540: 6c6f 7564 5f66 756e 6374 696f 6e5f 6d61  loud_function_ma
+0000f550: 785f 696e 7374 616e 6365 7320 2869 6e74  x_instances (int
+0000f560: 2c20 4f70 7469 6f6e 616c 293a 0a20 2020  , Optional):.   
+0000f570: 2020 2020 2020 2020 2020 2020 2054 6865               The
+0000f580: 206d 6178 696d 756d 6d20 696e 7374 616e   maximumm instan
+0000f590: 6365 2063 6f75 6e74 2066 6f72 2074 6865  ce count for the
+0000f5a0: 2063 6c6f 7564 2066 756e 6374 696f 6e20   cloud function 
+0000f5b0: 6372 6561 7465 642e 2054 6869 730a 2020  created. This.  
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+0000f5d0: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+0000f5e0: 7472 6f6c 2068 6f77 206d 616e 7920 636c  trol how many cl
+0000f5f0: 6f75 6420 6675 6e63 7469 6f6e 2069 6e73  oud function ins
+0000f600: 7461 6e63 6573 2063 616e 2062 650a 2020  tances can be.  
+0000f610: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+0000f620: 7469 7665 2061 7420 6d61 7820 6174 2061  tive at max at a
+0000f630: 6e79 2067 6976 656e 2070 6f69 6e74 206f  ny given point o
+0000f640: 6620 7469 6d65 2e20 4c6f 7765 7220 7365  f time. Lower se
+0000f650: 7474 696e 6720 6361 6e20 6865 6c70 0a20  tting can help. 
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f670: 6f6e 7472 6f6c 2074 6865 2073 7069 6b65  ontrol the spike
+0000f680: 2069 6e20 7468 6520 6269 6c6c 696e 672e   in the billing.
+0000f690: 2048 6967 6865 7220 7365 7474 696e 6720   Higher setting 
+0000f6a0: 6361 6e20 6865 6c70 0a20 2020 2020 2020  can help.       
+0000f6b0: 2020 2020 2020 2020 2073 7570 706f 7274           support
+0000f6c0: 2070 726f 6365 7373 696e 6720 6c61 7267   processing larg
+0000f6d0: 6572 2073 6361 6c65 2064 6174 612e 2057  er scale data. W
+0000f6e0: 6865 6e20 6e6f 7420 7370 6563 6966 6965  hen not specifie
+0000f6f0: 642c 2063 6c6f 7564 0a20 2020 2020 2020  d, cloud.       
+0000f700: 2020 2020 2020 2020 2066 756e 6374 696f           functio
+0000f710: 6e27 7320 6465 6661 756c 7420 7365 7474  n's default sett
+0000f720: 696e 6720 6170 706c 6965 732e 2046 6f72  ing applies. For
+0000f730: 206d 6f72 6520 6465 7461 696c 7320 7365   more details se
+0000f740: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f750: 2020 6874 7470 733a 2f2f 636c 6f75 642e    https://cloud.
+0000f760: 676f 6f67 6c65 2e63 6f6d 2f66 756e 6374  google.com/funct
+0000f770: 696f 6e73 2f64 6f63 732f 636f 6e66 6967  ions/docs/config
+0000f780: 7572 696e 672f 6d61 782d 696e 7374 616e  uring/max-instan
+0000f790: 6365 730a 2020 2020 2020 2020 5265 7475  ces.        Retu
+0000f7a0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000f7b0: 2063 616c 6c61 626c 653a 2041 2072 656d   callable: A rem
+0000f7c0: 6f74 6520 6675 6e63 7469 6f6e 206f 626a  ote function obj
+0000f7d0: 6563 7420 706f 696e 7469 6e67 2074 6f20  ect pointing to 
+0000f7e0: 7468 6520 636c 6f75 6420 6173 7365 7473  the cloud assets
+0000f7f0: 2063 7265 6174 6564 0a20 2020 2020 2020   created.       
+0000f800: 2020 2020 2069 6e20 7468 6520 6261 636b       in the back
+0000f810: 6772 6f75 6e64 2074 6f20 7375 7070 6f72  ground to suppor
+0000f820: 7420 7468 6520 7265 6d6f 7465 2065 7865  t the remote exe
+0000f830: 6375 7469 6f6e 2e20 5468 6520 636c 6f75  cution. The clou
+0000f840: 6420 6173 7365 7473 2063 616e 2062 650a  d assets can be.
+0000f850: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+0000f860: 7465 6420 7468 726f 7567 6820 7468 6520  ted through the 
+0000f870: 666f 6c6c 6f77 696e 6720 7072 6f70 6572  following proper
+0000f880: 7469 6573 2073 6574 2069 6e20 7468 6520  ties set in the 
+0000f890: 6f62 6a65 6374 3a0a 0a20 2020 2020 2020  object:..       
+0000f8a0: 2020 2020 2060 6269 6766 7261 6d65 735f       `bigframes_
+0000f8b0: 636c 6f75 645f 6675 6e63 7469 6f6e 6020  cloud_function` 
+0000f8c0: 2d20 5468 6520 676f 6f67 6c65 2063 6c6f  - The google clo
+0000f8d0: 7564 2066 756e 6374 696f 6e20 6465 706c  ud function depl
+0000f8e0: 6f79 6564 2066 6f72 2074 6865 2075 7365  oyed for the use
+0000f8f0: 7220 6465 6669 6e65 6420 636f 6465 2e0a  r defined code..
+0000f900: 0a20 2020 2020 2020 2020 2020 2060 6269  .            `bi
+0000f910: 6766 7261 6d65 735f 7265 6d6f 7465 5f66  gframes_remote_f
+0000f920: 756e 6374 696f 6e60 202d 2054 6865 2062  unction` - The b
+0000f930: 6967 7175 6572 7920 7265 6d6f 7465 2066  igquery remote f
+0000f940: 756e 6374 696f 6e20 6361 7061 626c 6520  unction capable 
+0000f950: 6f66 2063 616c 6c69 6e67 2069 6e74 6f20  of calling into 
+0000f960: 6062 6967 6672 616d 6573 5f63 6c6f 7564  `bigframes_cloud
+0000f970: 5f66 756e 6374 696f 6e60 2e0a 2020 2020  _function`..    
+0000f980: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f990: 7265 7475 726e 2062 6967 6672 616d 6573  return bigframes
+0000f9a0: 5f72 6628 0a20 2020 2020 2020 2020 2020  _rf(.           
+0000f9b0: 2069 6e70 7574 5f74 7970 6573 2c0a 2020   input_types,.  
+0000f9c0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+0000f9d0: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
+0000f9e0: 2020 2073 6573 7369 6f6e 3d73 656c 662c     session=self,
+0000f9f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000fa00: 6173 6574 3d64 6174 6173 6574 2c0a 2020  aset=dataset,.  
+0000fa10: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
+0000fa20: 7279 5f63 6f6e 6e65 6374 696f 6e3d 6269  ry_connection=bi
+0000fa30: 6771 7565 7279 5f63 6f6e 6e65 6374 696f  gquery_connectio
+0000fa40: 6e2c 0a20 2020 2020 2020 2020 2020 2072  n,.            r
+0000fa50: 6575 7365 3d72 6575 7365 2c0a 2020 2020  euse=reuse,.    
+0000fa60: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
+0000fa70: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+0000fa80: 6163 6b61 6765 733d 7061 636b 6167 6573  ackages=packages
+0000fa90: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+0000faa0: 6f75 645f 6675 6e63 7469 6f6e 5f73 6572  oud_function_ser
+0000fab0: 7669 6365 5f61 6363 6f75 6e74 3d63 6c6f  vice_account=clo
+0000fac0: 7564 5f66 756e 6374 696f 6e5f 7365 7276  ud_function_serv
+0000fad0: 6963 655f 6163 636f 756e 742c 0a20 2020  ice_account,.   
+0000fae0: 2020 2020 2020 2020 2063 6c6f 7564 5f66           cloud_f
+0000faf0: 756e 6374 696f 6e5f 6b6d 735f 6b65 795f  unction_kms_key_
+0000fb00: 6e61 6d65 3d63 6c6f 7564 5f66 756e 6374  name=cloud_funct
+0000fb10: 696f 6e5f 6b6d 735f 6b65 795f 6e61 6d65  ion_kms_key_name
+0000fb20: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+0000fb30: 6f75 645f 6675 6e63 7469 6f6e 5f64 6f63  oud_function_doc
+0000fb40: 6b65 725f 7265 706f 7369 746f 7279 3d63  ker_repository=c
+0000fb50: 6c6f 7564 5f66 756e 6374 696f 6e5f 646f  loud_function_do
+0000fb60: 636b 6572 5f72 6570 6f73 6974 6f72 792c  cker_repository,
+0000fb70: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000fb80: 5f62 6174 6368 696e 675f 726f 7773 3d6d  _batching_rows=m
+0000fb90: 6178 5f62 6174 6368 696e 675f 726f 7773  ax_batching_rows
+0000fba0: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+0000fbb0: 6f75 645f 6675 6e63 7469 6f6e 5f74 696d  oud_function_tim
+0000fbc0: 656f 7574 3d63 6c6f 7564 5f66 756e 6374  eout=cloud_funct
+0000fbd0: 696f 6e5f 7469 6d65 6f75 742c 0a20 2020  ion_timeout,.   
+0000fbe0: 2020 2020 2020 2020 2063 6c6f 7564 5f66           cloud_f
+0000fbf0: 756e 6374 696f 6e5f 6d61 785f 696e 7374  unction_max_inst
+0000fc00: 616e 6365 733d 636c 6f75 645f 6675 6e63  ances=cloud_func
+0000fc10: 7469 6f6e 5f6d 6178 5f69 6e73 7461 6e63  tion_max_instanc
+0000fc20: 6573 2c0a 2020 2020 2020 2020 290a 0a20  es,.        ).. 
+0000fc30: 2020 2064 6566 2072 6561 645f 6762 715f     def read_gbq_
+0000fc40: 6675 6e63 7469 6f6e 280a 2020 2020 2020  function(.      
+0000fc50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000fc60: 6675 6e63 7469 6f6e 5f6e 616d 653a 2073  function_name: s
+0000fc70: 7472 2c0a 2020 2020 293a 0a20 2020 2020  tr,.    ):.     
+0000fc80: 2020 2022 2222 4c6f 6164 7320 6120 4269     """Loads a Bi
+0000fc90: 6751 7565 7279 2066 756e 6374 696f 6e20  gQuery function 
+0000fca0: 6672 6f6d 2042 6967 5175 6572 792e 0a0a  from BigQuery...
+0000fcb0: 2020 2020 2020 2020 5468 656e 2069 7420          Then it 
+0000fcc0: 6361 6e20 6265 2061 7070 6c69 6564 2074  can be applied t
+0000fcd0: 6f20 6120 4461 7461 4672 616d 6520 6f72  o a DataFrame or
+0000fce0: 2053 6572 6965 732e 0a0a 2020 2020 2020   Series...      
+0000fcf0: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+0000fd00: 2020 2020 2020 2020 5468 6520 7265 7475          The retu
+0000fd10: 726e 2074 7970 6520 6f66 2074 6865 2066  rn type of the f
+0000fd20: 756e 6374 696f 6e20 6d75 7374 2062 6520  unction must be 
+0000fd30: 6578 706c 6963 6974 6c79 2073 7065 6369  explicitly speci
+0000fd40: 6669 6564 2069 6e20 7468 650a 2020 2020  fied in the.    
+0000fd50: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+0000fd60: 2773 206f 7269 6769 6e61 6c20 6465 6669  's original defi
+0000fd70: 6e69 7469 6f6e 2065 7665 6e20 6966 206e  nition even if n
+0000fd80: 6f74 206f 7468 6572 7769 7365 2072 6571  ot otherwise req
+0000fd90: 7569 7265 642e 0a0a 2020 2020 2020 2020  uired...        
+0000fda0: 4269 6751 7565 7279 2055 7469 6c73 2070  BigQuery Utils p
+0000fdb0: 726f 7669 6465 7320 6d61 6e79 2070 7562  rovides many pub
+0000fdc0: 6c69 6320 6675 6e63 7469 6f6e 7320 756e  lic functions un
+0000fdd0: 6465 7220 7468 6520 6060 6271 7574 696c  der the ``bqutil
+0000fde0: 6060 2070 726f 6a65 6374 206f 6e20 476f  `` project on Go
+0000fdf0: 6f67 6c65 2043 6c6f 7564 2050 6c61 7466  ogle Cloud Platf
+0000fe00: 6f72 6d20 7072 6f6a 6563 740a 2020 2020  orm project.    
+0000fe10: 2020 2020 2853 6565 3a20 6874 7470 733a      (See: https:
+0000fe20: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
+0000fe30: 676c 6543 6c6f 7564 506c 6174 666f 726d  gleCloudPlatform
+0000fe40: 2f62 6967 7175 6572 792d 7574 696c 732f  /bigquery-utils/
+0000fe50: 7472 6565 2f6d 6173 7465 722f 7564 6673  tree/master/udfs
+0000fe60: 2375 7369 6e67 2d74 6865 2d75 6466 7329  #using-the-udfs)
+0000fe70: 2e0a 2020 2020 2020 2020 596f 7520 6361  ..        You ca
+0000fe80: 6e20 6368 6563 6b6f 7574 2043 6f6d 6d75  n checkout Commu
+0000fe90: 6e69 7479 2055 4446 7320 746f 2075 7365  nity UDFs to use
+0000fea0: 2063 6f6d 6d75 6e69 7479 2d63 6f6e 7472   community-contr
+0000feb0: 6962 7574 6564 2066 756e 6374 696f 6e73  ibuted functions
+0000fec0: 2e0a 2020 2020 2020 2020 2853 6565 3a20  ..        (See: 
+0000fed0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000fee0: 6f6d 2f47 6f6f 676c 6543 6c6f 7564 506c  om/GoogleCloudPl
+0000fef0: 6174 666f 726d 2f62 6967 7175 6572 792d  atform/bigquery-
+0000ff00: 7574 696c 732f 7472 6565 2f6d 6173 7465  utils/tree/maste
+0000ff10: 722f 7564 6673 2f63 6f6d 6d75 6e69 7479  r/udfs/community
+0000ff20: 2363 6f6d 6d75 6e69 7479 2d75 6466 7329  #community-udfs)
+0000ff30: 2e0a 0a20 2020 2020 2020 202a 2a45 7861  ...        **Exa
+0000ff40: 6d70 6c65 733a 2a2a 0a0a 2020 2020 2020  mples:**..      
+0000ff50: 2020 5573 6520 7468 6520 6060 6377 5f6c    Use the ``cw_l
+0000ff60: 6f77 6572 5f63 6173 655f 6173 6369 695f  ower_case_ascii_
+0000ff70: 6f6e 6c79 6060 2066 756e 6374 696f 6e20  only`` function 
+0000ff80: 6672 6f6d 2043 6f6d 6d75 6e69 7479 2055  from Community U
+0000ff90: 4446 732e 0a20 2020 2020 2020 2028 6874  DFs..        (ht
+0000ffa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ffb0: 2f47 6f6f 676c 6543 6c6f 7564 506c 6174  /GoogleCloudPlat
+0000ffc0: 666f 726d 2f62 6967 7175 6572 792d 7574  form/bigquery-ut
+0000ffd0: 696c 732f 626c 6f62 2f6d 6173 7465 722f  ils/blob/master/
+0000ffe0: 7564 6673 2f63 6f6d 6d75 6e69 7479 2f63  udfs/community/c
+0000fff0: 775f 6c6f 7765 725f 6361 7365 5f61 7363  w_lower_case_asc
+00010000: 6969 5f6f 6e6c 792e 7371 6c78 290a 0a20  ii_only.sqlx).. 
+00010010: 2020 2020 2020 2020 2020 203e 3e3e 2069             >>> i
+00010020: 6d70 6f72 7420 6269 6766 7261 6d65 732e  mport bigframes.
+00010030: 7061 6e64 6173 2061 7320 6270 640a 2020  pandas as bpd.  
+00010040: 2020 2020 2020 2020 2020 3e3e 3e20 6270            >>> bp
+00010050: 642e 6f70 7469 6f6e 732e 6469 7370 6c61  d.options.displa
+00010060: 792e 7072 6f67 7265 7373 5f62 6172 203d  y.progress_bar =
+00010070: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
+00010080: 2020 203e 3e3e 2064 6620 3d20 6270 642e     >>> df = bpd.
+00010090: 4461 7461 4672 616d 6528 7b27 6964 273a  DataFrame({'id':
+000100a0: 205b 312c 2032 2c20 335d 2c20 276e 616d   [1, 2, 3], 'nam
+000100b0: 6527 3a20 5b27 4155 52c3 894c 4945 272c  e': ['AUR..LIE',
+000100c0: 2027 43c3 894c 4553 5449 4e45 272c 2027   'C..LESTINE', '
+000100d0: 4441 5048 4ec3 8927 5d7d 290a 2020 2020  DAPHN..']}).    
+000100e0: 2020 2020 2020 2020 3e3e 3e20 6466 0a20          >>> df. 
+000100f0: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00010100: 2020 2020 2020 206e 616d 650a 2020 2020         name.    
+00010110: 2020 2020 2020 2020 3020 2020 3120 2020          0   1   
+00010120: 2041 5552 c389 4c49 450a 2020 2020 2020   AUR..LIE.      
+00010130: 2020 2020 2020 3120 2020 3220 2043 c389        1   2  C..
+00010140: 4c45 5354 494e 450a 2020 2020 2020 2020  LESTINE.        
+00010150: 2020 2020 3220 2020 3320 2020 2020 4441      2   3     DA
+00010160: 5048 4ec3 890a 2020 2020 2020 2020 2020  PHN...          
+00010170: 2020 3c42 4c41 4e4b 4c49 4e45 3e0a 2020    <BLANKLINE>.  
+00010180: 2020 2020 2020 2020 2020 5b33 2072 6f77            [3 row
+00010190: 7320 7820 3220 636f 6c75 6d6e 735d 0a0a  s x 2 columns]..
+000101a0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000101b0: 6675 6e63 203d 2062 7064 2e72 6561 645f  func = bpd.read_
+000101c0: 6762 715f 6675 6e63 7469 6f6e 2822 6271  gbq_function("bq
+000101d0: 7574 696c 2e66 6e2e 6377 5f6c 6f77 6572  util.fn.cw_lower
+000101e0: 5f63 6173 655f 6173 6369 695f 6f6e 6c79  _case_ascii_only
+000101f0: 2229 0a20 2020 2020 2020 2020 2020 203e  ").            >
+00010200: 3e3e 2064 6631 203d 2064 662e 6173 7369  >> df1 = df.assi
+00010210: 676e 286e 6577 5f6e 616d 653d 6466 5b27  gn(new_name=df['
+00010220: 6e61 6d65 275d 2e61 7070 6c79 2866 756e  name'].apply(fun
+00010230: 6329 290a 2020 2020 2020 2020 2020 2020  c)).            
+00010240: 3e3e 3e20 6466 310a 2020 2020 2020 2020  >>> df1.        
+00010250: 2020 2020 2020 2069 6420 2020 2020 2020         id       
+00010260: 6e61 6d65 2020 206e 6577 5f6e 616d 650a  name   new_name.
+00010270: 2020 2020 2020 2020 2020 2020 3020 2020              0   
+00010280: 3120 2020 2041 5552 c389 4c49 4520 2020  1    AUR..LIE   
+00010290: 2061 7572 c389 6c69 650a 2020 2020 2020   aur..lie.      
+000102a0: 2020 2020 2020 3120 2020 3220 2043 c389        1   2  C..
+000102b0: 4c45 5354 494e 4520 2063 c389 6c65 7374  LESTINE  c..lest
+000102c0: 696e 650a 2020 2020 2020 2020 2020 2020  ine.            
+000102d0: 3220 2020 3320 2020 2020 4441 5048 4ec3  2   3     DAPHN.
+000102e0: 8920 2020 2020 6461 7068 6ec3 890a 2020  .     daphn...  
+000102f0: 2020 2020 2020 2020 2020 3c42 4c41 4e4b            <BLANK
+00010300: 4c49 4e45 3e0a 2020 2020 2020 2020 2020  LINE>.          
+00010310: 2020 5b33 2072 6f77 7320 7820 3320 636f    [3 rows x 3 co
+00010320: 6c75 6d6e 735d 0a0a 2020 2020 2020 2020  lumns]..        
+00010330: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00010340: 2020 6675 6e63 7469 6f6e 5f6e 616d 6520    function_name 
+00010350: 2873 7472 293a 0a20 2020 2020 2020 2020  (str):.         
+00010360: 2020 2020 2020 2074 6865 2066 756e 6374         the funct
+00010370: 696f 6e27 7320 6e61 6d65 2069 6e20 4269  ion's name in Bi
+00010380: 6751 7565 7279 2069 6e20 7468 6520 666f  gQuery in the fo
+00010390: 726d 6174 0a20 2020 2020 2020 2020 2020  rmat.           
+000103a0: 2020 2020 2060 7072 6f6a 6563 745f 6964       `project_id
+000103b0: 2e64 6174 6173 6574 5f69 642e 6675 6e63  .dataset_id.func
+000103c0: 7469 6f6e 5f6e 616d 6560 2c20 6f72 0a20  tion_name`, or. 
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+000103e0: 6461 7461 7365 745f 6964 2e66 756e 6374  dataset_id.funct
+000103f0: 696f 6e5f 6e61 6d65 6020 746f 206c 6f61  ion_name` to loa
+00010400: 6420 6672 6f6d 2074 6865 2064 6566 6175  d from the defau
+00010410: 6c74 2070 726f 6a65 6374 2c20 6f72 0a20  lt project, or. 
+00010420: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00010430: 6675 6e63 7469 6f6e 5f6e 616d 6560 2074  function_name` t
+00010440: 6f20 6c6f 6164 2066 726f 6d20 7468 6520  o load from the 
+00010450: 6465 6661 756c 7420 7072 6f6a 6563 7420  default project 
+00010460: 616e 6420 7468 6520 6461 7461 7365 740a  and the dataset.
+00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010480: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00010490: 7468 6520 6375 7272 656e 7420 7365 7373  the current sess
+000104a0: 696f 6e2e 0a0a 2020 2020 2020 2020 5265  ion...        Re
+000104b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000104c0: 2020 2063 616c 6c61 626c 653a 2041 2066     callable: A f
+000104d0: 756e 6374 696f 6e20 6f62 6a65 6374 2070  unction object p
+000104e0: 6f69 6e74 696e 6720 746f 2074 6865 2042  ointing to the B
+000104f0: 6967 5175 6572 7920 6675 6e63 7469 6f6e  igQuery function
+00010500: 2072 6561 640a 2020 2020 2020 2020 2020   read.          
+00010510: 2020 6672 6f6d 2042 6967 5175 6572 792e    from BigQuery.
+00010520: 0a0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00010530: 6520 6f62 6a65 6374 2069 7320 7369 6d69  e object is simi
+00010540: 6c61 7220 746f 2074 6865 206f 6e65 2063  lar to the one c
+00010550: 7265 6174 6564 2062 7920 7468 6520 6072  reated by the `r
+00010560: 656d 6f74 655f 6675 6e63 7469 6f6e 600a  emote_function`.
+00010570: 2020 2020 2020 2020 2020 2020 6465 636f              deco
+00010580: 7261 746f 722c 2069 6e63 6c75 6469 6e67  rator, including
+00010590: 2074 6865 2060 6269 6766 7261 6d65 735f   the `bigframes_
+000105a0: 7265 6d6f 7465 5f66 756e 6374 696f 6e60  remote_function`
+000105b0: 2070 726f 7065 7274 792c 2062 7574 0a20   property, but. 
+000105c0: 2020 2020 2020 2020 2020 206e 6f74 2069             not i
+000105d0: 6e63 6c75 6469 6e67 2074 6865 2060 6269  ncluding the `bi
+000105e0: 6766 7261 6d65 735f 636c 6f75 645f 6675  gframes_cloud_fu
+000105f0: 6e63 7469 6f6e 6020 7072 6f70 6572 7479  nction` property
+00010600: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00010610: 2020 2020 2020 2072 6574 7572 6e20 6269         return bi
+00010620: 6766 7261 6d65 735f 7267 6628 0a20 2020  gframes_rgf(.   
+00010630: 2020 2020 2020 2020 2066 756e 6374 696f           functio
+00010640: 6e5f 6e61 6d65 3d66 756e 6374 696f 6e5f  n_name=function_
+00010650: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00010660: 2020 7365 7373 696f 6e3d 7365 6c66 2c0a    session=self,.
+00010670: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00010680: 6566 205f 7072 6570 6172 655f 7175 6572  ef _prepare_quer
+00010690: 795f 6a6f 625f 636f 6e66 6967 280a 2020  y_job_config(.  
+000106a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000106b0: 2020 2020 6a6f 625f 636f 6e66 6967 3a20      job_config: 
+000106c0: 4f70 7469 6f6e 616c 5b62 6967 7175 6572  Optional[bigquer
+000106d0: 792e 5175 6572 794a 6f62 436f 6e66 6967  y.QueryJobConfig
+000106e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2920  ] = None,.    ) 
+000106f0: 2d3e 2062 6967 7175 6572 792e 5175 6572  -> bigquery.Quer
+00010700: 794a 6f62 436f 6e66 6967 3a0a 2020 2020  yJobConfig:.    
+00010710: 2020 2020 6966 206a 6f62 5f63 6f6e 6669      if job_confi
+00010720: 6720 6973 204e 6f6e 653a 0a20 2020 2020  g is None:.     
+00010730: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+00010740: 6720 3d20 6269 6771 7565 7279 2e51 7565  g = bigquery.Que
+00010750: 7279 4a6f 6243 6f6e 6669 6728 290a 2020  ryJobConfig().  
+00010760: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010770: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00010780: 2061 2063 6f70 7920 736f 2074 6861 7420   a copy so that 
+00010790: 7765 2064 6f6e 2774 206d 7574 6174 6520  we don't mutate 
+000107a0: 7468 6520 6f72 6967 696e 616c 2063 6f6e  the original con
+000107b0: 6669 6720 7061 7373 6564 0a20 2020 2020  fig passed.     
+000107c0: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+000107d0: 6720 3d20 7479 7069 6e67 2e63 6173 7428  g = typing.cast(
+000107e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000107f0: 2062 6967 7175 6572 792e 5175 6572 794a   bigquery.QueryJ
+00010800: 6f62 436f 6e66 6967 2c0a 2020 2020 2020  obConfig,.      
+00010810: 2020 2020 2020 2020 2020 6269 6771 7565            bigque
+00010820: 7279 2e51 7565 7279 4a6f 6243 6f6e 6669  ry.QueryJobConfi
+00010830: 672e 6672 6f6d 5f61 7069 5f72 6570 7228  g.from_api_repr(
+00010840: 6a6f 625f 636f 6e66 6967 2e74 6f5f 6170  job_config.to_ap
+00010850: 695f 7265 7072 2829 292c 0a20 2020 2020  i_repr()),.     
+00010860: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00010870: 2020 6966 2062 6967 6672 616d 6573 2e6f    if bigframes.o
+00010880: 7074 696f 6e73 2e63 6f6d 7075 7465 2e6d  ptions.compute.m
+00010890: 6178 696d 756d 5f62 7974 6573 5f62 696c  aximum_bytes_bil
+000108a0: 6c65 6420 6973 206e 6f74 204e 6f6e 653a  led is not None:
+000108b0: 0a20 2020 2020 2020 2020 2020 206a 6f62  .            job
+000108c0: 5f63 6f6e 6669 672e 6d61 7869 6d75 6d5f  _config.maximum_
+000108d0: 6279 7465 735f 6269 6c6c 6564 203d 2028  bytes_billed = (
+000108e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000108f0: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
+00010900: 6e73 2e63 6f6d 7075 7465 2e6d 6178 696d  ns.compute.maxim
+00010910: 756d 5f62 7974 6573 5f62 696c 6c65 640a  um_bytes_billed.
+00010920: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00010930: 2020 2020 2020 2063 7572 7265 6e74 5f6c         current_l
+00010940: 6162 656c 7320 3d20 6a6f 625f 636f 6e66  abels = job_conf
+00010950: 6967 2e6c 6162 656c 7320 6966 206a 6f62  ig.labels if job
+00010960: 5f63 6f6e 6669 672e 6c61 6265 6c73 2065  _config.labels e
+00010970: 6c73 6520 7b7d 0a20 2020 2020 2020 2066  lse {}.        f
+00010980: 6f72 206b 6579 2c20 7661 6c75 6520 696e  or key, value in
+00010990: 2062 6967 6672 616d 6573 2e6f 7074 696f   bigframes.optio
+000109a0: 6e73 2e63 6f6d 7075 7465 2e65 7874 7261  ns.compute.extra
+000109b0: 5f71 7565 7279 5f6c 6162 656c 732e 6974  _query_labels.it
+000109c0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+000109d0: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
+000109e0: 2063 7572 7265 6e74 5f6c 6162 656c 733a   current_labels:
+000109f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a00: 2063 7572 7265 6e74 5f6c 6162 656c 735b   current_labels[
+00010a10: 6b65 795d 203d 2076 616c 7565 0a20 2020  key] = value.   
+00010a20: 2020 2020 206a 6f62 5f63 6f6e 6669 672e       job_config.
+00010a30: 6c61 6265 6c73 203d 2063 7572 7265 6e74  labels = current
+00010a40: 5f6c 6162 656c 730a 0a20 2020 2020 2020  _labels..       
+00010a50: 2069 6620 7365 6c66 2e5f 6271 5f6b 6d73   if self._bq_kms
+00010a60: 5f6b 6579 5f6e 616d 653a 0a20 2020 2020  _key_name:.     
+00010a70: 2020 2020 2020 206a 6f62 5f63 6f6e 6669         job_confi
+00010a80: 672e 6465 7374 696e 6174 696f 6e5f 656e  g.destination_en
+00010a90: 6372 7970 7469 6f6e 5f63 6f6e 6669 6775  cryption_configu
+00010aa0: 7261 7469 6f6e 203d 2028 0a20 2020 2020  ration = (.     
+00010ab0: 2020 2020 2020 2020 2020 2062 6967 7175             bigqu
+00010ac0: 6572 792e 456e 6372 7970 7469 6f6e 436f  ery.EncryptionCo
+00010ad0: 6e66 6967 7572 6174 696f 6e28 6b6d 735f  nfiguration(kms_
+00010ae0: 6b65 795f 6e61 6d65 3d73 656c 662e 5f62  key_name=self._b
+00010af0: 715f 6b6d 735f 6b65 795f 6e61 6d65 290a  q_kms_key_name).
+00010b00: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00010b10: 2020 2020 2020 2072 6574 7572 6e20 6a6f         return jo
+00010b20: 625f 636f 6e66 6967 0a0a 2020 2020 6465  b_config..    de
+00010b30: 6620 5f70 7265 7061 7265 5f6c 6f61 645f  f _prepare_load_
+00010b40: 6a6f 625f 636f 6e66 6967 2873 656c 6629  job_config(self)
+00010b50: 202d 3e20 6269 6771 7565 7279 2e4c 6f61   -> bigquery.Loa
+00010b60: 644a 6f62 436f 6e66 6967 3a0a 2020 2020  dJobConfig:.    
+00010b70: 2020 2020 2320 4372 6561 7465 2061 2063      # Create a c
+00010b80: 6f70 7920 736f 2074 6861 7420 7765 2064  opy so that we d
+00010b90: 6f6e 2774 206d 7574 6174 6520 7468 6520  on't mutate the 
+00010ba0: 6f72 6967 696e 616c 2063 6f6e 6669 6720  original config 
+00010bb0: 7061 7373 6564 0a20 2020 2020 2020 206a  passed.        j
+00010bc0: 6f62 5f63 6f6e 6669 6720 3d20 6269 6771  ob_config = bigq
+00010bd0: 7565 7279 2e4c 6f61 644a 6f62 436f 6e66  uery.LoadJobConf
+00010be0: 6967 2829 0a0a 2020 2020 2020 2020 6966  ig()..        if
+00010bf0: 2073 656c 662e 5f62 715f 6b6d 735f 6b65   self._bq_kms_ke
+00010c00: 795f 6e61 6d65 3a0a 2020 2020 2020 2020  y_name:.        
+00010c10: 2020 2020 6a6f 625f 636f 6e66 6967 2e64      job_config.d
+00010c20: 6573 7469 6e61 7469 6f6e 5f65 6e63 7279  estination_encry
+00010c30: 7074 696f 6e5f 636f 6e66 6967 7572 6174  ption_configurat
+00010c40: 696f 6e20 3d20 280a 2020 2020 2020 2020  ion = (.        
+00010c50: 2020 2020 2020 2020 6269 6771 7565 7279          bigquery
+00010c60: 2e45 6e63 7279 7074 696f 6e43 6f6e 6669  .EncryptionConfi
+00010c70: 6775 7261 7469 6f6e 286b 6d73 5f6b 6579  guration(kms_key
+00010c80: 5f6e 616d 653d 7365 6c66 2e5f 6271 5f6b  _name=self._bq_k
+00010c90: 6d73 5f6b 6579 5f6e 616d 6529 0a20 2020  ms_key_name).   
+00010ca0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00010cb0: 2020 2020 7265 7475 726e 206a 6f62 5f63      return job_c
+00010cc0: 6f6e 6669 670a 0a20 2020 2064 6566 205f  onfig..    def _
+00010cd0: 7072 6570 6172 655f 636f 7079 5f6a 6f62  prepare_copy_job
+00010ce0: 5f63 6f6e 6669 6728 7365 6c66 2920 2d3e  _config(self) ->
+00010cf0: 2062 6967 7175 6572 792e 436f 7079 4a6f   bigquery.CopyJo
+00010d00: 6243 6f6e 6669 673a 0a20 2020 2020 2020  bConfig:.       
+00010d10: 2023 2043 7265 6174 6520 6120 636f 7079   # Create a copy
+00010d20: 2073 6f20 7468 6174 2077 6520 646f 6e27   so that we don'
+00010d30: 7420 6d75 7461 7465 2074 6865 206f 7269  t mutate the ori
+00010d40: 6769 6e61 6c20 636f 6e66 6967 2070 6173  ginal config pas
+00010d50: 7365 640a 2020 2020 2020 2020 6a6f 625f  sed.        job_
+00010d60: 636f 6e66 6967 203d 2062 6967 7175 6572  config = bigquer
+00010d70: 792e 436f 7079 4a6f 6243 6f6e 6669 6728  y.CopyJobConfig(
+00010d80: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00010d90: 6c66 2e5f 6271 5f6b 6d73 5f6b 6579 5f6e  lf._bq_kms_key_n
+00010da0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00010db0: 206a 6f62 5f63 6f6e 6669 672e 6465 7374   job_config.dest
+00010dc0: 696e 6174 696f 6e5f 656e 6372 7970 7469  ination_encrypti
+00010dd0: 6f6e 5f63 6f6e 6669 6775 7261 7469 6f6e  on_configuration
+00010de0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00010df0: 2020 2020 2062 6967 7175 6572 792e 456e       bigquery.En
+00010e00: 6372 7970 7469 6f6e 436f 6e66 6967 7572  cryptionConfigur
+00010e10: 6174 696f 6e28 6b6d 735f 6b65 795f 6e61  ation(kms_key_na
+00010e20: 6d65 3d73 656c 662e 5f62 715f 6b6d 735f  me=self._bq_kms_
+00010e30: 6b65 795f 6e61 6d65 290a 2020 2020 2020  key_name).      
+00010e40: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010e50: 2072 6574 7572 6e20 6a6f 625f 636f 6e66   return job_conf
+00010e60: 6967 0a0a 2020 2020 6465 6620 5f73 7461  ig..    def _sta
+00010e70: 7274 5f71 7565 7279 280a 2020 2020 2020  rt_query(.      
+00010e80: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00010e90: 7371 6c3a 2073 7472 2c0a 2020 2020 2020  sql: str,.      
+00010ea0: 2020 6a6f 625f 636f 6e66 6967 3a20 4f70    job_config: Op
+00010eb0: 7469 6f6e 616c 5b62 6967 7175 6572 792e  tional[bigquery.
+00010ec0: 6a6f 622e 5175 6572 794a 6f62 436f 6e66  job.QueryJobConf
+00010ed0: 6967 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ig] = None,.    
+00010ee0: 2020 2020 6d61 785f 7265 7375 6c74 733a      max_results:
+00010ef0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00010f00: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+00010f10: 696d 656f 7574 3a20 4f70 7469 6f6e 616c  imeout: Optional
+00010f20: 5b66 6c6f 6174 5d20 3d20 4e6f 6e65 2c0a  [float] = None,.
+00010f30: 2020 2020 2920 2d3e 2054 7570 6c65 5b62      ) -> Tuple[b
+00010f40: 6967 7175 6572 792e 7461 626c 652e 526f  igquery.table.Ro
+00010f50: 7749 7465 7261 746f 722c 2062 6967 7175  wIterator, bigqu
+00010f60: 6572 792e 5175 6572 794a 6f62 5d3a 0a20  ery.QueryJob]:. 
+00010f70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010f80: 2020 2053 7461 7274 7320 4269 6751 7565     Starts BigQue
+00010f90: 7279 2071 7565 7279 206a 6f62 2061 6e64  ry query job and
+00010fa0: 2077 6169 7473 2066 6f72 2072 6573 756c   waits for resul
+00010fb0: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
+00010fc0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+00010fd0: 6967 203d 2073 656c 662e 5f70 7265 7061  ig = self._prepa
+00010fe0: 7265 5f71 7565 7279 5f6a 6f62 5f63 6f6e  re_query_job_con
+00010ff0: 6669 6728 6a6f 625f 636f 6e66 6967 290a  fig(job_config).
+00011000: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00011010: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00011020: 2e5f 696f 2e62 6967 7175 6572 792e 7374  ._io.bigquery.st
+00011030: 6172 745f 7175 6572 795f 7769 7468 5f63  art_query_with_c
+00011040: 6c69 656e 7428 0a20 2020 2020 2020 2020  lient(.         
+00011050: 2020 2073 656c 662e 6271 636c 6965 6e74     self.bqclient
+00011060: 2c20 7371 6c2c 206a 6f62 5f63 6f6e 6669  , sql, job_confi
+00011070: 672c 206d 6178 5f72 6573 756c 7473 2c20  g, max_results, 
+00011080: 7469 6d65 6f75 740a 2020 2020 2020 2020  timeout.        
+00011090: 290a 0a20 2020 2064 6566 205f 7374 6172  )..    def _star
+000110a0: 745f 7175 6572 795f 6d6c 5f64 646c 280a  t_query_ml_ddl(.
+000110b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000110c0: 2020 2020 2020 7371 6c3a 2073 7472 2c0a        sql: str,.
+000110d0: 2020 2020 2920 2d3e 2054 7570 6c65 5b62      ) -> Tuple[b
+000110e0: 6967 7175 6572 792e 7461 626c 652e 526f  igquery.table.Ro
+000110f0: 7749 7465 7261 746f 722c 2062 6967 7175  wIterator, bigqu
+00011100: 6572 792e 5175 6572 794a 6f62 5d3a 0a20  ery.QueryJob]:. 
+00011110: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011120: 2020 2053 7461 7274 7320 4269 6751 7565     Starts BigQue
+00011130: 7279 204d 4c20 4444 4c20 7175 6572 7920  ry ML DDL query 
+00011140: 6a6f 6220 2843 5245 4154 4520 4d4f 4445  job (CREATE MODE
+00011150: 4c2f 414c 5445 5220 4d4f 4445 4c2f 2e2e  L/ALTER MODEL/..
+00011160: 2e29 2061 6e64 0a20 2020 2020 2020 2077  .) and.        w
+00011170: 6169 7473 2066 6f72 2072 6573 756c 7473  aits for results
+00011180: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00011190: 2020 2020 2020 6a6f 625f 636f 6e66 6967        job_config
+000111a0: 203d 2073 656c 662e 5f70 7265 7061 7265   = self._prepare
+000111b0: 5f71 7565 7279 5f6a 6f62 5f63 6f6e 6669  _query_job_confi
+000111c0: 6728 290a 0a20 2020 2020 2020 2023 2042  g()..        # B
+000111d0: 514d 4c20 6578 7065 6374 7320 6b6d 735f  QML expects kms_
+000111e0: 6b65 795f 6e61 6d65 2074 6872 6f75 6768  key_name through
+000111f0: 204f 5054 494f 4e53 2061 6e64 206e 6f74   OPTIONS and not
+00011200: 2074 6872 6f75 6768 206a 6f62 2063 6f6e   through job con
+00011210: 6669 672c 0a20 2020 2020 2020 2023 2073  fig,.        # s
+00011220: 6f20 7765 206d 7573 7420 7265 7365 7420  o we must reset 
+00011230: 616e 7920 656e 6372 7970 7469 6f6e 2073  any encryption s
+00011240: 6574 2069 6e20 7468 6520 6a6f 6220 636f  et in the job co
+00011250: 6e66 6967 0a20 2020 2020 2020 2023 2068  nfig.        # h
+00011260: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
+00011270: 676c 652e 636f 6d2f 6269 6771 7565 7279  gle.com/bigquery
+00011280: 2f64 6f63 732f 6375 7374 6f6d 6572 2d6d  /docs/customer-m
+00011290: 616e 6167 6564 2d65 6e63 7279 7074 696f  anaged-encryptio
+000112a0: 6e23 656e 6372 7970 742d 6d6f 6465 6c0a  n#encrypt-model.
+000112b0: 2020 2020 2020 2020 6a6f 625f 636f 6e66          job_conf
+000112c0: 6967 2e64 6573 7469 6e61 7469 6f6e 5f65  ig.destination_e
+000112d0: 6e63 7279 7074 696f 6e5f 636f 6e66 6967  ncryption_config
+000112e0: 7572 6174 696f 6e20 3d20 4e6f 6e65 0a0a  uration = None..
+000112f0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00011300: 6967 6672 616d 6573 2e73 6573 7369 6f6e  igframes.session
+00011310: 2e5f 696f 2e62 6967 7175 6572 792e 7374  ._io.bigquery.st
+00011320: 6172 745f 7175 6572 795f 7769 7468 5f63  art_query_with_c
+00011330: 6c69 656e 7428 0a20 2020 2020 2020 2020  lient(.         
+00011340: 2020 2073 656c 662e 6271 636c 6965 6e74     self.bqclient
+00011350: 2c20 7371 6c2c 206a 6f62 5f63 6f6e 6669  , sql, job_confi
+00011360: 670a 2020 2020 2020 2020 290a 0a20 2020  g.        )..   
+00011370: 2064 6566 205f 6361 6368 655f 7769 7468   def _cache_with
+00011380: 5f63 6c75 7374 6572 5f63 6f6c 7328 0a20  _cluster_cols(. 
+00011390: 2020 2020 2020 2073 656c 662c 2061 7272         self, arr
+000113a0: 6179 5f76 616c 7565 3a20 636f 7265 2e41  ay_value: core.A
+000113b0: 7272 6179 5661 6c75 652c 2063 6c75 7374  rrayValue, clust
+000113c0: 6572 5f63 6f6c 733a 2074 7970 696e 672e  er_cols: typing.
+000113d0: 5365 7175 656e 6365 5b73 7472 5d0a 2020  Sequence[str].  
+000113e0: 2020 2920 2d3e 2063 6f72 652e 4172 7261    ) -> core.Arra
+000113f0: 7956 616c 7565 3a0a 2020 2020 2020 2020  yValue:.        
+00011400: 2222 2245 7865 6375 7465 7320 7468 6520  """Executes the 
+00011410: 7175 6572 7920 616e 6420 7573 6573 2074  query and uses t
+00011420: 6865 2072 6573 756c 7469 6e67 2074 6162  he resulting tab
+00011430: 6c65 2074 6f20 7265 7772 6974 6520 6675  le to rewrite fu
+00011440: 7475 7265 2065 7865 6375 7469 6f6e 732e  ture executions.
+00011450: 2222 220a 2020 2020 2020 2020 2320 544f  """.        # TO
+00011460: 444f 3a20 5573 6520 7468 6973 2066 6f72  DO: Use this for
+00011470: 2061 6c6c 2065 7865 6375 7469 6f6e 733f   all executions?
+00011480: 2050 726f 626c 656d 2069 7320 7468 6174   Problem is that
+00011490: 2063 6163 6869 6e67 206d 6174 6572 6961   caching materia
+000114a0: 6c69 7a65 7320 6578 7472 610a 2020 2020  lizes extra.    
+000114b0: 2020 2020 2320 6f72 6465 7269 6e67 2063      # ordering c
+000114c0: 6f6c 756d 6e73 0a20 2020 2020 2020 2063  olumns.        c
+000114d0: 6f6d 7069 6c65 645f 7661 6c75 6520 3d20  ompiled_value = 
+000114e0: 7365 6c66 2e5f 636f 6d70 696c 655f 6f72  self._compile_or
+000114f0: 6465 7265 6428 6172 7261 795f 7661 6c75  dered(array_valu
+00011500: 6529 0a0a 2020 2020 2020 2020 6962 6973  e)..        ibis
+00011510: 5f65 7870 7220 3d20 636f 6d70 696c 6564  _expr = compiled
+00011520: 5f76 616c 7565 2e5f 746f 5f69 6269 735f  _value._to_ibis_
+00011530: 6578 7072 280a 2020 2020 2020 2020 2020  expr(.          
+00011540: 2020 6f72 6465 7269 6e67 5f6d 6f64 653d    ordering_mode=
+00011550: 2275 6e6f 7264 6572 6564 222c 2065 7870  "unordered", exp
+00011560: 6f73 655f 6869 6464 656e 5f63 6f6c 733d  ose_hidden_cols=
+00011570: 5472 7565 0a20 2020 2020 2020 2029 0a20  True.        ). 
+00011580: 2020 2020 2020 2074 6d70 5f74 6162 6c65         tmp_table
+00011590: 203d 2073 656c 662e 5f69 6269 735f 746f   = self._ibis_to
+000115a0: 5f74 656d 705f 7461 626c 6528 0a20 2020  _temp_table(.   
+000115b0: 2020 2020 2020 2020 2069 6269 735f 6578           ibis_ex
+000115c0: 7072 2c20 636c 7573 7465 725f 636f 6c73  pr, cluster_cols
+000115d0: 3d63 6c75 7374 6572 5f63 6f6c 732c 2061  =cluster_cols, a
+000115e0: 7069 5f6e 616d 653d 2263 6163 6865 6422  pi_name="cached"
+000115f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00011600: 2020 2074 6162 6c65 5f65 7870 7265 7373     table_express
+00011610: 696f 6e20 3d20 7365 6c66 2e69 6269 735f  ion = self.ibis_
+00011620: 636c 6965 6e74 2e74 6162 6c65 280a 2020  client.table(.  
+00011630: 2020 2020 2020 2020 2020 746d 705f 7461            tmp_ta
+00011640: 626c 652e 7461 626c 655f 6964 2c0a 2020  ble.table_id,.  
+00011650: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00011660: 3d74 6d70 5f74 6162 6c65 2e64 6174 6173  =tmp_table.datas
+00011670: 6574 5f69 642c 0a20 2020 2020 2020 2020  et_id,.         
+00011680: 2020 2064 6174 6162 6173 653d 746d 705f     database=tmp_
+00011690: 7461 626c 652e 7072 6f6a 6563 742c 0a20  table.project,. 
+000116a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000116b0: 206e 6577 5f63 6f6c 756d 6e73 203d 205b   new_columns = [
+000116c0: 7461 626c 655f 6578 7072 6573 7369 6f6e  table_expression
+000116d0: 5b63 6f6c 756d 6e5d 2066 6f72 2063 6f6c  [column] for col
+000116e0: 756d 6e20 696e 2063 6f6d 7069 6c65 645f  umn in compiled_
+000116f0: 7661 6c75 652e 636f 6c75 6d6e 5f69 6473  value.column_ids
+00011700: 5d0a 2020 2020 2020 2020 6e65 775f 6869  ].        new_hi
+00011710: 6464 656e 5f63 6f6c 756d 6e73 203d 205b  dden_columns = [
+00011720: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+00011730: 6c65 5f65 7870 7265 7373 696f 6e5b 636f  le_expression[co
+00011740: 6c75 6d6e 5d0a 2020 2020 2020 2020 2020  lumn].          
+00011750: 2020 666f 7220 636f 6c75 6d6e 2069 6e20    for column in 
+00011760: 636f 6d70 696c 6564 5f76 616c 7565 2e5f  compiled_value._
+00011770: 6869 6464 656e 5f6f 7264 6572 696e 675f  hidden_ordering_
+00011780: 636f 6c75 6d6e 5f6e 616d 6573 0a20 2020  column_names.   
+00011790: 2020 2020 205d 0a20 2020 2020 2020 2023       ].        #
+000117a0: 2054 4f44 4f3a 2049 6e73 7465 6164 2c20   TODO: Instead, 
+000117b0: 6b65 6570 2073 6573 7369 6f6e 2d77 6964  keep session-wid
+000117c0: 6520 6d61 7020 6f66 2063 6163 6865 6420  e map of cached 
+000117d0: 7265 7375 6c74 7320 616e 6420 6175 746f  results and auto
+000117e0: 6d61 7469 6361 6c6c 7920 7265 7573 650a  matically reuse.
+000117f0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00011800: 6f72 652e 4172 7261 7956 616c 7565 2e66  ore.ArrayValue.f
+00011810: 726f 6d5f 6962 6973 280a 2020 2020 2020  rom_ibis(.      
+00011820: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00011830: 2020 2020 2020 2020 7461 626c 655f 6578          table_ex
+00011840: 7072 6573 7369 6f6e 2c0a 2020 2020 2020  pression,.      
+00011850: 2020 2020 2020 636f 6c75 6d6e 733d 6e65        columns=ne
+00011860: 775f 636f 6c75 6d6e 732c 0a20 2020 2020  w_columns,.     
+00011870: 2020 2020 2020 2068 6964 6465 6e5f 6f72         hidden_or
+00011880: 6465 7269 6e67 5f63 6f6c 756d 6e73 3d6e  dering_columns=n
+00011890: 6577 5f68 6964 6465 6e5f 636f 6c75 6d6e  ew_hidden_column
+000118a0: 732c 0a20 2020 2020 2020 2020 2020 206f  s,.            o
+000118b0: 7264 6572 696e 673d 636f 6d70 696c 6564  rdering=compiled
+000118c0: 5f76 616c 7565 2e5f 6f72 6465 7269 6e67  _value._ordering
+000118d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+000118e0: 2064 6566 205f 6361 6368 655f 7769 7468   def _cache_with
+000118f0: 5f6f 6666 7365 7473 2873 656c 662c 2061  _offsets(self, a
+00011900: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
+00011910: 2e41 7272 6179 5661 6c75 6529 202d 3e20  .ArrayValue) -> 
+00011920: 636f 7265 2e41 7272 6179 5661 6c75 653a  core.ArrayValue:
+00011930: 0a20 2020 2020 2020 2022 2222 4578 6563  .        """Exec
+00011940: 7574 6573 2074 6865 2071 7565 7279 2061  utes the query a
+00011950: 6e64 2075 7365 7320 7468 6520 7265 7375  nd uses the resu
+00011960: 6c74 696e 6720 7461 626c 6520 746f 2072  lting table to r
+00011970: 6577 7269 7465 2066 7574 7572 6520 6578  ewrite future ex
+00011980: 6563 7574 696f 6e73 2e22 2222 0a20 2020  ecutions.""".   
+00011990: 2020 2020 2023 2054 4f44 4f3a 2055 7365       # TODO: Use
+000119a0: 2074 6869 7320 666f 7220 616c 6c20 6578   this for all ex
+000119b0: 6563 7574 696f 6e73 3f20 5072 6f62 6c65  ecutions? Proble
+000119c0: 6d20 6973 2074 6861 7420 6361 6368 696e  m is that cachin
+000119d0: 6720 6d61 7465 7269 616c 697a 6573 2065  g materializes e
+000119e0: 7874 7261 0a20 2020 2020 2020 2023 206f  xtra.        # o
+000119f0: 7264 6572 696e 6720 636f 6c75 6d6e 730a  rdering columns.
+00011a00: 2020 2020 2020 2020 636f 6d70 696c 6564          compiled
+00011a10: 5f76 616c 7565 203d 2073 656c 662e 5f63  _value = self._c
+00011a20: 6f6d 7069 6c65 5f6f 7264 6572 6564 2861  ompile_ordered(a
+00011a30: 7272 6179 5f76 616c 7565 290a 0a20 2020  rray_value)..   
+00011a40: 2020 2020 2069 6269 735f 6578 7072 203d       ibis_expr =
+00011a50: 2063 6f6d 7069 6c65 645f 7661 6c75 652e   compiled_value.
+00011a60: 5f74 6f5f 6962 6973 5f65 7870 7228 0a20  _to_ibis_expr(. 
+00011a70: 2020 2020 2020 2020 2020 206f 7264 6572             order
+00011a80: 696e 675f 6d6f 6465 3d22 6f66 6673 6574  ing_mode="offset
+00011a90: 5f63 6f6c 222c 206f 7264 6572 5f63 6f6c  _col", order_col
+00011aa0: 5f6e 616d 653d 2262 6967 6672 616d 6573  _name="bigframes
+00011ab0: 5f6f 6666 7365 7473 220a 2020 2020 2020  _offsets".      
+00011ac0: 2020 290a 2020 2020 2020 2020 746d 705f    ).        tmp_
+00011ad0: 7461 626c 6520 3d20 7365 6c66 2e5f 6962  table = self._ib
+00011ae0: 6973 5f74 6f5f 7465 6d70 5f74 6162 6c65  is_to_temp_table
+00011af0: 280a 2020 2020 2020 2020 2020 2020 6962  (.            ib
+00011b00: 6973 5f65 7870 722c 2063 6c75 7374 6572  is_expr, cluster
+00011b10: 5f63 6f6c 733d 5b22 6269 6766 7261 6d65  _cols=["bigframe
+00011b20: 735f 6f66 6673 6574 7322 5d2c 2061 7069  s_offsets"], api
+00011b30: 5f6e 616d 653d 2263 6163 6865 6422 0a20  _name="cached". 
+00011b40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011b50: 2074 6162 6c65 5f65 7870 7265 7373 696f   table_expressio
+00011b60: 6e20 3d20 7365 6c66 2e69 6269 735f 636c  n = self.ibis_cl
+00011b70: 6965 6e74 2e74 6162 6c65 280a 2020 2020  ient.table(.    
+00011b80: 2020 2020 2020 2020 746d 705f 7461 626c          tmp_tabl
+00011b90: 652e 7461 626c 655f 6964 2c0a 2020 2020  e.table_id,.    
+00011ba0: 2020 2020 2020 2020 7363 6865 6d61 3d74          schema=t
+00011bb0: 6d70 5f74 6162 6c65 2e64 6174 6173 6574  mp_table.dataset
+00011bc0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00011bd0: 2064 6174 6162 6173 653d 746d 705f 7461   database=tmp_ta
+00011be0: 626c 652e 7072 6f6a 6563 742c 0a20 2020  ble.project,.   
+00011bf0: 2020 2020 2029 0a20 2020 2020 2020 206e       ).        n
+00011c00: 6577 5f63 6f6c 756d 6e73 203d 205b 7461  ew_columns = [ta
+00011c10: 626c 655f 6578 7072 6573 7369 6f6e 5b63  ble_expression[c
+00011c20: 6f6c 756d 6e5d 2066 6f72 2063 6f6c 756d  olumn] for colum
+00011c30: 6e20 696e 2063 6f6d 7069 6c65 645f 7661  n in compiled_va
+00011c40: 6c75 652e 636f 6c75 6d6e 5f69 6473 5d0a  lue.column_ids].
+00011c50: 2020 2020 2020 2020 6e65 775f 6869 6464          new_hidd
+00011c60: 656e 5f63 6f6c 756d 6e73 203d 205b 7461  en_columns = [ta
+00011c70: 626c 655f 6578 7072 6573 7369 6f6e 5b22  ble_expression["
+00011c80: 6269 6766 7261 6d65 735f 6f66 6673 6574  bigframes_offset
+00011c90: 7322 5d5d 0a20 2020 2020 2020 2023 2054  s"]].        # T
+00011ca0: 4f44 4f3a 2049 6e73 7465 6164 2c20 6b65  ODO: Instead, ke
+00011cb0: 6570 2073 6573 7369 6f6e 2d77 6964 6520  ep session-wide 
+00011cc0: 6d61 7020 6f66 2063 6163 6865 6420 7265  map of cached re
+00011cd0: 7375 6c74 7320 616e 6420 6175 746f 6d61  sults and automa
+00011ce0: 7469 6361 6c6c 7920 7265 7573 650a 2020  tically reuse.  
+00011cf0: 2020 2020 2020 7265 7475 726e 2063 6f72        return cor
+00011d00: 652e 4172 7261 7956 616c 7565 2e66 726f  e.ArrayValue.fro
+00011d10: 6d5f 6962 6973 280a 2020 2020 2020 2020  m_ibis(.        
+00011d20: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00011d30: 2020 2020 2020 7461 626c 655f 6578 7072        table_expr
+00011d40: 6573 7369 6f6e 2c0a 2020 2020 2020 2020  ession,.        
+00011d50: 2020 2020 636f 6c75 6d6e 733d 6e65 775f      columns=new_
+00011d60: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
+00011d70: 2020 2020 2068 6964 6465 6e5f 6f72 6465       hidden_orde
+00011d80: 7269 6e67 5f63 6f6c 756d 6e73 3d6e 6577  ring_columns=new
+00011d90: 5f68 6964 6465 6e5f 636f 6c75 6d6e 732c  _hidden_columns,
+00011da0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+00011db0: 6572 696e 673d 6f72 6465 722e 4578 7072  ering=order.Expr
+00011dc0: 6573 7369 6f6e 4f72 6465 7269 6e67 2e66  essionOrdering.f
+00011dd0: 726f 6d5f 6f66 6673 6574 5f63 6f6c 2822  rom_offset_col("
+00011de0: 6269 6766 7261 6d65 735f 6f66 6673 6574  bigframes_offset
+00011df0: 7322 292c 0a20 2020 2020 2020 2029 0a0a  s"),.        )..
+00011e00: 2020 2020 6465 6620 5f73 696d 706c 6966      def _simplif
+00011e10: 795f 7769 7468 5f63 6163 6869 6e67 2873  y_with_caching(s
+00011e20: 656c 662c 2061 7272 6179 5f76 616c 7565  elf, array_value
+00011e30: 3a20 636f 7265 2e41 7272 6179 5661 6c75  : core.ArrayValu
+00011e40: 6529 202d 3e20 636f 7265 2e41 7272 6179  e) -> core.Array
+00011e50: 5661 6c75 653a 0a20 2020 2020 2020 2022  Value:.        "
+00011e60: 2222 4174 7465 6d70 7473 2074 6f20 6861  ""Attempts to ha
+00011e70: 6e64 6c65 2074 6865 2063 6f6d 706c 6578  ndle the complex
+00011e80: 6974 7920 6279 2063 6163 6869 6e67 2064  ity by caching d
+00011e90: 7570 6c69 6361 7465 6420 7375 6274 7265  uplicated subtre
+00011ea0: 6573 2061 6e64 2062 7265 616b 696e 6720  es and breaking 
+00011eb0: 7468 6520 7175 6572 7920 696e 746f 2070  the query into p
+00011ec0: 6965 6365 732e 2222 220a 2020 2020 2020  ieces.""".      
+00011ed0: 2020 6966 206e 6f74 2062 6967 6672 616d    if not bigfram
+00011ee0: 6573 2e6f 7074 696f 6e73 2e63 6f6d 7075  es.options.compu
+00011ef0: 7465 2e65 6e61 626c 655f 6d75 6c74 695f  te.enable_multi_
+00011f00: 7175 6572 795f 6578 6563 7574 696f 6e3a  query_execution:
+00011f10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011f20: 7572 6e20 6172 7261 795f 7661 6c75 650a  urn array_value.
+00011f30: 2020 2020 2020 2020 6e6f 6465 203d 2061          node = a
+00011f40: 7272 6179 5f76 616c 7565 2e6e 6f64 650a  rray_value.node.
+00011f50: 2020 2020 2020 2020 6966 206e 6f64 652e          if node.
+00011f60: 706c 616e 6e69 6e67 5f63 6f6d 706c 6578  planning_complex
+00011f70: 6974 7920 3c20 5155 4552 595f 434f 4d50  ity < QUERY_COMP
+00011f80: 4c45 5849 5459 5f4c 494d 4954 3a0a 2020  LEXITY_LIMIT:.  
+00011f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011fa0: 2061 7272 6179 5f76 616c 7565 0a0a 2020   array_value..  
+00011fb0: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
+00011fc0: 616e 6765 284d 4158 5f53 5542 5452 4545  ange(MAX_SUBTREE
+00011fd0: 5f46 4143 544f 5249 4e47 5329 3a0a 2020  _FACTORINGS):.  
+00011fe0: 2020 2020 2020 2020 2020 7570 6461 7465            update
+00011ff0: 6420 3d20 7365 6c66 2e5f 6361 6368 655f  d = self._cache_
+00012000: 6d6f 7374 5f63 6f6d 706c 6578 5f73 7562  most_complex_sub
+00012010: 7472 6565 286e 6f64 6529 0a20 2020 2020  tree(node).     
+00012020: 2020 2020 2020 2069 6620 7570 6461 7465         if update
+00012030: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
+00012040: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00012050: 6e20 636f 7265 2e41 7272 6179 5661 6c75  n core.ArrayValu
+00012060: 6528 6e6f 6465 290a 2020 2020 2020 2020  e(node).        
+00012070: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012080: 2020 2020 2020 2020 2020 6e6f 6465 203d            node =
+00012090: 2075 7064 6174 6564 0a0a 2020 2020 2020   updated..      
+000120a0: 2020 7265 7475 726e 2063 6f72 652e 4172    return core.Ar
+000120b0: 7261 7956 616c 7565 286e 6f64 6529 0a0a  rayValue(node)..
+000120c0: 2020 2020 6465 6620 5f63 6163 6865 5f6d      def _cache_m
+000120d0: 6f73 745f 636f 6d70 6c65 785f 7375 6274  ost_complex_subt
+000120e0: 7265 6528 0a20 2020 2020 2020 2073 656c  ree(.        sel
+000120f0: 662c 206e 6f64 653a 206e 6f64 6573 2e42  f, node: nodes.B
+00012100: 6967 4672 616d 654e 6f64 650a 2020 2020  igFrameNode.    
+00012110: 2920 2d3e 204f 7074 696f 6e61 6c5b 6e6f  ) -> Optional[no
+00012120: 6465 732e 4269 6746 7261 6d65 4e6f 6465  des.BigFrameNode
+00012130: 5d3a 0a20 2020 2020 2020 2023 2054 4f44  ]:.        # TOD
+00012140: 4f3a 2049 6620 7175 6572 7920 6661 696c  O: If query fail
+00012150: 732c 2072 6574 7279 2077 6974 6820 6c6f  s, retry with lo
+00012160: 7765 7220 636f 6d70 6c65 7869 7479 206c  wer complexity l
+00012170: 696d 6974 0a20 2020 2020 2020 2076 616c  imit.        val
+00012180: 6964 5f63 616e 6469 6461 7465 7320 3d20  id_candidates = 
+00012190: 7472 6176 6572 7361 6c73 2e63 6f75 6e74  traversals.count
+000121a0: 5f63 6f6d 706c 6578 5f6e 6f64 6573 280a  _complex_nodes(.
+000121b0: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+000121c0: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
+000121d0: 6e5f 636f 6d70 6c65 7869 7479 3d28 5155  n_complexity=(QU
+000121e0: 4552 595f 434f 4d50 4c45 5849 5459 5f4c  ERY_COMPLEXITY_L
+000121f0: 494d 4954 202f 2035 3030 292c 0a20 2020  IMIT / 500),.   
+00012200: 2020 2020 2020 2020 206d 6178 5f63 6f6d           max_com
+00012210: 706c 6578 6974 793d 5155 4552 595f 434f  plexity=QUERY_CO
+00012220: 4d50 4c45 5849 5459 5f4c 494d 4954 2c0a  MPLEXITY_LIMIT,.
+00012230: 2020 2020 2020 2020 292e 6974 656d 7328          ).items(
+00012240: 290a 2020 2020 2020 2020 2320 4865 7572  ).        # Heur
+00012250: 6973 7469 633a 2073 7562 7472 6565 5f63  istic: subtree_c
+00012260: 6f6d 706c 6569 7874 7920 2a20 2863 6f70  ompleixty * (cop
+00012270: 6965 7320 6f66 2073 7562 7472 6565 295e  ies of subtree)^
+00012280: 320a 2020 2020 2020 2020 6265 7374 5f63  2.        best_c
+00012290: 616e 6469 6461 7465 203d 206d 6178 280a  andidate = max(.
+000122a0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+000122b0: 645f 6361 6e64 6964 6174 6573 2c0a 2020  d_candidates,.  
+000122c0: 2020 2020 2020 2020 2020 6b65 793d 6c61            key=la
+000122d0: 6d62 6461 2069 3a20 695b 305d 2e70 6c61  mbda i: i[0].pla
+000122e0: 6e6e 696e 675f 636f 6d70 6c65 7869 7479  nning_complexity
+000122f0: 202b 2028 695b 315d 202a 2a20 3229 2c0a   + (i[1] ** 2),.
+00012300: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00012310: 756c 743d 4e6f 6e65 2c0a 2020 2020 2020  ult=None,.      
+00012320: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00012330: 6265 7374 5f63 616e 6469 6461 7465 2069  best_candidate i
+00012340: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00012350: 2020 2020 2320 4e6f 2067 6f6f 6420 7375      # No good su
+00012360: 6274 7265 6573 2074 6f20 6361 6368 652c  btrees to cache,
+00012370: 206a 7573 7420 7265 7475 726e 206f 7269   just return ori
+00012380: 6769 6e61 6c20 7472 6565 0a20 2020 2020  ginal tree.     
+00012390: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000123a0: 6e65 0a0a 2020 2020 2020 2020 2320 544f  ne..        # TO
+000123b0: 444f 3a20 4164 6420 636c 7573 7465 7269  DO: Add clusteri
+000123c0: 6e67 2063 6f6c 756d 6e73 2062 6173 6564  ng columns based
+000123d0: 206f 6e20 6163 6365 7373 2070 6174 7465   on access patte
+000123e0: 726e 730a 2020 2020 2020 2020 6d61 7465  rns.        mate
+000123f0: 7269 616c 697a 6564 203d 2073 656c 662e  rialized = self.
+00012400: 5f63 6163 6865 5f77 6974 685f 636c 7573  _cache_with_clus
+00012410: 7465 725f 636f 6c73 280a 2020 2020 2020  ter_cols(.      
+00012420: 2020 2020 2020 636f 7265 2e41 7272 6179        core.Array
+00012430: 5661 6c75 6528 6265 7374 5f63 616e 6469  Value(best_candi
+00012440: 6461 7465 5b30 5d29 2c20 5b5d 0a20 2020  date[0]), [].   
+00012450: 2020 2020 2029 2e6e 6f64 650a 0a20 2020       ).node..   
+00012460: 2020 2020 2072 6574 7572 6e20 7472 6176       return trav
+00012470: 6572 7361 6c73 2e72 6570 6c61 6365 5f6e  ersals.replace_n
+00012480: 6f64 6573 280a 2020 2020 2020 2020 2020  odes(.          
+00012490: 2020 6e6f 6465 2c20 746f 5f72 6570 6c61    node, to_repla
+000124a0: 6365 3d62 6573 745f 6361 6e64 6964 6174  ce=best_candidat
+000124b0: 655b 305d 2c20 7265 706c 6163 656d 656e  e[0], replacemen
+000124c0: 6574 3d6d 6174 6572 6961 6c69 7a65 640a  et=materialized.
+000124d0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+000124e0: 6566 205f 6973 5f74 7269 7669 616c 6c79  ef _is_trivially
+000124f0: 5f65 7865 6375 7461 626c 6528 7365 6c66  _executable(self
+00012500: 2c20 6172 7261 795f 7661 6c75 653a 2063  , array_value: c
+00012510: 6f72 652e 4172 7261 7956 616c 7565 293a  ore.ArrayValue):
+00012520: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012530: 2020 2020 2043 616e 2074 6865 2062 6c6f       Can the blo
+00012540: 636b 2062 6520 6576 616c 7561 7465 6420  ck be evaluated 
+00012550: 7665 7279 2063 6865 6170 6c79 3f0a 2020  very cheaply?.  
+00012560: 2020 2020 2020 4966 2054 7275 652c 2074        If True, t
+00012570: 6865 2061 7272 6179 5f76 616c 7565 2070  he array_value p
+00012580: 726f 6261 626c 7920 6973 206e 6f74 2077  robably is not w
+00012590: 6f72 7468 2063 6163 6869 6e67 2e0a 2020  orth caching..  
+000125a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000125b0: 2020 2320 4f6e 6365 2072 6577 7269 7469    # Once rewriti
+000125c0: 6e67 2069 7320 6176 6169 6c61 626c 652c  ng is available,
+000125d0: 2077 696c 6c20 7761 6e74 2074 6f20 7265   will want to re
+000125e0: 7772 6974 6520 6265 666f 7265 0a20 2020  write before.   
+000125f0: 2020 2020 2023 2065 7661 6c75 6174 696e       # evaluatin
+00012600: 6720 6578 6563 7574 696f 6e20 636f 7374  g execution cost
+00012610: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00012620: 2074 7261 7665 7273 616c 732e 6973 5f74   traversals.is_t
+00012630: 7269 7669 616c 6c79 5f65 7865 6375 7461  rivially_executa
+00012640: 626c 6528 6172 7261 795f 7661 6c75 652e  ble(array_value.
+00012650: 6e6f 6465 290a 0a20 2020 2064 6566 205f  node)..    def _
+00012660: 6578 6563 7574 6528 0a20 2020 2020 2020  execute(.       
+00012670: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
+00012680: 7272 6179 5f76 616c 7565 3a20 636f 7265  rray_value: core
+00012690: 2e41 7272 6179 5661 6c75 652c 0a20 2020  .ArrayValue,.   
+000126a0: 2020 2020 206a 6f62 5f63 6f6e 6669 673a       job_config:
+000126b0: 204f 7074 696f 6e61 6c5b 6269 6771 7565   Optional[bigque
+000126c0: 7279 2e6a 6f62 2e51 7565 7279 4a6f 6243  ry.job.QueryJobC
+000126d0: 6f6e 6669 675d 203d 204e 6f6e 652c 0a20  onfig] = None,. 
+000126e0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+000126f0: 2020 736f 7274 6564 3a20 626f 6f6c 203d    sorted: bool =
+00012700: 2054 7275 652c 0a20 2020 2020 2020 2064   True,.        d
+00012710: 7279 5f72 756e 3d46 616c 7365 2c0a 2020  ry_run=False,.  
+00012720: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
+00012730: 7272 6964 6573 3a20 4d61 7070 696e 675b  rrides: Mapping[
+00012740: 7374 722c 2073 7472 5d20 3d20 7b7d 2c0a  str, str] = {},.
+00012750: 2020 2020 2920 2d3e 2074 7570 6c65 5b62      ) -> tuple[b
+00012760: 6967 7175 6572 792e 7461 626c 652e 526f  igquery.table.Ro
+00012770: 7749 7465 7261 746f 722c 2062 6967 7175  wIterator, bigqu
+00012780: 6572 792e 5175 6572 794a 6f62 5d3a 0a20  ery.QueryJob]:. 
+00012790: 2020 2020 2020 2073 716c 203d 2073 656c         sql = sel
+000127a0: 662e 5f74 6f5f 7371 6c28 0a20 2020 2020  f._to_sql(.     
+000127b0: 2020 2020 2020 2061 7272 6179 5f76 616c         array_val
+000127c0: 7565 2c20 736f 7274 6564 3d73 6f72 7465  ue, sorted=sorte
+000127d0: 642c 2063 6f6c 5f69 645f 6f76 6572 7269  d, col_id_overri
+000127e0: 6465 733d 636f 6c5f 6964 5f6f 7665 7272  des=col_id_overr
+000127f0: 6964 6573 0a20 2020 2020 2020 2029 2020  ides.        )  
+00012800: 2320 7479 7065 3a69 676e 6f72 650a 2020  # type:ignore.  
+00012810: 2020 2020 2020 6966 206a 6f62 5f63 6f6e        if job_con
+00012820: 6669 6720 6973 204e 6f6e 653a 0a20 2020  fig is None:.   
+00012830: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00012840: 6669 6720 3d20 6269 6771 7565 7279 2e51  fig = bigquery.Q
+00012850: 7565 7279 4a6f 6243 6f6e 6669 6728 6472  ueryJobConfig(dr
+00012860: 795f 7275 6e3d 6472 795f 7275 6e29 0a20  y_run=dry_run). 
+00012870: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00012880: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+00012890: 6669 672e 6472 795f 7275 6e20 3d20 6472  fig.dry_run = dr
+000128a0: 795f 7275 6e0a 2020 2020 2020 2020 7265  y_run.        re
+000128b0: 7475 726e 2073 656c 662e 5f73 7461 7274  turn self._start
+000128c0: 5f71 7565 7279 280a 2020 2020 2020 2020  _query(.        
+000128d0: 2020 2020 7371 6c3d 7371 6c2c 0a20 2020      sql=sql,.   
+000128e0: 2020 2020 2020 2020 206a 6f62 5f63 6f6e           job_con
+000128f0: 6669 673d 6a6f 625f 636f 6e66 6967 2c0a  fig=job_config,.
+00012900: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00012910: 6566 205f 7065 656b 280a 2020 2020 2020  ef _peek(.      
+00012920: 2020 7365 6c66 2c20 6172 7261 795f 7661    self, array_va
+00012930: 6c75 653a 2063 6f72 652e 4172 7261 7956  lue: core.ArrayV
+00012940: 616c 7565 2c20 6e5f 726f 7773 3a20 696e  alue, n_rows: in
+00012950: 740a 2020 2020 2920 2d3e 2074 7570 6c65  t.    ) -> tuple
+00012960: 5b62 6967 7175 6572 792e 7461 626c 652e  [bigquery.table.
+00012970: 526f 7749 7465 7261 746f 722c 2062 6967  RowIterator, big
+00012980: 7175 6572 792e 5175 6572 794a 6f62 5d3a  query.QueryJob]:
+00012990: 0a20 2020 2020 2020 2022 2222 4120 2770  .        """A 'p
+000129a0: 6565 6b27 2065 6666 6963 6965 6e74 6c79  eek' efficiently
+000129b0: 2061 6363 6573 7365 7320 6120 736d 616c   accesses a smal
+000129c0: 6c20 6e75 6d62 6572 206f 6620 726f 7773  l number of rows
+000129d0: 2069 6e20 7468 6520 6461 7461 6672 616d   in the datafram
+000129e0: 652e 2222 220a 2020 2020 2020 2020 6966  e.""".        if
+000129f0: 206e 6f74 2074 7265 655f 7072 6f70 6572   not tree_proper
+00012a00: 7469 6573 2e70 6565 6b61 626c 6528 6172  ties.peekable(ar
+00012a10: 7261 795f 7661 6c75 652e 6e6f 6465 293a  ray_value.node):
+00012a20: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
+00012a30: 6e69 6e67 732e 7761 726e 2822 5065 656b  nings.warn("Peek
+00012a40: 696e 6720 7468 6973 2076 616c 7565 2063  ing this value c
+00012a50: 616e 6e6f 7420 6265 2064 6f6e 6520 6566  annot be done ef
+00012a60: 6669 6369 656e 746c 792e 2229 0a20 2020  ficiently.").   
+00012a70: 2020 2020 2073 716c 203d 2073 656c 662e       sql = self.
+00012a80: 5f63 6f6d 7069 6c65 5f75 6e6f 7264 6572  _compile_unorder
+00012a90: 6564 2861 7272 6179 5f76 616c 7565 292e  ed(array_value).
+00012aa0: 7065 656b 5f73 716c 286e 5f72 6f77 7329  peek_sql(n_rows)
+00012ab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012ac0: 7365 6c66 2e5f 7374 6172 745f 7175 6572  self._start_quer
+00012ad0: 7928 0a20 2020 2020 2020 2020 2020 2073  y(.            s
+00012ae0: 716c 3d73 716c 2c0a 2020 2020 2020 2020  ql=sql,.        
+00012af0: 290a 0a20 2020 2064 6566 205f 746f 5f73  )..    def _to_s
+00012b00: 716c 280a 2020 2020 2020 2020 7365 6c66  ql(.        self
+00012b10: 2c0a 2020 2020 2020 2020 6172 7261 795f  ,.        array_
+00012b20: 7661 6c75 653a 2063 6f72 652e 4172 7261  value: core.Arra
+00012b30: 7956 616c 7565 2c0a 2020 2020 2020 2020  yValue,.        
+00012b40: 6f66 6673 6574 5f63 6f6c 756d 6e3a 2074  offset_column: t
+00012b50: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00012b60: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00012b70: 2020 2020 636f 6c5f 6964 5f6f 7665 7272      col_id_overr
+00012b80: 6964 6573 3a20 7479 7069 6e67 2e4d 6170  ides: typing.Map
+00012b90: 7069 6e67 5b73 7472 2c20 7374 725d 203d  ping[str, str] =
+00012ba0: 207b 7d2c 0a20 2020 2020 2020 2073 6f72   {},.        sor
+00012bb0: 7465 643a 2062 6f6f 6c20 3d20 4661 6c73  ted: bool = Fals
+00012bc0: 652c 0a20 2020 2029 202d 3e20 7374 723a  e,.    ) -> str:
+00012bd0: 0a20 2020 2020 2020 2069 6620 6f66 6673  .        if offs
+00012be0: 6574 5f63 6f6c 756d 6e3a 0a20 2020 2020  et_column:.     
+00012bf0: 2020 2020 2020 2061 7272 6179 5f76 616c         array_val
+00012c00: 7565 203d 2061 7272 6179 5f76 616c 7565  ue = array_value
+00012c10: 2e70 726f 6d6f 7465 5f6f 6666 7365 7473  .promote_offsets
+00012c20: 286f 6666 7365 745f 636f 6c75 6d6e 290a  (offset_column).
+00012c30: 2020 2020 2020 2020 6966 2073 6f72 7465          if sorte
+00012c40: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+00012c50: 6574 7572 6e20 7365 6c66 2e5f 636f 6d70  eturn self._comp
+00012c60: 696c 655f 6f72 6465 7265 6428 6172 7261  ile_ordered(arra
+00012c70: 795f 7661 6c75 6529 2e74 6f5f 7371 6c28  y_value).to_sql(
+00012c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c90: 2063 6f6c 5f69 645f 6f76 6572 7269 6465   col_id_override
+00012ca0: 733d 636f 6c5f 6964 5f6f 7665 7272 6964  s=col_id_overrid
+00012cb0: 6573 2c20 736f 7274 6564 3d54 7275 650a  es, sorted=True.
+00012cc0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012cd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00012ce0: 662e 5f63 6f6d 7069 6c65 5f75 6e6f 7264  f._compile_unord
+00012cf0: 6572 6564 2861 7272 6179 5f76 616c 7565  ered(array_value
+00012d00: 292e 746f 5f73 716c 280a 2020 2020 2020  ).to_sql(.      
+00012d10: 2020 2020 2020 636f 6c5f 6964 5f6f 7665        col_id_ove
+00012d20: 7272 6964 6573 3d63 6f6c 5f69 645f 6f76  rrides=col_id_ov
+00012d30: 6572 7269 6465 730a 2020 2020 2020 2020  errides.        
+00012d40: 290a 0a20 2020 2064 6566 205f 636f 6d70  )..    def _comp
+00012d50: 696c 655f 6f72 6465 7265 6428 0a20 2020  ile_ordered(.   
+00012d60: 2020 2020 2073 656c 662c 2061 7272 6179       self, array
+00012d70: 5f76 616c 7565 3a20 636f 7265 2e41 7272  _value: core.Arr
+00012d80: 6179 5661 6c75 650a 2020 2020 2920 2d3e  ayValue.    ) ->
+00012d90: 2062 6967 6672 616d 6573 2e63 6f72 652e   bigframes.core.
+00012da0: 636f 6d70 696c 652e 4f72 6465 7265 6449  compile.OrderedI
+00012db0: 523a 0a20 2020 2020 2020 2072 6574 7572  R:.        retur
+00012dc0: 6e20 6269 6766 7261 6d65 732e 636f 7265  n bigframes.core
+00012dd0: 2e63 6f6d 7069 6c65 2e63 6f6d 7069 6c65  .compile.compile
+00012de0: 5f6f 7264 6572 6564 5f69 7228 6172 7261  _ordered_ir(arra
+00012df0: 795f 7661 6c75 652e 6e6f 6465 290a 0a20  y_value.node).. 
+00012e00: 2020 2064 6566 205f 636f 6d70 696c 655f     def _compile_
+00012e10: 756e 6f72 6465 7265 6428 0a20 2020 2020  unordered(.     
+00012e20: 2020 2073 656c 662c 2061 7272 6179 5f76     self, array_v
+00012e30: 616c 7565 3a20 636f 7265 2e41 7272 6179  alue: core.Array
+00012e40: 5661 6c75 650a 2020 2020 2920 2d3e 2062  Value.    ) -> b
+00012e50: 6967 6672 616d 6573 2e63 6f72 652e 636f  igframes.core.co
+00012e60: 6d70 696c 652e 556e 6f72 6465 7265 6449  mpile.UnorderedI
+00012e70: 523a 0a20 2020 2020 2020 2072 6574 7572  R:.        retur
+00012e80: 6e20 6269 6766 7261 6d65 732e 636f 7265  n bigframes.core
+00012e90: 2e63 6f6d 7069 6c65 2e63 6f6d 7069 6c65  .compile.compile
+00012ea0: 5f75 6e6f 7264 6572 6564 5f69 7228 6172  _unordered_ir(ar
+00012eb0: 7261 795f 7661 6c75 652e 6e6f 6465 290a  ray_value.node).
+00012ec0: 0a20 2020 2064 6566 205f 6765 745f 7461  .    def _get_ta
+00012ed0: 626c 655f 7369 7a65 2873 656c 662c 2064  ble_size(self, d
+00012ee0: 6573 7469 6e61 7469 6f6e 5f74 6162 6c65  estination_table
+00012ef0: 293a 0a20 2020 2020 2020 2074 6162 6c65  ):.        table
+00012f00: 203d 2073 656c 662e 6271 636c 6965 6e74   = self.bqclient
+00012f10: 2e67 6574 5f74 6162 6c65 2864 6573 7469  .get_table(desti
+00012f20: 6e61 7469 6f6e 5f74 6162 6c65 290a 2020  nation_table).  
+00012f30: 2020 2020 2020 7265 7475 726e 2074 6162        return tab
+00012f40: 6c65 2e6e 756d 5f62 7974 6573 0a0a 2020  le.num_bytes..  
+00012f50: 2020 6465 6620 5f72 6f77 735f 746f 5f64    def _rows_to_d
+00012f60: 6174 6166 7261 6d65 280a 2020 2020 2020  ataframe(.      
+00012f70: 2020 7365 6c66 2c20 726f 775f 6974 6572    self, row_iter
+00012f80: 6174 6f72 3a20 6269 6771 7565 7279 2e74  ator: bigquery.t
+00012f90: 6162 6c65 2e52 6f77 4974 6572 6174 6f72  able.RowIterator
+00012fa0: 2c20 6474 7970 6573 3a20 4469 6374 0a20  , dtypes: Dict. 
+00012fb0: 2020 2029 202d 3e20 7061 6e64 6173 2e44     ) -> pandas.D
+00012fc0: 6174 6146 7261 6d65 3a0a 2020 2020 2020  ataFrame:.      
+00012fd0: 2020 2320 4361 6e20 6967 6e6f 7265 2069    # Can ignore i
+00012fe0: 6e66 6572 7265 6420 6461 7461 7479 7065  nferred datatype
+00012ff0: 2075 6e74 696c 2064 7479 7065 2065 6d75   until dtype emu
+00013000: 6c61 7469 6f6e 2062 7265 616b 7320 313a  lation breaks 1:
+00013010: 3120 6d61 7070 696e 6720 6265 7477 6565  1 mapping betwee
+00013020: 6e20 4251 2074 7970 6573 2061 6e64 2062  n BQ types and b
+00013030: 6967 6672 616d 6573 2074 7970 6573 0a20  igframes types. 
+00013040: 2020 2020 2020 2064 7479 7065 735f 6672         dtypes_fr
+00013050: 6f6d 5f62 7120 3d20 6269 6766 7261 6d65  om_bq = bigframe
+00013060: 732e 6474 7970 6573 2e62 665f 7479 7065  s.dtypes.bf_type
+00013070: 5f66 726f 6d5f 7479 7065 5f6b 696e 6428  _from_type_kind(
+00013080: 726f 775f 6974 6572 6174 6f72 2e73 6368  row_iterator.sch
+00013090: 656d 6129 0a20 2020 2020 2020 2061 7272  ema).        arr
+000130a0: 6f77 5f74 6162 6c65 203d 2072 6f77 5f69  ow_table = row_i
+000130b0: 7465 7261 746f 722e 746f 5f61 7272 6f77  terator.to_arrow
+000130c0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000130d0: 6e20 6269 6766 7261 6d65 732e 7365 7373  n bigframes.sess
+000130e0: 696f 6e2e 5f69 6f2e 7061 6e64 6173 2e61  ion._io.pandas.a
+000130f0: 7272 6f77 5f74 6f5f 7061 6e64 6173 2861  rrow_to_pandas(a
+00013100: 7272 6f77 5f74 6162 6c65 2c20 6474 7970  rrow_table, dtyp
+00013110: 6573 5f66 726f 6d5f 6271 290a 0a20 2020  es_from_bq)..   
+00013120: 2064 6566 205f 7374 6172 745f 6765 6e65   def _start_gene
+00013130: 7269 635f 6a6f 6228 7365 6c66 2c20 6a6f  ric_job(self, jo
+00013140: 623a 2066 6f72 6d61 7474 696e 675f 6865  b: formatting_he
+00013150: 6c70 6572 732e 4765 6e65 7269 634a 6f62  lpers.GenericJob
+00013160: 293a 0a20 2020 2020 2020 2069 6620 6269  ):.        if bi
+00013170: 6766 7261 6d65 732e 6f70 7469 6f6e 732e  gframes.options.
+00013180: 6469 7370 6c61 792e 7072 6f67 7265 7373  display.progress
+00013190: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+000131a0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+000131b0: 726d 6174 7469 6e67 5f68 656c 7065 7273  rmatting_helpers
+000131c0: 2e77 6169 745f 666f 725f 6a6f 6228 0a20  .wait_for_job(. 
+000131d0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+000131e0: 6f62 2c20 6269 6766 7261 6d65 732e 6f70  ob, bigframes.op
+000131f0: 7469 6f6e 732e 6469 7370 6c61 792e 7072  tions.display.pr
+00013200: 6f67 7265 7373 5f62 6172 0a20 2020 2020  ogress_bar.     
+00013210: 2020 2020 2020 2029 2020 2320 5761 6974         )  # Wait
+00013220: 2066 6f72 2074 6865 206a 6f62 2074 6f20   for the job to 
+00013230: 636f 6d70 6c65 7465 0a20 2020 2020 2020  complete.       
+00013240: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013250: 2020 206a 6f62 2e72 6573 756c 7428 290a     job.result().
+00013260: 0a20 2020 2064 6566 205f 7261 6e64 6f6d  .    def _random
+00013270: 5f74 6162 6c65 2873 656c 662c 2073 6b69  _table(self, ski
+00013280: 705f 636c 6561 6e75 703a 2062 6f6f 6c20  p_cleanup: bool 
+00013290: 3d20 4661 6c73 6529 202d 3e20 6269 6771  = False) -> bigq
+000132a0: 7565 7279 2e54 6162 6c65 5265 6665 7265  uery.TableRefere
+000132b0: 6e63 653a 0a20 2020 2020 2020 2022 2222  nce:.        """
+000132c0: 4765 6e65 7261 7465 2061 2072 616e 646f  Generate a rando
+000132d0: 6d20 7461 626c 6520 4944 2077 6974 6820  m table ID with 
+000132e0: 4269 6751 7565 7279 2044 6174 6146 7261  BigQuery DataFra
+000132f0: 6d65 7320 7072 6566 6978 2e0a 0a20 2020  mes prefix...   
+00013300: 2020 2020 2054 6865 2067 656e 6572 6174       The generat
+00013310: 6564 2049 4420 7769 6c6c 2062 6520 7374  ed ID will be st
+00013320: 6f72 6564 2061 6e64 2063 6865 636b 6564  ored and checked
+00013330: 2066 6f72 2064 656c 6574 696f 6e20 7768   for deletion wh
+00013340: 656e 2074 6865 0a20 2020 2020 2020 2073  en the.        s
+00013350: 6573 7369 6f6e 2069 7320 636c 6f73 6564  ession is closed
+00013360: 2c20 756e 6c65 7373 2073 6b69 705f 636c  , unless skip_cl
+00013370: 6561 6e75 7020 6973 2054 7275 652e 0a0a  eanup is True...
+00013380: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00013390: 2020 2020 2020 2020 2020 736b 6970 5f63            skip_c
+000133a0: 6c65 616e 7570 2028 626f 6f6c 2c20 6465  leanup (bool, de
+000133b0: 6661 756c 7420 4661 6c73 6529 3a0a 2020  fault False):.  
+000133c0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+000133d0: 2054 7275 652c 2064 6f20 6e6f 7420 6164   True, do not ad
+000133e0: 6420 7468 6520 6765 6e65 7261 7465 6420  d the generated 
+000133f0: 4944 2074 6f20 7468 6520 6c69 7374 206f  ID to the list o
+00013400: 6620 7461 626c 6573 0a20 2020 2020 2020  f tables.       
+00013410: 2020 2020 2020 2020 2074 6f20 636c 6561           to clea
+00013420: 6e20 7570 2077 6865 6e20 7468 6520 7365  n up when the se
+00013430: 7373 696f 6e20 6973 2063 6c6f 7365 642e  ssion is closed.
+00013440: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00013450: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+00013460: 6f6f 676c 652e 636c 6f75 642e 6269 6771  oogle.cloud.bigq
+00013470: 7565 7279 2e54 6162 6c65 5265 6665 7265  uery.TableRefere
+00013480: 6e63 653a 0a20 2020 2020 2020 2020 2020  nce:.           
+00013490: 2020 2020 2046 756c 6c79 2071 7561 6c69       Fully quali
+000134a0: 6669 6564 2074 6162 6c65 2049 4420 6f66  fied table ID of
+000134b0: 2061 2074 6162 6c65 2074 6861 7420 646f   a table that do
+000134c0: 6573 6e27 7420 6578 6973 742e 0a20 2020  esn't exist..   
+000134d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000134e0: 2064 6174 6173 6574 203d 2073 656c 662e   dataset = self.
+000134f0: 5f61 6e6f 6e79 6d6f 7573 5f64 6174 6173  _anonymous_datas
+00013500: 6574 0a20 2020 2020 2020 2073 6573 7369  et.        sessi
+00013510: 6f6e 5f69 6420 3d20 7365 6c66 2e73 6573  on_id = self.ses
+00013520: 7369 6f6e 5f69 640a 2020 2020 2020 2020  sion_id.        
+00013530: 6e6f 7720 3d20 6461 7465 7469 6d65 2e64  now = datetime.d
+00013540: 6174 6574 696d 652e 6e6f 7728 6461 7465  atetime.now(date
+00013550: 7469 6d65 2e74 696d 657a 6f6e 652e 7574  time.timezone.ut
+00013560: 6329 0a20 2020 2020 2020 2072 616e 646f  c).        rando
+00013570: 6d5f 6964 203d 2075 7569 642e 7575 6964  m_id = uuid.uuid
+00013580: 3428 292e 6865 780a 2020 2020 2020 2020  4().hex.        
+00013590: 7461 626c 655f 6964 203d 205f 5445 4d50  table_id = _TEMP
+000135a0: 5f54 4142 4c45 5f49 445f 464f 524d 4154  _TABLE_ID_FORMAT
+000135b0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+000135c0: 2020 2020 2064 6174 653d 6e6f 772e 7374       date=now.st
+000135d0: 7266 7469 6d65 2822 2559 256d 2564 2229  rftime("%Y%m%d")
+000135e0: 2c20 7365 7373 696f 6e5f 6964 3d73 6573  , session_id=ses
+000135f0: 7369 6f6e 5f69 642c 2072 616e 646f 6d5f  sion_id, random_
+00013600: 6964 3d72 616e 646f 6d5f 6964 0a20 2020  id=random_id.   
+00013610: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00013620: 6620 6e6f 7420 736b 6970 5f63 6c65 616e  f not skip_clean
+00013630: 7570 3a0a 2020 2020 2020 2020 2020 2020  up:.            
+00013640: 7365 6c66 2e5f 7461 626c 655f 6964 732e  self._table_ids.
+00013650: 6170 7065 6e64 2874 6162 6c65 5f69 6429  append(table_id)
+00013660: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013670: 6461 7461 7365 742e 7461 626c 6528 7461  dataset.table(ta
+00013680: 626c 655f 6964 290a 0a0a 6465 6620 636f  ble_id)...def co
+00013690: 6e6e 6563 7428 636f 6e74 6578 743a 204f  nnect(context: O
+000136a0: 7074 696f 6e61 6c5b 6269 6771 7565 7279  ptional[bigquery
+000136b0: 5f6f 7074 696f 6e73 2e42 6967 5175 6572  _options.BigQuer
+000136c0: 794f 7074 696f 6e73 5d20 3d20 4e6f 6e65  yOptions] = None
+000136d0: 2920 2d3e 2053 6573 7369 6f6e 3a0a 2020  ) -> Session:.  
+000136e0: 2020 7265 7475 726e 2053 6573 7369 6f6e    return Session
+000136f0: 2863 6f6e 7465 7874 290a 0a0a 6465 6620  (context)...def 
+00013700: 5f63 616e 5f63 6c75 7374 6572 5f62 7128  _can_cluster_bq(
+00013710: 6669 656c 643a 2062 6967 7175 6572 792e  field: bigquery.
+00013720: 5363 6865 6d61 4669 656c 6429 3a0a 2020  SchemaField):.  
+00013730: 2020 2320 6874 7470 733a 2f2f 636c 6f75    # https://clou
+00013740: 642e 676f 6f67 6c65 2e63 6f6d 2f62 6967  d.google.com/big
+00013750: 7175 6572 792f 646f 6373 2f63 6c75 7374  query/docs/clust
+00013760: 6572 6564 2d74 6162 6c65 730a 2020 2020  ered-tables.    
+00013770: 2320 4e6f 7461 626c 792c 2066 6c6f 6174  # Notably, float
+00013780: 2069 7320 6578 636c 7564 6564 0a20 2020   is excluded.   
+00013790: 2074 7970 655f 203d 2066 6965 6c64 2e66   type_ = field.f
+000137a0: 6965 6c64 5f74 7970 650a 2020 2020 7265  ield_type.    re
+000137b0: 7475 726e 2074 7970 655f 2069 6e20 280a  turn type_ in (.
+000137c0: 2020 2020 2020 2020 2249 4e54 4547 4552          "INTEGER
+000137d0: 222c 0a20 2020 2020 2020 2022 494e 5436  ",.        "INT6
+000137e0: 3422 2c0a 2020 2020 2020 2020 2253 5452  4",.        "STR
+000137f0: 494e 4722 2c0a 2020 2020 2020 2020 224e  ING",.        "N
+00013800: 554d 4552 4943 222c 0a20 2020 2020 2020  UMERIC",.       
+00013810: 2022 4445 4349 4d41 4c22 2c0a 2020 2020   "DECIMAL",.    
+00013820: 2020 2020 2242 4947 4e55 4d45 5249 4322      "BIGNUMERIC"
+00013830: 2c0a 2020 2020 2020 2020 2242 4947 4445  ,.        "BIGDE
+00013840: 4349 4d41 4c22 2c0a 2020 2020 2020 2020  CIMAL",.        
+00013850: 2244 4154 4522 2c0a 2020 2020 2020 2020  "DATE",.        
+00013860: 2244 4154 4554 494d 4522 2c0a 2020 2020  "DATETIME",.    
+00013870: 2020 2020 2254 494d 4553 5441 4d50 222c      "TIMESTAMP",
+00013880: 0a20 2020 2020 2020 2022 424f 4f4c 222c  .        "BOOL",
+00013890: 0a20 2020 2020 2020 2022 424f 4f4c 4541  .        "BOOLEA
+000138a0: 4e22 2c0a 2020 2020 290a 0a0a 6465 6620  N",.    )...def 
+000138b0: 5f74 7261 6e73 666f 726d 5f72 6561 645f  _transform_read_
+000138c0: 6762 715f 636f 6e66 6967 7572 6174 696f  gbq_configuratio
+000138d0: 6e28 636f 6e66 6967 7572 6174 696f 6e3a  n(configuration:
+000138e0: 204f 7074 696f 6e61 6c5b 6469 6374 5d29   Optional[dict])
+000138f0: 202d 3e20 6469 6374 3a0a 2020 2020 2222   -> dict:.    ""
+00013900: 220a 2020 2020 466f 7220 6261 636b 7761  ".    For backwa
+00013910: 7264 732d 636f 6d70 6174 6962 696c 6974  rds-compatibilit
+00013920: 792c 2063 6f6e 7665 7274 2061 6e79 2070  y, convert any p
+00013930: 7265 7669 6f75 736c 7920 636c 6965 6e74  reviously client
+00013940: 2d73 6964 6520 6f6e 6c79 0a20 2020 2070  -side only.    p
+00013950: 6172 616d 6574 6572 7320 7375 6368 2061  arameters such a
+00013960: 7320 7469 6d65 6f75 744d 7320 746f 2074  s timeoutMs to t
+00013970: 6865 2070 726f 7065 7274 7920 6e61 6d65  he property name
+00013980: 2065 7870 6563 7465 6420 6279 2074 6865   expected by the
+00013990: 2052 4553 5420 4150 492e 0a0a 2020 2020   REST API...    
+000139a0: 4d61 6b65 7320 6120 636f 7079 206f 6620  Makes a copy of 
+000139b0: 636f 6e66 6967 7572 6174 696f 6e20 6966  configuration if
+000139c0: 2063 6861 6e67 6573 2061 7265 206e 6565   changes are nee
+000139d0: 6465 642e 0a20 2020 2022 2222 0a0a 2020  ded..    """..  
+000139e0: 2020 6966 2063 6f6e 6669 6775 7261 7469    if configurati
+000139f0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00013a00: 2020 2020 7265 7475 726e 207b 7d0a 0a20      return {}.. 
+00013a10: 2020 2074 696d 656f 7574 5f6d 7320 3d20     timeout_ms = 
+00013a20: 636f 6e66 6967 7572 6174 696f 6e2e 6765  configuration.ge
+00013a30: 7428 2271 7565 7279 222c 207b 7d29 2e67  t("query", {}).g
+00013a40: 6574 2822 7469 6d65 6f75 744d 7322 290a  et("timeoutMs").
+00013a50: 2020 2020 6966 2074 696d 656f 7574 5f6d      if timeout_m
+00013a60: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00013a70: 2020 2020 2020 2023 2054 7261 6e73 666f         # Transfo
+00013a80: 726d 2074 696d 656f 7574 4d73 2074 6f20  rm timeoutMs to 
+00013a90: 616e 2061 6374 7561 6c20 7365 7276 6572  an actual server
+00013aa0: 2d73 6964 6520 636f 6e66 6967 7572 6174  -side configurat
+00013ab0: 696f 6e2e 0a20 2020 2020 2020 2023 2068  ion..        # h
+00013ac0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00013ad0: 6d2f 676f 6f67 6c65 6170 6973 2f70 7974  m/googleapis/pyt
+00013ae0: 686f 6e2d 6269 6771 7565 7279 2d70 616e  hon-bigquery-pan
+00013af0: 6461 732f 6973 7375 6573 2f34 3739 0a20  das/issues/479. 
+00013b00: 2020 2020 2020 2063 6f6e 6669 6775 7261         configura
+00013b10: 7469 6f6e 203d 2063 6f70 792e 6465 6570  tion = copy.deep
+00013b20: 636f 7079 2863 6f6e 6669 6775 7261 7469  copy(configurati
+00013b30: 6f6e 290a 2020 2020 2020 2020 6465 6c20  on).        del 
+00013b40: 636f 6e66 6967 7572 6174 696f 6e5b 2271  configuration["q
+00013b50: 7565 7279 225d 5b22 7469 6d65 6f75 744d  uery"]["timeoutM
+00013b60: 7322 5d0a 2020 2020 2020 2020 636f 6e66  s"].        conf
+00013b70: 6967 7572 6174 696f 6e5b 226a 6f62 5469  iguration["jobTi
+00013b80: 6d65 6f75 744d 7322 5d20 3d20 7469 6d65  meoutMs"] = time
+00013b90: 6f75 745f 6d73 0a0a 2020 2020 7265 7475  out_ms..    retu
+00013ba0: 726e 2063 6f6e 6669 6775 7261 7469 6f6e  rn configuration
+00013bb0: 0a                                       .
```

### Comparing `bigframes-1.4.0/bigframes/session/_io/__init__.py` & `bigframes-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/session/_io/bigquery.py` & `bigframes-1.5.0/bigframes/session/_io/bigquery/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Private module: Helpers for I/O operations."""
+"""Private module: Helpers for BigQuery I/O operations."""
 
 from __future__ import annotations
 
 import datetime
 import itertools
 import os
 import textwrap
 import types
 from typing import Dict, Iterable, Optional, Sequence, Tuple, Union
-import uuid
-import warnings
 
 import google.api_core.exceptions
 import google.cloud.bigquery as bigquery
 
 import bigframes
 from bigframes.core import log_adapter
 import bigframes.formatting_helpers as formatting_helpers
 
 IO_ORDERING_ID = "bqdf_row_nums"
 MAX_LABELS_COUNT = 64
-TEMP_TABLE_PREFIX = "bqdf{date}_{random_id}"
+_LIST_TABLES_LIMIT = 10000  # calls to bqclient.list_tables
+# will be limited to this many tables
 
 LOGGING_NAME_ENV_VAR = "BIGFRAMES_PERFORMANCE_LOG_NAME"
 
 
 def create_job_configs_labels(
     job_configs_labels: Optional[Dict[str, str]],
     api_methods: Sequence[str],
@@ -95,118 +94,33 @@
         SELECT * EXCEPT ({IO_ORDERING_ID})
         FROM `{table_id}`
         ORDER BY {IO_ORDERING_ID}
         """
     )
 
 
-def random_table(dataset: bigquery.DatasetReference) -> bigquery.TableReference:
-    """Generate a random table ID with BigQuery DataFrames prefix.
-    Args:
-        dataset (google.cloud.bigquery.DatasetReference):
-            The dataset to make the table reference in. Usually the anonymous
-            dataset for the session.
-    Returns:
-        google.cloud.bigquery.TableReference:
-            Fully qualified table ID of a table that doesn't exist.
-    """
-    now = datetime.datetime.now(datetime.timezone.utc)
-    random_id = uuid.uuid4().hex
-    table_id = TEMP_TABLE_PREFIX.format(
-        date=now.strftime("%Y%m%d"), random_id=random_id
-    )
-    return dataset.table(table_id)
-
-
 def table_ref_to_sql(table: bigquery.TableReference) -> str:
     """Format a table reference as escaped SQL."""
     return f"`{table.project}`.`{table.dataset_id}`.`{table.table_id}`"
 
 
-def get_snapshot_datetime_and_table_metadata(
-    bqclient: bigquery.Client,
-    table_ref: bigquery.TableReference,
-    *,
-    api_name: str,
-    cache: Dict[bigquery.TableReference, Tuple[datetime.datetime, bigquery.Table]],
-    use_cache: bool = True,
-) -> Tuple[datetime.datetime, bigquery.Table]:
-    cached_table = cache.get(table_ref)
-    if use_cache and cached_table is not None:
-        snapshot_timestamp, _ = cached_table
-
-        # Cache hit could be unexpected. See internal issue 329545805.
-        # Raise a warning with more information about how to avoid the
-        # problems with the cache.
-        warnings.warn(
-            f"Reading cached table from {snapshot_timestamp} to avoid "
-            "incompatibilies with previous reads of this table. To read "
-            "the latest version, set `use_cache=False` or close the "
-            "current session with Session.close() or "
-            "bigframes.pandas.close_session().",
-            # There are many layers before we get to (possibly) the user's code:
-            # pandas.read_gbq_table
-            # -> with_default_session
-            # -> Session.read_gbq_table
-            # -> _read_gbq_table
-            # -> _get_snapshot_sql_and_primary_key
-            # -> get_snapshot_datetime_and_table_metadata
-            stacklevel=7,
-        )
-        return cached_table
-
-    # TODO(swast): It's possible that the table metadata is changed between now
-    # and when we run the CURRENT_TIMESTAMP() query to see when we can time
-    # travel to. Find a way to fetch the table metadata and BQ's current time
-    # atomically.
-    table = bqclient.get_table(table_ref)
-
-    # TODO(b/336521938): Refactor to make sure we set the "bigframes-api"
-    # whereever we execute a query.
-    job_config = bigquery.QueryJobConfig()
-    job_config.labels["bigframes-api"] = api_name
-    snapshot_timestamp = list(
-        bqclient.query(
-            "SELECT CURRENT_TIMESTAMP() AS `current_timestamp`",
-            job_config=job_config,
-        ).result()
-    )[0][0]
-    cached_table = (snapshot_timestamp, table)
-    cache[table_ref] = cached_table
-    return cached_table
-
-
-def create_snapshot_sql(
-    table_ref: bigquery.TableReference, current_timestamp: datetime.datetime
-) -> str:
-    """Query a table via 'time travel' for consistent reads."""
-    # If we have an anonymous query results table, it can't be modified and
-    # there isn't any BigQuery time travel.
-    if table_ref.dataset_id.startswith("_"):
-        return f"SELECT * FROM `{table_ref.project}`.`{table_ref.dataset_id}`.`{table_ref.table_id}`"
-
-    return textwrap.dedent(
-        f"""
-        SELECT *
-        FROM `{table_ref.project}`.`{table_ref.dataset_id}`.`{table_ref.table_id}`
-        FOR SYSTEM_TIME AS OF TIMESTAMP({repr(current_timestamp.isoformat())})
-        """
-    )
-
-
 def create_temp_table(
-    bqclient: bigquery.Client,
-    dataset: bigquery.DatasetReference,
+    session: bigframes.session.Session,
     expiration: datetime.datetime,
     *,
     schema: Optional[Iterable[bigquery.SchemaField]] = None,
     cluster_columns: Optional[list[str]] = None,
 ) -> str:
-    """Create an empty table with an expiration in the desired dataset."""
-    table_ref = random_table(dataset)
+    """Create an empty table with an expiration in the desired session.
+
+    The table will be deleted when the session is closed or the expiration
+    is reached.
+    """
+    bqclient: bigquery.Client = session.bqclient
+    table_ref = session._random_table()
     destination = bigquery.Table(table_ref)
     destination.expires = expiration
     destination.schema = schema
     if cluster_columns:
         destination.clustering_fields = cluster_columns
     bqclient.create_table(destination)
     return f"{table_ref.project}.{table_ref.dataset_id}.{table_ref.table_id}"
@@ -325,7 +239,75 @@
         return  # filter out mocks
     if query_job.configuration.dry_run:
         # dry runs don't process their total_bytes_processed
         bytes_processed = 0
     bytes_file = os.path.join(current_directory, test_name + ".bytesprocessed")
     with open(bytes_file, "a") as f:
         f.write(str(bytes_processed) + "\n")
+
+
+def delete_tables_matching_session_id(
+    client: bigquery.Client, dataset: bigquery.DatasetReference, session_id: str
+) -> None:
+    """Searches within the dataset for tables conforming to the
+    expected session_id form, and instructs bigquery to delete them.
+
+    Args:
+        client (bigquery.Client):
+            The client to use to list tables
+        dataset (bigquery.DatasetReference):
+            The dataset to search in
+        session_id (str):
+            The session id to match on in the table name
+
+    Returns:
+        None
+    """
+
+    tables = client.list_tables(
+        dataset, max_results=_LIST_TABLES_LIMIT, page_size=_LIST_TABLES_LIMIT
+    )
+    for table in tables:
+        split_id = table.table_id.split("_")
+        if not split_id[0].startswith("bqdf") or len(split_id) < 2:
+            continue
+        found_session_id = split_id[1]
+        if found_session_id == session_id:
+            client.delete_table(table, not_found_ok=True)
+            print("Deleting temporary table '{}'.".format(table.table_id))
+
+
+def create_bq_dataset_reference(
+    bq_client: bigquery.Client, location=None, project=None
+) -> bigquery.DatasetReference:
+    """Create and identify dataset(s) for temporary BQ resources.
+
+    bq_client project and location will be used unless kwargs "project"
+    and/or "location" are given. If given, location and project
+    will be passed through to
+    https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.client.Client#google_cloud_bigquery_client_Client_query
+
+    Args:
+        bq_client (bigquery.Client):
+            The bigquery.Client to use for the http request to
+            create the dataset reference.
+        location (str, default None):
+            The location of the project to create the dataset in.
+        project (str, default None):
+            The project id of the project to create the dataset in.
+
+    Returns:
+        bigquery.DatasetReference: The constructed reference to the anonymous dataset.
+    """
+    query_job = bq_client.query("SELECT 1", location=location, project=project)
+    query_job.result()  # blocks until finished
+
+    # The anonymous dataset is used by BigQuery to write query results and
+    # session tables. BigQuery DataFrames also writes temp tables directly
+    # to the dataset, no BigQuery Session required. Note: there is a
+    # different anonymous dataset per location. See:
+    # https://cloud.google.com/bigquery/docs/cached-results#how_cached_results_are_stored
+    query_destination = query_job.destination
+    return bigquery.DatasetReference(
+        query_destination.project,
+        query_destination.dataset_id,
+    )
```

### Comparing `bigframes-1.4.0/bigframes/session/_io/pandas.py` & `bigframes-1.5.0/bigframes/session/_io/pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/session/clients.py` & `bigframes-1.5.0/bigframes/session/clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/bigframes/version.py` & `bigframes-1.5.0/bigframes/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
```

### Comparing `bigframes-1.4.0/bigframes.egg-info/PKG-INFO` & `bigframes-1.5.0/bigframes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigframes
-Version: 1.4.0
+Version: 1.5.0
 Summary: BigQuery DataFrames -- scalable analytics and machine learning with BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-dataframes
 Author: Google LLC
 Author-email: bigframes-feedback@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bigframes-1.4.0/bigframes.egg-info/SOURCES.txt` & `bigframes-1.5.0/bigframes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 bigframes/__init__.py
 bigframes/clients.py
 bigframes/constants.py
 bigframes/dataframe.py
 bigframes/dtypes.py
+bigframes/enums.py
 bigframes/exceptions.py
 bigframes/features.py
 bigframes/formatting_helpers.py
 bigframes/py.typed
 bigframes/series.py
 bigframes/typing.py
 bigframes/version.py
@@ -23,14 +24,15 @@
 bigframes.egg-info/requires.txt
 bigframes.egg-info/top_level.txt
 bigframes/_config/__init__.py
 bigframes/_config/bigquery_options.py
 bigframes/_config/compute_options.py
 bigframes/_config/display_options.py
 bigframes/_config/sampling_options.py
+bigframes/bigquery/__init__.py
 bigframes/core/__init__.py
 bigframes/core/block_transforms.py
 bigframes/core/blocks.py
 bigframes/core/convert.py
 bigframes/core/eval.py
 bigframes/core/expression.py
 bigframes/core/global_session.py
@@ -99,16 +101,17 @@
 bigframes/operations/_matplotlib/__init__.py
 bigframes/operations/_matplotlib/core.py
 bigframes/operations/_matplotlib/hist.py
 bigframes/pandas/__init__.py
 bigframes/session/__init__.py
 bigframes/session/clients.py
 bigframes/session/_io/__init__.py
-bigframes/session/_io/bigquery.py
 bigframes/session/_io/pandas.py
+bigframes/session/_io/bigquery/__init__.py
+bigframes/session/_io/bigquery/read_gbq_table.py
 tests/__init__.py
 tests/data/hockey_players.json
 tests/data/hockey_players.jsonl
 tests/data/matrix_2by3.json
 tests/data/matrix_2by3.jsonl
 tests/data/matrix_3by4.json
 tests/data/matrix_3by4.jsonl
@@ -151,14 +154,16 @@
 tests/system/small/test_pandas_options.py
 tests/system/small/test_progress_bar.py
 tests/system/small/test_remote_function.py
 tests/system/small/test_scalar.py
 tests/system/small/test_series.py
 tests/system/small/test_session.py
 tests/system/small/test_window.py
+tests/system/small/bigquery/__init__.py
+tests/system/small/bigquery/test_array.py
 tests/system/small/ml/__init__.py
 tests/system/small/ml/conftest.py
 tests/system/small/ml/test_cluster.py
 tests/system/small/ml/test_core.py
 tests/system/small/ml/test_decomposition.py
 tests/system/small/ml/test_ensemble.py
 tests/system/small/ml/test_forecasting.py
@@ -201,14 +206,15 @@
 tests/unit/ml/test_golden_sql.py
 tests/unit/ml/test_pipeline.py
 tests/unit/ml/test_sql.py
 tests/unit/session/__init__.py
 tests/unit/session/test_clients.py
 tests/unit/session/test_io_bigquery.py
 tests/unit/session/test_io_pandas.py
+tests/unit/session/test_read_gbq_table.py
 tests/unit/session/test_session.py
 third_party/bigframes_vendored/__init__.py
 third_party/bigframes_vendored/py.typed
 third_party/bigframes_vendored/cpython/LICENSE
 third_party/bigframes_vendored/cpython/__init__.py
 third_party/bigframes_vendored/cpython/_pprint.py
 third_party/bigframes_vendored/google_cloud_bigquery/LICENSE
```

### Comparing `bigframes-1.4.0/bigframes.egg-info/requires.txt` & `bigframes-1.5.0/bigframes.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/setup.py` & `bigframes-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/__init__.py` & `bigframes-1.5.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/hockey_players.json` & `bigframes-1.5.0/tests/data/hockey_players.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/hockey_players.jsonl` & `bigframes-1.5.0/tests/data/hockey_players.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/nested.jsonl` & `bigframes-1.5.0/tests/data/nested.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/nested_schema.json` & `bigframes-1.5.0/tests/data/nested_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/penguins.jsonl` & `bigframes-1.5.0/tests/data/penguins.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/penguins_schema.json` & `bigframes-1.5.0/tests/data/penguins_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/scalars.jsonl` & `bigframes-1.5.0/tests/data/scalars.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/scalars_schema.json` & `bigframes-1.5.0/tests/data/scalars_schema.json`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/data/time_series.jsonl` & `bigframes-1.5.0/tests/data/time_series.jsonl`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/__init__.py` & `bigframes-1.5.0/tests/system/large/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/conftest.py` & `bigframes-1.5.0/tests/system/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from datetime import datetime
 import hashlib
 import logging
 import math
 import pathlib
 import textwrap
 import typing
-from typing import Dict, Optional
+from typing import Dict, Generator, Optional
 
 import google.api_core.exceptions
 import google.cloud.bigquery as bigquery
 import google.cloud.bigquery_connection_v1 as bigquery_connection_v1
 import google.cloud.exceptions
 import google.cloud.functions_v2 as functions_v2
 import google.cloud.resourcemanager_v3 as resourcemanager_v3
@@ -123,24 +123,31 @@
 def resourcemanager_client(
     session: bigframes.Session,
 ) -> resourcemanager_v3.ProjectsClient:
     return session.resourcemanagerclient
 
 
 @pytest.fixture(scope="session")
-def session() -> bigframes.Session:
-    return bigframes.Session()
+def session() -> Generator[bigframes.Session, None, None]:
+    context = bigframes.BigQueryOptions(
+        location="US",
+    )
+    session = bigframes.Session(context=context)
+    yield session
+    session.close()  # close generated session at cleanup time
 
 
 @pytest.fixture(scope="session")
-def session_tokyo(tokyo_location: str) -> bigframes.Session:
+def session_tokyo(tokyo_location: str) -> Generator[bigframes.Session, None, None]:
     context = bigframes.BigQueryOptions(
         location=tokyo_location,
     )
-    return bigframes.Session(context=context)
+    session = bigframes.Session(context=context)
+    yield session
+    session.close()  # close generated session at cleanup type
 
 
 @pytest.fixture(scope="session", autouse=True)
 def cleanup_datasets(bigquery_client: bigquery.Client) -> None:
     """Cleanup any datasets that were created but not cleaned up."""
     for dataset in bigquery_client.list_datasets():
         if prefixer.should_cleanup(dataset.dataset_id):
```

### Comparing `bigframes-1.4.0/tests/system/large/__init__.py` & `bigframes-1.5.0/tests/system/small/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_cluster.py` & `bigframes-1.5.0/tests/system/large/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_compose.py` & `bigframes-1.5.0/tests/system/large/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_core.py` & `bigframes-1.5.0/tests/system/large/ml/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pandas
+import pytest
 
 from bigframes.ml import globals
 
 
+# TODO(garrettwu): Re-enable or not check exact numbers.
+@pytest.mark.skip(reason="bqml regression")
 def test_bqml_e2e(session, dataset_id, penguins_df_default_index, new_penguins_df):
     df = penguins_df_default_index.dropna()
     X_train = df[
         [
             "species",
             "island",
             "culmen_length_mm",
```

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_decomposition.py` & `bigframes-1.5.0/tests/system/large/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_ensemble.py` & `bigframes-1.5.0/tests/system/large/ml/test_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 import pandas
 import pytest
 
 import bigframes.ml.ensemble
 
 
+# TODO(garrettwu): Re-enable or not check exact numbers.
+@pytest.mark.skip(reason="bqml regression")
 @pytest.mark.flaky(retries=2)
 def test_xgbregressor_default_params(penguins_df_default_index, dataset_id):
     model = bigframes.ml.ensemble.XGBRegressor()
 
     df = penguins_df_default_index.dropna()
     X_train = df[
         [
```

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_forecasting.py` & `bigframes-1.5.0/tests/system/large/ml/test_forecasting.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pandas as pd
+import pytest
 
 from bigframes.ml import forecasting
 
 ARIMA_EVALUATE_OUTPUT_COL = [
     "non_seasonal_p",
     "non_seasonal_d",
     "non_seasonal_q",
@@ -27,23 +28,30 @@
     "has_holiday_effect",
     "has_spikes_and_dips",
     "has_step_changes",
     "error_message",
 ]
 
 
-def test_arima_plus_model_fit_score(
-    time_series_df_default_index, dataset_id, new_time_series_df
-):
+@pytest.fixture(scope="module")
+def arima_model(time_series_df_default_index):
     model = forecasting.ARIMAPlus()
     X_train = time_series_df_default_index[["parsed_date"]]
     y_train = time_series_df_default_index[["total_visits"]]
     model.fit(X_train, y_train)
+    return model
 
-    result = model.score(
+
+def test_arima_plus_model_fit_score(
+    dataset_id,
+    new_time_series_df,
+    arima_model,
+):
+
+    result = arima_model.score(
         new_time_series_df[["parsed_date"]], new_time_series_df[["total_visits"]]
     ).to_pandas()
     expected = pd.DataFrame(
         {
             "mean_absolute_error": [154.742547],
             "mean_squared_error": [26844.868855],
             "root_mean_squared_error": [163.844038],
@@ -52,37 +60,47 @@
         },
         dtype="Float64",
     )
     expected = expected.reindex(index=expected.index.astype("Int64"))
     pd.testing.assert_frame_equal(result, expected, check_exact=False, rtol=0.1)
 
     # save, load to ensure configuration was kept
-    reloaded_model = model.to_gbq(f"{dataset_id}.temp_arima_plus_model", replace=True)
+    reloaded_model = arima_model.to_gbq(
+        f"{dataset_id}.temp_arima_plus_model", replace=True
+    )
     assert (
         f"{dataset_id}.temp_arima_plus_model" in reloaded_model._bqml_model.model_name
     )
 
 
-def test_arima_plus_model_fit_summary(time_series_df_default_index, dataset_id):
-    model = forecasting.ARIMAPlus()
-    X_train = time_series_df_default_index[["parsed_date"]]
-    y_train = time_series_df_default_index[["total_visits"]]
-    model.fit(X_train, y_train)
+def test_arima_plus_model_fit_summary(dataset_id, arima_model):
 
-    result = model.summary()
+    result = arima_model.summary()
     assert result.shape == (1, 12)
     assert all(column in result.columns for column in ARIMA_EVALUATE_OUTPUT_COL)
 
     # save, load to ensure configuration was kept
-    reloaded_model = model.to_gbq(f"{dataset_id}.temp_arima_plus_model", replace=True)
+    reloaded_model = arima_model.to_gbq(
+        f"{dataset_id}.temp_arima_plus_model", replace=True
+    )
     assert (
         f"{dataset_id}.temp_arima_plus_model" in reloaded_model._bqml_model.model_name
     )
 
 
+def test_arima_coefficients(arima_model):
+    got = arima_model.coef_
+    expected_columns = {
+        "ar_coefficients",
+        "ma_coefficients",
+        "intercept_or_drift",
+    }
+    assert set(got.columns) == expected_columns
+
+
 def test_arima_plus_model_fit_params(time_series_df_default_index, dataset_id):
     model = forecasting.ARIMAPlus(
         horizon=100,
         auto_arima=True,
         auto_arima_max_order=4,
         auto_arima_min_order=1,
         data_frequency="daily",
```

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_linear_model.py` & `bigframes-1.5.0/tests/system/large/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/ml/test_pipeline.py` & `bigframes-1.5.0/tests/system/large/ml/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,16 @@
     )
     pd.testing.assert_frame_equal(
         predictions[["predicted_sex"]],
         expected,
     )
 
 
+# TODO(garrettwu): Re-enable or not check exact numbers.
+@pytest.mark.skip(reason="bqml regression")
 @pytest.mark.flaky(retries=2)
 def test_pipeline_xgbregressor_fit_score_predict(session, penguins_df_default_index):
     """Test a supervised model with a minimal preprocessing step"""
     pl = pipeline.Pipeline(
         [
             ("scale", preprocessing.StandardScaler()),
             ("xgbreg", ensemble.XGBRegressor()),
@@ -293,14 +295,16 @@
         index=pd.Index([1633, 1672, 1690], name="tag_number", dtype="Int64"),
     )
     pd.testing.assert_frame_equal(
         predictions[["predicted_body_mass_g"]], expected, check_exact=False, rtol=0.1
     )
 
 
+# TODO(garrettwu): Re-enable or not check exact numbers.
+@pytest.mark.skip(reason="bqml regression")
 @pytest.mark.flaky(retries=2)
 def test_pipeline_random_forest_classifier_fit_score_predict(
     session, penguins_df_default_index
 ):
     """Test a supervised model with a minimal preprocessing step"""
     pl = pipeline.Pipeline(
         [
```

### Comparing `bigframes-1.4.0/tests/system/large/test_location.py` & `bigframes-1.5.0/tests/system/large/test_location.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/large/test_remote_function.py` & `bigframes-1.5.0/tests/system/large/test_remote_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1410,7 +1410,47 @@
 @pytest.mark.flaky(retries=2, delay=120)
 def test_remote_function_gcf_timeout_max_supported_exceeded(session):
     with pytest.raises(ValueError):
 
         @session.remote_function([int], int, reuse=False, cloud_function_timeout=1201)
         def square(x):
             return x * x
+
+
+@pytest.mark.parametrize(
+    ("max_instances_args", "expected_max_instances"),
+    [
+        pytest.param({}, 100, id="no-set"),
+        pytest.param({"cloud_function_max_instances": None}, 100, id="set-None"),
+        pytest.param({"cloud_function_max_instances": 1000}, 1000, id="set-explicit"),
+    ],
+)
+@pytest.mark.flaky(retries=2, delay=120)
+def test_remote_function_max_instances(
+    session, scalars_dfs, max_instances_args, expected_max_instances
+):
+    try:
+
+        def square(x):
+            return x * x
+
+        square_remote = session.remote_function(
+            [int], int, reuse=False, **max_instances_args
+        )(square)
+
+        # Assert that the GCF is created with the intended max instance count
+        gcf = session.cloudfunctionsclient.get_function(
+            name=square_remote.bigframes_cloud_function
+        )
+        assert gcf.service_config.max_instance_count == expected_max_instances
+
+        scalars_df, scalars_pandas_df = scalars_dfs
+
+        bf_result = scalars_df["int64_too"].apply(square_remote).to_pandas()
+        pd_result = scalars_pandas_df["int64_too"].apply(square)
+
+        pandas.testing.assert_series_equal(bf_result, pd_result, check_dtype=False)
+    finally:
+        # clean up the gcp assets created for the remote function
+        cleanup_remote_function_assets(
+            session.bqclient, session.cloudfunctionsclient, square_remote
+        )
```

### Comparing `bigframes-1.4.0/tests/system/load/test_large_tables.py` & `bigframes-1.5.0/tests/system/load/test_large_tables.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/load/test_llm.py` & `bigframes-1.5.0/tests/system/load/test_llm.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/__init__.py` & `bigframes-1.5.0/tests/system/small/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/__init__.py` & `bigframes-1.5.0/tests/system/small/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/conftest.py` & `bigframes-1.5.0/tests/system/small/ml/conftest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_cluster.py` & `bigframes-1.5.0/tests/system/small/ml/test_cluster.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_core.py` & `bigframes-1.5.0/tests/system/small/ml/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_decomposition.py` & `bigframes-1.5.0/tests/system/small/ml/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_ensemble.py` & `bigframes-1.5.0/tests/system/small/ml/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_forecasting.py` & `bigframes-1.5.0/tests/system/small/ml/test_forecasting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_imported.py` & `bigframes-1.5.0/tests/system/small/ml/test_imported.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_linear_model.py` & `bigframes-1.5.0/tests/system/small/ml/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_llm.py` & `bigframes-1.5.0/tests/system/small/ml/test_llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,60 +51,66 @@
 
 @pytest.mark.flaky(retries=2)
 def test_create_text_generator_model_default_session(
     bq_connection, llm_text_pandas_df, bigquery_client
 ):
     import bigframes.pandas as bpd
 
-    bpd.close_session()
-    bpd.options.bigquery.bq_connection = bq_connection
-    bpd.options.bigquery.location = "us"
-
-    model = llm.PaLM2TextGenerator()
-    assert model is not None
-    assert model._bqml_model is not None
-    assert (
-        model.connection_name.casefold()
-        == f"{bigquery_client.project}.us.bigframes-rf-conn"
-    )
-
-    llm_text_df = bpd.read_pandas(llm_text_pandas_df)
-
-    df = model.predict(llm_text_df).to_pandas()
-    assert df.shape == (3, 4)
-    assert "ml_generate_text_llm_result" in df.columns
-    series = df["ml_generate_text_llm_result"]
-    assert all(series.str.len() > 20)
+    # Note: This starts a thread-local session.
+    with bpd.option_context(
+        "bigquery.bq_connection",
+        bq_connection,
+        "bigquery.location",
+        "US",
+    ):
+        model = llm.PaLM2TextGenerator()
+        assert model is not None
+        assert model._bqml_model is not None
+        assert (
+            model.connection_name.casefold()
+            == f"{bigquery_client.project}.us.bigframes-rf-conn"
+        )
+
+        llm_text_df = bpd.read_pandas(llm_text_pandas_df)
+
+        df = model.predict(llm_text_df).to_pandas()
+        assert df.shape == (3, 4)
+        assert "ml_generate_text_llm_result" in df.columns
+        series = df["ml_generate_text_llm_result"]
+        assert all(series.str.len() > 20)
 
 
 @pytest.mark.flaky(retries=2)
 def test_create_text_generator_32k_model_default_session(
     bq_connection, llm_text_pandas_df, bigquery_client
 ):
     import bigframes.pandas as bpd
 
-    bpd.close_session()
-    bpd.options.bigquery.bq_connection = bq_connection
-    bpd.options.bigquery.location = "us"
-
-    model = llm.PaLM2TextGenerator(model_name="text-bison-32k")
-    assert model is not None
-    assert model._bqml_model is not None
-    assert (
-        model.connection_name.casefold()
-        == f"{bigquery_client.project}.us.bigframes-rf-conn"
-    )
-
-    llm_text_df = bpd.read_pandas(llm_text_pandas_df)
-
-    df = model.predict(llm_text_df).to_pandas()
-    assert df.shape == (3, 4)
-    assert "ml_generate_text_llm_result" in df.columns
-    series = df["ml_generate_text_llm_result"]
-    assert all(series.str.len() > 20)
+    # Note: This starts a thread-local session.
+    with bpd.option_context(
+        "bigquery.bq_connection",
+        bq_connection,
+        "bigquery.location",
+        "US",
+    ):
+        model = llm.PaLM2TextGenerator(model_name="text-bison-32k")
+        assert model is not None
+        assert model._bqml_model is not None
+        assert (
+            model.connection_name.casefold()
+            == f"{bigquery_client.project}.us.bigframes-rf-conn"
+        )
+
+        llm_text_df = bpd.read_pandas(llm_text_pandas_df)
+
+        df = model.predict(llm_text_df).to_pandas()
+        assert df.shape == (3, 4)
+        assert "ml_generate_text_llm_result" in df.columns
+        series = df["ml_generate_text_llm_result"]
+        assert all(series.str.len() > 20)
 
 
 @pytest.mark.flaky(retries=2)
 def test_create_text_generator_model_default_connection(
     llm_text_pandas_df, bigquery_client
 ):
     from bigframes import _config
@@ -228,35 +234,41 @@
     assert reloaded_model.model_name == "textembedding-gecko-multilingual"
     assert reloaded_model.connection_name == bq_connection
 
 
 def test_create_text_embedding_generator_model_defaults(bq_connection):
     import bigframes.pandas as bpd
 
-    bpd.close_session()
-    bpd.options.bigquery.bq_connection = bq_connection
-    bpd.options.bigquery.location = "us"
-
-    model = llm.PaLM2TextEmbeddingGenerator()
-    assert model is not None
-    assert model._bqml_model is not None
+    # Note: This starts a thread-local session.
+    with bpd.option_context(
+        "bigquery.bq_connection",
+        bq_connection,
+        "bigquery.location",
+        "US",
+    ):
+        model = llm.PaLM2TextEmbeddingGenerator()
+        assert model is not None
+        assert model._bqml_model is not None
 
 
 def test_create_text_embedding_generator_multilingual_model_defaults(bq_connection):
     import bigframes.pandas as bpd
 
-    bpd.close_session()
-    bpd.options.bigquery.bq_connection = bq_connection
-    bpd.options.bigquery.location = "us"
-
-    model = llm.PaLM2TextEmbeddingGenerator(
-        model_name="textembedding-gecko-multilingual"
-    )
-    assert model is not None
-    assert model._bqml_model is not None
+    # Note: This starts a thread-local session.
+    with bpd.option_context(
+        "bigquery.bq_connection",
+        bq_connection,
+        "bigquery.location",
+        "US",
+    ):
+        model = llm.PaLM2TextEmbeddingGenerator(
+            model_name="textembedding-gecko-multilingual"
+        )
+        assert model is not None
+        assert model._bqml_model is not None
 
 
 @pytest.mark.flaky(retries=2)
 def test_embedding_generator_predict_success(
     palm2_embedding_generator_model, llm_text_df
 ):
     df = palm2_embedding_generator_model.predict(llm_text_df).to_pandas()
```

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_metrics.py` & `bigframes-1.5.0/tests/system/small/ml/test_metrics.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_metrics_pairwise.py` & `bigframes-1.5.0/tests/system/small/ml/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_model_selection.py` & `bigframes-1.5.0/tests/system/small/ml/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_preprocessing.py` & `bigframes-1.5.0/tests/system/small/ml/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_register.py` & `bigframes-1.5.0/tests/system/small/ml/test_register.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/ml/test_remote.py` & `bigframes-1.5.0/tests/system/small/ml/test_remote.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/operations/__init__.py` & `bigframes-1.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/operations/test_datetimes.py` & `bigframes-1.5.0/tests/system/small/operations/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/operations/test_plotting.py` & `bigframes-1.5.0/tests/system/small/operations/test_plotting.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/operations/test_strings.py` & `bigframes-1.5.0/tests/system/small/operations/test_strings.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/regression/test_issue355_merge_after_filter.py` & `bigframes-1.5.0/tests/system/small/regression/test_issue355_merge_after_filter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_dataframe.py` & `bigframes-1.5.0/tests/system/small/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,26 +138,21 @@
         bf_result, pd_result, check_dtype=False, check_index_type=False
     )
 
 
 def test_df_construct_inline_respects_location():
     import bigframes.pandas as bpd
 
-    bpd.close_session()
-    bpd.options.bigquery.location = "europe-west1"
+    # Note: This starts a thread-local session.
+    with bpd.option_context("bigquery.location", "europe-west1"):
+        df = bpd.DataFrame([[1, 2, 3], [4, 5, 6]])
+        repr(df)
 
-    df = bpd.DataFrame([[1, 2, 3], [4, 5, 6]])
-    repr(df)
-
-    table = bpd.get_global_session().bqclient.get_table(df.query_job.destination)
-    assert table.location == "europe-west1"
-
-    # Reset global session
-    bpd.close_session()
-    bpd.options.bigquery.location = "us"
+        table = bpd.get_global_session().bqclient.get_table(df.query_job.destination)
+        assert table.location == "europe-west1"
 
 
 def test_get_column(scalars_dfs):
     scalars_df, scalars_pandas_df = scalars_dfs
     col_name = "int64_col"
     series = scalars_df[col_name]
     bf_result = series.to_pandas()
```

### Comparing `bigframes-1.4.0/tests/system/small/test_dataframe_io.py` & `bigframes-1.5.0/tests/system/small/test_dataframe_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
     expected = scalars_df_default_index.dtypes
     for df in scalars_df_default_index.to_pandas_batches():
         actual = df.dtypes
         pd.testing.assert_series_equal(actual, expected)
 
 
 @pytest.mark.parametrize(
-    ("index"),
-    [True, False],
+    ("index",),
+    [(True,), (False,)],
 )
 def test_to_csv_index(
     scalars_dfs: Tuple[bigframes.dataframe.DataFrame, pd.DataFrame],
     gcs_folder: str,
     index: bool,
 ):
     if pd.__version__.startswith("1."):
```

### Comparing `bigframes-1.4.0/tests/system/small/test_encryption.py` & `bigframes-1.5.0/tests/system/small/test_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,15 @@
 
 
 def test_session_load_job(bq_cmek, session_with_bq_cmek):
     if not bq_cmek:  # pragma: NO COVER
         pytest.skip("no cmek set for testing")  # pragma: NO COVER
 
     # Session should have cmek set in the default query and load job configs
-    load_table = bigframes.session._io.bigquery.random_table(
-        session_with_bq_cmek._anonymous_dataset
-    )
+    load_table = session_with_bq_cmek._random_table()
 
     df = pandas.DataFrame({"col0": [1, 2, 3]})
     load_job_config = session_with_bq_cmek._prepare_load_job_config()
     load_job_config.schema = [
         bigquery.SchemaField(df.columns[0], bigquery.enums.SqlTypeNames.INT64)
     ]
 
@@ -184,17 +182,15 @@
     # Write the result to BQ and assert encryption
     output_table_id = df.to_gbq()
     output_table = session_with_bq_cmek.bqclient.get_table(output_table_id)
     assert output_table.encryption_configuration.kms_key_name == bq_cmek
 
     # Write the result to BQ custom table and assert encryption
     session_with_bq_cmek.bqclient.get_table(output_table_id)
-    output_table_ref = bigframes.session._io.bigquery.random_table(
-        session_with_bq_cmek._anonymous_dataset
-    )
+    output_table_ref = session_with_bq_cmek._random_table()
     output_table_id = str(output_table_ref)
     df.to_gbq(output_table_id)
     output_table = session_with_bq_cmek.bqclient.get_table(output_table_id)
     assert output_table.encryption_configuration.kms_key_name == bq_cmek
 
     # Lastly, assert that the encryption is not because of any default set at
     # the dataset level
```

### Comparing `bigframes-1.4.0/tests/system/small/test_groupby.py` & `bigframes-1.5.0/tests/system/small/test_groupby.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_ibis.py` & `bigframes-1.5.0/tests/system/small/test_ibis.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_index.py` & `bigframes-1.5.0/tests/system/small/test_index.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_ipython.py` & `bigframes-1.5.0/tests/system/small/test_ipython.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_multiindex.py` & `bigframes-1.5.0/tests/system/small/test_multiindex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1187,7 +1187,26 @@
     pd_df = df.to_pandas()
     pandas.testing.assert_frame_equal(
         df["col0"].explode("col00").to_pandas(),
         pd_df["col0"].explode("col00"),
         check_dtype=False,
         check_index_type=False,
     )
+
+
+def test_column_multi_index_w_na_stack(scalars_df_index, scalars_pandas_df_index):
+    columns = ["int64_too", "int64_col", "rowindex_2"]
+    level1 = pandas.Index(["b", "c", "d"])
+    # Need resulting column to be pyarrow string rather than object dtype
+    level2 = pandas.Index([None, "b", "b"], dtype="string[pyarrow]")
+    multi_columns = pandas.MultiIndex.from_arrays([level1, level2])
+    bf_df = scalars_df_index[columns].copy()
+    bf_df.columns = multi_columns
+    pd_df = scalars_pandas_df_index[columns].copy()
+    pd_df.columns = multi_columns
+
+    pd_result = pd_df.stack()
+    bf_result = bf_df.stack().to_pandas()
+
+    # Pandas produces pd.NA, where bq dataframes produces NaN
+    pd_result["c"] = pd_result["c"].replace(pandas.NA, np.nan)
+    pandas.testing.assert_frame_equal(bf_result, pd_result, check_dtype=False)
```

### Comparing `bigframes-1.4.0/tests/system/small/test_numpy.py` & `bigframes-1.5.0/tests/system/small/test_numpy.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_pandas.py` & `bigframes-1.5.0/tests/system/small/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_pandas_options.py` & `bigframes-1.5.0/tests/system/small/test_pandas_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 from unittest import mock
+import warnings
 
 import google.api_core.exceptions
 import google.auth
 import google.auth.exceptions
 import pytest
 
 import bigframes.core.global_session
 import bigframes.pandas as bpd
 
 
 @pytest.fixture(autouse=True)
 def reset_default_session_and_location():
-    bpd.close_session()
-    bpd.options.bigquery.location = None
+    # Note: This starts a thread-local session and closes it once the test
+    # finishes.
+    with bpd.option_context("bigquery.location", None):
+        bpd.options.bigquery.location = None
+        yield
 
 
 @pytest.mark.parametrize(
     ("read_method", "query_prefix"),
     [
         (bpd.read_gbq, None),
         (bpd.read_gbq, "SELECT COUNT(1) FROM "),
@@ -75,15 +79,17 @@
     # Now read_gbq* from another location should fail
     with pytest.raises(
         (google.api_core.exceptions.NotFound, ValueError),
         match=dataset_id_permanent,
     ):
         read_method(query)
 
-    # Close global session to start over
+    # Close the global session to start over.
+    # Note: This is a thread-local operation because of the
+    # reset_default_session_and_location fixture above.
     bpd.close_session()
 
     # There should still be the previous location set in the bigquery options
     assert bpd.options.bigquery.location == tokyo_location
 
     # Reset the location to be able to query another location
     bpd.options.bigquery.location = None
@@ -250,15 +256,15 @@
 
     # Starting user journey with read_gbq* should work for a table in the same
     # location, in this case tokyo
     df = read_method(query_tokyo)
     assert df is not None
 
 
-def test_close_session_after_credentials_need_reauthentication(monkeypatch):
+def test_credentials_need_reauthentication(monkeypatch):
     # Use a simple test query to verify that default session works to interact
     # with BQ
     test_query = "SELECT 1"
 
     # Confirm that default session has BQ client with valid credentials
     session = bpd.get_global_session()
     assert session.bqclient._credentials.valid
@@ -284,14 +290,30 @@
             query_job = session.bqclient.query(test_query)
             query_job.result()  # blocks until finished
 
         # Confirm that as a result bigframes.pandas interface is unusable
         with pytest.raises(google.auth.exceptions.RefreshError):
             bpd.read_gbq(test_query)
 
-        # Now verify that closing the session works
-        bpd.close_session()
-        assert bigframes.core.global_session._global_session is None
+        # Now verify that closing the session works We look at the
+        # thread-local session because of the
+        # reset_default_session_and_location fixture and that this test mutates
+        # state that might otherwise be used by tests running in parallel.
+        assert (
+            bigframes.core.global_session._global_session_state.thread_local_session
+            is not None
+        )
+
+        with warnings.catch_warnings(record=True) as warned:
+            bpd.close_session()  # CleanupFailedWarning: can't clean up
+
+        assert len(warned) == 1
+        assert warned[0].category == bigframes.exceptions.CleanupFailedWarning
+
+        assert (
+            bigframes.core.global_session._global_session_state.thread_local_session
+            is None
+        )
 
     # Now verify that use is able to start over
     df = bpd.read_gbq(test_query)
     assert df is not None
```

### Comparing `bigframes-1.4.0/tests/system/small/test_progress_bar.py` & `bigframes-1.5.0/tests/system/small/test_progress_bar.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,66 +19,72 @@
 import pandas as pd
 
 import bigframes as bf
 import bigframes.formatting_helpers as formatting_helpers
 from bigframes.session import MAX_INLINE_DF_BYTES
 
 job_load_message_regex = r"\w+ job [\w-]+ is \w+\."
+EXPECTED_DRY_RUN_MESSAGE = "Computation deferred. Computation will process"
 
 
 def test_progress_bar_dataframe(
     penguins_df_default_index: bf.dataframe.DataFrame, capsys
 ):
-    bf.options.display.progress_bar = "terminal"
     capsys.readouterr()  # clear output
-    penguins_df_default_index.to_pandas()
+
+    with bf.option_context("display.progress_bar", "terminal"):
+        penguins_df_default_index.to_pandas()
 
     assert_loading_msg_exist(capsys.readouterr().out)
     assert penguins_df_default_index.query_job is not None
 
 
 def test_progress_bar_series(penguins_df_default_index: bf.dataframe.DataFrame, capsys):
-    bf.options.display.progress_bar = "terminal"
     series = penguins_df_default_index["body_mass_g"].head(10)
     capsys.readouterr()  # clear output
-    series.to_pandas()
+
+    with bf.option_context("display.progress_bar", "terminal"):
+        series.to_pandas()
 
     assert_loading_msg_exist(capsys.readouterr().out)
     assert series.query_job is not None
 
 
 def test_progress_bar_scalar(penguins_df_default_index: bf.dataframe.DataFrame, capsys):
-    bf.options.display.progress_bar = "terminal"
     capsys.readouterr()  # clear output
-    penguins_df_default_index["body_mass_g"].head(10).mean()
+
+    with bf.option_context("display.progress_bar", "terminal"):
+        penguins_df_default_index["body_mass_g"].head(10).mean()
 
     assert_loading_msg_exist(capsys.readouterr().out)
 
 
 def test_progress_bar_extract_jobs(
     penguins_df_default_index: bf.dataframe.DataFrame, gcs_folder, capsys
 ):
-    bf.options.display.progress_bar = "terminal"
     path = gcs_folder + "test_read_csv_progress_bar*.csv"
     capsys.readouterr()  # clear output
-    penguins_df_default_index.to_csv(path)
+
+    with bf.option_context("display.progress_bar", "terminal"):
+        penguins_df_default_index.to_csv(path)
 
     assert_loading_msg_exist(capsys.readouterr().out)
 
 
 def test_progress_bar_load_jobs(
     session: bf.Session, penguins_pandas_df_default_index: pd.DataFrame, capsys
 ):
     # repeat the DF to be big enough to trigger the load job.
     df = penguins_pandas_df_default_index
     while len(df) < MAX_INLINE_DF_BYTES:
         df = pd.DataFrame(np.repeat(df.values, 2, axis=0))
 
-    bf.options.display.progress_bar = "terminal"
-    with tempfile.TemporaryDirectory() as dir:
+    with bf.option_context(
+        "display.progress_bar", "terminal"
+    ), tempfile.TemporaryDirectory() as dir:
         path = dir + "/test_read_csv_progress_bar*.csv"
         df.to_csv(path, index=False)
         capsys.readouterr()  # clear output
         session.read_csv(path)
 
     assert_loading_msg_exist(capsys.readouterr().out)
 
@@ -92,19 +98,20 @@
     for line in lines:
         if re.match(pattern, line) is not None:
             numLoadingMsg += 1
     assert numLoadingMsg > 0
 
 
 def test_query_job_repr_html(penguins_df_default_index: bf.dataframe.DataFrame):
-    bf.options.display.progress_bar = "terminal"
-    penguins_df_default_index.to_pandas()
-    query_job_repr = formatting_helpers.repr_query_job_html(
-        penguins_df_default_index.query_job
-    ).value
+    with bf.option_context("display.progress_bar", "terminal"):
+        penguins_df_default_index.to_pandas()
+        query_job_repr = formatting_helpers.repr_query_job_html(
+            penguins_df_default_index.query_job
+        ).value
+
     string_checks = [
         "Job Id",
         "Destination Table",
         "Slot Time",
         "Bytes Processed",
         "Cache hit",
     ]
@@ -122,7 +129,25 @@
         "Destination Table",
         "Slot Time",
         "Bytes Processed",
         "Cache hit",
     ]
     for string in string_checks:
         assert string in query_job_repr
+
+
+def test_query_job_dry_run_dataframe(penguins_df_default_index: bf.dataframe.DataFrame):
+    with bf.option_context("display.repr_mode", "deferred"):
+        df_result = repr(penguins_df_default_index)
+        assert EXPECTED_DRY_RUN_MESSAGE in df_result
+
+
+def test_query_job_dry_run_index(penguins_df_default_index: bf.dataframe.DataFrame):
+    with bf.option_context("display.repr_mode", "deferred"):
+        index_result = repr(penguins_df_default_index.index)
+        assert EXPECTED_DRY_RUN_MESSAGE in index_result
+
+
+def test_query_job_dry_run_series(penguins_df_default_index: bf.dataframe.DataFrame):
+    with bf.option_context("display.repr_mode", "deferred"):
+        series_result = repr(penguins_df_default_index["body_mass_g"])
+        assert EXPECTED_DRY_RUN_MESSAGE in series_result
```

### Comparing `bigframes-1.4.0/tests/system/small/test_remote_function.py` & `bigframes-1.5.0/tests/system/small/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_scalar.py` & `bigframes-1.5.0/tests/system/small/test_scalar.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_series.py` & `bigframes-1.5.0/tests/system/small/test_series.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/small/test_session.py` & `bigframes-1.5.0/tests/system/small/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,14 +401,32 @@
             """
 
     df = session.read_gbq(query, configuration=config)
 
     assert df.shape == (9, 3)
 
 
+def test_read_gbq_with_custom_global_labels(
+    session: bigframes.Session, scalars_table_id: str
+):
+    bigframes.options.compute.assign_extra_query_labels(test1=1, test2="abc")
+    bigframes.options.compute.extra_query_labels["test3"] = False
+
+    job_labels = session.read_gbq(scalars_table_id).query_job.labels  # type:ignore
+    expected_labels = {"test1": "1", "test2": "abc", "test3": "false"}
+
+    assert all(job_labels.get(key) == value for key, value in expected_labels.items())
+
+    del bigframes.options.compute.extra_query_labels["test1"]
+    del bigframes.options.compute.extra_query_labels["test2"]
+    del bigframes.options.compute.extra_query_labels["test3"]
+
+    assert len(bigframes.options.compute.extra_query_labels) == 0
+
+
 def test_read_gbq_model(session, penguins_linear_model_name):
     model = session.read_gbq_model(penguins_linear_model_name)
     assert isinstance(model, bigframes.ml.linear_model.LinearRegression)
 
 
 def test_read_pandas(session, scalars_dfs):
     _, scalars_pandas_df = scalars_dfs
@@ -520,15 +538,19 @@
     pd.testing.assert_series_equal(df.dtypes, scalars_df.dtypes)
 
 
 def test_read_csv_gcs_bq_engine(session, scalars_dfs, gcs_folder):
     scalars_df, _ = scalars_dfs
     path = gcs_folder + "test_read_csv_gcs_bq_engine_w_index*.csv"
     scalars_df.to_csv(path, index=False)
-    df = session.read_csv(path, engine="bigquery")
+    df = session.read_csv(
+        path,
+        engine="bigquery",
+        index_col=bigframes.enums.DefaultIndexKind.SEQUENTIAL_INT64,
+    )
 
     # TODO(chelsealin): If we serialize the index, can more easily compare values.
     pd.testing.assert_index_equal(df.columns, scalars_df.columns)
 
     # The auto detects of BigQuery load job have restrictions to detect the bytes,
     # datetime, numeric and geometry types, so they're skipped here.
     df = df.drop(columns=["bytes_col", "datetime_col", "numeric_col", "geography_col"])
@@ -625,52 +647,32 @@
         scalars_df = scalars_df.drop(
             columns=["bytes_col", "datetime_col", "numeric_col", "geography_col"]
         )
         assert df.shape[0] == scalars_df.shape[0]
         pd.testing.assert_series_equal(df.dtypes, scalars_df.dtypes)
 
 
-@pytest.mark.parametrize(
-    ("kwargs", "match"),
-    [
-        pytest.param(
-            {"engine": "bigquery", "names": []},
-            "BigQuery engine does not support these arguments",
-            id="with_names",
-        ),
-        pytest.param(
-            {"engine": "bigquery", "dtype": {}},
-            "BigQuery engine does not support these arguments",
-            id="with_dtype",
-        ),
-        pytest.param(
-            {"engine": "bigquery", "index_col": False},
-            "BigQuery engine only supports a single column name for `index_col`.",
-            id="with_index_col_false",
-        ),
-        pytest.param(
-            {"engine": "bigquery", "index_col": 5},
-            "BigQuery engine only supports a single column name for `index_col`.",
-            id="with_index_col_not_str",
-        ),
-        pytest.param(
-            {"engine": "bigquery", "usecols": [1, 2]},
-            "BigQuery engine only supports an iterable of strings for `usecols`.",
-            id="with_usecols_invalid",
-        ),
-        pytest.param(
-            {"engine": "bigquery", "encoding": "ASCII"},
-            "BigQuery engine only supports the following encodings",
-            id="with_encoding_invalid",
-        ),
-    ],
-)
-def test_read_csv_bq_engine_throws_not_implemented_error(session, kwargs, match):
-    with pytest.raises(NotImplementedError, match=match):
-        session.read_csv("", **kwargs)
+def test_read_csv_bq_engine_supports_index_col_false(
+    session, scalars_df_index, gcs_folder
+):
+    path = gcs_folder + "test_read_csv_bq_engine_supports_index_col_false*.csv"
+    read_path = utils.get_first_file_from_wildcard(path)
+    scalars_df_index.to_csv(path)
+
+    df = session.read_csv(
+        read_path,
+        # Normally, pandas uses the first column as the index. index_col=False
+        # turns off that behavior.
+        index_col=False,
+    )
+    assert df.shape[0] == scalars_df_index.shape[0]
+
+    # We use a default index because of index_col=False, so the previous index
+    # column is just loaded as a column.
+    assert len(df.columns) == len(scalars_df_index.columns) + 1
 
 
 @pytest.mark.parametrize(
     ("kwargs", "match"),
     [
         pytest.param(
             {"chunksize": 5},
```

### Comparing `bigframes-1.4.0/tests/system/small/test_window.py` & `bigframes-1.5.0/tests/system/small/test_window.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/system/utils.py` & `bigframes-1.5.0/tests/system/utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/__init__.py` & `bigframes-1.5.0/tests/unit/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/_config/__init__.py` & `bigframes-1.5.0/tests/unit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/_config/test_bigquery_options.py` & `bigframes-1.5.0/tests/unit/_config/test_bigquery_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/core/__init__.py` & `bigframes-1.5.0/tests/unit/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/core/test_bf_utils.py` & `bigframes-1.5.0/tests/unit/core/test_bf_utils.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/core/test_blocks.py` & `bigframes-1.5.0/tests/unit/core/test_blocks.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/core/test_expression.py` & `bigframes-1.5.0/tests/unit/core/test_expression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/core/test_log_adapter.py` & `bigframes-1.5.0/tests/unit/core/test_log_adapter.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/__init__.py` & `bigframes-1.5.0/tests/unit/session/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/test_api_primitives.py` & `bigframes-1.5.0/tests/unit/ml/test_api_primitives.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/test_compose.py` & `bigframes-1.5.0/tests/unit/ml/test_compose.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/test_golden_sql.py` & `bigframes-1.5.0/tests/unit/ml/test_golden_sql.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/test_pipeline.py` & `bigframes-1.5.0/tests/unit/ml/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/ml/test_sql.py` & `bigframes-1.5.0/tests/unit/ml/test_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,24 @@
     mock_df = mock.create_autospec(spec=bpd.DataFrame)
     mock_df.sql = "input_X_y_sql"
     mock_df._to_sql_query.return_value = "input_X_sql", None, None
 
     return mock_df
 
 
+def test_ml_arima_coefficients(
+    model_manipulation_sql_generator: ml_sql.ModelManipulationSqlGenerator,
+):
+    sql = model_manipulation_sql_generator.ml_arima_coefficients()
+    assert (
+        sql
+        == """SELECT * FROM ML.ARIMA_COEFFICIENTS(MODEL `my_project_id.my_dataset_id.my_model_id`)"""
+    )
+
+
 def test_options_correct(base_sql_generator: ml_sql.BaseSqlGenerator):
     sql = base_sql_generator.options(
         model_type="lin_reg", input_label_cols=["col_a"], l1_reg=0.6
     )
     assert (
         sql
         == """OPTIONS(
```

### Comparing `bigframes-1.4.0/tests/unit/resources.py` & `bigframes-1.5.0/tests/unit/resources.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/session/__init__.py` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/session/test_clients.py` & `bigframes-1.5.0/tests/unit/session/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/session/test_io_bigquery.py` & `bigframes-1.5.0/tests/unit/session/test_io_bigquery.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 from typing import Iterable
-import unittest.mock as mock
 
 import google.cloud.bigquery as bigquery
 import pytest
 
 import bigframes
 from bigframes.core import log_adapter
 import bigframes.pandas as bpd
@@ -133,42 +132,25 @@
     assert len(labels) == 64
     assert "dataframe-max" in labels.values()
     assert "dataframe-head" not in labels.values()
     assert "bigframes-api" in labels.keys()
     assert "source" in labels.keys()
 
 
-def test_create_snapshot_sql_doesnt_timetravel_anonymous_datasets():
-    table_ref = bigquery.TableReference.from_string(
-        "my-test-project._e8166e0cdb.anonbb92cd"
-    )
-
-    sql = bigframes.session._io.bigquery.create_snapshot_sql(
-        table_ref, datetime.datetime.now(datetime.timezone.utc)
-    )
-
-    # Anonymous query results tables don't support time travel.
-    assert "SYSTEM_TIME" not in sql
-
-    # Need fully-qualified table name.
-    assert "`my-test-project`.`_e8166e0cdb`.`anonbb92cd`" in sql
-
-
 def test_create_temp_table_default_expiration():
     """Make sure the created table has an expiration."""
-    bqclient = mock.create_autospec(bigquery.Client)
-    dataset = bigquery.DatasetReference("test-project", "test_dataset")
     expiration = datetime.datetime(
         2023, 11, 2, 13, 44, 55, 678901, datetime.timezone.utc
     )
 
-    bigframes.session._io.bigquery.create_temp_table(bqclient, dataset, expiration)
+    session = resources.create_bigquery_session()
+    bigframes.session._io.bigquery.create_temp_table(session, expiration)
 
-    bqclient.create_table.assert_called_once()
-    call_args = bqclient.create_table.call_args
+    session.bqclient.create_table.assert_called_once()
+    call_args = session.bqclient.create_table.call_args
     table = call_args.args[0]
     assert table.project == "test-project"
     assert table.dataset_id == "test_dataset"
     assert table.table_id.startswith("bqdf")
     assert (
         (expiration - datetime.timedelta(minutes=1))
         < table.expires
```

### Comparing `bigframes-1.4.0/tests/unit/session/test_io_pandas.py` & `bigframes-1.5.0/tests/unit/session/test_io_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_clients.py` & `bigframes-1.5.0/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_compute_options.py` & `bigframes-1.5.0/tests/unit/test_compute_options.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_core.py` & `bigframes-1.5.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_dataframe.py` & `bigframes-1.5.0/tests/unit/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_dtypes.py` & `bigframes-1.5.0/tests/unit/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_features.py` & `bigframes-1.5.0/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_formatting_helper.py` & `bigframes-1.5.0/tests/unit/test_formatting_helper.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_formatting_helpers.py` & `bigframes-1.5.0/tests/unit/test_formatting_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_pandas.py` & `bigframes-1.5.0/tests/unit/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/tests/unit/test_remote_function.py` & `bigframes-1.5.0/tests/unit/test_remote_function.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/cpython/LICENSE` & `bigframes-1.5.0/third_party/bigframes_vendored/cpython/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/cpython/_pprint.py` & `bigframes-1.5.0/third_party/bigframes_vendored/cpython/_pprint.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/__init__.py` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/__init__.py` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/__init__.py` & `bigframes-1.5.0/tests/system/small/bigquery/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py` & `bigframes-1.5.0/third_party/bigframes_vendored/google_cloud_bigquery/tests/unit/test_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/LICENSE.txt` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/README.md` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/compiler.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/datatypes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/backends/bigquery/registry.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/analytic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py` & `bigframes-1.5.0/third_party/bigframes_vendored/ibis/expr/operations/reductions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/AUTHORS.md` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/LICENSE` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/README.md` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/README.md`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/arrow/accessors.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/arrays/datetimelike.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/common.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/align.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/align.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/common.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/engines.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/engines.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/eval.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/eval.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/expr.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/expr.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/ops.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/ops.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/parsing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/computation/scope.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/computation/scope.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/config_init.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/config_init.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/dtypes/inference.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/frame.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             'bigframes-dev.birds.test-numbers'
 
         Write a DataFrame to a temporary BigQuery table in the anonymous dataset.
 
             >>> df = bpd.DataFrame({'col1': [1, 2], 'col2': [3, 4]})
             >>> destination = df.to_gbq(ordering_id="ordering_id")
             >>> # The table created can be read outside of the current session.
-            >>> bpd.close_session()  # For demonstration, only.
+            >>> bpd.close_session()  # Optional, to demonstrate a new session.
             >>> bpd.read_gbq(destination, index_col="ordering_id")
                          col1  col2
             ordering_id
             0               1     3
             1               2     4
             <BLANKLINE>
             [2 rows x 2 columns]
```

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/generic.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/generic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/groupby/__init__.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/accessor.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/base.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexes/multi.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/indexing.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/indexing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/concat.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/encoding.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/merge.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/reshape/tile.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/series.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/series.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/strings/accessor.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/tools/datetimes.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/core/window/rolling.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/common.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/common.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/gbq.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/gbq.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,46 +2,54 @@
 """ Google BigQuery support """
 
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, Literal, Optional, Tuple, Union
 
 from bigframes import constants
+import bigframes.enums
 
 FilterOps = Literal["in", "not in", "<", "<=", "==", "!=", ">=", ">", "LIKE"]
 FilterType = Tuple[str, FilterOps, Any]
 FiltersType = Union[Iterable[FilterType], Iterable[Iterable[FilterType]]]
 
 
 class GBQIOMixin:
     def read_gbq(
         self,
         query_or_table: str,
         *,
-        index_col: Iterable[str] | str = (),
+        index_col: Union[Iterable[str], str, bigframes.enums.DefaultIndexKind] = (),
         columns: Iterable[str] = (),
         configuration: Optional[Dict] = None,
         max_results: Optional[int] = None,
         filters: FiltersType = (),
         use_cache: Optional[bool] = None,
         col_order: Iterable[str] = (),
     ):
         """Loads a DataFrame from BigQuery.
 
         BigQuery tables are an unordered, unindexed data source. To add support
-        pandas-compatibility, the following indexing options are supported:
+        pandas-compatibility, the following indexing options are supported via
+        the ``index_col`` parameter:
 
-        * (Default behavior) Add an arbitrary sequential index and ordering
-          using an an analytic windowed operation that prevents filtering
-          push down.
+        * (Empty iterable, default) A default index. **Behavior may change.**
+          Explicitly set ``index_col`` if your application makes use of
+          specific index values.
+
+          If a table has primary key(s), those are used as the index,
+          otherwise a sequential index is generated.
+        * (:attr:`bigframes.enums.DefaultIndexKind.SEQUENTIAL_INT64`) Add an
+          arbitrary sequential index and ordering. **Warning** This uses an
+          analytic windowed operation that prevents filtering push down. Avoid
+          using on large clustered or partitioned tables.
         * (Recommended) Set the ``index_col`` argument to one or more columns.
           Unique values for the row labels are recommended. Duplicate labels
           are possible, but note that joins on a non-unique index can duplicate
-          rows and operations like ``cumsum()`` that window across a non-unique
-          index can have some non-deternimism.
+          rows via pandas-like outer join behavior.
 
         .. note::
             By default, even SQL query inputs with an ORDER BY clause create a
             DataFrame with an arbitrary ordering. Use ``row_number() OVER
             (ORDER BY ...) AS rowindex`` in your SQL query and set
             ``index_col='rowindex'`` to preserve the desired ordering.
 
@@ -103,19 +111,26 @@
         Args:
             query_or_table (str):
                 A SQL string to be executed or a BigQuery table to be read. The
                 table must be specified in the format of
                 `project.dataset.tablename` or `dataset.tablename`.
                 Can also take wildcard table name, such as `project.dataset.table_prefix*`.
                 In tha case, will read all the matched table as one DataFrame.
-            index_col (Iterable[str] or str):
+            index_col (Iterable[str], str, bigframes.enums.DefaultIndexKind):
                 Name of result column(s) to use for index in results DataFrame.
 
+                If an empty iterable, such as ``()``, a default index is
+                generated. Do not depend on specific index values in this case.
+
                 **New in bigframes version 1.3.0**: If ``index_cols`` is not
                 set, the primary key(s) of the table are used as the index.
+
+                **New in bigframes version 1.4.0**: Support
+                :class:`bigframes.enums.DefaultIndexKind` to override default index
+                behavior.
             columns (Iterable[str]):
                 List of BigQuery column names in the desired order for results
                 DataFrame.
             configuration (dict, optional):
                 Query config parameters for job processing.
                 For example: configuration = {'query': {'useQueryCache': False}}.
                 For more information see `BigQuery REST API Reference
@@ -137,11 +152,16 @@
             use_cache (Optional[bool], default None):
                 Caches query results if set to `True`. When `None`, it behaves
                 as `True`, but should not be combined with `useQueryCache` in
                 `configuration` to avoid conflicts.
             col_order (Iterable[str]):
                 Alias for columns, retained for backwards compatibility.
 
+        Raises:
+            bigframes.exceptions.DefaultIndexWarning:
+                Using the default index is discouraged, such as with clustered
+                or partitioned tables without primary keys.
+
         Returns:
             bigframes.dataframe.DataFrame: A DataFrame representing results of the query or table.
         """
         raise NotImplementedError(constants.ABSTRACT_METHOD_ERROR_MESSAGE)
```

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parquet.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parquet.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/parsers/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,35 @@
     Tuple,
     Union,
 )
 
 import numpy as np
 
 from bigframes import constants
+import bigframes.enums
 
 
 class ReaderIOMixin:
     def read_csv(
         self,
         filepath_or_buffer: str,
         *,
         sep: Optional[str] = ",",
         header: Optional[int] = 0,
         names: Optional[
             Union[MutableSequence[Any], np.ndarray[Any, Any], Tuple[Any, ...], range]
         ] = None,
         index_col: Optional[
-            Union[int, str, Sequence[Union[str, int]], Literal[False]]
+            Union[
+                int,
+                str,
+                Sequence[Union[str, int]],
+                bigframes.enums.DefaultIndexKind,
+                Literal[False],
+            ]
         ] = None,
         usecols=None,
         dtype: Optional[Dict] = None,
         engine: Optional[
             Literal["c", "python", "pyarrow", "python-fwf", "bigquery"]
         ] = None,
         encoding: Optional[str] = None,
```

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/io/pickle.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/io/pickle.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/pandas/_typing.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/pandas/_typing.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/plotting/_core.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/plotting/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         This function groups the values of all given Series in the DataFrame
         into bins and draws all bins in one :class:`matplotlib.axes.Axes`.
         This is useful when the DataFrame's Series are in a similar scale.
 
         **Examples:**
 
             >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
             >>> import numpy as np
             >>> bpd.options.display.progress_bar = None
             >>> df = bpd.DataFrame(np.random.randint(1, 7, 6000), columns=['one'])
             >>> df['two'] = np.random.randint(1, 7, 6000) + np.random.randint(1, 7, 6000)
             >>> ax = df.plot.hist(bins=12, alpha=0.5)
 
         Args:
@@ -231,14 +232,15 @@
 
         **Examples:**
 
         Let's see how to draw a scatter plot using coordinates from the values
         in a DataFrame's columns.
 
             >>> import bigframes.pandas as bpd
+            >>> bpd.options.display.progress_bar = None
             >>> df = bpd.DataFrame([[5.1, 3.5, 0], [4.9, 3.0, 0], [7.0, 3.2, 1],
             ...                    [6.4, 3.2, 1], [5.9, 3.0, 2]],
             ...                   columns=['length', 'width', 'species'])
             >>> ax1 = df.plot.scatter(x='length',
             ...                       y='width',
             ...                       c='DarkBlue')
```

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_exceptions.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/util/_exceptions.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/pandas/util/_validators.py` & `bigframes-1.5.0/third_party/bigframes_vendored/pandas/util/_validators.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/COPYING` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/COPYING`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/base.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/compose/_column_transformer.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/ensemble/_forest.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/linear_model/_base.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/linear_model/_logistic.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_ranking.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/metrics/pairwise.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/pipeline.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_data.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_discretization.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_encoder.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py` & `bigframes-1.5.0/third_party/bigframes_vendored/sklearn/preprocessing/_label.py`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/xgboost/LICENSE` & `bigframes-1.5.0/third_party/bigframes_vendored/xgboost/LICENSE`

 * *Files identical despite different names*

### Comparing `bigframes-1.4.0/third_party/bigframes_vendored/xgboost/sklearn.py` & `bigframes-1.5.0/third_party/bigframes_vendored/xgboost/sklearn.py`

 * *Files identical despite different names*

