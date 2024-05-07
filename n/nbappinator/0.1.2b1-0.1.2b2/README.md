# Comparing `tmp/nbappinator-0.1.2b1.tar.gz` & `tmp/nbappinator-0.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.1.2b1.tar", last modified: Tue May  7 01:52:14 2024, max compression
+gzip compressed data, was "nbappinator-0.1.2b2.tar", last modified: Tue May  7 02:17:25 2024, max compression
```

## Comparing `nbappinator-0.1.2b1.tar` & `nbappinator-0.1.2b2.tar`

### file list

```diff
@@ -1,27 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/browser_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/jinjamagic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/nbappinator/treew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-07 01:52:14.000000 nbappinator-0.1.2b1/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 01:52:14.000000 nbappinator-0.1.2b1/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:52:14.000000 nbappinator-0.1.2b1/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 01:52:14.000000 nbappinator-0.1.2b1/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 01:52:14.000000 nbappinator-0.1.2b1/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:52:14.934273 nbappinator-0.1.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/snapshot_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/test_fails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 01:51:22.000000 nbappinator-0.1.2b1/tests/test_nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:17:25.817486 nbappinator-0.1.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 02:17:25.817486 nbappinator-0.1.2b2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:17:25.813486 nbappinator-0.1.2b2/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/jinjamagic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:17:25.813486 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 02:17:25.000000 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-07 02:17:25.000000 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:17:25.000000 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 02:17:25.000000 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 02:17:25.000000 nbappinator-0.1.2b2/nbappinator/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/nbappinator/treew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:17:25.817486 nbappinator-0.1.2b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:17:25.813486 nbappinator-0.1.2b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 02:16:33.000000 nbappinator-0.1.2b2/tests/test_nb.py
```

### Comparing `nbappinator-0.1.2b1/LICENSE.md` & `nbappinator-0.1.2b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/aggridhelper.py` & `nbappinator-0.1.2b2/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/appinator.py` & `nbappinator-0.1.2b2/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/browser_title.py` & `nbappinator-0.1.2b2/nbappinator/browser_title.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/datagrid.py` & `nbappinator-0.1.2b2/nbappinator/datagrid.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/plotly_charts.py` & `nbappinator-0.1.2b2/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/nbappinator/treew.py` & `nbappinator-0.1.2b2/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/pyproject.toml` & `nbappinator-0.1.2b2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "nbappinator"
-version = "0.1.2b1"
+version = "0.1.2b2"
 description = "Jupyter Notebook Application Builder"
 authors = [{ name = "Paul T", email = "paul@iqmo.com" }]
 maintainers =  [{ name = "Paul T", email = "paul@iqmo.com" }]
 dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
+requires-python = ">=3.9"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/iqmo-org/nbappinator"
@@ -21,8 +22,17 @@
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 
 [tool.pyright]
 typeCheckingMode = "basic"
 reportGeneralTypeIssues = false
-reportPrivateImportUsage = false
+reportPrivateImportUsage = false
+
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "pytest-xdist"
+]
+
+[tool.setuptools]
+package-dir = {"" = "nbappinator"}
```

### Comparing `nbappinator-0.1.2b1/tests/test_fails.py` & `nbappinator-0.1.2b2/tests/test_fails.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.2b1/tests/test_nb.py` & `nbappinator-0.1.2b2/tests/test_nb.py`

 * *Files identical despite different names*

