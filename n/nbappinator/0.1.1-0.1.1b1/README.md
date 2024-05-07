# Comparing `tmp/nbappinator-0.1.1.tar.gz` & `tmp/nbappinator-0.1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbappinator-0.1.1.tar", last modified: Tue May  7 01:41:04 2024, max compression
+gzip compressed data, was "nbappinator-0.1.1b1.tar", last modified: Tue May  7 01:28:00 2024, max compression
```

## Comparing `nbappinator-0.1.1.tar` & `nbappinator-0.1.1b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:41:04.021704 nbappinator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 01:40:12.000000 nbappinator-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 01:41:04.021704 nbappinator-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:41:04.021704 nbappinator-0.1.1/nbappinator/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/aggridhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/appinator.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/browser_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/jinjamagic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 01:40:12.000000 nbappinator-0.1.1/nbappinator/treew.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:41:04.021704 nbappinator-0.1.1/nbappinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-07 01:41:04.000000 nbappinator-0.1.1/nbappinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 01:41:04.000000 nbappinator-0.1.1/nbappinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:41:04.000000 nbappinator-0.1.1/nbappinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 01:41:04.000000 nbappinator-0.1.1/nbappinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 01:41:04.000000 nbappinator-0.1.1/nbappinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-07 01:40:12.000000 nbappinator-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 01:41:04.021704 nbappinator-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:41:04.021704 nbappinator-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/env_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/snapshot_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/test_fails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 01:40:12.000000 nbappinator-0.1.1/tests/test_nb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/nbappinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/aggridhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/appinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/browser_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/jinjamagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/nbappinator/treew.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/nbappinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 01:28:00.000000 nbappinator-0.1.1b1/nbappinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 01:28:00.000000 nbappinator-0.1.1b1/nbappinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:28:00.000000 nbappinator-0.1.1b1/nbappinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 01:28:00.000000 nbappinator-0.1.1b1/nbappinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 01:28:00.000000 nbappinator-0.1.1b1/nbappinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:28:00.404266 nbappinator-0.1.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/env_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/snapshot_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/test_fails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 01:27:07.000000 nbappinator-0.1.1b1/tests/test_nb.py
```

### Comparing `nbappinator-0.1.1/LICENSE.md` & `nbappinator-0.1.1b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/aggridhelper.py` & `nbappinator-0.1.1b1/nbappinator/aggridhelper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/appinator.py` & `nbappinator-0.1.1b1/nbappinator/appinator.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/browser_title.py` & `nbappinator-0.1.1b1/nbappinator/browser_title.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/datagrid.py` & `nbappinator-0.1.1b1/nbappinator/datagrid.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/plotly_charts.py` & `nbappinator-0.1.1b1/nbappinator/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator/treew.py` & `nbappinator-0.1.1b1/nbappinator/treew.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/nbappinator.egg-info/SOURCES.txt` & `nbappinator-0.1.1b1/nbappinator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/pyproject.toml` & `nbappinator-0.1.1b1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "nbappinator"
-version = "0.1.1"
+version = "0.1.1b1"
 description = "Jupyter Notebook Application Builder"
-authors = [{ name = "Paul T", email = "paul@iqmo.com" }]
-maintainers =  [{ name = "Paul T", email = "paul@iqmo.com" }]
+authors = [{ name = "Paul Timmins", email = "paul@iqmo.com" }]
+maintainers =  [{ name = "Paul Timmins", email = "paul@iqmo.com" }]
 dependencies = ["ipywidgets~=7.8.0", "plotly", "ipyvuetify>=1.9", "ipyaggrid", "ipytree", "pandas>=1.5.3"]
 readme = "README.md"
 
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nbappinator-0.1.1/tests/conftest.py` & `nbappinator-0.1.1b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/tests/env_helper.py` & `nbappinator-0.1.1b1/tests/env_helper.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/tests/snapshot_mgr.py` & `nbappinator-0.1.1b1/tests/snapshot_mgr.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/tests/test_fails.py` & `nbappinator-0.1.1b1/tests/test_fails.py`

 * *Files identical despite different names*

### Comparing `nbappinator-0.1.1/tests/test_nb.py` & `nbappinator-0.1.1b1/tests/test_nb.py`

 * *Files identical despite different names*
