# Comparing `tmp/silverback-0.4.1.tar.gz` & `tmp/silverback-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.4.1.tar", last modified: Sat May  4 17:42:22 2024, max compression
+gzip compressed data, was "silverback-0.4.2.tar", last modified: Tue May  7 20:03:19 2024, max compression
```

## Comparing `silverback-0.4.1.tar` & `silverback-0.4.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.978196 silverback-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.978196 silverback-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-04 17:41:26.000000 silverback-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-04 17:41:26.000000 silverback-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-04 17:41:26.000000 silverback-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-04 17:41:26.000000 silverback-0.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-04 17:41:26.000000 silverback-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-04 17:42:22.986196 silverback-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-04 17:41:26.000000 silverback-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-04 17:41:26.000000 silverback-0.4.1/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-04 17:41:26.000000 silverback-0.4.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 17:41:26.000000 silverback-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 17:42:22.986196 silverback-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-04 17:41:26.000000 silverback-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-07 20:02:19.000000 silverback-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-07 20:02:19.000000 silverback-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-07 20:02:19.000000 silverback-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 20:02:19.000000 silverback-0.4.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-07 20:02:19.000000 silverback-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-07 20:03:19.032619 silverback-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-07 20:02:19.000000 silverback-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-07 20:02:19.000000 silverback-0.4.2/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-07 20:02:19.000000 silverback-0.4.2/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 20:02:19.000000 silverback-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:03:19.032619 silverback-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-07 20:02:19.000000 silverback-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/test_types.py
```

### Comparing `silverback-0.4.1/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.4.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.4.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.4.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/release-drafter.yml` & `silverback-0.4.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/codeql.yaml` & `silverback-0.4.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/commitlint.yaml` & `silverback-0.4.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/docs.yaml` & `silverback-0.4.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/prtitle.yaml` & `silverback-0.4.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/publish.yaml` & `silverback-0.4.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.github/workflows/test.yaml` & `silverback-0.4.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.gitignore` & `silverback-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/.pre-commit-config.yaml` & `silverback-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/CONTRIBUTING.md` & `silverback-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/Dockerfile` & `silverback-0.4.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/LICENSE` & `silverback-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/PKG-INFO` & `silverback-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.1
+Version: 0.4.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.1/README.md` & `silverback-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/build_docs.py` & `silverback-0.4.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/_static/custom.css` & `silverback-0.4.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/_static/custom.js` & `silverback-0.4.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/_templates/layout.html` & `silverback-0.4.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/conf.py` & `silverback-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/favicon.ico` & `silverback-0.4.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/logo.gif` & `silverback-0.4.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/docs/userguides/development.md` & `silverback-0.4.2/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/example.py` & `silverback-0.4.2/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/pyproject.toml` & `silverback-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/setup.py` & `silverback-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
-        "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
+        # "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24",  # Auto-formatter and linter
+        "mypy>=1.10",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
-        "isort>=5.10.1,<6",  # Import sorting linter
-        "mdformat>=0.7.17",  # Auto-formatter for markdown
-        "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
-        "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
+        "flake8>=7",  # Style linter
+        "isort>=5.13",  # Import sorting linter
+        "mdformat>=0.7",  # Auto-formatter for markdown
+        "mdformat-gfm>=0.3.6",  # Needed for formatting GitHub-flavored markdown
+        "mdformat-frontmatter>=2.0",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "myst-parser>=1.0.0,<2",  # Parse markdown docs
         "sphinx-click>=4.4.0,<5",  # For documenting CLI
         "Sphinx>=6.1.3,<7",  # Documentation generator
         "sphinx_rtd_theme>=1.2.0,<2",  # Readthedocs.org theme
@@ -68,15 +68,15 @@
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
         "eth-ape>=0.7,<1.0",
         "ethpm-types>=0.6.10",  # lower pin only, `eth-ape` governs upper pin
         "eth-pydantic-types",  # Use same version as eth-ape
         "pydantic_settings",  # Use same version as eth-ape
-        "taskiq[metrics]>=0.10.4,<0.11.0",
+        "taskiq[metrics]>=0.11.3,<0.12",
     ],
     entry_points={
         "console_scripts": ["silverback=silverback._cli:cli"],
     },
     python_requires=">=3.10,<4",
     extras_require=extras_require,
     py_modules=["silverback"],
```

### Comparing `silverback-0.4.1/silverback/_cli.py` & `silverback-0.4.2/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/_importer.py` & `silverback-0.4.2/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/application.py` & `silverback-0.4.2/silverback/application.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/exceptions.py` & `silverback-0.4.2/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/middlewares.py` & `silverback-0.4.2/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/recorder.py` & `silverback-0.4.2/silverback/recorder.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/runner.py` & `silverback-0.4.2/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/settings.py` & `silverback-0.4.2/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/state.py` & `silverback-0.4.2/silverback/state.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/subscriptions.py` & `silverback-0.4.2/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/types.py` & `silverback-0.4.2/silverback/types.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback/utils.py` & `silverback-0.4.2/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/silverback.egg-info/PKG-INFO` & `silverback-0.4.2/silverback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.1
+Version: 0.4.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.1/silverback.egg-info/SOURCES.txt` & `silverback-0.4.2/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.4.1/tests/test_types.py` & `silverback-0.4.2/tests/test_types.py`

 * *Files identical despite different names*

