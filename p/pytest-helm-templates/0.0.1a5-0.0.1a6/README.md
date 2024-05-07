# Comparing `tmp/pytest_helm_templates-0.0.1a5.tar.gz` & `tmp/pytest_helm_templates-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_helm_templates-0.0.1a5.tar", last modified: Tue May  7 13:50:04 2024, max compression
+gzip compressed data, was "pytest_helm_templates-0.0.1a6.tar", last modified: Tue May  7 17:02:48 2024, max compression
```

## Comparing `pytest_helm_templates-0.0.1a5.tar` & `pytest_helm_templates-0.0.1a6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.321327 pytest_helm_templates-0.0.1a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/main-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/other-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.321327 pytest_helm_templates-0.0.1a5/.meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/.meta/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 13:50:01.000000 pytest_helm_templates-0.0.1a5/.meta/coverage/badge.svg
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 13:50:01.000000 pytest_helm_templates-0.0.1a5/.meta/coverage/report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/show_values_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/template_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/helm_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/show_values_command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/template_command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/helm_runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 13:49:41.000000 pytest_helm_templates-0.0.1a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.036376 pytest_helm_templates-0.0.1a6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.024376 pytest_helm_templates-0.0.1a6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.024376 pytest_helm_templates-0.0.1a6/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 17:02:44.000000 pytest_helm_templates-0.0.1a6/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 17:02:44.000000 pytest_helm_templates-0.0.1a6/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 17:02:48.036376 pytest_helm_templates-0.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 17:02:47.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/commands/show_values_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/commands/template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/helm_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.032376 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 17:02:47.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-07 17:02:48.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:02:47.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 17:02:47.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 17:02:47.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/commands/show_values_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/commands/template_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/helm_runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.028376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.024376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.032376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.024376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.032376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.032376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:48.032376 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/test-connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 17:02:27.000000 pytest_helm_templates-0.0.1a6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:02:48.036376 pytest_helm_templates-0.0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 17:02:05.000000 pytest_helm_templates-0.0.1a6/whitelist.txt
```

### Comparing `pytest_helm_templates-0.0.1a5/.github/workflows/main-branch.yaml` & `pytest_helm_templates-0.0.1a6/.github/workflows/main-branch.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/.github/workflows/other-branch.yaml` & `pytest_helm_templates-0.0.1a6/.github/workflows/other-branch.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/.github/workflows/release.yaml` & `pytest_helm_templates-0.0.1a6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/.gitignore` & `pytest_helm_templates-0.0.1a6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -157,7 +157,10 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Auto-generated
 pytest_helm_templates/__version__.py
+
+Chart.lock
+*.tgz
```

### Comparing `pytest_helm_templates-0.0.1a5/.meta/coverage/badge.svg` & `pytest_helm_templates-0.0.1a6/.meta/coverage/badge.svg`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/.meta/coverage/report.txt` & `pytest_helm_templates-0.0.1a6/.meta/coverage/report.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name                                                    Stmts   Miss  Cover
 ---------------------------------------------------------------------------
 pytest_helm_templates/__init__.py                           2      0   100%
 pytest_helm_templates/commands/__init__.py                  3      0   100%
 pytest_helm_templates/commands/show_values_command.py      12      0   100%
 pytest_helm_templates/commands/template_command.py         45      0   100%
-pytest_helm_templates/helm_runner.py                       83      6    93%
+pytest_helm_templates/helm_runner.py                       85      6    93%
 ---------------------------------------------------------------------------
-TOTAL                                                     145      6    96%
+TOTAL                                                     147      6    96%
```

### Comparing `pytest_helm_templates-0.0.1a5/.pre-commit-config.yaml` & `pytest_helm_templates-0.0.1a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/LICENSE` & `pytest_helm_templates-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/PKG-INFO` & `pytest_helm_templates-0.0.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Pytest fixtures for unit testing the output of helm templates
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Source, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Tracker, https://github.com/tdg5/pytest-helm-templates/issues
 Classifier: Framework :: Pytest
```

### Comparing `pytest_helm_templates-0.0.1a5/README.md` & `pytest_helm_templates-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pyproject.toml` & `pytest_helm_templates-0.0.1a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/template_command.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates/commands/template_command.py`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates/helm_runner.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates/helm_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,24 @@
             if not isinstance(values_output, Dict):
                 raise ValueError(
                     "Unexpected computed values. Expected dict, got"
                     f" {type(values_output)}: {values_output}"
                 )
             return values_output
 
+    def dependency_build(self, chart: str) -> None:
+        self._run(
+            [
+                "helm",
+                "dependency",
+                "build",
+                chart,
+            ]
+        )
+
     def notes(
         self,
         chart: str,
         name: str,
         api_versions: Optional[List[str]] = None,
         dry_run: Optional[str] = None,
         is_upgrade: Optional[bool] = None,
```

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/PKG-INFO` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Pytest fixtures for unit testing the output of helm templates
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Source, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Tracker, https://github.com/tdg5/pytest-helm-templates/issues
 Classifier: Framework :: Pytest
```

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/SOURCES.txt` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/show_values_command_test.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/commands/show_values_command_test.py`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/template_command_test.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/commands/template_command_test.py`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/helm_runner_test.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/helm_runner_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,30 @@
         "config": True,
         "enabled": True,
         "global": {},
     }
     assert values == expected_values
 
 
+@pytest.mark.parametrize(
+    "use_relative_chart_path",
+    (False, True),
+)
+def test_dependency_build_runs_without_exception(use_relative_chart_path: bool) -> None:
+    test_chart_absolute_path = fixture_path("charts/test-chart")
+    test_chart_path = test_chart_absolute_path
+    charts_path: Optional[str] = None
+    if use_relative_chart_path:
+        charts_path = fixture_path("charts")
+        test_chart_path = path.relpath(test_chart_path, charts_path)
+
+    helm_runner = HelmRunner(cwd=charts_path)
+    helm_runner.dependency_build(chart=test_chart_path)
+
+
 def test_notes_raises_error_if_local_chart_not_found() -> None:
     with pytest.raises(ValueError) as ex:
         HelmRunner().notes(chart="/almost/certainly/not/a/real/path", name="test-chart")
 
     expected_error = "Notes can only be rendered for local charts."
     assert expected_error in str(ex)
```

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/__init__.py` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml` & `pytest_helm_templates-0.0.1a6/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml`

 * *Files identical despite different names*

### Comparing `pytest_helm_templates-0.0.1a5/requirements.txt` & `pytest_helm_templates-0.0.1a6/requirements.txt`

 * *Files identical despite different names*

