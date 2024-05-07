# Comparing `tmp/simple-ubl-invoice-generator-0.2.0.tar.gz` & `tmp/simple-ubl-invoice-generator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-ubl-invoice-generator-0.2.0.tar", last modified: Tue Apr  9 12:44:57 2024, max compression
+gzip compressed data, was "simple-ubl-invoice-generator-0.3.0.tar", last modified: Tue May  7 15:43:07 2024, max compression
```

## Comparing `simple-ubl-invoice-generator-0.2.0.tar` & `simple-ubl-invoice-generator-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.574445 simple-ubl-invoice-generator-0.2.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      625 2024-04-09 12:44:41.000000 simple-ubl-invoice-generator-0.2.0/.bumpversion.cfg
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2181 2024-04-09 12:44:41.000000 simple-ubl-invoice-generator-0.2.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      196 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.569445 simple-ubl-invoice-generator-0.2.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.571445 simple-ubl-invoice-generator-0.2.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1474 2024-04-08 17:03:40.000000 simple-ubl-invoice-generator-0.2.0/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      686 2024-04-08 15:29:21.000000 simple-ubl-invoice-generator-0.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/AUTHORS.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      231 2024-04-09 12:44:12.000000 simple-ubl-invoice-generator-0.2.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2517 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1332 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      402 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3087 2024-04-09 12:44:57.574445 simple-ubl-invoice-generator-0.2.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3408 2024-04-09 12:44:41.000000 simple-ubl-invoice-generator-0.2.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.571445 simple-ubl-invoice-generator-0.2.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.569445 simple-ubl-invoice-generator-0.2.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.569445 simple-ubl-invoice-generator-0.2.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.571445 simple-ubl-invoice-generator-0.2.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1953 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/ci/templates/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1354 2024-04-08 12:21:11.000000 simple-ubl-invoice-generator-0.2.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      968 2024-04-08 16:31:31.000000 simple-ubl-invoice-generator-0.2.0/pytest.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-09 12:44:57.574445 simple-ubl-invoice-generator-0.2.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2908 2024-04-09 12:44:41.000000 simple-ubl-invoice-generator-0.2.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.569445 simple-ubl-invoice-generator-0.2.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.572445 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-09 12:44:41.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      402 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/__main__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2158 2024-04-08 16:43:06.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/cli.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3138 2024-04-09 12:39:30.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/core.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)     4909 2024-04-09 12:17:48.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/template.xml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1413 2024-04-09 12:31:39.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/types.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)       86 2024-04-08 16:28:33.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/utils.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.574445 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3087 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1225 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/SOURCES.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/dependency_links.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       64 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/entry_points.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-09 12:44:56.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/not-zip-safe
--rw-r--r--   0 ionel     (1000) ionel     (1000)       17 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/requires.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       29 2024-04-09 12:44:57.000000 simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-09 12:44:57.574445 simple-ubl-invoice-generator-0.2.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)      126 2024-04-08 15:41:04.000000 simple-ubl-invoice-generator-0.2.0/tests/conftest.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      484 2024-04-09 12:00:48.000000 simple-ubl-invoice-generator-0.2.0/tests/test_all_defaults.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      536 2024-04-08 16:43:06.000000 simple-ubl-invoice-generator-0.2.0/tests/test_cli.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    15018 2024-04-09 12:39:30.000000 simple-ubl-invoice-generator-0.2.0/tests/test_core.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      740 2024-04-09 12:31:05.000000 simple-ubl-invoice-generator-0.2.0/tests/test_filename.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      434 2024-04-09 12:13:12.000000 simple-ubl-invoice-generator-0.2.0/tests/test_no_customer_match_1.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      295 2024-04-09 12:13:12.000000 simple-ubl-invoice-generator-0.2.0/tests/test_no_customer_match_2.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      455 2024-04-09 12:13:12.000000 simple-ubl-invoice-generator-0.2.0/tests/test_no_defaults.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1247 2024-04-08 12:21:29.000000 simple-ubl-invoice-generator-0.2.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.452802 simple-ubl-invoice-generator-0.3.0/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      625 2024-05-07 15:43:04.000000 simple-ubl-invoice-generator-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2181 2024-05-07 15:43:04.000000 simple-ubl-invoice-generator-0.3.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      196 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.448802 simple-ubl-invoice-generator-0.3.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.450802 simple-ubl-invoice-generator-0.3.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1474 2024-04-08 17:03:40.000000 simple-ubl-invoice-generator-0.3.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      686 2024-04-08 15:29:21.000000 simple-ubl-invoice-generator-0.3.0/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/AUTHORS.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      335 2024-05-07 15:42:29.000000 simple-ubl-invoice-generator-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2517 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     1332 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      402 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3190 2024-05-07 15:43:07.452802 simple-ubl-invoice-generator-0.3.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3408 2024-05-07 15:43:04.000000 simple-ubl-invoice-generator-0.3.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.450802 simple-ubl-invoice-generator-0.3.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/ci/bootstrap.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.448802 simple-ubl-invoice-generator-0.3.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.448802 simple-ubl-invoice-generator-0.3.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.450802 simple-ubl-invoice-generator-0.3.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1953 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1354 2024-04-08 12:21:11.000000 simple-ubl-invoice-generator-0.3.0/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      968 2024-04-08 16:31:31.000000 simple-ubl-invoice-generator-0.3.0/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-05-07 15:43:07.452802 simple-ubl-invoice-generator-0.3.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2907 2024-05-07 15:43:04.000000 simple-ubl-invoice-generator-0.3.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.448802 simple-ubl-invoice-generator-0.3.0/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.451802 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-05-07 15:43:04.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      402 2024-04-08 11:31:49.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2163 2024-04-17 14:07:18.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/cli.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2547 2024-04-17 20:15:20.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/generator.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2693 2024-04-17 20:13:09.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/schema.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4921 2024-04-17 20:11:48.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/template.xml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       86 2024-04-17 18:49:33.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/utils.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.452802 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3190 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1317 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       64 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-05-07 15:43:06.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       16 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       29 2024-05-07 15:43:07.000000 simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-05-07 15:43:07.452802 simple-ubl-invoice-generator-0.3.0/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      126 2024-04-08 15:41:04.000000 simple-ubl-invoice-generator-0.3.0/tests/conftest.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      533 2024-04-17 18:57:13.000000 simple-ubl-invoice-generator-0.3.0/tests/test_cli.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    16558 2024-04-17 19:46:02.000000 simple-ubl-invoice-generator-0.3.0/tests/test_core.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      740 2024-04-17 18:36:38.000000 simple-ubl-invoice-generator-0.3.0/tests/test_filename.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      484 2024-04-09 12:00:48.000000 simple-ubl-invoice-generator-0.3.0/tests/test_generation_all_defaults.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      455 2024-04-09 12:13:12.000000 simple-ubl-invoice-generator-0.3.0/tests/test_generation_no_defaults.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      300 2024-04-17 18:38:56.000000 simple-ubl-invoice-generator-0.3.0/tests/test_validation_missing_fields.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      551 2024-04-17 16:58:39.000000 simple-ubl-invoice-generator-0.3.0/tests/test_validation_no_customer_match_1.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      295 2024-04-09 12:13:12.000000 simple-ubl-invoice-generator-0.3.0/tests/test_validation_no_customer_match_2.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1247 2024-04-17 15:16:13.000000 simple-ubl-invoice-generator-0.3.0/tox.ini
```

### Comparing `simple-ubl-invoice-generator-0.2.0/.bumpversion.cfg` & `simple-ubl-invoice-generator-0.3.0/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `simple-ubl-invoice-generator-0.2.0/.cookiecutterrc` & `simple-ubl-invoice-generator-0.3.0/.cookiecutterrc`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "no"
     sphinx_docs_hosting: "https://python-simple-ubl-invoice-generator.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
     tests_inside_package: "no"
-    version: 0.2.0
+    version: 0.3.0
     version_manager: "bump2version"
     website: "https://blog.ionelmc.ro"
     year_from: "2024"
     year_to: "2024"
```

### Comparing `simple-ubl-invoice-generator-0.2.0/.github/workflows/github-actions.yml` & `simple-ubl-invoice-generator-0.3.0/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/.pre-commit-config.yaml` & `simple-ubl-invoice-generator-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/CONTRIBUTING.rst` & `simple-ubl-invoice-generator-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/LICENSE` & `simple-ubl-invoice-generator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/PKG-INFO` & `simple-ubl-invoice-generator-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ubl-invoice-generator
-Version: 0.2.0
+Version: 0.3.0
 Summary: An example package. Generated with cookiecutter-pylibrary.
 Home-page: https://github.com/ionelmc/python-simple-ubl-invoice-generator
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/ionelmc/python-simple-ubl-invoice-generator/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-simple-ubl-invoice-generator/issues
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: typeguard
+Requires-Dist: pydantic
 Requires-Dist: jinja2
 
 ========
 Overview
 ========
 
 
@@ -96,14 +96,20 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.3.0 (2024-05-07)
+------------------
+
+* Changed validation to use Pydantic.
+* Added rounding options.
+
 0.2.0 (2024-04-09)
 ------------------
 
 * Allow customising filename.
 * Improved validation error messages.
 * Renamed some configuration fields.
```

### Comparing `simple-ubl-invoice-generator-0.2.0/README.rst` & `simple-ubl-invoice-generator-0.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/simple-ubl-invoice-generator
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/simple-ubl-invoice-generator.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/simple-ubl-invoice-generator
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-simple-ubl-invoice-generator/v0.2.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-simple-ubl-invoice-generator/v0.3.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-simple-ubl-invoice-generator/compare/v0.2.0...main
+    :target: https://github.com/ionelmc/python-simple-ubl-invoice-generator/compare/v0.3.0...main
 
 .. end-badges
 
 An example package. Generated with cookiecutter-pylibrary.
 
 * Free software: BSD 2-Clause License
```

### Comparing `simple-ubl-invoice-generator-0.2.0/ci/bootstrap.py` & `simple-ubl-invoice-generator-0.3.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/ci/templates/.github/workflows/github-actions.yml` & `simple-ubl-invoice-generator-0.3.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/pyproject.toml` & `simple-ubl-invoice-generator-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/pytest.ini` & `simple-ubl-invoice-generator-0.3.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `simple-ubl-invoice-generator-0.2.0/setup.py` & `simple-ubl-invoice-generator-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="simple-ubl-invoice-generator",
-    version="0.2.0",
+    version="0.3.0",
     license="BSD-2-Clause",
     description="An example package. Generated with cookiecutter-pylibrary.",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Ionel Cristian Mărieș",
@@ -57,15 +57,15 @@
         "Issue Tracker": "https://github.com/ionelmc/python-simple-ubl-invoice-generator/issues",
     },
     keywords=[
         # eg: "keyword1", "keyword2", "keyword3",
     ],
     python_requires=">=3.11",
     install_requires=[
-        "typeguard",
+        "pydantic",
         "jinja2",
     ],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=='3.8'": ["backports.zoneinfo"],
     },
```

### Comparing `simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/cli.py` & `simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import argparse
 import logging
 import tomllib
 from decimal import Decimal
 from pathlib import Path
 
 from . import __version__
-from .core import generate
+from .generator import generate
 from .utils import pformat
 
 logger = logging.getLogger(__name__)
 
 template_path = Path(__file__).parent / "template.xml"
 
 parser = argparse.ArgumentParser(description="Command description.")
```

### Comparing `simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/template.xml` & `simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/template.xml`

 * *Files 0% similar despite different names*

#### Comparing `simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator/template.xml` & `simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator/template.xml`

```diff
@@ -73,15 +73,15 @@
     <cbc:TaxExclusiveAmount currencyID="RON">{{ invoice.total }}</cbc:TaxExclusiveAmount>
     <cbc:TaxInclusiveAmount currencyID="RON">{{ invoice.total }}</cbc:TaxInclusiveAmount>
     <cbc:PayableAmount currencyID="RON">{{ invoice.total }}</cbc:PayableAmount>
   </cac:LegalMonetaryTotal>
   {% for line in invoice.lines %}
   <cac:InvoiceLine>
     <cbc:ID>{{ loop.index }}</cbc:ID>
-    <cbc:InvoicedQuantity unitCode="HUR">{{ line.amount }}</cbc:InvoicedQuantity>
+    <cbc:InvoicedQuantity unitCode="{{ line.unit }}">{{ line.amount }}</cbc:InvoicedQuantity>
     <cbc:LineExtensionAmount currencyID="RON">{{ line.total }}</cbc:LineExtensionAmount>
     <cac:Item>
       <cbc:Name>{{ line.service }}</cbc:Name>
       <cac:ClassifiedTaxCategory>
         <cbc:ID>O</cbc:ID>
         <cac:TaxScheme>
           <cbc:ID>VAT</cbc:ID>
```

### Comparing `simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/PKG-INFO` & `simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ubl-invoice-generator
-Version: 0.2.0
+Version: 0.3.0
 Summary: An example package. Generated with cookiecutter-pylibrary.
 Home-page: https://github.com/ionelmc/python-simple-ubl-invoice-generator
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Changelog, https://github.com/ionelmc/python-simple-ubl-invoice-generator/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/ionelmc/python-simple-ubl-invoice-generator/issues
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: typeguard
+Requires-Dist: pydantic
 Requires-Dist: jinja2
 
 ========
 Overview
 ========
 
 
@@ -96,14 +96,20 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+0.3.0 (2024-05-07)
+------------------
+
+* Changed validation to use Pydantic.
+* Added rounding options.
+
 0.2.0 (2024-04-09)
 ------------------
 
 * Allow customising filename.
 * Improved validation error messages.
 * Renamed some configuration fields.
```

### Comparing `simple-ubl-invoice-generator-0.2.0/src/simple_ubl_invoice_generator.egg-info/SOURCES.txt` & `simple-ubl-invoice-generator-0.3.0/src/simple_ubl_invoice_generator.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 src/simple_ubl_invoice_generator/__init__.py
 src/simple_ubl_invoice_generator/__main__.py
 src/simple_ubl_invoice_generator/cli.py
-src/simple_ubl_invoice_generator/core.py
+src/simple_ubl_invoice_generator/generator.py
+src/simple_ubl_invoice_generator/schema.py
 src/simple_ubl_invoice_generator/template.xml
-src/simple_ubl_invoice_generator/types.py
 src/simple_ubl_invoice_generator/utils.py
 src/simple_ubl_invoice_generator.egg-info/PKG-INFO
 src/simple_ubl_invoice_generator.egg-info/SOURCES.txt
 src/simple_ubl_invoice_generator.egg-info/dependency_links.txt
 src/simple_ubl_invoice_generator.egg-info/entry_points.txt
 src/simple_ubl_invoice_generator.egg-info/not-zip-safe
 src/simple_ubl_invoice_generator.egg-info/requires.txt
 src/simple_ubl_invoice_generator.egg-info/top_level.txt
 tests/conftest.py
-tests/test_all_defaults.toml
 tests/test_cli.py
 tests/test_core.py
 tests/test_filename.toml
-tests/test_no_customer_match_1.toml
-tests/test_no_customer_match_2.toml
-tests/test_no_defaults.toml
+tests/test_generation_all_defaults.toml
+tests/test_generation_no_defaults.toml
+tests/test_validation_missing_fields.toml
+tests/test_validation_no_customer_match_1.toml
+tests/test_validation_no_customer_match_2.toml
```

### Comparing `simple-ubl-invoice-generator-0.2.0/tests/test_cli.py` & `simple-ubl-invoice-generator-0.3.0/tests/test_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 def test_version():
     assert subprocess.check_output(["sublig", "--version"], text=True).startswith("sublig v")
 
 
 def test_bad_template(tmp_path, tests_path):
     with pytest.raises(subprocess.CalledProcessError) as exc:
         subprocess.check_output(
-            ["sublig", f"--template={tmp_path / 'foobar'}", tests_path / "test_no_defaults.toml"], text=True, stderr=subprocess.STDOUT
+            ["sublig", f"--template={tmp_path / 'foobar'}", tests_path / "test_filename.toml"], text=True, stderr=subprocess.STDOUT
         )
-    assert exc.value.returncode == 1
     assert exc.value.stdout.endswith("foobar does not exist.")
+    assert exc.value.returncode == 1
```

### Comparing `simple-ubl-invoice-generator-0.2.0/tests/test_core.py` & `simple-ubl-invoice-generator-0.3.0/tests/test_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,63 @@
 import tomllib
+import traceback
 from decimal import Decimal
-from operator import itemgetter
 
 import pytest
+from pydantic.version import version_short
 
 from simple_ubl_invoice_generator.cli import template_path
-from simple_ubl_invoice_generator.core import ValidationError
-from simple_ubl_invoice_generator.core import generate
+from simple_ubl_invoice_generator.generator import ConfigError
+from simple_ubl_invoice_generator.generator import generate
+
+pydantic_version = version_short()
 
 
 @pytest.mark.parametrize(
     ("config", "error"),
     [
-        ("test_no_customer_match_1.toml", "Failed processing FACT001: Missing customer field."),
-        ("test_no_customer_match_2.toml", "Failed processing FACT001: Customer 'blabla' not in customers table."),
+        ("test_validation_no_customer_match_1.toml", "Failed processing FACT001: Missing customer field."),
+        ("test_validation_no_customer_match_2.toml", "Failed processing FACT001: Customer 'blabla' not in customers table."),
+        (
+            "test_validation_missing_fields.toml",
+            """Failed validating config {'supplier': {'street': 'asdf street', 'city': 'asdf city', 'county': 'asdf county', 'country': 'asdf country', 'fiscal_id': '1234', 'name': 'ASDF S.R.L.'}, 'invoices': {'FACT002': {'customer': {'street': 'qwer street', 'city': 'qwer city', 'county': 'qwer county', 'country': 'qwer country', 'fiscal_id': 'RO234', 'name': 'QWER S.R.L'}}}}: 3 validation errors for Config
+invoices.FACT002.date
+  Field required [type=missing, input_value={'customer': {'street': '..., 'name': 'QWER S.R.L'}}, input_type=dict]"""
+            f"""
+    For further information visit https://errors.pydantic.dev/{pydantic_version}/v/missing"""
+            """
+invoices.FACT002.lines
+  Field required [type=missing, input_value={'customer': {'street': '..., 'name': 'QWER S.R.L'}}, input_type=dict]"""
+            f"""
+    For further information visit https://errors.pydantic.dev/{pydantic_version}/v/missing"""
+            """
+supplier.iban
+  Field required [type=missing, input_value={'street': 'asdf street',..., 'name': 'ASDF S.R.L.'}, input_type=dict]"""
+            f"""
+    For further information visit https://errors.pydantic.dev/{pydantic_version}/v/missing""",
+        ),
+    ],
+    ids=[
+        "no_customer_match_1",
+        "no_customer_match_2",
+        "missing_fields",
     ],
-    ids=itemgetter(0),
 )
-def test_no_customer_match(tmp_path, tests_path, config, error):
-    with pytest.raises(ValidationError) as exc:
+def test_validation(tmp_path, tests_path, config, error):
+    with pytest.raises(ConfigError) as exc:
         generate(template_path, tomllib.loads(tests_path.joinpath(config).read_text(), parse_float=Decimal), tmp_path)
+    traceback.print_exception(exc.value)
     assert str(exc.value) == error
 
 
 @pytest.mark.parametrize(
     "config",
     [
-        "test_no_defaults.toml",
-        "test_all_defaults.toml",
+        "test_generation_no_defaults.toml",
+        "test_generation_all_defaults.toml",
     ],
 )
 def test_generation(tmp_path, tests_path, config):
     generate(template_path, tomllib.loads(tests_path.joinpath(config).read_text(), parse_float=Decimal), tmp_path)
     assert (
         tmp_path.joinpath("FACT001.xml").read_text()
         == """<?xml version="1.0" encoding="UTF-8"?>
@@ -92,31 +118,31 @@
     </cac:PaymentMeans>
     <cac:PaymentTerms>
         <cbc:Note></cbc:Note>
     </cac:PaymentTerms>
     <cac:TaxTotal>
         <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
         <cac:TaxSubtotal>
-            <cbc:TaxableAmount currencyID="RON">1230</cbc:TaxableAmount>
+            <cbc:TaxableAmount currencyID="RON">1230.00</cbc:TaxableAmount>
             <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
             <cac:TaxCategory>
                 <cbc:ID>O</cbc:ID>
                 <cbc:Percent>0.00</cbc:Percent>
                 <cbc:TaxExemptionReasonCode>VATEX-EU-O</cbc:TaxExemptionReasonCode>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:TaxCategory>
         </cac:TaxSubtotal>
     </cac:TaxTotal>
     <cac:LegalMonetaryTotal>
-        <cbc:LineExtensionAmount currencyID="RON">1230</cbc:LineExtensionAmount>
-        <cbc:TaxExclusiveAmount currencyID="RON">1230</cbc:TaxExclusiveAmount>
-        <cbc:TaxInclusiveAmount currencyID="RON">1230</cbc:TaxInclusiveAmount>
-        <cbc:PayableAmount currencyID="RON">1230</cbc:PayableAmount>
+        <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
+        <cbc:TaxExclusiveAmount currencyID="RON">1230.00</cbc:TaxExclusiveAmount>
+        <cbc:TaxInclusiveAmount currencyID="RON">1230.00</cbc:TaxInclusiveAmount>
+        <cbc:PayableAmount currencyID="RON">1230.00</cbc:PayableAmount>
     </cac:LegalMonetaryTotal>
     <cac:InvoiceLine>
         <cbc:ID>1</cbc:ID>
         <cbc:InvoicedQuantity unitCode="HUR">10</cbc:InvoicedQuantity>
         <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
         <cac:Item>
             <cbc:Name>Service</cbc:Name>
@@ -124,15 +150,15 @@
                 <cbc:ID>O</cbc:ID>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:ClassifiedTaxCategory>
         </cac:Item>
         <cac:Price>
-            <cbc:PriceAmount currencyID="RON">123.00</cbc:PriceAmount>
+            <cbc:PriceAmount currencyID="RON">123.0000</cbc:PriceAmount>
         </cac:Price>
     </cac:InvoiceLine>
 </Invoice>
 """
     )
 
 
@@ -202,31 +228,31 @@
     </cac:PaymentMeans>
     <cac:PaymentTerms>
         <cbc:Note></cbc:Note>
     </cac:PaymentTerms>
     <cac:TaxTotal>
         <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
         <cac:TaxSubtotal>
-            <cbc:TaxableAmount currencyID="RON">1230</cbc:TaxableAmount>
+            <cbc:TaxableAmount currencyID="RON">1230.00</cbc:TaxableAmount>
             <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
             <cac:TaxCategory>
                 <cbc:ID>O</cbc:ID>
                 <cbc:Percent>0.00</cbc:Percent>
                 <cbc:TaxExemptionReasonCode>VATEX-EU-O</cbc:TaxExemptionReasonCode>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:TaxCategory>
         </cac:TaxSubtotal>
     </cac:TaxTotal>
     <cac:LegalMonetaryTotal>
-        <cbc:LineExtensionAmount currencyID="RON">1230</cbc:LineExtensionAmount>
-        <cbc:TaxExclusiveAmount currencyID="RON">1230</cbc:TaxExclusiveAmount>
-        <cbc:TaxInclusiveAmount currencyID="RON">1230</cbc:TaxInclusiveAmount>
-        <cbc:PayableAmount currencyID="RON">1230</cbc:PayableAmount>
+        <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
+        <cbc:TaxExclusiveAmount currencyID="RON">1230.00</cbc:TaxExclusiveAmount>
+        <cbc:TaxInclusiveAmount currencyID="RON">1230.00</cbc:TaxInclusiveAmount>
+        <cbc:PayableAmount currencyID="RON">1230.00</cbc:PayableAmount>
     </cac:LegalMonetaryTotal>
     <cac:InvoiceLine>
         <cbc:ID>1</cbc:ID>
         <cbc:InvoicedQuantity unitCode="HUR">10</cbc:InvoicedQuantity>
         <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
         <cac:Item>
             <cbc:Name>Service</cbc:Name>
@@ -234,15 +260,15 @@
                 <cbc:ID>O</cbc:ID>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:ClassifiedTaxCategory>
         </cac:Item>
         <cac:Price>
-            <cbc:PriceAmount currencyID="RON">123.00</cbc:PriceAmount>
+            <cbc:PriceAmount currencyID="RON">123.0000</cbc:PriceAmount>
         </cac:Price>
     </cac:InvoiceLine>
 </Invoice>
 """
     )
     assert (
         tmp_path.joinpath("2001-01 FACT002.xml").read_text()
@@ -304,31 +330,31 @@
     </cac:PaymentMeans>
     <cac:PaymentTerms>
         <cbc:Note></cbc:Note>
     </cac:PaymentTerms>
     <cac:TaxTotal>
         <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
         <cac:TaxSubtotal>
-            <cbc:TaxableAmount currencyID="RON">1230</cbc:TaxableAmount>
+            <cbc:TaxableAmount currencyID="RON">1230.00</cbc:TaxableAmount>
             <cbc:TaxAmount currencyID="RON">0.00</cbc:TaxAmount>
             <cac:TaxCategory>
                 <cbc:ID>O</cbc:ID>
                 <cbc:Percent>0.00</cbc:Percent>
                 <cbc:TaxExemptionReasonCode>VATEX-EU-O</cbc:TaxExemptionReasonCode>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:TaxCategory>
         </cac:TaxSubtotal>
     </cac:TaxTotal>
     <cac:LegalMonetaryTotal>
-        <cbc:LineExtensionAmount currencyID="RON">1230</cbc:LineExtensionAmount>
-        <cbc:TaxExclusiveAmount currencyID="RON">1230</cbc:TaxExclusiveAmount>
-        <cbc:TaxInclusiveAmount currencyID="RON">1230</cbc:TaxInclusiveAmount>
-        <cbc:PayableAmount currencyID="RON">1230</cbc:PayableAmount>
+        <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
+        <cbc:TaxExclusiveAmount currencyID="RON">1230.00</cbc:TaxExclusiveAmount>
+        <cbc:TaxInclusiveAmount currencyID="RON">1230.00</cbc:TaxInclusiveAmount>
+        <cbc:PayableAmount currencyID="RON">1230.00</cbc:PayableAmount>
     </cac:LegalMonetaryTotal>
     <cac:InvoiceLine>
         <cbc:ID>1</cbc:ID>
         <cbc:InvoicedQuantity unitCode="HUR">10</cbc:InvoicedQuantity>
         <cbc:LineExtensionAmount currencyID="RON">1230.00</cbc:LineExtensionAmount>
         <cac:Item>
             <cbc:Name>Service</cbc:Name>
@@ -336,13 +362,13 @@
                 <cbc:ID>O</cbc:ID>
                 <cac:TaxScheme>
                     <cbc:ID>VAT</cbc:ID>
                 </cac:TaxScheme>
             </cac:ClassifiedTaxCategory>
         </cac:Item>
         <cac:Price>
-            <cbc:PriceAmount currencyID="RON">123.00</cbc:PriceAmount>
+            <cbc:PriceAmount currencyID="RON">123.0000</cbc:PriceAmount>
         </cac:Price>
     </cac:InvoiceLine>
 </Invoice>
 """
     )
```

### Comparing `simple-ubl-invoice-generator-0.2.0/tests/test_filename.toml` & `simple-ubl-invoice-generator-0.3.0/tests/test_filename.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 due = { days = 1 }
 lines = { unit = "HUR", service = "Service" }
 customer = "C1"
 
 [invoices.FACT001]
 correction = true
 date = 2001-01-01
-due = 2001-02-02
+due = 2001-01-02
 lines = [{ amount = 10, price = 123.00 }]
 filename = "{{ date.strftime('%Y-%m') }} {{ id }} {{ customer.name }}.xml"
 
 [invoices.FACT002]
 date = 2001-01-01
-due = 2001-02-02
+due = 2001-01-02
 lines = [{  amount = 10, price = 123.00 }]
```

### Comparing `simple-ubl-invoice-generator-0.2.0/tox.ini` & `simple-ubl-invoice-generator-0.3.0/tox.ini`

 * *Files identical despite different names*

