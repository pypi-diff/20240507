# Comparing `tmp/pytest-helm-templates-0.0.1a4.tar.gz` & `tmp/pytest_helm_templates-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-helm-templates-0.0.1a4.tar", last modified: Fri Apr  5 13:07:10 2024, max compression
+gzip compressed data, was "pytest_helm_templates-0.0.1a5.tar", last modified: Tue May  7 13:50:04 2024, max compression
```

## Comparing `pytest-helm-templates-0.0.1a4.tar` & `pytest_helm_templates-0.0.1a5.tar`

### file list

```diff
@@ -1,61 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.192400 pytest-helm-templates-0.0.1a4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.176400 pytest-helm-templates-0.0.1a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.180400 pytest-helm-templates-0.0.1a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/.github/workflows/main-build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/.github/workflows/other-check-quality-and-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.176400 pytest-helm-templates-0.0.1a4/.meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.180400 pytest-helm-templates-0.0.1a4/.meta/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-05 13:07:06.000000 pytest-helm-templates-0.0.1a4/.meta/coverage/badge.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 13:07:06.000000 pytest-helm-templates-0.0.1a4/.meta/coverage/report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 13:07:10.192400 pytest-helm-templates-0.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/commands/template_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/helm_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.188400 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 13:07:10.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/commands/template_command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/helm_runner_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.180400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.184400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.188400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:07:10.188400 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/test-connection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-05 13:06:45.000000 pytest-helm-templates-0.0.1a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:07:10.192400 pytest-helm-templates-0.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 13:06:14.000000 pytest-helm-templates-0.0.1a4/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.321327 pytest_helm_templates-0.0.1a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.321327 pytest_helm_templates-0.0.1a5/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 13:50:01.000000 pytest_helm_templates-0.0.1a5/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 13:50:01.000000 pytest_helm_templates-0.0.1a5/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/show_values_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/template_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/helm_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 13:50:04.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/show_values_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/template_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/helm_runner_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.329327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.325327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:50:04.333327 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/tests/test-connection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-07 13:49:41.000000 pytest_helm_templates-0.0.1a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:50:04.337328 pytest_helm_templates-0.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 13:49:11.000000 pytest_helm_templates-0.0.1a5/whitelist.txt
```

### Comparing `pytest-helm-templates-0.0.1a4/.github/workflows/main-build-and-publish.yml` & `pytest_helm_templates-0.0.1a5/.github/workflows/main-branch.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 name: Test, build, and publish the package
 
 on:
   push:
     branches: [main]
 
 jobs:
-  test-build-and-publish:
+  test-and-build-and-update-metadata:
     name: Test, build, and publish the package
     runs-on: ubuntu-latest
 
     steps:
       - name: Check out code
         uses: actions/checkout@v3
         with:
           token: ${{ secrets.PAT_GITHUB_ACTIONS }}
 
       - uses: actions/setup-python@v4
         with:
+          cache: pip
           python-version: '3.9'
 
       - name: Install dependencies
         run: |
           python -m venv venv
           source venv/bin/activate
           pip install -r requirements.txt
 
       - name: Check requirements.txt is up to date
         run: |
           source venv/bin/activate
           pip install .[all]
           pip uninstall -y pytest-helm-templates
           pip freeze > requirements.txt
+
           if ! `git diff --quiet`; then
             echo "pip freeze caused file changes, failing!"
+            git diff
             exit 1
           fi
 
       - name: Check style
         run: |
           source venv/bin/activate
           make style
+
           if ! `git diff --quiet`; then
             echo "make style caused file changes, failing!"
+            git diff
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           coverage run -m pytest
           coverage report | tee .meta/coverage/report.txt
           coverage-badge -f -o .meta/coverage/badge.svg
-          export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_PYTEST_HELM_TEMPLATES="$(cat VERSION)"
           python -m build
 
       - name: Checkout tdg5/github-action-pack
         uses: actions/checkout@v4
         with:
           path: .github/actions/tdg5/github-action-pack
           ref: v0.0.5
@@ -66,33 +70,7 @@
         with:
           authorEmail: dannyguinther+spamburglar@gmail.com
           authorName: Spamburglar
           commitMessage: "[skip actions] Update code coverage snapshot"
           optionalFilePaths: |
             .meta/coverage/badge.svg
             .meta/coverage/report.txt
-
-      - name: Increment version
-        uses: ./.github/actions/tdg5/github-action-pack/packages/increment-version-file-action/src
-        with:
-          authorEmail: dannyguinther+spamburglar@gmail.com
-          authorName: Spamburglar
-          commitMessage: "[skip actions] Increment version for next development cycle"
-          versionFilePath: VERSION
-          versionFormat: python
-
-      - name: Publish package to pypi
-        env:
-          TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
-          TWINE_USERNAME: __token__
-        run: |
-          source venv/bin/activate
-          python -m twine upload dist/*
-
-      # Add the tag after publishing the package so it is more likely that we
-      # end up with a package without a tag than a tag without a package.
-      - name: Create and push tag for published version
-        run: |
-          VERSION="$(git show HEAD~1:VERSION)"
-          TAG_NAME="v${VERSION}"
-          git tag "$TAG_NAME" HEAD~1
-          git push origin "$TAG_NAME"
```

### Comparing `pytest-helm-templates-0.0.1a4/.github/workflows/other-check-quality-and-tests.yml` & `pytest_helm_templates-0.0.1a5/.github/workflows/other-branch.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     steps:
       - name: Check out code
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
+          cache: pip
           python-version: '3.9'
 
       - name: Install dependencies
         run: |
           python -m venv venv
           source venv/bin/activate
           pip install -r requirements.txt
@@ -44,9 +45,8 @@
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           coverage run -m pytest
           coverage report
-          export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_PYTEST_HELM_TEMPLATES="$(cat VERSION)"
           python -m build
```

### Comparing `pytest-helm-templates-0.0.1a4/.gitignore` & `pytest_helm_templates-0.0.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/.meta/coverage/badge.svg` & `pytest_helm_templates-0.0.1a5/.meta/coverage/badge.svg`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/.pre-commit-config.yaml` & `pytest_helm_templates-0.0.1a5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         files: requirements.txt
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
       - id: end-of-file-fixer
-        exclude: README.md|VERSION
+        exclude: README.md
       - id: check-docstring-first
       - id: debug-statements
       - id: name-tests-test
         args: ["--pytest-test-first"]
         exclude: factories.py
       - id: requirements-txt-fixer
       - id: check-toml
```

### Comparing `pytest-helm-templates-0.0.1a4/LICENSE` & `pytest_helm_templates-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/PKG-INFO` & `pytest_helm_templates-0.0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Pytest fixtures for unit testing the output of helm templates
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Source, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Tracker, https://github.com/tdg5/pytest-helm-templates/issues
 Classifier: Framework :: Pytest
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: dev
-Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: black~=24.3; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: coverage~=7.4.4; extra == "dev"
 Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
 Requires-Dist: dlint~=0.14.1; extra == "dev"
 Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
 Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
```

### Comparing `pytest-helm-templates-0.0.1a4/README.md` & `pytest_helm_templates-0.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pyproject.toml` & `pytest_helm_templates-0.0.1a5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 license = {text = "MIT"}
 name = "pytest-helm-templates"
 readme = "README.md"
 requires-python = ">3.9.0"
 
 [project.optional-dependencies]
 dev = [
-  "black~=24.2.0",
+  "black~=24.3",
   "build~=1.0.3",
   "coverage~=7.4.4",
   "coverage-badge~=1.1.0",
   "dlint~=0.14.1",
   "flake8-comprehensions~=3.14.0",
   "flake8-eradicate~=1.5.0",
   "flake8-pyproject~=1.2.3",
@@ -62,14 +62,25 @@
 Tracker = "https://github.com/tdg5/pytest-helm-templates/issues"
 
 [tool.black]
 include = "pytest_helm_templates(_test)?/.*\\.py$"
 line-length = 88
 target-version = ["py39"]
 
+[tool.coverage.run]
+omit = [
+  "pytest_helm_templates/__version__.py",
+]
+source = [
+  "pytest_helm_templates",
+]
+
+[tool.coverage.report]
+fail_under = 96
+
 [tool.flake8]
 ignore = ["E203", "E251", "E701", "N805", "W503", "DAR101", "DAR201", "DAR301", "DAR401"]
 max-line-length = 88
 min_python_version = 3.9
 
 [tool.isort]
 include_trailing_comma = true
```

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates/commands/template_command.py` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates/commands/template_command.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/PKG-INFO` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-helm-templates
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Pytest fixtures for unit testing the output of helm templates
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Source, https://github.com/tdg5/pytest-helm-templates
 Project-URL: Tracker, https://github.com/tdg5/pytest-helm-templates/issues
 Classifier: Framework :: Pytest
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: dev
-Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: black~=24.3; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: coverage~=7.4.4; extra == "dev"
 Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
 Requires-Dist: dlint~=0.14.1; extra == "dev"
 Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
 Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
```

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates.egg-info/SOURCES.txt` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 .gitignore
 .pre-commit-config.yaml
 .safety-policy.yml
 LICENSE
 Makefile
 README.md
-VERSION
 pyproject.toml
 requirements.txt
 whitelist.txt
-.github/workflows/main-build-and-publish.yml
-.github/workflows/other-check-quality-and-tests.yml
+.github/workflows/main-branch.yaml
+.github/workflows/other-branch.yaml
+.github/workflows/release.yaml
 .meta/coverage/badge.svg
 .meta/coverage/report.txt
 pytest_helm_templates/__init__.py
 pytest_helm_templates/__version__.py
 pytest_helm_templates/helm_runner.py
 pytest_helm_templates/py.typed
 pytest_helm_templates.egg-info/PKG-INFO
 pytest_helm_templates.egg-info/SOURCES.txt
 pytest_helm_templates.egg-info/dependency_links.txt
 pytest_helm_templates.egg-info/requires.txt
 pytest_helm_templates.egg-info/top_level.txt
 pytest_helm_templates/commands/__init__.py
+pytest_helm_templates/commands/show_values_command.py
 pytest_helm_templates/commands/template_command.py
 pytest_helm_templates_test/__init__.py
 pytest_helm_templates_test/conftest.py
 pytest_helm_templates_test/helm_runner_test.py
+pytest_helm_templates_test/commands/show_values_command_test.py
 pytest_helm_templates_test/commands/template_command_test.py
 pytest_helm_templates_test/test_helpers/__init__.py
 pytest_helm_templates_test/test_helpers/py.typed
 pytest_helm_templates_test/test_helpers/fixtures/__init__.py
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/.helmignore
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/Chart.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml
+pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/Chart.yaml
+pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/charts/dependency/values.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/service.yaml
 pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/serviceaccount.yaml
```

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/commands/template_command_test.py` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/commands/template_command_test.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/__init__.py` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `pytest-helm-templates-0.0.1a4/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml` & `pytest_helm_templates-0.0.1a5/pytest_helm_templates_test/test_helpers/fixtures/charts/test-chart/values.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Default values for test-chart.
 # This is a YAML-formatted file.
 # Declare variables to be passed into your templates.
 
+dependency:
+  enabled: false
+
 replicaCount: 1
 
 image:
   repository: nginx
   pullPolicy: IfNotPresent
   # Overrides the image tag whose default is the chart appVersion.
   tag: ""
```

### Comparing `pytest-helm-templates-0.0.1a4/requirements.txt` & `pytest_helm_templates-0.0.1a5/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 attrs==23.2.0
-black==24.2.0
+black==24.4.2
 build==1.0.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 charset-normalizer==3.3.2
 click==8.1.7
 coverage==7.4.4
```

