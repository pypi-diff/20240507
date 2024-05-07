# Comparing `tmp/quickmin_step-2024.5.3.tar.gz` & `tmp/quickmin_step-2024.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickmin_step-2024.5.3.tar", last modified: Fri May  3 20:24:11 2024, max compression
+gzip compressed data, was "quickmin_step-2024.5.7.tar", last modified: Tue May  7 13:37:49 2024, max compression
```

## Comparing `quickmin_step-2024.5.3.tar` & `quickmin_step-2024.5.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.503210 quickmin_step-2024.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/api/quickmin_step.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9544 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.507210 quickmin_step-2024.5.3/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/quickmin_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/quickmin_step/tk_quickmin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/quickmin_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 20:24:11.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:24:00.000000 quickmin_step-2024.5.3/quickmin_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:24:11.511210 quickmin_step-2024.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/tests/test_quickmin_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-03 20:23:57.000000 quickmin_step-2024.5.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.469725 quickmin_step-2024.5.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.469725 quickmin_step-2024.5.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.469725 quickmin_step-2024.5.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/api/quickmin_step.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9544 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.473725 quickmin_step-2024.5.7/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.473725 quickmin_step-2024.5.7/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.473725 quickmin_step-2024.5.7/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/quickmin_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/quickmin_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.473725 quickmin_step-2024.5.7/quickmin_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/quickmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/quickmin_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/quickmin_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/quickmin_step/tk_quickmin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/quickmin_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 13:37:49.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:37:32.000000 quickmin_step-2024.5.7/quickmin_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:37:49.477725 quickmin_step-2024.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/tests/test_quickmin_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-07 13:37:29.000000 quickmin_step-2024.5.7/versioneer.py
```

### Comparing `quickmin_step-2024.5.3/CONTRIBUTING.rst` & `quickmin_step-2024.5.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/HISTORY.rst` & `quickmin_step-2024.5.7/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2024.5.7 -- Bugfix: Corrected sign on gradients.
+    * OpenBabel calls "forces" "gradients", so needed to take the negative to get the
+      actual gradients.
+      
 2024.5.3 -- Added single point energy and Results.json
     * Added control to allow a single point energy as well as optimization. This
       supports using QuickMin with e.g energy scans.
     * Standardized the name of the energy to simply "energy" to better support other
       plug-ins and codes understanding the results.
       
 2023.11.15 -- Bugfix: structure handling
```

### Comparing `quickmin_step-2024.5.3/LICENSE` & `quickmin_step-2024.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/PKG-INFO` & `quickmin_step-2024.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickmin_step
-Version: 2024.5.3
+Version: 2024.5.7
 Summary: A SEAMM plug-in for simple, quick minimization
 Home-page: https://github.com/molssi-seamm/quickmin_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -110,14 +110,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.7 -- Bugfix: Corrected sign on gradients.
+    * OpenBabel calls "forces" "gradients", so needed to take the negative to get the
+      actual gradients.
+      
 2024.5.3 -- Added single point energy and Results.json
     * Added control to allow a single point energy as well as optimization. This
       supports using QuickMin with e.g energy scans.
     * Standardized the name of the energy to simply "energy" to better support other
       plug-ins and codes understanding the results.
       
 2023.11.15 -- Bugfix: structure handling
```

### Comparing `quickmin_step-2024.5.3/README.rst` & `quickmin_step-2024.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/Makefile` & `quickmin_step-2024.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/SEAMM Inverted 288x181.png` & `quickmin_step-2024.5.7/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/SEAMM logo.png` & `quickmin_step-2024.5.7/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/molssi_main_logo.png` & `quickmin_step-2024.5.7/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/molssi_main_logo_inverted_white.png` & `quickmin_step-2024.5.7/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/molssi_square.png` & `quickmin_step-2024.5.7/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/_static/nsf.png` & `quickmin_step-2024.5.7/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/api/quickmin_step.rst` & `quickmin_step-2024.5.7/docs/api/quickmin_step.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/conf.py` & `quickmin_step-2024.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/developer_guide/installation.rst` & `quickmin_step-2024.5.7/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/getting_started/index.rst` & `quickmin_step-2024.5.7/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/index.rst` & `quickmin_step-2024.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/make.bat` & `quickmin_step-2024.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/docs/user_guide/index.rst` & `quickmin_step-2024.5.7/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/__init__.py` & `quickmin_step-2024.5.7/quickmin_step/__init__.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/data/references.bib` & `quickmin_step-2024.5.7/quickmin_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/metadata.py` & `quickmin_step-2024.5.7/quickmin_step/metadata.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/quickmin.py` & `quickmin_step-2024.5.7/quickmin_step/quickmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,16 +356,16 @@
                         continue
                     if calculation == "optimization":
                         obFF.ConjugateGradients(P["n_steps"])
 
                     energy = obFF.Energy(True)
                     units = obFF.GetUnit()
 
-                    # Capture the gradients
-                    factor = Q_(1.0, units).m_as("kJ/mol")
+                    # Capture the gradients. These appear to be forces, so negate
+                    factor = -Q_(1.0, units).m_as("kJ/mol")
                     for atom in openbabel.OBMolAtomIter(obmol):
                         # vector objects have to be de-referenced individually (sigh)
                         grad = obFF.GetGradient(atom)
                         gradients.append(
                             [
                                 factor * grad.GetX(),
                                 factor * grad.GetY(),
@@ -398,16 +398,16 @@
                 if calculation == "optimization":
                     obFF.ConjugateGradients(P["n_steps"])
                     obFF.GetCoordinates(obmol)
 
                 energy = obFF.Energy(True)
                 units = obFF.GetUnit()
 
-                # Capture the gradients
-                factor = Q_(1.0, units).m_as("kJ/mol")
+                # Capture the gradients. These appear to be forces, so negate
+                factor = -Q_(1.0, units).m_as("kJ/mol")
                 for atom in openbabel.OBMolAtomIter(obmol):
                     # vector objects have to be de-referenced individually (sigh)
                     grad = obFF.GetGradient(atom)
                     gradients.append(
                         [
                             factor * grad.GetX(),
                             factor * grad.GetY(),
```

### Comparing `quickmin_step-2024.5.3/quickmin_step/quickmin_parameters.py` & `quickmin_step-2024.5.7/quickmin_step/quickmin_parameters.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/quickmin_step.py` & `quickmin_step-2024.5.7/quickmin_step/quickmin_step.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step/tk_quickmin.py` & `quickmin_step-2024.5.7/quickmin_step/tk_quickmin.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/quickmin_step.egg-info/PKG-INFO` & `quickmin_step-2024.5.7/quickmin_step.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickmin_step
-Version: 2024.5.3
+Version: 2024.5.7
 Summary: A SEAMM plug-in for simple, quick minimization
 Home-page: https://github.com/molssi-seamm/quickmin_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -110,14 +110,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.7 -- Bugfix: Corrected sign on gradients.
+    * OpenBabel calls "forces" "gradients", so needed to take the negative to get the
+      actual gradients.
+      
 2024.5.3 -- Added single point energy and Results.json
     * Added control to allow a single point energy as well as optimization. This
       supports using QuickMin with e.g energy scans.
     * Standardized the name of the energy to simply "energy" to better support other
       plug-ins and codes understanding the results.
       
 2023.11.15 -- Bugfix: structure handling
```

### Comparing `quickmin_step-2024.5.3/quickmin_step.egg-info/SOURCES.txt` & `quickmin_step-2024.5.7/quickmin_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/setup.py` & `quickmin_step-2024.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `quickmin_step-2024.5.3/versioneer.py` & `quickmin_step-2024.5.7/versioneer.py`

 * *Files identical despite different names*

