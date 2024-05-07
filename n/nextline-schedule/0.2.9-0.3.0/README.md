# Comparing `tmp/nextline_schedule-0.2.9.tar.gz` & `tmp/nextline_schedule-0.3.0.tar.gz`

## Comparing `nextline_schedule-0.2.9.tar` & `nextline_schedule-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,90 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/release.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/release.yml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/py.typed
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/factory.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/auto/machine.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/AutoMode.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/queries/Version.gql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_fsm.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_plugin.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_request.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_scratch.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/queries/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/tests/schema/queries/test_version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/LICENSE.txt
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/README.md
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 nextline_schedule-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/dummy.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/py.typed
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/auto_mode.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/factory.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/machine.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/AutoModeTurnOff.gql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/AutoModeTurnOn.gql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/mutations/QueuePush.gql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/AutoMode.gql
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/QueueItems.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/queries/Version.gql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/pubsub_queue.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/queue.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/queue/strategies.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/mutation.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/query.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/auto/subscription.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/mutation.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/query.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/subscription.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/schema/queue/types.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/safe.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/utc.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/datetime.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/misc.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/src/nextline_schedule/utils/strategies/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_request.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_scratch.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/auto/state_machine/test_fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/test_pubsub_queue.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/queue/test_queue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/mutations/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/mutations/test_queue_push.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/test_queue_items.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/schema/queries/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/test_safe_compare.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/test_safe_min_max.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_datetimes.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_ints.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_python_scripts.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/tests/utils/strategies/test_st_ranges.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/README.md
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 nextline_schedule-0.3.0/PKG-INFO
```

### Comparing `nextline_schedule-0.2.9/.github/workflows/pypi.yml` & `nextline_schedule-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/.github/workflows/release.yml` & `nextline_schedule-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/.github/workflows/type-check.yml` & `nextline_schedule-0.3.0/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/.github/workflows/unit-test.yml` & `nextline_schedule-0.3.0/.github/workflows/unit-test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -44,8 +44,9 @@
         run: pytest -vv --cov --cov-report=xml
 
       - name: Upload coverage to Codecov
         if: matrix.os == 'ubuntu-latest'
         uses: codecov/codecov-action@v1
         with:
           fail_ci_if_error: true
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `nextline_schedule-0.2.9/src/nextline_schedule/auto/factory.py` & `nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/src/nextline_schedule/auto/machine.py` & `nextline_schedule-0.3.0/src/nextline_schedule/auto/state_machine/machine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import asyncio
-from collections.abc import AsyncIterator
+from collections.abc import AsyncIterator, Callable
 from logging import getLogger
-from typing import Protocol
+from typing import Any, Protocol
 
 from nextline.utils import pubsub
 
 from .factory import build_state_machine
 
 
 class CallbackType(Protocol):
+    async def on_state_changed(self, state: str) -> None:
+        ...
+
     async def wait(self) -> None:
         ...
 
     async def pull(self) -> None:
         ...
 
     async def run(self, started: asyncio.Event) -> None:
@@ -23,16 +26,23 @@
     '''The finite state machine for auto mode.'''
 
     def __init__(self, callback: CallbackType):
         self._callback = callback
         self._tasks = set[asyncio.Task]()
         self._pubsub_state = pubsub.PubSubItem[str]()
         self._logger = getLogger(__name__)
+
         machine = build_state_machine(model=self)
-        machine.after_state_change = self.after_state_change.__name__  # type: ignore
+        machine.after_state_change = [self.after_state_change.__name__]
+
+        self.state: str  # attached by machine
+        self.start: Callable[..., Any]  # attached by machine
+
+        assert isinstance(self.state, str)
+        assert callable(self.start)
 
     def subscribe_state(self) -> AsyncIterator[str]:
         return self._pubsub_state.subscribe()
 
     async def on_enter_auto_waiting(self) -> None:
         task = asyncio.create_task(self._callback.wait())
         self._task = task
@@ -48,15 +58,16 @@
         task = asyncio.create_task(self._callback.run(started=started))
         await started.wait()
         self._task = task
         self._tasks.add(task)
 
     async def after_state_change(self) -> None:
         await self._collect_tasks()
-        await self._pubsub_state.publish(self.state)  # type: ignore
+        await self._callback.on_state_changed(self.state)
+        await self._pubsub_state.publish(self.state)
 
     async def cancel_task(self) -> None:
         self._task.cancel()
 
     async def _collect_tasks(self) -> None:
         if not self._tasks:
             return
@@ -71,13 +82,13 @@
         self._tasks -= done
 
     async def close(self) -> None:
         await self._collect_tasks()
         await self._pubsub_state.close()
 
     async def __aenter__(self) -> 'AutoModeStateMachine':
-        await self.start()  # type: ignore
+        await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         del exc_type, exc_value, traceback
         await self.close()
```

### Comparing `nextline_schedule-0.2.9/src/nextline_schedule/graphql/__init__.py` & `nextline_schedule-0.3.0/src/nextline_schedule/graphql/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from pathlib import Path
 
 pwd = Path(__file__).resolve().parent
 
 sub = pwd / 'mutations'
 MUTATE_AUTO_MODE_TURN_ON = (sub / 'AutoModeTurnOn.gql').read_text()
 MUTATE_AUTO_MODE_TURN_OFF = (sub / 'AutoModeTurnOff.gql').read_text()
+MUTATE_QUEUE_PUSH = (sub / 'QueuePush.gql').read_text()
 
 
 sub = pwd / 'queries'
 QUERY_AUTO_MODE = (sub / 'AutoMode.gql').read_text()
 QUERY_SCHEDULER = (sub / 'Scheduler.gql').read_text()
 QUERY_VERSION = (sub / 'Version.gql').read_text()
+QUERY_SCHEDULE_QUEUE_ITEMS = (sub / 'QueueItems.gql').read_text()
 
 sub = pwd / 'subscriptions'
 SUBSCRIBE_AUTO_MODE_STATE = (sub / 'ScheduleAutoModeState.gql').read_text()
```

### Comparing `nextline_schedule-0.2.9/src/nextline_schedule/schema/mutation.py` & `nextline_schedule-0.3.0/src/nextline_schedule/schema/mutation.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,75 +2,68 @@
 
 import strawberry
 from nextline import Nextline
 from strawberry.types import Info
 
 from nextline_schedule.scheduler import RequestStatement
 
-
-async def mutate_turn_on(info: Info) -> bool:
-    auto_mode = info.context["auto_mode"]
-    await auto_mode.turn_on()
-    return True
-
-
-async def mutate_turn_off(info: Info) -> bool:
-    auto_mode = info.context["auto_mode"]
-    await auto_mode.turn_off()
-    return True
-
-
-@strawberry.type
-class MutationAutoMode:
-    turn_on: bool = strawberry.field(resolver=mutate_turn_on)
-    turn_off: bool = strawberry.field(resolver=mutate_turn_off)
+from .auto import MutationScheduleAutoMode
+from .queue import MutationScheduleQueue
 
 
 @strawberry.input
 class MutationSchedulerInput:
     api_url: Optional[str] = None
     length_minutes: Optional[int] = None
     policy: Optional[str] = None
 
 
 @strawberry.type
 class MutationScheduler:
     @strawberry.mutation
     def update(self, info: Info, input: MutationSchedulerInput) -> bool:
-        scheduler = info.context["scheduler"]
+        scheduler = info.context['schedule']['scheduler']
+        assert isinstance(scheduler, RequestStatement)
         if input.api_url is not None:
             scheduler._api_url = input.api_url
         if input.length_minutes is not None:
             scheduler._length_minutes = input.length_minutes
         if input.policy is not None:
             scheduler._policy = input.policy
         return True
 
 
 async def mutate_load_script(info: Info) -> bool:
-    nextline: Nextline = info.context["nextline"]
-    scheduler: RequestStatement = info.context["scheduler"]
+    nextline = info.context["nextline"]
+    assert isinstance(nextline, Nextline)
+    scheduler = info.context['schedule']['scheduler']
+    assert callable(scheduler)
     statement = await scheduler()
+    assert isinstance(statement, str)
     await nextline.reset(statement=statement)
     return True
 
 
 @strawberry.type
 class MutationSchedule:
     @strawberry.field
-    def auto_mode(self, info: Info) -> MutationAutoMode:
-        return MutationAutoMode()
+    def auto_mode(self, info: Info) -> MutationScheduleAutoMode:
+        return MutationScheduleAutoMode()
 
     @strawberry.field
     def scheduler(self, info: Info) -> MutationScheduler:
         return MutationScheduler()
 
     @strawberry.mutation
     async def load_script(self, info: Info) -> bool:
         return await mutate_load_script(info)
 
+    @strawberry.field
+    def queue(self) -> MutationScheduleQueue:
+        return MutationScheduleQueue()
+
 
 @strawberry.type
 class Mutation:
     @strawberry.field
     def schedule(self, info: Info) -> MutationSchedule:
         return MutationSchedule()
```

### Comparing `nextline_schedule-0.2.9/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.3.0/src/nextline_schedule/schema/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import strawberry
 from strawberry.types import Info
 
-import nextline_schedule
+from nextline_schedule import __version__
+from nextline_schedule.scheduler import RequestStatement
 
-
-def query_auto_mode_state(info: Info) -> str:
-    auto_mode = info.context["auto_mode"]
-    return auto_mode.state
-
-
-@strawberry.type
-class QueryAutoMode:
-    state: str = strawberry.field(resolver=query_auto_mode_state)
+from .auto import QueryScheduleAutoMode
+from .queue import QueryScheduleQueue
 
 
 def query_scheduler_api_url(info: Info) -> str:
-    scheduler = info.context["scheduler"]
+    scheduler = info.context['schedule']['scheduler']
+    assert isinstance(scheduler, RequestStatement)
     return scheduler._api_url
 
 
 def query_scheduler_length_minutes(info: Info) -> int:
-    scheduler = info.context["scheduler"]
+    scheduler = info.context['schedule']['scheduler']
+    assert isinstance(scheduler, RequestStatement)
     return scheduler._length_minutes
 
 
 def query_scheduler_policy(info: Info) -> str:
-    scheduler = info.context["scheduler"]
+    scheduler = info.context['schedule']['scheduler']
+    assert isinstance(scheduler, RequestStatement)
     return scheduler._policy
 
 
 @strawberry.type
 class QueryScheduler:
     api_url: str = strawberry.field(resolver=query_scheduler_api_url)
     length_minutes: int = strawberry.field(resolver=query_scheduler_length_minutes)
     policy: str = strawberry.field(resolver=query_scheduler_policy)
 
 
 @strawberry.type
 class QuerySchedule:
-    version: str = nextline_schedule.__version__
+    version: str = __version__
 
     @strawberry.field
-    def auto_mode(self, info: Info) -> QueryAutoMode:
-        return QueryAutoMode()
+    def auto_mode(self, info: Info) -> QueryScheduleAutoMode:
+        return QueryScheduleAutoMode()
 
     @strawberry.field
     def scheduler(self, info: Info) -> QueryScheduler:
         return QueryScheduler()
 
+    @strawberry.field
+    def queue(self) -> QueryScheduleQueue:
+        return QueryScheduleQueue()
+
 
 @strawberry.type
 class Query:
     @strawberry.field
     def schedule(self, info: Info) -> QuerySchedule:
         return QuerySchedule()
```

### Comparing `nextline_schedule-0.2.9/tests/test_fsm.py` & `nextline_schedule-0.3.0/tests/auto/state_machine/test_fsm.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 from hypothesis import given
 from hypothesis import strategies as st
 from transitions import Machine
 from transitions.extensions.markup import HierarchicalMarkupMachine
 
-from nextline_schedule.auto.factory import build_state_machine
+from nextline_schedule.auto.state_machine.factory import build_state_machine
 
 
 def test_model_default():
     machine = build_state_machine()
     assert not machine.models
```

### Comparing `nextline_schedule-0.2.9/tests/test_plugin.py` & `nextline_schedule-0.3.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/tests/test_request.py` & `nextline_schedule-0.3.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/tests/test_scratch.py` & `nextline_schedule-0.3.0/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/tests/auto/test_auto.py` & `nextline_schedule-0.3.0/tests/auto/test_auto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 import asyncio
 
 from nextline import Nextline
 
-from nextline_schedule.auto import AutoModeStateMachine, build_auto_mode_state_machine
+from nextline_schedule.auto import AutoMode
 
-STATEMENT = '''
+STATEMENT_SCHEDULER = '''
 """run_no: {run_no}"""
 import time
 time.sleep(0.01)
 '''
 
+STATEMENT_QUEUE = '''
+"""queue"""
+import time
+time.sleep(0.01)
+'''
 
-class RequestStatement:
+
+class MockScheduler:
     def __init__(self, nextline: Nextline):
         self._nextline = nextline
 
     async def __call__(self) -> str:
-        return STATEMENT.format(run_no=self._nextline.run_no + 1)
+        return STATEMENT_SCHEDULER.format(run_no=self._nextline.run_no + 1)
+
+
+async def mock_queue() -> str:
+    return STATEMENT_QUEUE
 
 
 async def test_one() -> None:
     run_no = 1
-    statement = STATEMENT.format(run_no=run_no)
+    statement = STATEMENT_SCHEDULER.format(run_no=run_no)
     nextline = Nextline(statement=statement, run_no_start_from=run_no)
-    request_statement = RequestStatement(nextline=nextline)
-    auto_mode = build_auto_mode_state_machine(
-        nextline=nextline, request_statement=request_statement
-    )
+    scheduler = MockScheduler(nextline=nextline)
+    auto_mode = AutoMode(nextline=nextline, scheduler=scheduler, queue=mock_queue)
 
     states = asyncio.create_task(subscribe_state(auto_mode))
 
     async with auto_mode:
         async with nextline:
             await control(auto_mode, nextline)
 
@@ -42,18 +50,18 @@
         'auto_pulling',
         'auto_running',
         'off',
     ]
     assert expected == await states
 
 
-async def control(auto_mode: AutoModeStateMachine, nextline: Nextline):
+async def control(auto_mode: AutoMode, nextline: Nextline):
     assert auto_mode.state == 'off'  # type: ignore
     await auto_mode.turn_on()  # type: ignore
     async for run_info in nextline.subscribe_run_info():
         if run_info.run_no == 3 and run_info.state == 'running':
             break
     await auto_mode.turn_off()  # type: ignore
 
 
-async def subscribe_state(auto_mode: AutoModeStateMachine):
+async def subscribe_state(auto_mode: AutoMode):
     return [state async for state in auto_mode.subscribe_state()]
```

### Comparing `nextline_schedule-0.2.9/.gitignore` & `nextline_schedule-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/LICENSE.txt` & `nextline_schedule-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.2.9/pyproject.toml` & `nextline_schedule-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,30 @@
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["transitions>=0.9", "httpx>=0.23"]
+dependencies = [
+  "transitions>=0.9",
+  "httpx>=0.23",
+  "hypothesis>=6.65",
+  "black>=23.10",
+]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 host = ["nextline-graphql>=0.7.7"]
 tests = [
   "async-asgi-testclient>=1.4",
   "pytest-asyncio>=0.18",
   "pytest-cov>=3.0",
   "pytest-timeout>=2.1",
   "pytest>=7.0",
-  "hypothesis>=6.65",
   "pytest-httpx>=0.21",
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/simonsobs/nextline-schedule#readme"
 Issues = "https://github.com/simonsobs/nextline-schedule/issues"
@@ -62,14 +66,15 @@
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 timeout = 60
 addopts = "--doctest-modules"
 # doctest_optionflags = ["ELLIPSIS", "NORMALIZE_WHITESPACE",]
 doctest_optionflags = ["ELLIPSIS"]
 norecursedirs = "build"
+filterwarnings = ["ignore::hypothesis.errors.NonInteractiveExampleWarning"]
 log_cli = false
 log_cli_level = "INFO"
 
 [tool.black]
 skip-string-normalization = true
 target_version = ['py310', 'py311', 'py312']
 
@@ -84,13 +89,9 @@
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 plugins = "strawberry.ext.mypy_plugin"
 
 [[tool.mypy.overrides]]
-module = [
-  "dynaconf.*",
-  "async_asgi_testclient.*",
-  "apluggy.*",
-]
+module = ["dynaconf.*", "async_asgi_testclient.*", "apluggy.*"]
 ignore_missing_imports = true
```

