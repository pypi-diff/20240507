# Comparing `tmp/quaxed-0.4.1.tar.gz` & `tmp/quaxed-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Apr 26 20:56:36 2024, max compression
+gzip compressed data, last modified: Tue May  7 20:50:11 2024, max compression
```

## Comparing `quaxed-0.4.1.tar` & `quaxed-0.4.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      380 2024-04-26 20:56:36.000000 quaxed-0.4.1/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-04-26 20:56:36.000000 quaxed-0.4.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-26 20:56:36.000000 quaxed-0.4.1/.gitattributes
--rw-r--r--   0        0        0     2942 2024-04-26 20:56:36.000000 quaxed-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-26 20:56:36.000000 quaxed-0.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     2778 2024-04-26 20:56:36.000000 quaxed-0.4.1/noxfile.py
--rw-r--r--   0        0        0     2387 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1539 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1641 2024-04-26 20:56:36.000000 quaxed-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      834 2024-04-26 20:56:36.000000 quaxed-0.4.1/docs/conf.py
--rw-r--r--   0        0        0      193 2024-04-26 20:56:36.000000 quaxed-0.4.1/docs/index.md
--rw-r--r--   0        0        0     1058 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/__init__.py
--rw-r--r--   0        0        0     1728 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_jax.py
--rw-r--r--   0        0        0      707 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_types.py
--rw-r--r--   0        0        0      231 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_utils.py
--rw-r--r--   0        0        0      411 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_version.py
--rw-r--r--   0        0        0       82 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/_version.pyi
--rw-r--r--   0        0        0      620 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/lax.py
--rw-r--r--   0        0        0      547 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/operator.py
--rw-r--r--   0        0        0     2044 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/operator.pyi
--rw-r--r--   0        0        0        0 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/py.typed
--rw-r--r--   0        0        0     1764 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/__init__.py
--rw-r--r--   0        0        0      145 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_constants.py
--rw-r--r--   0        0        0     7849 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_creation_functions.py
--rw-r--r--   0        0        0      894 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_data_type_functions.py
--rw-r--r--   0        0        0      124 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_dispatch.py
--rw-r--r--   0        0        0     6645 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_elementwise_functions.py
--rw-r--r--   0        0        0      293 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_indexing_functions.py
--rw-r--r--   0        0        0      762 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_linear_algebra_functions.py
--rw-r--r--   0        0        0     1722 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_manipulation_functions.py
--rw-r--r--   0        0        0      778 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_searching_functions.py
--rw-r--r--   0        0        0      636 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_set_functions.py
--rw-r--r--   0        0        0      629 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_sorting_functions.py
--rw-r--r--   0        0        0     1925 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_statistical_functions.py
--rw-r--r--   0        0        0      575 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/_utility_functions.py
--rw-r--r--   0        0        0     3453 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/fft.py
--rw-r--r--   0        0        0     3726 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/array_api/linalg.py
--rw-r--r--   0        0        0      532 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/__init__.py
--rw-r--r--   0        0        0    16627 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/__init__.pyi
--rw-r--r--   0        0        0     9490 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_core.py
--rw-r--r--   0        0        0     5767 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_creation_functions.py
--rw-r--r--   0        0        0      106 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_dispatch.py
--rw-r--r--   0        0        0     7533 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/_higher_order.py
--rw-r--r--   0        0        0       60 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/fft.py
--rw-r--r--   0        0        0       63 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/numpy/linalg.py
--rw-r--r--   0        0        0       84 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/special.py
--rw-r--r--   0        0        0     1925 2024-04-26 20:56:36.000000 quaxed-0.4.1/src/quaxed/scipy/special.pyi
--rw-r--r--   0        0        0       21 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0    38875 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/myarray.py
--rw-r--r--   0        0        0      177 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/test_package.py
--rw-r--r--   0        0        0       31 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/__init__.py
--rw-r--r--   0        0        0     1710 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/test_jax.py
--rw-r--r--   0        0        0    35919 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/array_api/test_myarray.py
--rw-r--r--   0        0        0       27 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/numpy/__init__.py
--rw-r--r--   0        0        0    50679 2024-04-26 20:56:36.000000 quaxed-0.4.1/tests/numpy/test_jax.py
--rw-r--r--   0        0        0     2218 2024-04-26 20:56:36.000000 quaxed-0.4.1/.gitignore
--rw-r--r--   0        0        0     1528 2024-04-26 20:56:36.000000 quaxed-0.4.1/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-26 20:56:36.000000 quaxed-0.4.1/README.md
--rw-r--r--   0        0        0     4339 2024-04-26 20:56:36.000000 quaxed-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3289 2024-04-26 20:56:36.000000 quaxed-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-05-07 20:50:11.000000 quaxed-0.4.2/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-05-07 20:50:11.000000 quaxed-0.4.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-07 20:50:11.000000 quaxed-0.4.2/.gitattributes
+-rw-r--r--   0        0        0     2942 2024-05-07 20:50:11.000000 quaxed-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-07 20:50:11.000000 quaxed-0.4.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2778 2024-05-07 20:50:11.000000 quaxed-0.4.2/noxfile.py
+-rw-r--r--   0        0        0     2387 2024-05-07 20:50:11.000000 quaxed-0.4.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-07 20:50:11.000000 quaxed-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-07 20:50:11.000000 quaxed-0.4.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1539 2024-05-07 20:50:11.000000 quaxed-0.4.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1641 2024-05-07 20:50:11.000000 quaxed-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      834 2024-05-07 20:50:11.000000 quaxed-0.4.2/docs/conf.py
+-rw-r--r--   0        0        0      193 2024-05-07 20:50:11.000000 quaxed-0.4.2/docs/index.md
+-rw-r--r--   0        0        0     1058 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/__init__.py
+-rw-r--r--   0        0        0     1728 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/_jax.py
+-rw-r--r--   0        0        0      707 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/_types.py
+-rw-r--r--   0        0        0      346 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/_utils.py
+-rw-r--r--   0        0        0      411 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/_version.py
+-rw-r--r--   0        0        0       82 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/_version.pyi
+-rw-r--r--   0        0        0      620 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/lax.py
+-rw-r--r--   0        0        0      547 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/operator.py
+-rw-r--r--   0        0        0     2044 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/operator.pyi
+-rw-r--r--   0        0        0        0 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/py.typed
+-rw-r--r--   0        0        0     1764 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_constants.py
+-rw-r--r--   0        0        0     7849 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_creation_functions.py
+-rw-r--r--   0        0        0     1078 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_data_type_functions.py
+-rw-r--r--   0        0        0      124 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_dispatch.py
+-rw-r--r--   0        0        0     6645 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_elementwise_functions.py
+-rw-r--r--   0        0        0      293 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_indexing_functions.py
+-rw-r--r--   0        0        0      762 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_linear_algebra_functions.py
+-rw-r--r--   0        0        0     1722 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_manipulation_functions.py
+-rw-r--r--   0        0        0      778 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_searching_functions.py
+-rw-r--r--   0        0        0      636 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_set_functions.py
+-rw-r--r--   0        0        0      629 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_sorting_functions.py
+-rw-r--r--   0        0        0     1925 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_statistical_functions.py
+-rw-r--r--   0        0        0      575 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/_utility_functions.py
+-rw-r--r--   0        0        0     3453 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/fft.py
+-rw-r--r--   0        0        0     3726 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/array_api/linalg.py
+-rw-r--r--   0        0        0      532 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/__init__.py
+-rw-r--r--   0        0        0    16627 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/__init__.pyi
+-rw-r--r--   0        0        0     9490 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/_core.py
+-rw-r--r--   0        0        0     5767 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/_creation_functions.py
+-rw-r--r--   0        0        0      106 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/_dispatch.py
+-rw-r--r--   0        0        0     7533 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/_higher_order.py
+-rw-r--r--   0        0        0       60 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/fft.py
+-rw-r--r--   0        0        0       63 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/numpy/linalg.py
+-rw-r--r--   0        0        0       84 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/scipy/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/scipy/special.py
+-rw-r--r--   0        0        0     1925 2024-05-07 20:50:11.000000 quaxed-0.4.2/src/quaxed/scipy/special.pyi
+-rw-r--r--   0        0        0       21 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0    38875 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/myarray.py
+-rw-r--r--   0        0        0      177 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/test_package.py
+-rw-r--r--   0        0        0       31 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/array_api/__init__.py
+-rw-r--r--   0        0        0     1710 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/array_api/test_jax.py
+-rw-r--r--   0        0        0    35933 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/array_api/test_myarray.py
+-rw-r--r--   0        0        0       27 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    50679 2024-05-07 20:50:11.000000 quaxed-0.4.2/tests/numpy/test_jax.py
+-rw-r--r--   0        0        0     2218 2024-05-07 20:50:11.000000 quaxed-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1528 2024-05-07 20:50:11.000000 quaxed-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2232 2024-05-07 20:50:11.000000 quaxed-0.4.2/README.md
+-rw-r--r--   0        0        0     4339 2024-05-07 20:50:11.000000 quaxed-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3968 2024-05-07 20:50:11.000000 quaxed-0.4.2/PKG-INFO
```

### Comparing `quaxed-0.4.1/.pre-commit-config.yaml` & `quaxed-0.4.2/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "style: pre-commit fixes"
   autoupdate_schedule: "monthly"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.24.0
+    rev: v3.25.0
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
 
   - repo: meta
     hooks:
@@ -50,15 +50,15 @@
     rev: 0.28.2
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.1"
+    rev: "v0.4.3"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
```

### Comparing `quaxed-0.4.1/noxfile.py` & `quaxed-0.4.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/.github/CONTRIBUTING.md` & `quaxed-0.4.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/.github/matchers/pylint.json` & `quaxed-0.4.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/.github/workflows/cd.yml` & `quaxed-0.4.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/.github/workflows/ci.yml` & `quaxed-0.4.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
       - name: Test package
         run: >-
           python -m pytest tests/ src/ docs/ -ra --cov --cov-report=xml
           --cov-report=term --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.3.0
+        uses: codecov/codecov-action@v4.3.1
```

### Comparing `quaxed-0.4.1/docs/conf.py` & `quaxed-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/__init__.py` & `quaxed-0.4.2/src/quaxed/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/_jax.py` & `quaxed-0.4.2/src/quaxed/_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/_types.py` & `quaxed-0.4.2/src/quaxed/_types.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/lax.py` & `quaxed-0.4.2/src/quaxed/lax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/operator.py` & `quaxed-0.4.2/src/quaxed/operator.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/operator.pyi` & `quaxed-0.4.2/src/quaxed/operator.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/__init__.py` & `quaxed-0.4.2/src/quaxed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_creation_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_data_type_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_data_type_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 __all__ = ["astype", "can_cast", "finfo", "iinfo", "isdtype", "result_type"]
 
 
 from jax.experimental import array_api
-from jax.experimental.array_api._data_type_functions import FInfo, IInfo
+from jax.experimental.array_api._data_type_functions import FInfo
 from jaxtyping import ArrayLike
 
 from quaxed._types import DType
-from quaxed._utils import quaxify
+from quaxed._utils import JAX_VERSION, quaxify
+
+if JAX_VERSION < (0, 4, 27):
+    from jax.experimental.array_api._data_type_functions import IInfo
+else:
+    from jax.experimental.array_api import iinfo as IInfo  # noqa: N812
 
 
 @quaxify
 def astype(x: ArrayLike, dtype: DType, /, *, copy: bool = True) -> ArrayLike:
     return array_api.astype(x, dtype, copy=copy)
```

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_elementwise_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_linear_algebra_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_manipulation_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_searching_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_searching_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_set_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_set_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_sorting_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_sorting_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_statistical_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_statistical_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/_utility_functions.py` & `quaxed-0.4.2/src/quaxed/array_api/_utility_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/fft.py` & `quaxed-0.4.2/src/quaxed/array_api/fft.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/array_api/linalg.py` & `quaxed-0.4.2/src/quaxed/array_api/linalg.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/numpy/__init__.py` & `quaxed-0.4.2/src/quaxed/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/numpy/__init__.pyi` & `quaxed-0.4.2/src/quaxed/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/numpy/_core.py` & `quaxed-0.4.2/src/quaxed/numpy/_core.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/numpy/_creation_functions.py` & `quaxed-0.4.2/src/quaxed/numpy/_creation_functions.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/numpy/_higher_order.py` & `quaxed-0.4.2/src/quaxed/numpy/_higher_order.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/scipy/special.py` & `quaxed-0.4.2/src/quaxed/scipy/special.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/src/quaxed/scipy/special.pyi` & `quaxed-0.4.2/src/quaxed/scipy/special.pyi`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/tests/myarray.py` & `quaxed-0.4.2/tests/myarray.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/tests/array_api/test_jax.py` & `quaxed-0.4.2/tests/array_api/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/tests/array_api/test_myarray.py` & `quaxed-0.4.2/tests/array_api/test_myarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import pytest
 from jax import Array
 from jax._src.numpy.setops import (
     _UniqueAllResult,
     _UniqueCountsResult,
     _UniqueInverseResult,
 )
-from jax.experimental.array_api._data_type_functions import FInfo, IInfo
 
 import quaxed.array_api as xp
+from quaxed.array_api._data_type_functions import FInfo, IInfo
 
 from ..myarray import MyArray
 
 ###############################################################################
 
 # =============================================================================
 # Constants
@@ -231,15 +231,15 @@
 
 def test_iinfo():
     """Test `iinfo`."""
     got = xp.iinfo(jnp.int32)
     expected = jax_xp.iinfo(jnp.int32)
 
     assert isinstance(got, IInfo)
-    for attr in IInfo.__slots__:
+    for attr in ("kind", "bits", "min", "max", "dtype"):
         assert getattr(got, attr) == getattr(expected, attr)
 
 
 def test_isdtype():
     """Test `isdtype`."""
     # True by definition
```

### Comparing `quaxed-0.4.1/tests/numpy/test_jax.py` & `quaxed-0.4.2/tests/numpy/test_jax.py`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/.gitignore` & `quaxed-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/LICENSE` & `quaxed-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/README.md` & `quaxed-0.4.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,8 +27,27 @@
 [rtd-link]:                 https://quaxed.readthedocs.io/en/latest/?badge=latest
 [zenodo-badge]:             https://zenodo.org/badge/732262318.svg
 [zenodo-link]:              https://zenodo.org/doi/10.5281/zenodo.10850521
 
 
 <!-- prettier-ignore-end -->
 
-`Quaxed` is a compatibility layer for `JAX` using `quax`.
+`Quaxed` wraps [jax](https://jax.readthedocs.io/en/latest/) libraries (using
+[`quax`](https://docs.kidger.site/quax/)) to enable using those libraries with
+custom array-ish objects, not only jax arrays.
+
+To understand how `quax` works it's magic, see
+[`quax.quaxify`](https://docs.kidger.site/quax/api/quax/#quax.quaxify) and the
+[tutorials](https://docs.kidger.site/quax/examples/custom_rules/).
+
+To use this library, it's as simple as:
+
+```pycon
+# Import pre-quaxified library
+>>> import quaxed.numpy as qnp  # this is quaxify(jax.numpy)
+
+# As an example, let's import an array-ish object
+>>> from unxt import Quantity
+>>> x = Quantity(2, "km")
+>>> qnp.square(w)
+Quantity['area'](Array(4, dtype=int64, weak_type=True), unit='km2')
+```
```

### Comparing `quaxed-0.4.1/pyproject.toml` & `quaxed-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quaxed-0.4.1/PKG-INFO` & `quaxed-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quaxed
-Version: 0.4.1
+Version: 0.4.2
 Summary: Array-API JAX compatibility
 Project-URL: Homepage, https://github.com/GalacticDynamics/quaxed
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/quaxed/issues
 Project-URL: Discussions, https://github.com/GalacticDynamics/quaxed/discussions
 Project-URL: Changelog, https://github.com/GalacticDynamics/quaxed/releases
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License-File: LICENSE
@@ -69,8 +69,27 @@
 [rtd-link]:                 https://quaxed.readthedocs.io/en/latest/?badge=latest
 [zenodo-badge]:             https://zenodo.org/badge/732262318.svg
 [zenodo-link]:              https://zenodo.org/doi/10.5281/zenodo.10850521
 
 
 <!-- prettier-ignore-end -->
 
-`Quaxed` is a compatibility layer for `JAX` using `quax`.
+`Quaxed` wraps [jax](https://jax.readthedocs.io/en/latest/) libraries (using
+[`quax`](https://docs.kidger.site/quax/)) to enable using those libraries with
+custom array-ish objects, not only jax arrays.
+
+To understand how `quax` works it's magic, see
+[`quax.quaxify`](https://docs.kidger.site/quax/api/quax/#quax.quaxify) and the
+[tutorials](https://docs.kidger.site/quax/examples/custom_rules/).
+
+To use this library, it's as simple as:
+
+```pycon
+# Import pre-quaxified library
+>>> import quaxed.numpy as qnp  # this is quaxify(jax.numpy)
+
+# As an example, let's import an array-ish object
+>>> from unxt import Quantity
+>>> x = Quantity(2, "km")
+>>> qnp.square(w)
+Quantity['area'](Array(4, dtype=int64, weak_type=True), unit='km2')
+```
```

