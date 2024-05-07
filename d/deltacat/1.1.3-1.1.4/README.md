# Comparing `tmp/deltacat-1.1.3.tar.gz` & `tmp/deltacat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deltacat-1.1.3.tar", last modified: Tue Apr 30 02:54:02 2024, max compression
+gzip compressed data, was "dist/deltacat-1.1.4.tar", last modified: Tue May  7 00:10:23 2024, max compression
```

## Comparing `deltacat-1.1.3.tar` & `deltacat-1.1.4.tar`

### file list

```diff
@@ -1,268 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 02:42:11.000000 deltacat-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-30 02:54:02.000000 deltacat-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 02:42:11.000000 deltacat-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/aws/redshift/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/aws/s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/benchmark_parquet_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/benchmarking/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/default_catalog_impl/
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/default_catalog_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/catalog/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compaction_session_audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/compactor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/dedupe_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/repartition_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/model/table_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/repartition_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/steps/repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_file_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/steps/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/content_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/compactor_v2/utils/task_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/daft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/model/merge_on_read_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/merge_on_read/utils/delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/compute/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/io/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/io/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/storage/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/delete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/table_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/storage/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/aws/test_clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/catalog/test_default_catalog_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compact_partition_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/steps/test_repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor/utils/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_hashlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/compute/test_util_create_table_deltas_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_cloudpickle_bug_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/io/test_s3_object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/local_deltacat_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/local_deltacat_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/stats/test_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/test_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/tests/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_record_batch_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/tests/utils/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/partial_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/types/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat/utils/ray_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/ray_utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 02:42:11.000000 deltacat-1.1.3/deltacat/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-30 02:54:02.000000 deltacat-1.1.3/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 02:54:01.000000 deltacat-1.1.3/deltacat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:54:02.000000 deltacat-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-30 02:42:11.000000 deltacat-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 23:58:02.000000 deltacat-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 00:10:23.000000 deltacat-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-06 23:58:02.000000 deltacat-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/benchmark_parquet_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/default_catalog_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/default_catalog_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compaction_session_audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compactor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/dedupe_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/repartition_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/table_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/repartition_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25193 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_file_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/content_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/task_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/daft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/merge_on_read_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/delete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/test_s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/catalog/test_default_catalog_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compact_partition_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/test_repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_hashlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_create_table_deltas_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_cloudpickle_bug_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_s3_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/local_deltacat_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/local_deltacat_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/stats/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_record_batch_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/partial_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:10:23.000000 deltacat-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-06 23:58:02.000000 deltacat-1.1.4/setup.py
```

### Comparing `deltacat-1.1.3/PKG-INFO` & `deltacat-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.3
+Version: 1.1.4
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.3/README.md` & `deltacat-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/__init__.py` & `deltacat-1.1.4/deltacat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     SortOrder,
 )
 from deltacat.types.media import ContentEncoding, ContentType, TableType
 from deltacat.types.tables import TableWriteMode
 
 deltacat.logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-1.1.3/deltacat/aws/clients.py` & `deltacat-1.1.4/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/aws/redshift/model/manifest.py` & `deltacat-1.1.4/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/aws/s3u.py` & `deltacat-1.1.4/deltacat/aws/s3u.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     wait_random_exponential,
 )
 from deltacat.utils.ray_utils.concurrency import invoke_parallel
 import deltacat.aws.clients as aws_utils
 from deltacat import logs
 from deltacat.aws.constants import (
     TIMEOUT_ERROR_CODES,
-    DOWNLOAD_MANIFEST_ENTRY_METRIC_PREFIX,
-    UPLOAD_SLICED_TABLE_METRIC_PREFIX,
 )
 from deltacat.exceptions import NonRetryableError, RetryableError
 from deltacat.storage import (
     DistributedDataset,
     LocalDataset,
     LocalTable,
     Manifest,
@@ -50,15 +48,14 @@
     TABLE_TYPE_TO_READER_FUNC,
     TABLE_TYPE_TO_DATASET_CREATE_FUNC_REFS,
     DISTRIBUTED_DATASET_TYPE_TO_READER_FUNC,
     get_table_length,
 )
 from deltacat.types.partial_download import PartialFileDownloadParams
 from deltacat.utils.common import ReadKwargsProvider
-from deltacat.utils.metrics import metrics
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 # TODO(raghumdani): refactor redshift datasource to reuse the
 # same module for writing output files.
 
 
@@ -117,14 +114,40 @@
     ) -> str:
         write_path = f"{base_path}/{str(uuid4())}"
         self.write_paths.append(write_path)
         if block:
             self.block_refs.append(block)
         return write_path
 
+    def __call__(
+        self,
+        base_path: str,
+        *,
+        filesystem: Optional[pa.filesystem.FileSystem] = None,
+        dataset_uuid: Optional[str] = None,
+        block: Optional[ObjectRef[Block]] = None,
+        block_index: Optional[int] = None,
+        file_format: Optional[str] = None,
+    ) -> str:
+        """
+        TODO: BlockWritePathProvider is deprecated as of Ray version 2.20.0. Please use FilenameProvider.
+        See: https://docs.ray.io/en/master/data/api/doc/ray.data.datasource.FilenameProvider.html
+        Also See: https://github.com/ray-project/deltacat/issues/299
+
+        Hence, this class only works with Ray version 2.20.0 or lower when used in Ray Dataset.
+        """
+        return self._get_write_path_for_block(
+            base_path,
+            filesystem=filesystem,
+            dataset_uuid=dataset_uuid,
+            block=block,
+            block_index=block_index,
+            file_format=file_format,
+        )
+
 
 class S3Url:
     def __init__(self, url: str):
 
         from urllib.parse import urlparse
 
         self._parsed = urlparse(url, allow_fragments=False)  # support '#' in path
@@ -239,15 +262,14 @@
             f"Read has failed for {s3_url} and content_type={content_type} "
             f"and encoding={content_encoding}. Error: {e}",
             exc_info=True,
         )
         raise e
 
 
-@metrics(prefix=UPLOAD_SLICED_TABLE_METRIC_PREFIX)
 def upload_sliced_table(
     table: Union[LocalTable, DistributedDataset],
     s3_url_prefix: str,
     s3_file_system: s3fs.S3FileSystem,
     max_records_per_entry: Optional[int],
     s3_table_writer_func: Callable,
     table_slicer_func: Callable,
@@ -348,15 +370,14 @@
                 f"Upload has failed for {s3_url} and content_type={content_type}. Error: {e}",
                 exc_info=True,
             )
             raise e
     return manifest_entries
 
 
-@metrics(prefix=DOWNLOAD_MANIFEST_ENTRY_METRIC_PREFIX)
 def download_manifest_entry(
     manifest_entry: ManifestEntry,
     token_holder: Optional[Dict[str, Any]] = None,
     table_type: TableType = TableType.PYARROW,
     column_names: Optional[List[str]] = None,
     include_columns: Optional[List[str]] = None,
     file_reader_kwargs_provider: Optional[ReadKwargsProvider] = None,
```

### Comparing `deltacat-1.1.3/deltacat/benchmarking/benchmark_parquet_reads.py` & `deltacat-1.1.4/deltacat/benchmarking/benchmark_parquet_reads.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/benchmarking/conftest.py` & `deltacat-1.1.4/deltacat/benchmarking/conftest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/catalog/default_catalog_impl/__init__.py` & `deltacat-1.1.4/deltacat/catalog/default_catalog_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/catalog/delegate.py` & `deltacat-1.1.4/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/catalog/interface.py` & `deltacat-1.1.4/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/catalog/model/catalog.py` & `deltacat-1.1.4/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/catalog/model/table_definition.py` & `deltacat-1.1.4/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/__init__.py` & `deltacat-1.1.4/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/compaction_session.py` & `deltacat-1.1.4/deltacat/compute/compactor/compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/compact_partition_params.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/compaction_session_audit_info.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/compaction_session_audit_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/model/table_object_store.py` & `deltacat-1.1.4/deltacat/compute/compactor/model/table_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/repartition_session.py` & `deltacat-1.1.4/deltacat/compute/compactor/repartition_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/steps/dedupe.py` & `deltacat-1.1.4/deltacat/compute/compactor/steps/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-1.1.4/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/steps/materialize.py` & `deltacat-1.1.4/deltacat/compute/compactor/steps/materialize.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/steps/repartition.py` & `deltacat-1.1.4/deltacat/compute/compactor/steps/repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/utils/io.py` & `deltacat-1.1.4/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-1.1.4/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-1.1.4/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import logging
 from typing import Dict, Any
 from deltacat import logs
 from deltacat.compute.compactor import RoundCompletionInfo
 from deltacat.storage import PartitionLocator
 from deltacat.aws import s3u as s3_utils
 from typing import Optional
+from deltacat.utils.metrics import metrics
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 def get_round_completion_file_s3_url(
     bucket: str, source_partition_locator: PartitionLocator
 ) -> str:
 
     base_url = source_partition_locator.path(f"s3://{bucket}")
     return f"{base_url}.json"
 
 
+@metrics
 def read_round_completion_file(
     bucket: str,
     source_partition_locator: PartitionLocator,
     **s3_client_kwargs: Optional[Dict[str, Any]],
 ) -> RoundCompletionInfo:
 
     round_completion_file_url = get_round_completion_file_s3_url(
@@ -34,14 +36,15 @@
     if result:
         json_str = result["Body"].read().decode("utf-8")
         round_completion_info = RoundCompletionInfo(json.loads(json_str))
         logger.info(f"read round completion info: {round_completion_info}")
     return round_completion_info
 
 
+@metrics
 def write_round_completion_file(
     bucket: Optional[str],
     source_partition_locator: Optional[PartitionLocator],
     round_completion_info: RoundCompletionInfo,
     completion_file_s3_url: str = None,
     **s3_client_kwargs: Optional[Dict[str, Any]],
 ) -> str:
```

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/utils/sort_key.py` & `deltacat-1.1.4/deltacat/compute/compactor/utils/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-1.1.4/deltacat/compute/compactor/utils/system_columns.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/compaction_session.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/compaction_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     invoke_parallel,
     task_resource_options_provider,
 )
 from deltacat.compute.compactor_v2.steps import merge as mg
 from deltacat.compute.compactor_v2.steps import hash_bucket as hb
 from deltacat.compute.compactor_v2.utils import io
 from deltacat.compute.compactor.utils import round_completion_file as rcf
+from deltacat.utils.metrics import metrics
 
 from typing import List, Optional, Tuple
 from collections import defaultdict
 from deltacat.compute.compactor.model.compaction_session_audit_info import (
     CompactionSessionAuditInfo,
 )
 from deltacat.utils.resources import (
@@ -69,14 +70,15 @@
 if importlib.util.find_spec("memray"):
     import memray
 
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
+@metrics
 def compact_partition(params: CompactPartitionParams, **kwargs) -> Optional[str]:
 
     assert (
         params.hash_bucket_count is not None and params.hash_bucket_count >= 1
     ), "hash_bucket_count is a required arg for compactor v2"
 
     with memray.Tracker(
```

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/constants.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,10 +61,7 @@
 MERGE_FAILURE_COUNT = "merge_failure_count"
 
 # Metric prefix for discover deltas
 DISCOVER_DELTAS_METRIC_PREFIX = "discover_deltas"
 
 # Metric prefix for prepare deletes
 PREPARE_DELETES_METRIC_PREFIX = "prepare_deletes"
-
-# Metric prefix for materialize
-MATERIALIZE_METRIC_PREFIX = "delta_materialize"
```

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/model.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/model.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/deletes/utils.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/model/hash_bucket_input.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_file_group.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_file_group.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/model/merge_input.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/steps/hash_bucket.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/steps/merge.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/steps/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/content_type_params.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/content_type_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/dedupe.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/delta.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/io.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/merge.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,22 +27,19 @@
 )
 from deltacat.compute.compactor_v2.deletes.delete_strategy import (
     DeleteStrategy,
 )
 from deltacat.compute.compactor_v2.deletes.delete_file_envelope import (
     DeleteFileEnvelope,
 )
-from deltacat.utils.metrics import metrics
-from deltacat.compute.compactor_v2.constants import MATERIALIZE_METRIC_PREFIX
 
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
-@metrics(prefix=MATERIALIZE_METRIC_PREFIX)
 def materialize(
     input: MergeInput,
     task_index: int,
     compacted_tables: List[pa.Table],
 ) -> MaterializeResult:
     compacted_table = pa.concat_tables(compacted_tables)
     if input.compacted_file_content_type in DELIMITED_TEXT_CONTENT_TYPES:
```

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/primary_key_index.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/compactor_v2/utils/task_options.py` & `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/merge_on_read/daft.py` & `deltacat-1.1.4/deltacat/compute/merge_on_read/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/merge_on_read/model/merge_on_read_params.py` & `deltacat-1.1.4/deltacat/compute/merge_on_read/model/merge_on_read_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/merge_on_read/utils/delta.py` & `deltacat-1.1.4/deltacat/compute/merge_on_read/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/meta_stats.py` & `deltacat-1.1.4/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-1.1.4/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-1.1.4/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/stats.py` & `deltacat-1.1.4/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/utils/constants.py` & `deltacat-1.1.4/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/utils/io.py` & `deltacat-1.1.4/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-1.1.4/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-1.1.4/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/basic.py` & `deltacat-1.1.4/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-1.1.4/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/models/delta_stats.py` & `deltacat-1.1.4/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-1.1.4/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-1.1.4/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/models/stats_result.py` & `deltacat-1.1.4/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/utils/intervals.py` & `deltacat-1.1.4/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/utils/io.py` & `deltacat-1.1.4/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-1.1.4/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/constants.py` & `deltacat-1.1.4/deltacat/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-1.1.4/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/dataset.py` & `deltacat-1.1.4/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/file_object_store.py` & `deltacat-1.1.4/deltacat/io/file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/memcached_object_store.py` & `deltacat-1.1.4/deltacat/io/memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/object_store.py` & `deltacat-1.1.4/deltacat/io/object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/ray_plasma_object_store.py` & `deltacat-1.1.4/deltacat/io/ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/read_api.py` & `deltacat-1.1.4/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/redis_object_store.py` & `deltacat-1.1.4/deltacat/io/redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/io/s3_object_store.py` & `deltacat-1.1.4/deltacat/io/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/logs.py` & `deltacat-1.1.4/deltacat/logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import json
 import pathlib
 from logging import FileHandler, Handler, Logger, LoggerAdapter, handlers
 from typing import Any, Dict, Optional, Union
 
 import ray
 from ray.runtime_context import RuntimeContext
 
@@ -15,21 +16,114 @@
     DELTACAT_APP_INFO_LOG_BASE_FILE_NAME,
     DELTACAT_SYS_INFO_LOG_BASE_FILE_NAME,
     DELTACAT_APP_DEBUG_LOG_BASE_FILE_NAME,
     DELTACAT_SYS_DEBUG_LOG_BASE_FILE_NAME,
 )
 
 DEFAULT_LOG_LEVEL = "INFO"
-DEFAULT_LOG_FORMAT = (
-    "%(asctime)s\t%(levelname)s pid=%(process)d %(filename)s:%(lineno)s -- %(message)s"
-)
+DEFAULT_LOG_FORMAT = {
+    "level": "levelname",
+    "message": "message",
+    "loggerName": "name",
+    "processName": "processName",
+    "processID": "process",
+    "threadName": "threadName",
+    "timestamp": "asctime",
+    "filename": "filename",
+    "lineno": "lineno",
+}
 DEFAULT_MAX_BYTES_PER_LOG = 2 ^ 20 * 256  # 256 MiB
 DEFAULT_BACKUP_COUNT = 0
 
 
+class JsonFormatter(logging.Formatter):
+    """
+    Formatter that outputs JSON strings after parsing the LogRecord.
+
+    @param dict fmt_dict: Key: logging format attribute pairs. Defaults to {"message": "message"}.
+    @param str time_format: time.strftime() format string. Default: "%Y-%m-%dT%H:%M:%S"
+    @param str msec_format: Microsecond formatting. Appended at the end. Default: "%s.%03dZ"
+    """
+
+    def __init__(
+        self,
+        fmt_dict: dict = None,
+        time_format: str = "%Y-%m-%dT%H:%M:%S",
+        msec_format: str = "%s.%03dZ",
+    ):
+        self.fmt_dict = fmt_dict if fmt_dict is not None else {"message": "message"}
+        self.default_time_format = time_format
+        self.default_msec_format = msec_format
+        self.datefmt = None
+        if ray.is_initialized():
+            self.ray_runtime_ctx: RuntimeContext = ray.get_runtime_context()
+            self.context = {}
+            self.context["worker_id"] = self.ray_runtime_ctx.get_worker_id()
+            self.context["node_id"] = self.ray_runtime_ctx.get_node_id()
+            self.context["job_id"] = self.ray_runtime_ctx.get_job_id()
+        else:
+            self.ray_runtime_ctx = None
+            self.context = {}
+
+    def usesTime(self) -> bool:
+        """
+        Overwritten to look for the attribute in the format dict values instead of the fmt string.
+        """
+        return "asctime" in self.fmt_dict.values()
+
+    def formatMessage(self, record) -> dict:
+        """
+        Overwritten to return a dictionary of the relevant LogRecord attributes instead of a string.
+        KeyError is raised if an unknown attribute is provided in the fmt_dict.
+        """
+        return {
+            fmt_key: record.__dict__[fmt_val]
+            for fmt_key, fmt_val in self.fmt_dict.items()
+        }
+
+    def format(self, record) -> str:
+        """
+        Mostly the same as the parent's class method, the difference being that a dict is manipulated and dumped as JSON
+        instead of a string.
+        """
+        record.message = record.getMessage()
+
+        if self.usesTime():
+            record.asctime = self.formatTime(record, self.datefmt)
+
+        message_dict = self.formatMessage(record)
+
+        if record.exc_info:
+            # Cache the traceback text to avoid converting it multiple times
+            # (it's constant anyway)
+            if not record.exc_text:
+                record.exc_text = self.formatException(record.exc_info)
+
+        if record.exc_text:
+            message_dict["exc_info"] = record.exc_text
+
+        if record.stack_info:
+            message_dict["stack_info"] = self.formatStack(record.stack_info)
+
+        if self.ray_runtime_ctx:
+            # only workers will have task ID
+            if (
+                self.ray_runtime_ctx.worker
+                and self.ray_runtime_ctx.worker.mode == ray._private.worker.WORKER_MODE
+            ):
+                self.context["task_id"] = self.ray_runtime_ctx.get_task_id()
+                self.context[
+                    "assigned_resources"
+                ] = self.ray_runtime_ctx.get_assigned_resources()
+
+            message_dict["ray_runtime_context"] = self.context
+
+        return json.dumps(message_dict, default=str)
+
+
 class DeltaCATLoggerAdapter(logging.LoggerAdapter):
     """
     Logger Adapter class with additional functionality
     """
 
     def __init__(self, logger: Logger, extra: Optional[Dict[str, Any]] = {}):
         super().__init__(logger, extra)
@@ -47,152 +141,115 @@
             self.warning(msg, *args, **kwargs)
 
     def error_conditional(self, msg, do_print: bool, *args, **kwargs):
         if do_print:
             self.error(msg, *args, **kwargs)
 
 
-class RayRuntimeContextLoggerAdapter(DeltaCATLoggerAdapter):
-    """
-    Logger Adapter for injecting Ray Runtime Context into logging messages.
-    """
-
-    def __init__(self, logger: Logger, runtime_context: RuntimeContext):
-        super().__init__(logger, {})
-        self.runtime_context = runtime_context
-
-    def process(self, msg, kwargs):
-        """
-        Injects Ray Runtime Context details into each log message.
-
-        This may include information such as the raylet node ID, task/actor ID, job ID,
-        placement group ID of the worker, and assigned resources to the task/actor.
-
-        Args:
-            msg: The original log message
-            kwargs: Keyword arguments for the log message
-
-        Returns: A log message with Ray Runtime Context details
-
-        """
-        runtime_context_dict = self.runtime_context.get()
-        runtime_context_dict[
-            "worker_id"
-        ] = self.runtime_context.worker.core_worker.get_worker_id()
-        if self.runtime_context.get_task_id() or self.runtime_context.get_actor_id():
-            runtime_context_dict[
-                "pg_id"
-            ] = self.runtime_context.get_placement_group_id()
-            runtime_context_dict[
-                "assigned_resources"
-            ] = self.runtime_context.get_assigned_resources()
-
-        return "(ray_runtime_context=%s) -- %s" % (runtime_context_dict, msg), kwargs
-
-    def __reduce__(self):
-        """
-        Used to unpickle the class during Ray object store transfer.
-        """
-
-        def deserializer(*args):
-            return RayRuntimeContextLoggerAdapter(args[0], ray.get_runtime_context())
-
-        return deserializer, (self.logger,)
-
-
 def _add_logger_handler(logger: Logger, handler: Handler) -> Logger:
 
     logger.setLevel(logging.getLevelName("DEBUG"))
     logger.addHandler(handler)
     return logger
 
 
 def _create_rotating_file_handler(
     log_directory: str,
     log_base_file_name: str,
-    logging_level: str = DEFAULT_LOG_LEVEL,
+    logging_level: Union[str, int] = DEFAULT_LOG_LEVEL,
     max_bytes_per_log_file: int = DEFAULT_MAX_BYTES_PER_LOG,
     backup_count: int = DEFAULT_BACKUP_COUNT,
-    logging_format: str = DEFAULT_LOG_FORMAT,
+    logging_format: Union[str, dict] = DEFAULT_LOG_FORMAT,
 ) -> FileHandler:
 
     if type(logging_level) is str:
         logging_level = logging.getLevelName(logging_level.upper())
     assert log_base_file_name, "log file name is required"
     assert log_directory, "log directory is required"
     log_dir_path = pathlib.Path(log_directory)
     log_dir_path.mkdir(parents=True, exist_ok=True)
     handler = handlers.RotatingFileHandler(
         os.path.join(log_directory, log_base_file_name),
         maxBytes=max_bytes_per_log_file,
         backupCount=backup_count,
     )
-    handler.setFormatter(logging.Formatter(logging_format))
+
+    if type(logging_format) is str:
+        handler.setFormatter(logging.Formatter(logging_format))
+    else:
+        handler.setFormatter(JsonFormatter(logging_format))
+
     handler.setLevel(logging_level)
     return handler
 
 
 def _file_handler_exists(logger: Logger, log_dir: str, log_base_file_name: str) -> bool:
 
     handler_exists = False
     base_file_path = os.path.join(log_dir, log_base_file_name)
-    if len(logger.handlers) > 0:
+
+    if logger.handlers:
         norm_base_file_path = os.path.normpath(base_file_path)
         handler_exists = any(
             [
                 isinstance(handler, logging.FileHandler)
                 and os.path.normpath(handler.baseFilename) == norm_base_file_path
                 for handler in logger.handlers
             ]
         )
     return handler_exists
 
 
 def _configure_logger(
     logger: Logger,
-    log_level: str,
+    log_level: int,
     log_dir: str,
     log_base_file_name: str,
     debug_log_base_file_name: str,
 ) -> Union[Logger, LoggerAdapter]:
+    # This maintains log level of rotating file handlers
     primary_log_level = log_level
     logger.propagate = False
-    if log_level.upper() == "DEBUG":
+    if log_level <= logging.getLevelName("DEBUG"):
         if not _file_handler_exists(logger, log_dir, debug_log_base_file_name):
             handler = _create_rotating_file_handler(
                 log_dir, debug_log_base_file_name, "DEBUG"
             )
             _add_logger_handler(logger, handler)
-            primary_log_level = "INFO"
+            primary_log_level = logging.getLevelName("INFO")
     if not _file_handler_exists(logger, log_dir, log_base_file_name):
         handler = _create_rotating_file_handler(
             log_dir, log_base_file_name, primary_log_level
         )
         _add_logger_handler(logger, handler)
-    if ray.is_initialized():
-        ray_runtime_ctx = ray.get_runtime_context()
-        if ray_runtime_ctx.worker.connected:
-            logger = RayRuntimeContextLoggerAdapter(logger, ray_runtime_ctx)
-    else:
-        logger = DeltaCATLoggerAdapter(logger)
 
-    return logger
+    return DeltaCATLoggerAdapter(logger)
+
 
+def configure_deltacat_logger(
+    logger: Logger, level: int = None
+) -> Union[Logger, LoggerAdapter]:
+    if level is None:
+        level = logging.getLevelName(DELTACAT_SYS_LOG_LEVEL)
 
-def configure_deltacat_logger(logger: Logger) -> Union[Logger, LoggerAdapter]:
     return _configure_logger(
         logger,
-        DELTACAT_SYS_LOG_LEVEL,
+        level,
         DELTACAT_SYS_LOG_DIR,
         DELTACAT_SYS_INFO_LOG_BASE_FILE_NAME,
         DELTACAT_SYS_DEBUG_LOG_BASE_FILE_NAME,
     )
 
 
-def configure_application_logger(logger: Logger) -> Union[Logger, LoggerAdapter]:
+def configure_application_logger(
+    logger: Logger, level: int = None
+) -> Union[Logger, LoggerAdapter]:
+    if level is None:
+        level = logging.getLevelName(DELTACAT_APP_LOG_LEVEL)
+
     return _configure_logger(
         logger,
-        DELTACAT_APP_LOG_LEVEL,
+        level,
         DELTACAT_APP_LOG_DIR,
         DELTACAT_APP_INFO_LOG_BASE_FILE_NAME,
         DELTACAT_APP_DEBUG_LOG_BASE_FILE_NAME,
     )
```

### Comparing `deltacat-1.1.3/deltacat/storage/__init__.py` & `deltacat-1.1.4/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/interface.py` & `deltacat-1.1.4/deltacat/storage/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/delete_parameters.py` & `deltacat-1.1.4/deltacat/storage/model/delete_parameters.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/delta.py` & `deltacat-1.1.4/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/list_result.py` & `deltacat-1.1.4/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/locator.py` & `deltacat-1.1.4/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/namespace.py` & `deltacat-1.1.4/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/partition.py` & `deltacat-1.1.4/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/sort_key.py` & `deltacat-1.1.4/deltacat/storage/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/stream.py` & `deltacat-1.1.4/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/table.py` & `deltacat-1.1.4/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/table_version.py` & `deltacat-1.1.4/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/storage/model/types.py` & `deltacat-1.1.4/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/aws/test_clients.py` & `deltacat-1.1.4/deltacat/tests/aws/test_clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/catalog/test_default_catalog_impl.py` & `deltacat-1.1.4/deltacat/tests/catalog/test_default_catalog_impl.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py` & `deltacat-1.1.4/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compact_partition_test_cases.py` & `deltacat-1.1.4/deltacat/tests/compute/compact_partition_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compactor/steps/test_repartition.py` & `deltacat-1.1.4/deltacat/tests/compute/compactor/steps/test_repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compactor/utils/test_io.py` & `deltacat-1.1.4/deltacat/tests/compute/compactor/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compactor_v2/test_compaction_session.py` & `deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/compactor_v2/utils/test_task_options.py` & `deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/test_task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_incremental.py` & `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_params.py` & `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py` & `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_util_common.py` & `deltacat-1.1.4/deltacat/tests/compute/test_util_common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_util_constant.py` & `deltacat-1.1.4/deltacat/tests/compute/test_util_constant.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/compute/test_util_create_table_deltas_repo.py` & `deltacat-1.1.4/deltacat/tests/compute/test_util_create_table_deltas_repo.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_cloudpickle_bug_fix.py` & `deltacat-1.1.4/deltacat/tests/io/test_cloudpickle_bug_fix.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_file_object_store.py` & `deltacat-1.1.4/deltacat/tests/io/test_file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_memcached_object_store.py` & `deltacat-1.1.4/deltacat/tests/io/test_memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_ray_plasma_object_store.py` & `deltacat-1.1.4/deltacat/tests/io/test_ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_redis_object_store.py` & `deltacat-1.1.4/deltacat/tests/io/test_redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/io/test_s3_object_store.py` & `deltacat-1.1.4/deltacat/tests/io/test_s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/local_deltacat_storage/__init__.py` & `deltacat-1.1.4/deltacat/tests/local_deltacat_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/stats/test_intervals.py` & `deltacat-1.1.4/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/test_utils/pyarrow.py` & `deltacat-1.1.4/deltacat/tests/test_utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/test_utils/storage.py` & `deltacat-1.1.4/deltacat/tests/test_utils/storage.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_cloudpickle.py` & `deltacat-1.1.4/deltacat/tests/utils/test_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_daft.py` & `deltacat-1.1.4/deltacat/tests/utils/test_daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_metrics.py` & `deltacat-1.1.4/deltacat/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_pyarrow.py` & `deltacat-1.1.4/deltacat/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_record_batch_tables.py` & `deltacat-1.1.4/deltacat/tests/utils/test_record_batch_tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/tests/utils/test_resources.py` & `deltacat-1.1.4/deltacat/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/types/media.py` & `deltacat-1.1.4/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/types/partial_download.py` & `deltacat-1.1.4/deltacat/types/partial_download.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/types/tables.py` & `deltacat-1.1.4/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/arguments.py` & `deltacat-1.1.4/deltacat/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/cloudpickle.py` & `deltacat-1.1.4/deltacat/utils/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/common.py` & `deltacat-1.1.4/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/daft.py` & `deltacat-1.1.4/deltacat/utils/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/metrics.py` & `deltacat-1.1.4/deltacat/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/numpy.py` & `deltacat-1.1.4/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/pandas.py` & `deltacat-1.1.4/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/performance.py` & `deltacat-1.1.4/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/placement.py` & `deltacat-1.1.4/deltacat/utils/placement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import re
 import time
 from dataclasses import dataclass
+from packaging.version import Version
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import ray
 import yaml
 from ray.experimental.state.api import get_node, get_placement_group
 from ray.util.placement_group import placement_group, placement_group_table
 from ray.util.scheduling_strategies import PlacementGroupSchedulingStrategy
@@ -15,14 +16,24 @@
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 # Limitation of current node group or placement group manager
 # Must run on driver or head node bc state.api needs to query dashboard api server at 127.0.0.1.
 # Issue: https://github.com/ray-project/ray/issues/29959
 
 
+def _get_available_resources_per_node():
+    # This API changed after this commit
+    # https://github.com/ray-project/ray/pull/43252
+    # TODO: Use this method from a durable State API once it's available
+    if Version(ray.__version__) >= Version("2.10.0"):
+        return ray._private.state.available_resources_per_node()
+    else:
+        return ray._private.state.state._available_resources_per_node()
+
+
 @dataclass
 class PlacementGroupConfig:
     def __init__(self, opts, resource, node_ips):
         self.opts = opts
         self.resource = resource
         self.node_ips = node_ips
 
@@ -86,17 +97,15 @@
 
     def _parse_node_resources(self) -> Dict[str, Dict[str, float]]:
         """
         Parse resources per node to get detailed resource tighted to each node group
         Returns:
                 group_res: a dict of resources, e.g., {'CPU':0,'memory':0,'object_store_memory':0}
         """
-        all_available_resources = (
-            ray._private.state.state._available_resources_per_node()
-        )
+        all_available_resources = _get_available_resources_per_node()
         group_keys = [x[0] for x in self.init_groups]
         group_res = {}
         for k in group_keys:
             group_res[k] = {
                 "CPU": 0,
                 "memory": 0,
                 "object_store_memory": 0,
@@ -123,17 +132,15 @@
         """
         Get the realtime resource of a node group
         Args:
                 gname: name of node group
         Returns:
                 group_res: dict of updated resource(cpu, memory, object store memory) for a given group
         """
-        all_available_resources = (
-            ray._private.state.state._available_resources_per_node()
-        )
+        all_available_resources = _get_available_resources_per_node()
         group_res = {"CPU": 0, "memory": 0, "object_store_memory": 0, "node_id": []}
         for v in all_available_resources.values():
             keys = v.keys()
             r = re.compile("node:")
             node_id = list(filter(r.match, list(keys)))
             if len(node_id) > 0:
                 node_id = node_id[0]
@@ -281,15 +288,15 @@
     pg_id = placement_group_table(pg)["placement_group_id"]
     pg_details = get_placement_group(pg_id)
     bundles = pg_details["bundles"]
     node_ids = []
     for bd in bundles:
         node_ids.append(bd["node_id"])
     # query available resources given list of node id
-    all_nodes_available_res = ray._private.state.state._available_resources_per_node()
+    all_nodes_available_res = _get_available_resources_per_node()
     pg_res = {"CPU": 0, "memory": 0, "object_store_memory": 0}
     node_ips = []
     for node_id in node_ids:
         if node_id in all_nodes_available_res:
             v = all_nodes_available_res[node_id]
             node_detail = get_node(node_id)
             pg_res["CPU"] += node_detail["resources_total"]["CPU"]
```

### Comparing `deltacat-1.1.3/deltacat/utils/pyarrow.py` & `deltacat-1.1.4/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/ray_utils/collections.py` & `deltacat-1.1.4/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/ray_utils/concurrency.py` & `deltacat-1.1.4/deltacat/utils/ray_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/ray_utils/dataset.py` & `deltacat-1.1.4/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/ray_utils/runtime.py` & `deltacat-1.1.4/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/resources.py` & `deltacat-1.1.4/deltacat/utils/resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/s3fs.py` & `deltacat-1.1.4/deltacat/utils/s3fs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat/utils/schema.py` & `deltacat-1.1.4/deltacat/utils/schema.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.3/deltacat.egg-info/PKG-INFO` & `deltacat-1.1.4/deltacat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.3
+Version: 1.1.4
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.3/deltacat.egg-info/SOURCES.txt` & `deltacat-1.1.4/deltacat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,18 @@
 deltacat/storage/model/partition.py
 deltacat/storage/model/sort_key.py
 deltacat/storage/model/stream.py
 deltacat/storage/model/table.py
 deltacat/storage/model/table_version.py
 deltacat/storage/model/types.py
 deltacat/tests/__init__.py
+deltacat/tests/test_logs.py
 deltacat/tests/aws/__init__.py
 deltacat/tests/aws/test_clients.py
+deltacat/tests/aws/test_s3u.py
 deltacat/tests/catalog/__init__.py
 deltacat/tests/catalog/test_default_catalog_impl.py
 deltacat/tests/compute/__init__.py
 deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
 deltacat/tests/compute/compact_partition_test_cases.py
 deltacat/tests/compute/test_compact_partition_incremental.py
 deltacat/tests/compute/test_compact_partition_params.py
@@ -179,14 +181,15 @@
 deltacat/tests/test_utils/pyarrow.py
 deltacat/tests/test_utils/storage.py
 deltacat/tests/test_utils/utils.py
 deltacat/tests/utils/__init__.py
 deltacat/tests/utils/test_cloudpickle.py
 deltacat/tests/utils/test_daft.py
 deltacat/tests/utils/test_metrics.py
+deltacat/tests/utils/test_placement.py
 deltacat/tests/utils/test_pyarrow.py
 deltacat/tests/utils/test_record_batch_tables.py
 deltacat/tests/utils/test_resources.py
 deltacat/tests/utils/data/__init__.py
 deltacat/types/__init__.py
 deltacat/types/media.py
 deltacat/types/partial_download.py
```

### Comparing `deltacat-1.1.3/setup.py` & `deltacat-1.1.4/setup.py`

 * *Files identical despite different names*

