# Comparing `tmp/UnleashClient-5.9.1.tar.gz` & `tmp/UnleashClient-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/unleash-client-python/unleash-client-python/dist/.tmp-p208pru6/UnleashClient-5.9.1.tar", last modified: Sat Oct 28 11:57:41 2023, max compression
+gzip compressed data, was "UnleashClient-5.9.2.tar", last modified: Tue Oct 31 10:51:49 2023, max compression
```

## Comparing `UnleashClient-5.9.1.tar` & `UnleashClient-5.9.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      292 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.devcontainer/post_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/workflows/add-to-project.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/workflows/release-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.lift.toml
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/
--rw-r--r--   0 runner    (1001) docker     (127)    23300 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/api/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/api/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/api/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/features/
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/features/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/periodic_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/periodic_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/periodic_tasks/fetch_and_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/periodic_tasks/send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/ApplicationHostname.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/Default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/FlexibleRolloutStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/GradualRolloutRandom.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/GradualRolloutSessionId.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/GradualRolloutUserId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/RemoteAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/Strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/UserWithId.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient/variants/
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/variants/Variants.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/UnleashClient/variants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/UnleashClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/basecache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/customcache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/customstrategies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/eventcallbacks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/filecache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/strategy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/unleashclient.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/docs/wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/scripts/get-spec.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/integration_tests/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/integration_tests/integration_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/integration_tests/integration_unleashheroku.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/integration_tests/integration_unleashhosted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/specification_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/specification_tests/test_client_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/unit_tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/api/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/api/test_register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/unit_tests/periodic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/periodic/test_fetch_and_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_applicationhostname.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_defaultstrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_flexiblerollout.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_gradualrolloutrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_remoteaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_strategy_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/strategies/test_userwithids.py
--rw-r--r--   0 runner    (1001) docker     (127)    25446 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/unit_tests/test_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/utilities/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_all_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_custom_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/mocks/mock_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:41.000000 UnleashClient-5.9.1/tests/utilities/old_code/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/old_code/StrategyV2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/old_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tests/utilities/testing_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-28 11:57:04.000000 UnleashClient-5.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.945425 UnleashClient-5.9.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      292 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.devcontainer/post_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.945425 UnleashClient-5.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.945425 UnleashClient-5.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/workflows/add-to-project.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/workflows/release-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.lift.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient/
+-rw-r--r--   0 runner    (1001) docker     (127)    23300 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/features/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient/periodic_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/periodic_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/periodic_tasks/fetch_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/periodic_tasks/send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.953426 UnleashClient-5.9.2/UnleashClient/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/ApplicationHostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/Default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/FlexibleRolloutStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/GradualRolloutRandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/GradualRolloutSessionId.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/GradualRolloutUserId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/RemoteAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/Strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/UserWithId.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.953426 UnleashClient-5.9.2/UnleashClient/variants/
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/variants/Variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/UnleashClient/variants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.949425 UnleashClient-5.9.2/UnleashClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2023-10-31 10:51:49.000000 UnleashClient-5.9.2/UnleashClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2023-10-31 10:51:49.000000 UnleashClient-5.9.2/UnleashClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 10:51:49.000000 UnleashClient-5.9.2/UnleashClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-31 10:51:49.000000 UnleashClient-5.9.2/UnleashClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 10:51:49.000000 UnleashClient-5.9.2/UnleashClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.953426 UnleashClient-5.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/basecache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/customcache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/customstrategies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/eventcallbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/filecache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/strategy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/unleashclient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.953426 UnleashClient-5.9.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/scripts/get-spec.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/integration_tests/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/integration_tests/integration_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/integration_tests/integration_unleashheroku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/integration_tests/integration_unleashhosted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/specification_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/specification_tests/test_client_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/unit_tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/api/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/api/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.957426 UnleashClient-5.9.2/tests/unit_tests/periodic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/periodic/test_fetch_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/tests/unit_tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_applicationhostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_defaultstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_flexiblerollout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_gradualrolloutrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_gradualrolloutwithsessionid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_gradualrolloutwithuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_remoteaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_strategy_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/strategies/test_userwithids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25446 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/unit_tests/test_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/tests/utilities/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_all_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_custom_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/mocks/mock_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:49.961426 UnleashClient-5.9.2/tests/utilities/old_code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/old_code/StrategyV2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/old_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tests/utilities/testing_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-31 10:51:05.000000 UnleashClient-5.9.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `UnleashClient-5.9.1/.devcontainer/Dockerfile` & `UnleashClient-5.9.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.devcontainer/devcontainer.json` & `UnleashClient-5.9.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `UnleashClient-5.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `UnleashClient-5.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.github/PULL_REQUEST_TEMPLATE.md` & `UnleashClient-5.9.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.github/workflows/codeql-analysis.yml` & `UnleashClient-5.9.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/.github/workflows/pull_request.yml` & `UnleashClient-5.9.2/.github/workflows/pull_request.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   pull_request:
 
 jobs:
   main:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - name: Set up Python 3.7
+      - name: Set up Python 3.8
         uses: actions/setup-python@v4
         with:
           python-version: "3.8"
       - name: Install packages
         run: |
           make install
       - name: Linting
```

### Comparing `UnleashClient-5.9.1/.github/workflows/release-package.yml` & `UnleashClient-5.9.2/.github/workflows/release-package.yml`

 * *Files 21% similar despite different names*

```diff
@@ -4,31 +4,32 @@
   release:
     types: [published]
 
 jobs:
   main:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v1
-      - name: Set up Python 3.7
-        uses: actions/setup-python@v1
+      - uses: actions/checkout@v4
+      - name: Set up Python 3.10
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: "3.10"
       - name: Install dependencies
         run: |
           make install
       - name: Build package
         run: |
           make build
         env:
           TWINE_USERNAME: ${{ secrets.pypi_username }}
           TWINE_PASSWORD: ${{ secrets.pypi_password }}
       - name: Build docs
         run: |
           cd docs
+          make install-docs
           make html
       - name: Deploy docs
         uses: peaceiris/actions-gh-pages@v3
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./docs/_build/html
       - name: Notify Slack of pipeline completion
```

### Comparing `UnleashClient-5.9.1/.gitignore` & `UnleashClient-5.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/CHANGELOG.md` & `UnleashClient-5.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+## v5.9.2
+* (Bugfix) Update variants to use a seed value for their hash.  This fixes an issue with variant distribution & gradual rollouts where users were seeing very non-random distributions.
+
 ## v5.9.1
 * (Minor) Add support for Semver 3 while maintaining backwards compatibility.  Thanks @@chaitanya-parsana!
 
 ## v5.9.0
 * (Major) Support for dependent features.  Thanks @Tymek!
 * (Major) Add request timeout and request retrie paremeters/overides.  Thanks @snosratiershad!
-* (Bugfixes) Make `check_date_operators` works with dateutil < 2.9.1.
-* (Bugfixes) Update responses mock for etag test.  Thanks @yjabri!
+* (Bugfix) Make `check_date_operators` works with dateutil < 2.9.1.
+* (Bugfix) Update responses mock for etag test.  Thanks @yjabri!
 * (Bugfix) Fix broken link in client spec ddocs.  Thanks @sjaanus!
 
 ## v5.8.0
 * (Major) Added support for Strategy Variants.
 
 ## v5.7.1
 * (Bugfix) Fix dependency issue.
```

### Comparing `UnleashClient-5.9.1/CODE_OF_CONDUCT.md` & `UnleashClient-5.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/CONTRIBUTING.md` & `UnleashClient-5.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/LICENSE.md` & `UnleashClient-5.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/Makefile` & `UnleashClient-5.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/PKG-INFO` & `UnleashClient-5.9.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.9.1
+Version: 5.9.2
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
@@ -16,14 +16,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: fcache
+Requires-Dist: mmhash3
+Requires-Dist: apscheduler<4.0.0
+Requires-Dist: importlib_metadata
+Requires-Dist: python-dateutil
+Requires-Dist: semver<4.0.0
 
 # unleash-client-python
 
 ![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://docs.getunleash.io/client-specification) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
```

### Comparing `UnleashClient-5.9.1/README.md` & `UnleashClient-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/__init__.py` & `UnleashClient-5.9.2/UnleashClient/__init__.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/api/features.py` & `UnleashClient-5.9.2/UnleashClient/api/features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/api/metrics.py` & `UnleashClient-5.9.2/UnleashClient/api/metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/api/register.py` & `UnleashClient-5.9.2/UnleashClient/api/register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/cache.py` & `UnleashClient-5.9.2/UnleashClient/cache.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/constants.py` & `UnleashClient-5.9.2/UnleashClient/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Library
 SDK_NAME = "unleash-client-python"
 SDK_VERSION = version("UnleashClient")
 REQUEST_TIMEOUT = 30
 REQUEST_RETRIES = 3
 METRIC_LAST_SENT_TIME = "mlst"
-CLIENT_SPEC_VERSION = "4.5.0"
+CLIENT_SPEC_VERSION = "5.0.2"
 
 # =Unleash=
 APPLICATION_HEADERS = {
     "Content-Type": "application/json",
     "Unleash-Client-Spec": CLIENT_SPEC_VERSION,
 }
 DISABLED_VARIATION = {"name": "disabled", "enabled": False}
```

### Comparing `UnleashClient-5.9.1/UnleashClient/constraints/Constraint.py` & `UnleashClient-5.9.2/UnleashClient/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/deprecation_warnings.py` & `UnleashClient-5.9.2/UnleashClient/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/events.py` & `UnleashClient-5.9.2/UnleashClient/events.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/features/Feature.py` & `UnleashClient-5.9.2/UnleashClient/features/Feature.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/loader.py` & `UnleashClient-5.9.2/UnleashClient/loader.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/periodic_tasks/fetch_and_load.py` & `UnleashClient-5.9.2/UnleashClient/periodic_tasks/fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/periodic_tasks/send_metrics.py` & `UnleashClient-5.9.2/UnleashClient/periodic_tasks/send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/FlexibleRolloutStrategy.py` & `UnleashClient-5.9.2/UnleashClient/strategies/FlexibleRolloutStrategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/GradualRolloutSessionId.py` & `UnleashClient-5.9.2/UnleashClient/strategies/GradualRolloutSessionId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/GradualRolloutUserId.py` & `UnleashClient-5.9.2/UnleashClient/strategies/GradualRolloutUserId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/RemoteAddress.py` & `UnleashClient-5.9.2/UnleashClient/strategies/RemoteAddress.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/Strategy.py` & `UnleashClient-5.9.2/UnleashClient/strategies/Strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/strategies/UserWithId.py` & `UnleashClient-5.9.2/UnleashClient/strategies/UserWithId.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/UnleashClient/utils.py` & `UnleashClient-5.9.2/UnleashClient/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,21 @@
             if key in self:
                 self.instances[key] += 1
             else:
                 self.instances[key] = 1
 
 
 def normalized_hash(
-    identifier: str, activation_group: str, normalizer: int = 100
+    identifier: str, activation_group: str, normalizer: int = 100, seed: int = 0
 ) -> int:
-    return mmh3.hash(f"{activation_group}:{identifier}", signed=False) % normalizer + 1
+    return (
+        mmh3.hash(f"{activation_group}:{identifier}", signed=False, seed=seed)
+        % normalizer
+        + 1
+    )
 
 
 def get_identifier(context_key_name: str, context: dict) -> Any:
     if context_key_name in context.keys():
         value = context[context_key_name]
     elif (
         "properties" in context.keys()
```

### Comparing `UnleashClient-5.9.1/UnleashClient/variants/Variants.py` & `UnleashClient-5.9.2/UnleashClient/variants/Variants.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import copy
 import random
 from typing import Dict, Optional  # noqa: F401
 
 from UnleashClient import utils
 from UnleashClient.constants import DISABLED_VARIATION
 
+VARIANT_HASH_SEED = 86028157
+
 
 class Variants:
     def __init__(
         self, variants_list: list, group_id: str, is_feature_variants: bool = True
     ) -> None:
         """
         Represents an A/B test
@@ -99,14 +101,15 @@
                 else "default"
             )
 
             target = utils.normalized_hash(
                 self._get_seed(context, stickiness_selector),
                 self.group_id,
                 total_weight,
+                seed=VARIANT_HASH_SEED,
             )
             counter = 0
             for variation in self.variants:
                 counter += variation["weight"]
 
                 if counter >= target:
                     return self._format_variation(variation, flag_status)
```

### Comparing `UnleashClient-5.9.1/UnleashClient.egg-info/PKG-INFO` & `UnleashClient-5.9.2/UnleashClient.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnleashClient
-Version: 5.9.1
+Version: 5.9.2
 Summary: Python client for the Unleash feature toggle system!
 Author-email: Ivan Lee <ivanklee86@gmail.com>
 Project-URL: Homepage, https://github.com/Unleash/unleash-client-python
 Project-URL: Documentation, https://docs.getunleash.io/unleash-client-python
 Project-URL: Changelog, https://github.com/Unleash/unleash-client-python/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/Unleash/unleash-client-python
 Project-URL: Issues, https://github.com/Unleash/unleash-client-python/issues
@@ -16,14 +16,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: fcache
+Requires-Dist: mmhash3
+Requires-Dist: apscheduler<4.0.0
+Requires-Dist: importlib_metadata
+Requires-Dist: python-dateutil
+Requires-Dist: semver<4.0.0
 
 # unleash-client-python
 
 ![](https://github.com/unleash/unleash-client-python/workflows/CI/badge.svg?branch=main) [![Coverage Status](https://coveralls.io/repos/github/Unleash/unleash-client-python/badge.svg?branch=main)](https://coveralls.io/github/Unleash/unleash-client-python?branch=main) [![PyPI version](https://badge.fury.io/py/UnleashClient.svg)](https://badge.fury.io/py/UnleashClient) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/UnleashClient.svg) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 
 This is the Python client for [Unleash](https://github.com/unleash/unleash).  It implements [Client Specifications 1.0](https://docs.getunleash.io/client-specification) and checks compliance based on spec in [unleash/client-specifications](https://github.com/Unleash/client-specification)
```

### Comparing `UnleashClient-5.9.1/UnleashClient.egg-info/SOURCES.txt` & `UnleashClient-5.9.2/UnleashClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/Makefile` & `UnleashClient-5.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/celery.rst` & `UnleashClient-5.9.2/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/conf.py` & `UnleashClient-5.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/customcache.rst` & `UnleashClient-5.9.2/docs/customcache.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/customstrategies.rst` & `UnleashClient-5.9.2/docs/customstrategies.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/development.rst` & `UnleashClient-5.9.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/eventcallbacks.rst` & `UnleashClient-5.9.2/docs/eventcallbacks.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/index.rst` & `UnleashClient-5.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/make.bat` & `UnleashClient-5.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/usage.rst` & `UnleashClient-5.9.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/docs/wsgi.rst` & `UnleashClient-5.9.2/docs/wsgi.rst`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/pyproject.toml` & `UnleashClient-5.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/conftest.py` & `UnleashClient-5.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/integration_tests/integration.py` & `UnleashClient-5.9.2/tests/integration_tests/integration.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/integration_tests/integration_gitlab.py` & `UnleashClient-5.9.2/tests/integration_tests/integration_gitlab.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/integration_tests/integration_unleashheroku.py` & `UnleashClient-5.9.2/tests/integration_tests/integration_unleashheroku.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/integration_tests/integration_unleashhosted.py` & `UnleashClient-5.9.2/tests/integration_tests/integration_unleashhosted.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/specification_tests/test_client_specs.py` & `UnleashClient-5.9.2/tests/specification_tests/test_client_specs.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/api/test_feature.py` & `UnleashClient-5.9.2/tests/unit_tests/api/test_feature.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/api/test_metrics.py` & `UnleashClient-5.9.2/tests/unit_tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/api/test_register.py` & `UnleashClient-5.9.2/tests/unit_tests/api/test_register.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py` & `UnleashClient-5.9.2/tests/unit_tests/periodic/test_aggregate_and_send_metrics.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/periodic/test_fetch_and_load.py` & `UnleashClient-5.9.2/tests/unit_tests/periodic/test_fetch_and_load.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/strategies/test_flexiblerollout.py` & `UnleashClient-5.9.2/tests/unit_tests/strategies/test_flexiblerollout.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/strategies/test_remoteaddress.py` & `UnleashClient-5.9.2/tests/unit_tests/strategies/test_remoteaddress.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/strategies/test_strategy_variants.py` & `UnleashClient-5.9.2/tests/unit_tests/strategies/test_strategy_variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "environment": "prod",
         "customField": "1",
     }
     result: EvaluationResult = strategy.get_result(context)
     assert result.enabled
     assert result.variant == {
         "enabled": True,
-        "name": "VarB",
-        "payload": {"type": "string", "value": "Test 2"},
+        "name": "VarC",
+        "payload": {"type": "string", "value": "Test 3"},
     }
 
 
 def test_flexiblerollout_does_not_satisfy_constraints_returns_default_variant(strategy):
     context = {
         "userId": "12234",
         "appName": "test2",
```

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_client.py` & `UnleashClient-5.9.2/tests/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_constraints.py` & `UnleashClient-5.9.2/tests/unit_tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_custom_strategy.py` & `UnleashClient-5.9.2/tests/unit_tests/test_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_features.py` & `UnleashClient-5.9.2/tests/unit_tests/test_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,29 +103,29 @@
     assert isinstance(selected_variant, dict)
     assert selected_variant["name"] == "disabled"
 
 
 def test_select_variation_variation(test_feature_variants):
     selected_variant = test_feature_variants.get_variant({"userId": "2"})
     assert selected_variant["enabled"]
-    assert selected_variant["name"] == "VarB"
+    assert selected_variant["name"] == "VarC"
 
 
 def test_variant_metrics_are_reset(test_feature_variants):
     test_feature_variants.get_variant({"userId": "2"})
-    assert test_feature_variants.variant_counts["VarB"] == 1
+    assert test_feature_variants.variant_counts["VarC"] == 1
 
     test_feature_variants.reset_stats()
     assert not test_feature_variants.variant_counts
 
 
 def test_variant_metrics_with_existing_variant(test_feature_variants):
     for iteration in range(1, 7):
         test_feature_variants.get_variant({"userId": "2"})
-        assert test_feature_variants.variant_counts["VarB"] == iteration
+        assert test_feature_variants.variant_counts["VarC"] == iteration
 
 
 def test_variant_metrics_with_disabled_feature(test_feature_variants):
     test_feature_variants.enabled = False
     assert not test_feature_variants.is_enabled()
     for iteration in range(1, 7):
         test_feature_variants.get_variant({})
@@ -145,16 +145,16 @@
         "environment": "prod",
         "customField": "1",
     }
     variant = test_feature_strategy_variants.get_variant(context)
 
     assert variant == {
         "enabled": True,
-        "name": "VarB",
-        "payload": {"type": "string", "value": "Test 2"},
+        "name": "VarC",
+        "payload": {"type": "string", "value": "Test 3"},
     }
 
 
 def test_dependencies(test_feature_dependencies):
     assert isinstance(test_feature_dependencies.dependencies, list)
     assert all(
         isinstance(item, dict) for item in test_feature_dependencies.dependencies
```

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_loader.py` & `UnleashClient-5.9.2/tests/unit_tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/unit_tests/test_variants.py` & `UnleashClient-5.9.2/tests/unit_tests/test_variants.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     assert context["customField"] == variations._get_seed(context, "customField")
 
 
 def test_variation_selectvariation_happypath(variations):
     variant = variations.get_variant({"userId": "2"})
     assert variant
     assert "payload" in variant
-    assert variant["name"] == "VarC"
+    assert variant["name"] == "VarA"
 
 
 def test_variation_customvariation(variations_with_stickiness):
     variations = variations_with_stickiness
     variant = variations.get_variant({"customField": "ActuallyAmAHamster1234"})
     assert variant
     assert "payload" in variant
```

### Comparing `UnleashClient-5.9.1/tests/utilities/mocks/mock_all_features.py` & `UnleashClient-5.9.2/tests/utilities/mocks/mock_all_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/mocks/mock_constraints.py` & `UnleashClient-5.9.2/tests/utilities/mocks/mock_constraints.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/mocks/mock_custom_strategy.py` & `UnleashClient-5.9.2/tests/utilities/mocks/mock_custom_strategy.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/mocks/mock_features.py` & `UnleashClient-5.9.2/tests/utilities/mocks/mock_features.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/mocks/mock_variants.py` & `UnleashClient-5.9.2/tests/utilities/mocks/mock_variants.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/old_code/StrategyV2.py` & `UnleashClient-5.9.2/tests/utilities/old_code/StrategyV2.py`

 * *Files identical despite different names*

### Comparing `UnleashClient-5.9.1/tests/utilities/testing_constants.py` & `UnleashClient-5.9.2/tests/utilities/testing_constants.py`

 * *Files identical despite different names*

