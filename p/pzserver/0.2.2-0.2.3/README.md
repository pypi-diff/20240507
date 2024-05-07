# Comparing `tmp/pzserver-0.2.2.tar.gz` & `tmp/pzserver-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzserver-0.2.2.tar", last modified: Wed Mar 20 20:47:00 2024, max compression
+gzip compressed data, was "pzserver-0.2.3.tar", last modified: Tue May  7 15:21:48 2024, max compression
```

## Comparing `pzserver-0.2.2.tar` & `pzserver-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.602051 pzserver-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-20 20:46:51.000000 pzserver-0.2.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.594051 pzserver-0.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-20 20:46:51.000000 pzserver-0.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-20 20:46:51.000000 pzserver-0.2.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-20 20:46:51.000000 pzserver-0.2.2/.devcontainer/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.594051 pzserver-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.594051 pzserver-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-20 20:46:51.000000 pzserver-0.2.2/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-20 20:46:51.000000 pzserver-0.2.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-20 20:46:51.000000 pzserver-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-20 20:46:51.000000 pzserver-0.2.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-20 20:46:51.000000 pzserver-0.2.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-20 20:46:51.000000 pzserver-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-03-20 20:46:51.000000 pzserver-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-20 20:46:51.000000 pzserver-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-20 20:46:51.000000 pzserver-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-20 20:47:00.602051 pzserver-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-20 20:46:51.000000 pzserver-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:51.000000 pzserver-0.2.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.598051 pzserver-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/nbs.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.598051 pzserver-0.2.2/docs/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.598051 pzserver-0.2.2/docs/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (127)   359278 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/notebooks/images/ScreenShotTokenGenerator.png
--rw-r--r--   0 runner    (1001) docker     (127)    90099 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/notebooks/images/ScreenShotTokenMenu.png
--rw-r--r--   0 runner    (1001) docker     (127)    89261 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/notebooks/images/linea.png
--rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/notebooks/images/rubin.png
--rw-r--r--   0 runner    (1001) docker     (127)    30948 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/notebooks/intro_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-20 20:46:51.000000 pzserver-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-20 20:46:51.000000 pzserver-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 20:47:00.602051 pzserver-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.598051 pzserver-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-03-20 20:46:51.000000 pzserver-0.2.2/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.598051 pzserver-0.2.2/src/pzserver/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-20 20:46:51.000000 pzserver-0.2.2/src/pzserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-20 20:46:51.000000 pzserver-0.2.2/src/pzserver/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    16731 2024-03-20 20:46:51.000000 pzserver-0.2.2/src/pzserver/communicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-03-20 20:46:51.000000 pzserver-0.2.2/src/pzserver/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.602051 pzserver-0.2.2/src/pzserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 20:47:00.000000 pzserver-0.2.2/src/pzserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.602051 pzserver-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-03-20 20:46:51.000000 pzserver-0.2.2/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:47:00.602051 pzserver-0.2.2/tests/pzserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:46:51.000000 pzserver-0.2.2/tests/pzserver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 20:46:51.000000 pzserver-0.2.2/tests/pzserver/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.113192 pzserver-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 15:21:41.000000 pzserver-0.2.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.105192 pzserver-0.2.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 15:21:41.000000 pzserver-0.2.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-07 15:21:41.000000 pzserver-0.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-07 15:21:41.000000 pzserver-0.2.3/.devcontainer/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.101192 pzserver-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.105192 pzserver-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-07 15:21:41.000000 pzserver-0.2.3/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-07 15:21:41.000000 pzserver-0.2.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 15:21:41.000000 pzserver-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 15:21:41.000000 pzserver-0.2.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-07 15:21:41.000000 pzserver-0.2.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-07 15:21:41.000000 pzserver-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-07 15:21:41.000000 pzserver-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 15:21:41.000000 pzserver-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 15:21:41.000000 pzserver-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-07 15:21:48.113192 pzserver-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 15:21:41.000000 pzserver-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:41.000000 pzserver-0.2.3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.109192 pzserver-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/nbs.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.109192 pzserver-0.2.3/docs/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.109192 pzserver-0.2.3/docs/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   359278 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/images/ScreenShotTokenGenerator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90099 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/images/ScreenShotTokenMenu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89261 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/images/linea.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/images/rubin.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30963 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/intro_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27340 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/public-specz-compilation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20679 2024-05-07 15:21:41.000000 pzserver-0.2.3/docs/notebooks/public-training-set-des-dr2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-07 15:21:41.000000 pzserver-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 15:21:41.000000 pzserver-0.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 15:21:41.000000 pzserver-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:21:48.113192 pzserver-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.109192 pzserver-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-07 15:21:41.000000 pzserver-0.2.3/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.109192 pzserver-0.2.3/src/pzserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 15:21:41.000000 pzserver-0.2.3/src/pzserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 15:21:41.000000 pzserver-0.2.3/src/pzserver/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16731 2024-05-07 15:21:41.000000 pzserver-0.2.3/src/pzserver/communicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-07 15:21:41.000000 pzserver-0.2.3/src/pzserver/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.113192 pzserver-0.2.3/src/pzserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 15:21:48.000000 pzserver-0.2.3/src/pzserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.113192 pzserver-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-05-07 15:21:41.000000 pzserver-0.2.3/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:48.113192 pzserver-0.2.3/tests/pzserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:21:41.000000 pzserver-0.2.3/tests/pzserver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 15:21:41.000000 pzserver-0.2.3/tests/pzserver/test_catalog.py
```

### Comparing `pzserver-0.2.2/.devcontainer/devcontainer.json` & `pzserver-0.2.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/.devcontainer/docker-compose.yml` & `pzserver-0.2.3/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/.github/workflows/build-documentation.yml` & `pzserver-0.2.3/.github/workflows/smoke-test.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-# This workflow will install Python dependencies, build the package and then build the documentation.
+# This workflow will run daily at 06:45.
+# It will install Python dependencies and run tests with a variety of Python versions.
 
-name: Build documentation
+name: Unit test smoke test
 
 on:
-  push:
-    branches: [ main ]
+  schedule:
+    - cron: 45 6 * * *
 
 jobs:
   build:
-    name: build_doc
+    name: smoke_test
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ['3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.10
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-        if [ -f docs/requirements.txt ]; then pip install -r docs/requirements.txt; fi
-    - name: Install notebook requirements
+        if [ -f requirements-dev.txt ]; then pip install -r requirements-dev.txt; fi
+    - name: Run unit tests with pytest
       run: |
-        sudo apt-get install pandoc
-    - name: Build docs
-      run: |
-        sphinx-build -T -E -b html -d docs/build/doctrees ./docs docs/build/html
-    - name: Run ghp-import
-      run: | 
-        ghp-import -n -p -f -x docs/ docs/build/html
+        python -m pytest tests
```

### Comparing `pzserver-0.2.2/.github/workflows/linting.yml` & `pzserver-0.2.3/.github/workflows/linting.yml`

 * *Files 18% similar despite different names*

```diff
@@ -26,12 +26,13 @@
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        if [ -f requirements-dev.txt ]; then pip install -r requirements-dev.txt; fi
     - name: Analyze code with linter
 
       run: |
         pylint -rn -sn --recursive=y ./src --rcfile=./src/.pylintrc
```

### Comparing `pzserver-0.2.2/.github/workflows/publish-to-pypi.yml` & `pzserver-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/.github/workflows/smoke-test.yml` & `pzserver-0.2.3/.github/workflows/testing-and-coverage.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# This workflow will run daily at 06:45.
-# It will install Python dependencies and run tests with a variety of Python versions.
+# This workflow will install Python dependencies, run tests and report code coverage with a variety of Python versions
+# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Unit test smoke test
+name: Unit test and code coverage
 
 on:
-  schedule:
-    - cron: 45 6 * * *
+  push:
+    branches: [ main ]
+  pull_request:
+    branches: [ main ]
 
 jobs:
   build:
-    name: smoke_test
+    name: test_and_coverage
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v3
@@ -24,10 +26,13 @@
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        if [ -f requirements-dev.txt ]; then pip install -r requirements-dev.txt; fi
     - name: Run unit tests with pytest
       run: |
-        python -m pytest tests
+        python -m pytest tests --cov=pzserver --cov-report=xml
+    - name: Upload coverage report to codecov
+      uses: codecov/codecov-action@v3
```

### Comparing `pzserver-0.2.2/.gitignore` & `pzserver-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/.pre-commit-config.yaml` & `pzserver-0.2.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 repos:
 
     # Compare the local template version to the latest remote template version
     # This hook should always pass. It will print a message if the local version 
     # is out of date.
   - repo: https://github.com/lincc-frameworks/pre-commit-hooks
-    rev: v0.1
+    rev: v0.1.2
     hooks:
       - id: check-lincc-frameworks-template-version
         name: Check template version
         description: Compare current template version against latest
         verbose: true
 
     # Clear output from jupyter notebooks so that only the input cells are committed.
@@ -36,35 +36,35 @@
         entry: bash -c "if python -m pytest --co -qq; then python -m pytest --cov=./src --cov-report=html; fi"
         language: system
         pass_filenames: false
         always_run: true
 
     # prevents committing directly branches named 'main' and 'master'.
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: no-commit-to-branch
         name: Prevent main branch commits
         description: Prevent the user from committing directly to the primary branch.
       - id: check-added-large-files
         name: Check for large files
         description: Prevent the user from committing very large files.
         args: ['--maxkb=500']
 
     # verify that pyproject.toml is well formed
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.16
     hooks:
       - id: validate-pyproject
         name: Validate pyproject.toml
         description: Verify that pyproject.toml adheres to the established schema.
 
     # Automatically sort the imports used in .py files
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
         name: isort (python files in src/ and tests/)
         description: Sort and organize imports in .py files.
         types: [python]
         files: ^(src|tests)/
```

### Comparing `pzserver-0.2.2/LICENSE` & `pzserver-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/PKG-INFO` & `pzserver-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pzserver
-Version: 0.2.2
+Version: 0.2.3
 Author-email: LIneA <itteam@linea.org.br>
 License: MIT License
         
         Copyright (c) 2023 LIneA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,41 +30,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.13,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deprecated
 Requires-Dist: numpy>=1.23
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: requests>=2.23.0
 Requires-Dist: astropy>=5.0.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: tables_io>=0.7.9
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: ipython>=8.5.0
 Requires-Dist: h5py>=3.8.0
+Requires-Dist: pyarrow>=15.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: sphinx<8,>=7.0.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme<2,>=1.2.0; extra == "dev"
 Requires-Dist: sphinx-autoapi<4,>=3.0.0; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: nbconvert; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: ghp-import; extra == "dev"
 
 # Pz Server Library
 
 ![PyPI](https://img.shields.io/pypi/v/pzserver?label=PyPI)
 ![PyPI - Status](https://img.shields.io/pypi/status/pzserver)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/linea-it/pzserver/build-documentation.yml?label=docs)
 ![GitHub](https://img.shields.io/github/license/linea-it/pzserver)
```

### Comparing `pzserver-0.2.2/README.md` & `pzserver-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/Makefile` & `pzserver-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/conf.py` & `pzserver-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/index.rst` & `pzserver-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/make.bat` & `pzserver-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/notebooks/images/ScreenShotTokenGenerator.png` & `pzserver-0.2.3/docs/notebooks/images/ScreenShotTokenGenerator.png`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/notebooks/images/ScreenShotTokenMenu.png` & `pzserver-0.2.3/docs/notebooks/images/ScreenShotTokenMenu.png`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/notebooks/images/linea.png` & `pzserver-0.2.3/docs/notebooks/images/linea.png`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/notebooks/images/rubin.png` & `pzserver-0.2.3/docs/notebooks/images/rubin.png`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/docs/notebooks/intro_notebook.ipynb` & `pzserver-0.2.3/docs/notebooks/intro_notebook.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947378337639965%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(7, 'Last verified run: 2024-May-06<br>')], delete: [7]}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)', 'name': 'python3'}}"}*

```diff
@@ -7,15 +7,15 @@
                 "<img align=\"left\" src = \"images/linea.png\" width=120 style=\"padding: 20px\"> \n",
                 "<img align=\"left\" src = \"images/rubin.png\" width=180 style=\"padding: 20px\"> \n",
                 "\n",
                 "# Photo-z Server - Tutorial Notebook\n",
                 "\n",
                 "Contact author: [Julia Gschwend](mailto:julia@linea.org.br)\n",
                 "\n",
-                "Last verified run: 2024-Jan-23<br>"
+                "Last verified run: 2024-May-06<br>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
@@ -923,17 +923,17 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "pz-lib",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "pz-lib"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `pzserver-0.2.2/src/.pylintrc` & `pzserver-0.2.3/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/src/pzserver/catalog.py` & `pzserver-0.2.3/src/pzserver/catalog.py`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/src/pzserver/communicate.py` & `pzserver-0.2.3/src/pzserver/communicate.py`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/src/pzserver/core.py` & `pzserver-0.2.3/src/pzserver/core.py`

 * *Files identical despite different names*

### Comparing `pzserver-0.2.2/src/pzserver.egg-info/PKG-INFO` & `pzserver-0.2.3/src/pzserver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pzserver
-Version: 0.2.2
+Version: 0.2.3
 Author-email: LIneA <itteam@linea.org.br>
 License: MIT License
         
         Copyright (c) 2023 LIneA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,41 +30,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.13,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deprecated
 Requires-Dist: numpy>=1.23
 Requires-Dist: pandas>=1.2.0
 Requires-Dist: requests>=2.23.0
 Requires-Dist: astropy>=5.0.0
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: tables_io>=0.7.9
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: ipython>=8.5.0
 Requires-Dist: h5py>=3.8.0
+Requires-Dist: pyarrow>=15.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: sphinx<8,>=7.0.0; extra == "dev"
 Requires-Dist: sphinx_rtd_theme<2,>=1.2.0; extra == "dev"
 Requires-Dist: sphinx-autoapi<4,>=3.0.0; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: nbconvert; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: ghp-import; extra == "dev"
 
 # Pz Server Library
 
 ![PyPI](https://img.shields.io/pypi/v/pzserver?label=PyPI)
 ![PyPI - Status](https://img.shields.io/pypi/status/pzserver)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/linea-it/pzserver/build-documentation.yml?label=docs)
 ![GitHub](https://img.shields.io/github/license/linea-it/pzserver)
```

### Comparing `pzserver-0.2.2/src/pzserver.egg-info/SOURCES.txt` & `pzserver-0.2.3/src/pzserver.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.md
 __init__.py
 pyproject.toml
+requirements-dev.txt
+requirements.txt
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .devcontainer/docker-compose.yml
 .github/workflows/build-documentation.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/nbs.rst
-docs/requirements.txt
 docs/notebooks/intro_notebook.ipynb
+docs/notebooks/public-specz-compilation.ipynb
+docs/notebooks/public-training-set-des-dr2.ipynb
 docs/notebooks/images/ScreenShotTokenGenerator.png
 docs/notebooks/images/ScreenShotTokenMenu.png
 docs/notebooks/images/linea.png
 docs/notebooks/images/rubin.png
 src/.pylintrc
 src/pzserver/__init__.py
 src/pzserver/_version.py
```

### Comparing `pzserver-0.2.2/tests/.pylintrc` & `pzserver-0.2.3/tests/.pylintrc`

 * *Files identical despite different names*

