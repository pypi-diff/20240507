# Comparing `tmp/dbt_exasol-1.7.0.tar.gz` & `tmp/dbt_exasol-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_exasol-1.7.0.tar", max compression
+gzip compressed data, was "dbt_exasol-1.7.1.tar", max compression
```

## Comparing `dbt_exasol-1.7.0.tar` & `dbt_exasol-1.7.1.tar`

### file list

```diff
@@ -1,77 +1,80 @@
--rw-r--r--   0        0        0    35148 2023-11-26 03:06:29.271819 dbt_exasol-1.7.0/LICENSE
--rw-r--r--   0        0        0     3885 2024-03-16 01:22:55.149838 dbt_exasol-1.7.0/README.md
--rw-r--r--   0        0        0       65 2023-11-26 03:06:29.272133 dbt_exasol-1.7.0/dbt/__init__.py
--rw-r--r--   0        0        0       65 2023-11-26 03:06:29.272275 dbt_exasol-1.7.0/dbt/adapters/__init__.py
--rw-r--r--   0        0        0      508 2023-11-26 03:06:29.272415 dbt_exasol-1.7.0/dbt/adapters/exasol/__init__.py
--rw-r--r--   0        0        0       18 2023-11-26 03:06:29.272504 dbt_exasol-1.7.0/dbt/adapters/exasol/__version__.py
--rw-r--r--   0        0        0     3675 2023-11-26 03:06:29.272598 dbt_exasol-1.7.0/dbt/adapters/exasol/column.py
--rw-r--r--   0        0        0    11372 2023-11-26 03:06:29.272740 dbt_exasol-1.7.0/dbt/adapters/exasol/connections.py
--rw-r--r--   0        0        0     8338 2024-03-07 17:53:05.709798 dbt_exasol-1.7.0/dbt/adapters/exasol/impl.py
--rw-r--r--   0        0        0     1959 2023-11-26 03:06:29.272973 dbt_exasol-1.7.0/dbt/adapters/exasol/relation.py
--rw-r--r--   0        0        0       65 2023-11-26 03:06:29.273118 dbt_exasol-1.7.0/dbt/include/__init__.py
--rw-r--r--   0        0        0       52 2023-11-26 03:06:29.273246 dbt_exasol-1.7.0/dbt/include/exasol/__init__.py
--rw-r--r--   0        0        0      236 2023-11-26 03:06:29.273385 dbt_exasol-1.7.0/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0       74 2023-11-26 03:06:29.273464 dbt_exasol-1.7.0/dbt/include/exasol/dbt_project.yml
--rw-r--r--   0        0        0     8032 2023-11-26 03:06:29.273627 dbt_exasol-1.7.0/dbt/include/exasol/macros/adapters.sql
--rw-r--r--   0        0        0      673 2023-11-26 03:06:29.273716 dbt_exasol-1.7.0/dbt/include/exasol/macros/apply_grants.sql
--rw-r--r--   0        0        0     3796 2024-03-07 17:53:05.710695 dbt_exasol-1.7.0/dbt/include/exasol/macros/catalog.sql
--rw-r--r--   0        0        0     3493 2023-11-26 03:06:29.273978 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      259 2023-11-26 03:06:29.274073 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0     6113 2023-11-26 03:06:29.274187 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/merge.sql
--rw-r--r--   0        0        0      470 2023-11-26 03:06:29.274293 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/seed.sql
--rw-r--r--   0        0        0     8044 2023-11-26 03:06:29.274407 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/snapshot.sql
--rw-r--r--   0        0        0      748 2023-11-26 03:06:29.274503 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     3255 2023-11-26 03:06:29.274602 dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/strategies.sql
--rw-r--r--   0        0        0      178 2023-11-26 03:06:29.274739 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/any_value.sql
--rw-r--r--   0        0        0       85 2023-11-26 03:06:29.274819 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      469 2023-11-26 03:06:29.274912 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      441 2023-11-26 03:06:29.274994 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/datediff.sql
--rw-r--r--   0        0        0      130 2023-11-26 03:06:29.275203 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/hash.sql
--rw-r--r--   0        0        0      381 2023-11-26 03:06:29.275327 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/last_day.sql
--rw-r--r--   0        0        0      415 2023-11-26 03:06:29.275435 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/listagg.sql
--rw-r--r--   0        0        0      775 2023-11-26 03:06:29.275534 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      165 2023-11-26 03:06:29.275635 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/split_part.sql
--rw-r--r--   0        0        0      519 2023-11-26 03:06:29.275769 dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/timestamps.sql
--rw-r--r--   0        0        0      177 2023-11-26 03:06:29.275854 dbt_exasol-1.7.0/dbt/include/exasol/macros/validate_sql.sql
--rw-r--r--   0        0        0      374 2023-11-26 03:06:29.275938 dbt_exasol-1.7.0/dbt/include/exasol/profile_template.yml
--rw-r--r--   0        0        0     1030 2024-03-15 10:50:32.649784 dbt_exasol-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      606 2023-11-26 03:06:29.277201 dbt_exasol-1.7.0/tests/conftest.py
--rw-r--r--   0        0        0      640 2023-11-26 03:06:29.277442 dbt_exasol-1.7.0/tests/functional/adapter/aliases/test_aliases.py
--rw-r--r--   0        0        0     1252 2023-11-26 03:06:29.277581 dbt_exasol-1.7.0/tests/functional/adapter/concurrency/test_concurrency.py
--rw-r--r--   0        0        0     4827 2024-03-07 17:53:05.711214 dbt_exasol-1.7.0/tests/functional/adapter/constraints/fixtures.py
--rw-r--r--   0        0        0     9305 2023-11-26 03:06:29.277850 dbt_exasol-1.7.0/tests/functional/adapter/constraints/test_constraints.py
--rw-r--r--   0        0        0     3581 2023-11-26 03:06:29.277996 dbt_exasol-1.7.0/tests/functional/adapter/debug/test_dbt_debug.py
--rw-r--r--   0        0        0     1271 2023-11-26 03:06:29.278140 dbt_exasol-1.7.0/tests/functional/adapter/ephemeral/test_ephemeral.py
--rw-r--r--   0        0        0     7729 2023-11-26 03:06:29.278240 dbt_exasol-1.7.0/tests/functional/adapter/expected_catalog.py
--rw-r--r--   0        0        0     1438 2023-11-26 03:06:29.278343 dbt_exasol-1.7.0/tests/functional/adapter/files.py
--rw-r--r--   0        0        0      521 2023-11-26 03:06:29.278435 dbt_exasol-1.7.0/tests/functional/adapter/fixtures.py
--rw-r--r--   0        0        0     1080 2023-11-26 03:06:29.278569 dbt_exasol-1.7.0/tests/functional/adapter/grants/test_grants.py
--rw-r--r--   0        0        0      180 2023-11-26 03:06:29.278716 dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0        0        0      193 2023-11-26 03:06:29.278807 dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0        0        0     1082 2023-11-26 03:06:29.278900 dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0        0        0      972 2023-11-26 03:06:29.278991 dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_run_result.py
--rw-r--r--   0        0        0     8096 2023-11-26 03:06:29.279100 dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_unique_id.py
--rw-r--r--   0        0        0      161 2023-11-26 03:06:29.279227 dbt_exasol-1.7.0/tests/functional/adapter/limit/fixtures.py
--rw-r--r--   0        0        0     1062 2023-11-26 03:06:29.279320 dbt_exasol-1.7.0/tests/functional/adapter/limit/test_limit.py
--rw-r--r--   0        0        0     2185 2023-11-26 03:06:29.279458 dbt_exasol-1.7.0/tests/functional/adapter/persist_docs/test_persist_docs.py
--rw-r--r--   0        0        0      676 2023-11-26 03:06:29.279603 dbt_exasol-1.7.0/tests/functional/adapter/query_comment_tests/test_query_comment.py
--rw-r--r--   0        0        0      190 2023-11-26 03:06:29.279740 dbt_exasol-1.7.0/tests/functional/adapter/relations/test_changing_relation_type.py
--rw-r--r--   0        0        0     1495 2023-11-26 03:06:29.279882 dbt_exasol-1.7.0/tests/functional/adapter/simple_copy/test_simple_copy.py
--rw-r--r--   0        0        0      506 2023-11-26 03:06:29.280020 dbt_exasol-1.7.0/tests/functional/adapter/simple_seed/test_simple_seed.py
--rw-r--r--   0        0        0     2356 2023-11-26 03:06:29.280115 dbt_exasol-1.7.0/tests/functional/adapter/simple_seed/test_simple_seed_override.py
--rw-r--r--   0        0        0     1608 2023-11-26 03:06:29.280269 dbt_exasol-1.7.0/tests/functional/adapter/simple_snapshot/test_simple_snapshot.py
--rw-r--r--   0        0        0      180 2023-11-26 03:06:29.280416 dbt_exasol-1.7.0/tests/functional/adapter/store_test_failures_tests/test_store_test_failures.py
--rw-r--r--   0        0        0     2819 2024-03-07 17:53:05.711438 dbt_exasol-1.7.0/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0    12762 2023-11-26 03:06:29.280683 dbt_exasol-1.7.0/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0        0        0     2068 2023-11-26 03:06:29.280869 dbt_exasol-1.7.0/tests/functional/adapter/test_failing_test.py
--rw-r--r--   0        0        0     1350 2023-11-26 03:06:29.281093 dbt_exasol-1.7.0/tests/functional/adapter/utils/data_types/test_data_types.py
--rw-r--r--   0        0        0      591 2023-11-26 03:06:29.281195 dbt_exasol-1.7.0/tests/functional/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0      496 2023-11-26 03:06:29.281290 dbt_exasol-1.7.0/tests/functional/adapter/utils/test_mixed_type_retrieval.py
--rw-r--r--   0        0        0      244 2023-11-26 03:06:29.281374 dbt_exasol-1.7.0/tests/functional/adapter/utils/test_null_compare.py
--rw-r--r--   0        0        0     1167 2023-11-26 03:06:29.281523 dbt_exasol-1.7.0/tests/functional/adapter/utils/test_timestamps.py
--rw-r--r--   0        0        0    12212 2023-11-26 03:06:29.281654 dbt_exasol-1.7.0/tests/functional/adapter/utils/test_utils.py
--rw-r--r--   0        0        0      306 2023-11-26 03:06:29.281743 dbt_exasol-1.7.0/tests/functional/adapter/utils/test_validate_sql.py
--rw-r--r--   0        0        0    14464 2023-11-26 03:06:29.281881 dbt_exasol-1.7.0/tests/functional/adapter/utils/utils_fixtures.py
--rw-r--r--   0        0        0     1465 2023-11-26 03:06:29.281970 dbt_exasol-1.7.0/tests/functional/test_issues.py
--rw-r--r--   0        0        0      831 2023-11-26 03:06:29.282065 dbt_exasol-1.7.0/tests/functional/test_view_comment.py
--rw-r--r--   0        0        0     4839 1970-01-01 00:00:00.000000 dbt_exasol-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-11-26 03:06:29.271819 dbt_exasol-1.7.1/LICENSE
+-rw-r--r--   0        0        0     3766 2024-05-07 13:06:21.592753 dbt_exasol-1.7.1/README.md
+-rw-r--r--   0        0        0       65 2023-11-26 03:06:29.272133 dbt_exasol-1.7.1/dbt/__init__.py
+-rw-r--r--   0        0        0       65 2023-11-26 03:06:29.272275 dbt_exasol-1.7.1/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      508 2023-11-26 03:06:29.272415 dbt_exasol-1.7.1/dbt/adapters/exasol/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-07 13:00:03.317303 dbt_exasol-1.7.1/dbt/adapters/exasol/__version__.py
+-rw-r--r--   0        0        0     3675 2023-11-26 03:06:29.272598 dbt_exasol-1.7.1/dbt/adapters/exasol/column.py
+-rw-r--r--   0        0        0    11372 2023-11-26 03:06:29.272740 dbt_exasol-1.7.1/dbt/adapters/exasol/connections.py
+-rw-r--r--   0        0        0     8452 2024-05-07 12:58:16.926003 dbt_exasol-1.7.1/dbt/adapters/exasol/impl.py
+-rw-r--r--   0        0        0     1959 2023-11-26 03:06:29.272973 dbt_exasol-1.7.1/dbt/adapters/exasol/relation.py
+-rw-r--r--   0        0        0       65 2023-11-26 03:06:29.273118 dbt_exasol-1.7.1/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2023-11-26 03:06:29.273246 dbt_exasol-1.7.1/dbt/include/exasol/__init__.py
+-rw-r--r--   0        0        0      236 2023-11-26 03:06:29.273385 dbt_exasol-1.7.1/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0       74 2023-11-26 03:06:29.273464 dbt_exasol-1.7.1/dbt/include/exasol/dbt_project.yml
+-rw-r--r--   0        0        0     8032 2023-11-26 03:06:29.273627 dbt_exasol-1.7.1/dbt/include/exasol/macros/adapters.sql
+-rw-r--r--   0        0        0      673 2023-11-26 03:06:29.273716 dbt_exasol-1.7.1/dbt/include/exasol/macros/apply_grants.sql
+-rw-r--r--   0        0        0     3796 2024-03-07 17:53:05.710695 dbt_exasol-1.7.1/dbt/include/exasol/macros/catalog.sql
+-rw-r--r--   0        0        0     3493 2023-11-26 03:06:29.273978 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      259 2023-11-26 03:06:29.274073 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     6113 2023-11-26 03:06:29.274187 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/merge.sql
+-rw-r--r--   0        0        0      470 2023-11-26 03:06:29.274293 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/seed.sql
+-rw-r--r--   0        0        0     8044 2023-11-26 03:06:29.274407 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/snapshot.sql
+-rw-r--r--   0        0        0      748 2023-11-26 03:06:29.274503 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     3255 2023-11-26 03:06:29.274602 dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/strategies.sql
+-rw-r--r--   0        0        0      812 2024-05-07 12:57:31.872052 dbt_exasol-1.7.1/dbt/include/exasol/macros/metadata.sql
+-rw-r--r--   0        0        0      178 2023-11-26 03:06:29.274739 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/any_value.sql
+-rw-r--r--   0        0        0       85 2023-11-26 03:06:29.274819 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      469 2023-11-26 03:06:29.274912 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      441 2023-11-26 03:06:29.274994 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      130 2023-11-26 03:06:29.275203 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/hash.sql
+-rw-r--r--   0        0        0      381 2023-11-26 03:06:29.275327 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      415 2023-11-26 03:06:29.275435 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      775 2023-11-26 03:06:29.275534 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      165 2023-11-26 03:06:29.275635 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      519 2023-11-26 03:06:29.275769 dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/timestamps.sql
+-rw-r--r--   0        0        0      177 2023-11-26 03:06:29.275854 dbt_exasol-1.7.1/dbt/include/exasol/macros/validate_sql.sql
+-rw-r--r--   0        0        0      374 2023-11-26 03:06:29.275938 dbt_exasol-1.7.1/dbt/include/exasol/profile_template.yml
+-rw-r--r--   0        0        0     1030 2024-05-07 12:59:33.024701 dbt_exasol-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-11-26 03:06:29.277201 dbt_exasol-1.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      640 2023-11-26 03:06:29.277442 dbt_exasol-1.7.1/tests/functional/adapter/aliases/test_aliases.py
+-rw-r--r--   0        0        0     1252 2023-11-26 03:06:29.277581 dbt_exasol-1.7.1/tests/functional/adapter/concurrency/test_concurrency.py
+-rw-r--r--   0        0        0     4827 2024-03-07 17:53:05.711214 dbt_exasol-1.7.1/tests/functional/adapter/constraints/fixtures.py
+-rw-r--r--   0        0        0     9305 2023-11-26 03:06:29.277850 dbt_exasol-1.7.1/tests/functional/adapter/constraints/test_constraints.py
+-rw-r--r--   0        0        0     3581 2023-11-26 03:06:29.277996 dbt_exasol-1.7.1/tests/functional/adapter/debug/test_dbt_debug.py
+-rw-r--r--   0        0        0     1271 2023-11-26 03:06:29.278140 dbt_exasol-1.7.1/tests/functional/adapter/ephemeral/test_ephemeral.py
+-rw-r--r--   0        0        0     7729 2023-11-26 03:06:29.278240 dbt_exasol-1.7.1/tests/functional/adapter/expected_catalog.py
+-rw-r--r--   0        0        0     1438 2023-11-26 03:06:29.278343 dbt_exasol-1.7.1/tests/functional/adapter/files.py
+-rw-r--r--   0        0        0      521 2023-11-26 03:06:29.278435 dbt_exasol-1.7.1/tests/functional/adapter/fixtures.py
+-rw-r--r--   0        0        0     1080 2023-11-26 03:06:29.278569 dbt_exasol-1.7.1/tests/functional/adapter/grants/test_grants.py
+-rw-r--r--   0        0        0      180 2023-11-26 03:06:29.278716 dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0        0        0      193 2023-11-26 03:06:29.278807 dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0        0        0     1082 2023-11-26 03:06:29.278900 dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0        0        0      972 2023-11-26 03:06:29.278991 dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_run_result.py
+-rw-r--r--   0        0        0     8096 2023-11-26 03:06:29.279100 dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_unique_id.py
+-rw-r--r--   0        0        0      161 2023-11-26 03:06:29.279227 dbt_exasol-1.7.1/tests/functional/adapter/limit/fixtures.py
+-rw-r--r--   0        0        0     1062 2023-11-26 03:06:29.279320 dbt_exasol-1.7.1/tests/functional/adapter/limit/test_limit.py
+-rw-r--r--   0        0        0     2185 2023-11-26 03:06:29.279458 dbt_exasol-1.7.1/tests/functional/adapter/persist_docs/test_persist_docs.py
+-rw-r--r--   0        0        0      676 2023-11-26 03:06:29.279603 dbt_exasol-1.7.1/tests/functional/adapter/query_comment_tests/test_query_comment.py
+-rw-r--r--   0        0        0      190 2023-11-26 03:06:29.279740 dbt_exasol-1.7.1/tests/functional/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0     1495 2023-11-26 03:06:29.279882 dbt_exasol-1.7.1/tests/functional/adapter/simple_copy/test_simple_copy.py
+-rw-r--r--   0        0        0      506 2023-11-26 03:06:29.280020 dbt_exasol-1.7.1/tests/functional/adapter/simple_seed/test_simple_seed.py
+-rw-r--r--   0        0        0     2356 2023-11-26 03:06:29.280115 dbt_exasol-1.7.1/tests/functional/adapter/simple_seed/test_simple_seed_override.py
+-rw-r--r--   0        0        0     1608 2023-11-26 03:06:29.280269 dbt_exasol-1.7.1/tests/functional/adapter/simple_snapshot/test_simple_snapshot.py
+-rw-r--r--   0        0        0      180 2023-11-26 03:06:29.280416 dbt_exasol-1.7.1/tests/functional/adapter/store_test_failures_tests/test_store_test_failures.py
+-rw-r--r--   0        0        0     2819 2024-03-07 17:53:05.711438 dbt_exasol-1.7.1/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0    12762 2023-11-26 03:06:29.280683 dbt_exasol-1.7.1/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0        0        0     2068 2023-11-26 03:06:29.280869 dbt_exasol-1.7.1/tests/functional/adapter/test_failing_test.py
+-rw-r--r--   0        0        0     2141 2024-05-07 12:57:31.873463 dbt_exasol-1.7.1/tests/functional/adapter/test_get_relation_last_modified.py
+-rw-r--r--   0        0        0     1350 2023-11-26 03:06:29.281093 dbt_exasol-1.7.1/tests/functional/adapter/utils/data_types/test_data_types.py
+-rw-r--r--   0        0        0      591 2023-11-26 03:06:29.281195 dbt_exasol-1.7.1/tests/functional/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0      496 2023-11-26 03:06:29.281290 dbt_exasol-1.7.1/tests/functional/adapter/utils/test_mixed_type_retrieval.py
+-rw-r--r--   0        0        0      244 2023-11-26 03:06:29.281374 dbt_exasol-1.7.1/tests/functional/adapter/utils/test_null_compare.py
+-rw-r--r--   0        0        0     1167 2023-11-26 03:06:29.281523 dbt_exasol-1.7.1/tests/functional/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0    12212 2023-11-26 03:06:29.281654 dbt_exasol-1.7.1/tests/functional/adapter/utils/test_utils.py
+-rw-r--r--   0        0        0      306 2023-11-26 03:06:29.281743 dbt_exasol-1.7.1/tests/functional/adapter/utils/test_validate_sql.py
+-rw-r--r--   0        0        0    14464 2023-11-26 03:06:29.281881 dbt_exasol-1.7.1/tests/functional/adapter/utils/utils_fixtures.py
+-rw-r--r--   0        0        0      970 2024-05-07 12:57:31.873650 dbt_exasol-1.7.1/tests/functional/artifacts/test_override.py
+-rw-r--r--   0        0        0     1465 2023-11-26 03:06:29.281970 dbt_exasol-1.7.1/tests/functional/test_issues.py
+-rw-r--r--   0        0        0      831 2023-11-26 03:06:29.282065 dbt_exasol-1.7.1/tests/functional/test_view_comment.py
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 dbt_exasol-1.7.1/PKG-INFO
```

### Comparing `dbt_exasol-1.7.0/LICENSE` & `dbt_exasol-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/README.md` & `dbt_exasol-1.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,14 @@
   <li><strong>protocol_version</strong>: default: v3</li>
   <li><strong>row_separator</strong>: default: CRLF for windows - LF otherwise</li>
   <li><strong>timestamp_format</strong>: default: YYYY-MM-DDTHH:MI:SS.FF6</li>
 </ul>
 
 # Known isues
 
-## source freshness not yet implemented
-Implementation for last_commit from EXA_ALL_OBJECTS per dbt model is missing.
-
 ## Using encryption in Exasol 7 vs. 8
 Starting from Exasol 8, encryption is enforced by default. If you are still using Exasol 7 and have trouble connecting, you can disable encryption in profiles.yaml (see optional parameters).
 
 ## Materialized View & Clone operations
 In Exasol materialized views and clone operations are not suported. Default behaviour from dbt-core will fail accordingly.
 
 ## Null handling in test_utils null safe handling
```

### Comparing `dbt_exasol-1.7.0/dbt/adapters/exasol/column.py` & `dbt_exasol-1.7.1/dbt/adapters/exasol/column.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/adapters/exasol/connections.py` & `dbt_exasol-1.7.1/dbt/adapters/exasol/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/adapters/exasol/impl.py` & `dbt_exasol-1.7.1/dbt/adapters/exasol/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
         ConstraintType.not_null: ConstraintSupport.ENFORCED,
         ConstraintType.unique: ConstraintSupport.NOT_SUPPORTED,
         ConstraintType.primary_key: ConstraintSupport.ENFORCED,
         ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
     }
 
     _capabilities = CapabilityDict(
-        {Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full)}
+        {
+            Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
+            Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
+        }
     )
 
     @classmethod
     def date_function(cls):
         return "current_timestamp()"
 
     @classmethod
```

### Comparing `dbt_exasol-1.7.0/dbt/adapters/exasol/relation.py` & `dbt_exasol-1.7.1/dbt/adapters/exasol/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/adapters.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/apply_grants.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/catalog.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/incremental.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/merge.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/snapshot.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/materializations/strategies.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/materializations/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/safe_cast.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/dbt/include/exasol/macros/utils/timestamps.sql` & `dbt_exasol-1.7.1/dbt/include/exasol/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/pyproject.toml` & `dbt_exasol-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-exasol"
-version = "1.7.0"
+version = "1.7.1"
 description = "Adapter to dbt-core for warehouse Exasol"
 authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
 homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
 repository = "https://github.com/tglunde/dbt-exasol"
 packages = [
   { include = "dbt" },
   { include = "dbt/**/*.py" },
```

### Comparing `dbt_exasol-1.7.0/tests/conftest.py` & `dbt_exasol-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/aliases/test_aliases.py` & `dbt_exasol-1.7.1/tests/functional/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/concurrency/test_concurrency.py` & `dbt_exasol-1.7.1/tests/functional/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/constraints/fixtures.py` & `dbt_exasol-1.7.1/tests/functional/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/constraints/test_constraints.py` & `dbt_exasol-1.7.1/tests/functional/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/debug/test_dbt_debug.py` & `dbt_exasol-1.7.1/tests/functional/adapter/debug/test_dbt_debug.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/ephemeral/test_ephemeral.py` & `dbt_exasol-1.7.1/tests/functional/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/expected_catalog.py` & `dbt_exasol-1.7.1/tests/functional/adapter/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/files.py` & `dbt_exasol-1.7.1/tests/functional/adapter/files.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/fixtures.py` & `dbt_exasol-1.7.1/tests/functional/adapter/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/grants/test_grants.py` & `dbt_exasol-1.7.1/tests/functional/adapter/grants/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_predicates.py` & `dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_run_result.py` & `dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_run_result.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/incremental/test_incremental_unique_id.py` & `dbt_exasol-1.7.1/tests/functional/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/limit/test_limit.py` & `dbt_exasol-1.7.1/tests/functional/adapter/limit/test_limit.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/persist_docs/test_persist_docs.py` & `dbt_exasol-1.7.1/tests/functional/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/query_comment_tests/test_query_comment.py` & `dbt_exasol-1.7.1/tests/functional/adapter/query_comment_tests/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/simple_copy/test_simple_copy.py` & `dbt_exasol-1.7.1/tests/functional/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/simple_seed/test_simple_seed_override.py` & `dbt_exasol-1.7.1/tests/functional/adapter/simple_seed/test_simple_seed_override.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/simple_snapshot/test_simple_snapshot.py` & `dbt_exasol-1.7.1/tests/functional/adapter/simple_snapshot/test_simple_snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/test_basic.py` & `dbt_exasol-1.7.1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/test_docs_generate.py` & `dbt_exasol-1.7.1/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/test_failing_test.py` & `dbt_exasol-1.7.1/tests/functional/adapter/test_failing_test.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/utils/data_types/test_data_types.py` & `dbt_exasol-1.7.1/tests/functional/adapter/utils/data_types/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/utils/data_types/test_type_bigint.py` & `dbt_exasol-1.7.1/tests/functional/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/utils/test_timestamps.py` & `dbt_exasol-1.7.1/tests/functional/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/utils/test_utils.py` & `dbt_exasol-1.7.1/tests/functional/adapter/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/adapter/utils/utils_fixtures.py` & `dbt_exasol-1.7.1/tests/functional/adapter/utils/utils_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/test_issues.py` & `dbt_exasol-1.7.1/tests/functional/test_issues.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/tests/functional/test_view_comment.py` & `dbt_exasol-1.7.1/tests/functional/test_view_comment.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.7.0/PKG-INFO` & `dbt_exasol-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-exasol
-Version: 1.7.0
+Version: 1.7.1
 Summary: Adapter to dbt-core for warehouse Exasol
 Home-page: https://alligatorcompany.gitlab.io/dbt-exasol
 License: GPL3
 Author: Torsten Glunde
 Author-email: torsten.glunde@alligator-company.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
@@ -58,17 +58,14 @@
   <li><strong>protocol_version</strong>: default: v3</li>
   <li><strong>row_separator</strong>: default: CRLF for windows - LF otherwise</li>
   <li><strong>timestamp_format</strong>: default: YYYY-MM-DDTHH:MI:SS.FF6</li>
 </ul>
 
 # Known isues
 
-## source freshness not yet implemented
-Implementation for last_commit from EXA_ALL_OBJECTS per dbt model is missing.
-
 ## Using encryption in Exasol 7 vs. 8
 Starting from Exasol 8, encryption is enforced by default. If you are still using Exasol 7 and have trouble connecting, you can disable encryption in profiles.yaml (see optional parameters).
 
 ## Materialized View & Clone operations
 In Exasol materialized views and clone operations are not suported. Default behaviour from dbt-core will fail accordingly.
 
 ## Null handling in test_utils null safe handling
```

