# Comparing `tmp/behaverse-0.0.2.dev2.tar.gz` & `tmp/behaverse-0.0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.2.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.2.dev4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.2.dev2.tar` & `behaverse-0.0.2.dev4.tar`

### file list

```diff
@@ -1,11 +1,25 @@
--rw-r--r--   0        0        0     1238 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0        6 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/.gitignore
--rw-r--r--   0        0        0      158 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/.pypirc
--rw-r--r--   0        0        0      267 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/LICENSE
--rw-r--r--   0        0        0      352 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/README.md
--rw-r--r--   0        0        0       99 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/environment.yml
--rw-r--r--   0        0        0     1276 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/pyproject.toml
--rw-r--r--   0        0        0       59 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/src/behaverse/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 08:05:14.117584 behaverse-0.0.2.dev2/tests/conftest.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 behaverse-0.0.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1240 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      100 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/LICENSE
+-rw-r--r--   0        0        0      890 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/README.md
+-rw-r--r--   0        0        0       54 2024-05-07 04:17:49.832949 behaverse-0.0.2.dev4/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1392 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/_quarto.yml
+-rw-r--r--   0        0        0     1172 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/getting_started.qmd
+-rw-r--r--   0        0        0      176 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/docs/index.qmd
+-rw-r--r--   0        0        0      209 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/environment.yml
+-rw-r--r--   0        0        0     1627 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/conftest.py
+-rw-r--r--   0        0        0     6773 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset.py
+-rw-r--r--   0        0        0      238 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset_description.py
+-rw-r--r--   0        0        0     1369 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/dataset_test.py
+-rw-r--r--   0        0        0     2487 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/functional.py
+-rw-r--r--   0        0        0       28 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/functions_test.py
+-rw-r--r--   0        0        0     3722 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/utils.py
+-rw-r--r--   0        0        0      178 2024-05-07 04:17:49.836949 behaverse-0.0.2.dev4/src/behaverse/utils_test.py
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 behaverse-0.0.2.dev4/PKG-INFO
```

### Comparing `behaverse-0.0.2.dev2/.github/workflows/pypi-publish.yml` & `behaverse-0.0.2.dev4/.github/workflows/pypi-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Publish Python Package
 
 on:
   release:
     types: [published]
   # push:
   #   branches:
-  #     - main
+  #     - python
 
 permissions:
   contents: read
 
 jobs:
   build:
     name: 📦 Build distribution
```

### Comparing `behaverse-0.0.2.dev2/LICENSE` & `behaverse-0.0.2.dev4/LICENSE`

 * *Files identical despite different names*

