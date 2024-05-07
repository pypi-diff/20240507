# Comparing `tmp/nbappinator-0.1.4.tar.gz` & `tmp/nbappinator-0.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.1.4.tar", last modified: Tue May  7 11:13:14 2024, max compression
+gzip compressed data, was "nbappinator-0.1.5b1.tar", last modified: Tue May  7 20:58:41 2024, max compression
```

## Comparing `nbappinator-0.1.4.tar` & `nbappinator-0.1.5b1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 11:12:18.000000 nbappinator-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-07 11:13:14.050385 nbappinator-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-07 11:12:18.000000 nbappinator-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.046385 nbappinator-0.1.4/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/browser_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/jinjamagic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 11:13:14.000000 nbappinator-0.1.4/nbappinator/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 11:12:18.000000 nbappinator-0.1.4/nbappinator/treew.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 11:12:18.000000 nbappinator-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:13:14.050385 nbappinator-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:13:14.050385 nbappinator-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 11:12:18.000000 nbappinator-0.1.4/tests/test_fails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 11:12:18.000000 nbappinator-0.1.4/tests/test_nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.625769 nbappinator-0.1.5b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/jinjamagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/treew.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/nbappinator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 20:58:41.000000 nbappinator-0.1.5b1/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:58:41.625769 nbappinator-0.1.5b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:58:41.621769 nbappinator-0.1.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 20:57:49.000000 nbappinator-0.1.5b1/tests/test_nb.py
```

### Comparing `nbappinator-0.1.4/LICENSE.md` & `nbappinator-0.1.5b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/PKG-INFO` & `nbappinator-0.1.5b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: nbappinator
-Version: 0.1.4
+Version: 0.1.5b1
 Summary: Jupyter Notebook Application Builder
 Author-email: Paul T <paul@iqmo.com>
 Maintainer-email: Paul T <paul@iqmo.com>
 Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
 Project-URL: Repository, https://github.com/iqmo-org/nbappinator
 Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ipywidgets~=7.8.0
+Requires-Dist: ipywidgets<=8.0,>=7.8
 Requires-Dist: plotly
 Requires-Dist: ipyvuetify>=1.9
 Requires-Dist: ipyaggrid
 Requires-Dist: ipytree
 Requires-Dist: pandas>=1.5.3
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-xdist; extra == "test"
 
 [![PyPI Version](https://badge.fury.io/py/nbappinator.svg)](https://pypi.python.org/pypi/nbappinator)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/nbappinator/badges/version.svg)](https://anaconda.org/conda-forge/nbappinator)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml)
 
 <!--[![Coverage badge](https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)-->
```

### Comparing `nbappinator-0.1.4/README.md` & `nbappinator-0.1.5b1/README.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/aggridhelper.py` & `nbappinator-0.1.5b1/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/appinator.py` & `nbappinator-0.1.5b1/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/browser_title.py` & `nbappinator-0.1.5b1/nbappinator/browser_title.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/datagrid.py` & `nbappinator-0.1.5b1/nbappinator/datagrid.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/nbappinator.egg-info/PKG-INFO` & `nbappinator-0.1.5b1/nbappinator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: nbappinator
-Version: 0.1.4
+Version: 0.1.5b1
 Summary: Jupyter Notebook Application Builder
 Author-email: Paul T <paul@iqmo.com>
 Maintainer-email: Paul T <paul@iqmo.com>
 Project-URL: Homepage, https://github.com/iqmo-org/nbappinator
 Project-URL: Repository, https://github.com/iqmo-org/nbappinator
 Project-URL: Issues, https://github.com/iqmo-org/nbappinator/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ipywidgets~=7.8.0
+Requires-Dist: ipywidgets<=8.0,>=7.8
 Requires-Dist: plotly
 Requires-Dist: ipyvuetify>=1.9
 Requires-Dist: ipyaggrid
 Requires-Dist: ipytree
 Requires-Dist: pandas>=1.5.3
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-xdist; extra == "test"
 
 [![PyPI Version](https://badge.fury.io/py/nbappinator.svg)](https://pypi.python.org/pypi/nbappinator)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/nbappinator/badges/version.svg)](https://anaconda.org/conda-forge/nbappinator)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/build_release.yml)
 [![Tests](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml/badge.svg)](https://github.com/iqmo-org/nbappinator/actions/workflows/test_coverage.yml)
 
 <!--[![Coverage badge](https://raw.githubusercontent.com/iqmo-org/nbappinator/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/iqmo-org/nbappinator/blob/python-coverage-comment-action-data/htmlcov/index.html)-->
```

### Comparing `nbappinator-0.1.4/nbappinator/plotly_charts.py` & `nbappinator-0.1.5b1/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/nbappinator/treew.py` & `nbappinator-0.1.5b1/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/pyproject.toml` & `nbappinator-0.1.5b1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "nbappinator"
-version = "0.1.4"
+dynamic = ["version"]
 description = "Jupyter Notebook Application Builder"
 authors = [{ name = "Paul T", email = "paul@iqmo.com" }]
 maintainers =  [{ name = "Paul T", email = "paul@iqmo.com" }]
-dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
+dependencies = ["ipywidgets>=7.8,<=8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
 requires-python = ">=3.9"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
@@ -24,15 +24,15 @@
 ignore-init-module-imports = true
 
 [tool.pyright]
 typeCheckingMode = "basic"
 reportGeneralTypeIssues = false
 reportPrivateImportUsage = false
 
-[project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-xdist"
-]
+#[tools.setuptools]
+#packages = ["nbappinator"]
 
-[tool.setuptools]
-package-dir = {"" = "nbappinator"}
+[tool.setuptools.dynamic]
+version = {attr = "nbappinator.version.__version__"}
+
+[tool.setuptools.package-dir]
+mypkg = "nbappinator"
```

### Comparing `nbappinator-0.1.4/tests/test_fails.py` & `nbappinator-0.1.5b1/tests/test_fails.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.4/tests/test_nb.py` & `nbappinator-0.1.5b1/tests/test_nb.py`

 * *Files identical despite different names*

