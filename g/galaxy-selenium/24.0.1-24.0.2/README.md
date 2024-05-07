# Comparing `tmp/galaxy_selenium-24.0.1.tar.gz` & `tmp/galaxy_selenium-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_selenium-24.0.1.tar", last modified: Thu May  2 13:48:28 2024, max compression
+gzip compressed data, was "galaxy_selenium-24.0.2.tar", last modified: Tue May  7 14:33:33 2024, max compression
```

## Comparing `galaxy_selenium-24.0.1.tar` & `galaxy_selenium-24.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.001793 galaxy_selenium-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/axe_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/has_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)   101236 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/navigates_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/sizzle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:27.000000 galaxy_selenium-24.0.1/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 13:48:28.005793 galaxy_selenium-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_selenium-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.668953 galaxy_selenium-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_selenium-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-07 14:33:33.668953 galaxy_selenium-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.664953 galaxy_selenium-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.664953 galaxy_selenium-24.0.2/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/axe_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101236 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.664953 galaxy_selenium-24.0.2/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.664953 galaxy_selenium-24.0.2/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:33.668953 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:33:33.000000 galaxy_selenium-24.0.2/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-07 14:33:33.668953 galaxy_selenium-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_selenium-24.0.2/test-requirements.txt
```

### Comparing `galaxy_selenium-24.0.1/HISTORY.rst` & `galaxy_selenium-24.0.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_selenium-24.0.1/LICENSE` & `galaxy_selenium-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/PKG-INFO` & `galaxy_selenium-24.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/axe_results.py` & `galaxy_selenium-24.0.2/galaxy/selenium/axe_results.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/cli.py` & `galaxy_selenium-24.0.2/galaxy/selenium/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/context.py` & `galaxy_selenium-24.0.2/galaxy/selenium/context.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/driver_factory.py` & `galaxy_selenium-24.0.2/galaxy/selenium/driver_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/has_driver.py` & `galaxy_selenium-24.0.2/galaxy/selenium/has_driver.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/navigates_galaxy.py` & `galaxy_selenium-24.0.2/galaxy/selenium/navigates_galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/scripts/dump_tour.py` & `galaxy_selenium-24.0.2/galaxy/selenium/scripts/dump_tour.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/sizzle.py` & `galaxy_selenium-24.0.2/galaxy/selenium/sizzle.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy/selenium/smart_components.py` & `galaxy_selenium-24.0.2/galaxy/selenium/smart_components.py`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/galaxy_selenium.egg-info/PKG-INFO` & `galaxy_selenium-24.0.2/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,14 +49,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.2 (2024-05-07)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 24.0.1 (2024-05-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy_selenium-24.0.1/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy_selenium-24.0.2/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_selenium-24.0.1/setup.cfg` & `galaxy_selenium-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-selenium
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	galaxy-util
 	axe-selenium-python
```

