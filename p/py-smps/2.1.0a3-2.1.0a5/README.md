# Comparing `tmp/py_smps-2.1.0a3.tar.gz` & `tmp/py_smps-2.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_smps-2.1.0a3.tar", max compression
+gzip compressed data, was "py_smps-2.1.0a5.tar", max compression
```

## Comparing `py_smps-2.1.0a3.tar` & `py_smps-2.1.0a5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 12:07:26.930735 py_smps-2.1.0a3/LICENSE
--rw-r--r--   0        0        0     2361 2023-07-14 12:07:26.930735 py_smps-2.1.0a3/README.md
--rw-r--r--   0        0        0      933 2023-07-14 12:07:26.966736 py_smps-2.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      176 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/__init__.py
--rw-r--r--   0        0        0    19832 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/fit.py
--rw-r--r--   0        0        0     7881 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/io.py
--rw-r--r--   0        0        0    30952 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/models.py
--rw-r--r--   0        0        0     5414 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/plots.py
--rw-r--r--   0        0        0      801 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/rcmod.py
--rw-r--r--   0        0        0     9321 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/utils.py
--rw-r--r--   0        0        0     3359 1970-01-01 00:00:00.000000 py_smps-2.1.0a3/setup.py
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 py_smps-2.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-07 02:59:20.275804 py_smps-2.1.0a5/LICENSE
+-rw-r--r--   0        0        0     2614 2024-05-07 02:59:20.275804 py_smps-2.1.0a5/README.md
+-rw-r--r--   0        0        0     1183 2024-05-07 02:59:20.287804 py_smps-2.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/__init__.py
+-rw-r--r--   0        0        0    19832 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/fit.py
+-rw-r--r--   0        0        0     7881 2024-05-07 02:59:20.319804 py_smps-2.1.0a5/smps/io.py
+-rw-r--r--   0        0        0    30952 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/models.py
+-rw-r--r--   0        0        0     5414 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/plots.py
+-rw-r--r--   0        0        0      801 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/rcmod.py
+-rw-r--r--   0        0        0     9321 2024-05-07 02:59:20.323804 py_smps-2.1.0a5/smps/utils.py
+-rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 py_smps-2.1.0a5/PKG-INFO
```

### Comparing `py_smps-2.1.0a3/LICENSE` & `py_smps-2.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/README.md` & `py_smps-2.1.0a5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -46,14 +46,25 @@
 
 ## Contributing to Development
 
 We welcome all contributions from the community in the form of issues reporting, feature requests, bug fixes, etc.
 
 If there is a feature you would like to see or a bug you would like to report, please open an issue. We will try to get to things as promptly as possible. Otherwise, feel free to send PR's!
 
+### Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
 
 # Documentation
 
 Documentation is available [here](https://quant-aq.github.io/py-smps/). To build locally, you must first install [pandoc](https://pandoc.org/). Docs are built using Sphinx and can be built locally by doing the following:
 
 ```sh
 # Activate the virtualenv
@@ -62,8 +73,8 @@
 # Build the docs
 $ cd docs/
 $ make clean
 $ make html
 $ cd ..
 ```
 
-Then, you can navigate to your local directory at `docs/build/html/` and open up the `index.html` file in your preferred browser window.
+Then, you can navigate to your local directory at `docs/build/html/` and open up the `index.html` file in your preferred browser window.
```

### Comparing `py_smps-2.1.0a3/smps/fit.py` & `py_smps-2.1.0a5/smps/fit.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/smps/io.py` & `py_smps-2.1.0a5/smps/io.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/smps/models.py` & `py_smps-2.1.0a5/smps/models.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/smps/plots.py` & `py_smps-2.1.0a5/smps/plots.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/smps/rcmod.py` & `py_smps-2.1.0a5/smps/rcmod.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/smps/utils.py` & `py_smps-2.1.0a5/smps/utils.py`

 * *Files identical despite different names*

### Comparing `py_smps-2.1.0a3/PKG-INFO` & `py_smps-2.1.0a5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: py-smps
-Version: 2.1.0a3
-Summary: A simple python library to import and visualize data from particle sizing instruments.
+Version: 2.1.0a5
+Summary: A simple python library to import and visualize data from particle sizing instruments
 Home-page: https://github.com/quant-aq/py-smps
 License: MIT
 Author: David H Hagan
 Author-email: david.hagan@quant-aq.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: joblib (>=1.2,<2.0)
-Requires-Dist: numpy (>=1.23,<2.0)
-Requires-Dist: pandas (>=1.4,<2.0)
-Requires-Dist: requests (>=2.24,<3.0)
-Requires-Dist: scipy (>=1.9,<2.0)
-Requires-Dist: seaborn (>=0.12,<0.13)
-Requires-Dist: setuptools (>=65.0,<66.0)
-Requires-Dist: statsmodels (>=0.13,<0.14)
+Requires-Dist: joblib (>=1.3,<2.0)
+Requires-Dist: lock (>=2018.3.25.2110,<2019.0.0.0)
+Requires-Dist: matplotlib (>=3.4,!=3.6.1)
+Requires-Dist: numpy (>1.20,!=1.24.0)
+Requires-Dist: pandas (>=1.2)
+Requires-Dist: scipy (>1.7)
+Requires-Dist: seaborn (>=0.12)
+Requires-Dist: setuptools (>48.0)
+Requires-Dist: statsmodels (>=0.12.0)
+Project-URL: Bug Tracker, https://github.com/quant-aq/py-smps/issues
+Project-URL: Documentation, https://github.com/quant-aq/py-smps
 Project-URL: Repository, https://github.com/quant-aq/py-smps
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/py-smps.svg)](https://badge.fury.io/py/py-smps)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Coverage Status](https://coveralls.io/repos/github/dhhagan/py-smps/badge.svg?branch=master)](https://coveralls.io/github/dhhagan/py-smps?branch=master)
 [![ci.tests](https://github.com/quant-aq/py-smps/actions/workflows/test-and-report.yml/badge.svg)](https://github.com/quant-aq/py-smps/actions/workflows/test-and-report.yml)
@@ -72,14 +75,25 @@
 
 ## Contributing to Development
 
 We welcome all contributions from the community in the form of issues reporting, feature requests, bug fixes, etc.
 
 If there is a feature you would like to see or a bug you would like to report, please open an issue. We will try to get to things as promptly as possible. Otherwise, feel free to send PR's!
 
+### Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
 
 # Documentation
 
 Documentation is available [here](https://quant-aq.github.io/py-smps/). To build locally, you must first install [pandoc](https://pandoc.org/). Docs are built using Sphinx and can be built locally by doing the following:
 
 ```sh
 # Activate the virtualenv
@@ -89,7 +103,8 @@
 $ cd docs/
 $ make clean
 $ make html
 $ cd ..
 ```
 
 Then, you can navigate to your local directory at `docs/build/html/` and open up the `index.html` file in your preferred browser window.
+
```

