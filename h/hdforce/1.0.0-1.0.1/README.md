# Comparing `tmp/hdforce-1.0.0.tar.gz` & `tmp/hdforce-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdforce-1.0.0.tar", max compression
+gzip compressed data, was "hdforce-1.0.1.tar", max compression
```

## Comparing `hdforce-1.0.0.tar` & `hdforce-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      587 2024-05-07 03:52:23.135546 hdforce-1.0.0/hdforce/__init__.py
--rw-r--r--   0        0        0     7107 2024-05-07 03:52:23.110866 hdforce-1.0.0/hdforce/AuthManager.py
--rw-r--r--   0        0        0     4999 2024-05-07 03:52:23.116878 hdforce-1.0.0/hdforce/GetAthletes.py
--rw-r--r--   0        0        0     5770 2024-05-07 03:52:23.118366 hdforce-1.0.0/hdforce/GetForceTime.py
--rw-r--r--   0        0        0     4141 2024-05-07 03:52:23.118366 hdforce-1.0.0/hdforce/GetGroups.py
--rw-r--r--   0        0        0     4711 2024-05-07 03:52:23.121004 hdforce-1.0.0/hdforce/GetMetrics.py
--rw-r--r--   0        0        0     4235 2024-05-07 03:52:23.122655 hdforce-1.0.0/hdforce/GetTags.py
--rw-r--r--   0        0        0     4188 2024-05-07 03:52:23.122655 hdforce-1.0.0/hdforce/GetTeams.py
--rw-r--r--   0        0        0     6165 2024-05-07 03:52:23.125197 hdforce-1.0.0/hdforce/GetTests.py
--rw-r--r--   0        0        0     6751 2024-05-07 03:52:23.125702 hdforce-1.0.0/hdforce/GetTestsAth.py
--rw-r--r--   0        0        0     6656 2024-05-07 03:52:23.128636 hdforce-1.0.0/hdforce/GetTestsGroup.py
--rw-r--r--   0        0        0     6765 2024-05-07 03:52:23.129871 hdforce-1.0.0/hdforce/GetTestsTeam.py
--rw-r--r--   0        0        0     7722 2024-05-07 03:52:23.131247 hdforce-1.0.0/hdforce/GetTestsType.py
--rw-r--r--   0        0        0     4111 2024-05-07 03:52:23.133558 hdforce-1.0.0/hdforce/GetTypes.py
--rw-r--r--   0        0        0     1968 2024-05-07 03:52:23.133558 hdforce-1.0.0/hdforce/LoggerConfig.py
--rw-r--r--   0        0        0    10963 2024-05-07 03:52:23.137952 hdforce-1.0.0/hdforce/utils.py
--rw-r--r--   0        0        0     1072 2024-05-07 03:52:23.059561 hdforce-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1107 2024-05-07 04:15:54.831825 hdforce-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11905 2024-05-07 03:52:23.059561 hdforce-1.0.0/README.md
--rw-r--r--   0        0        0    12877 1970-01-01 00:00:00.000000 hdforce-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      587 2024-05-07 03:52:23.135546 hdforce-1.0.1/hdforce/__init__.py
+-rw-r--r--   0        0        0     7107 2024-05-07 03:52:23.110866 hdforce-1.0.1/hdforce/AuthManager.py
+-rw-r--r--   0        0        0     4999 2024-05-07 03:52:23.116878 hdforce-1.0.1/hdforce/GetAthletes.py
+-rw-r--r--   0        0        0     5770 2024-05-07 03:52:23.118366 hdforce-1.0.1/hdforce/GetForceTime.py
+-rw-r--r--   0        0        0     4141 2024-05-07 03:52:23.118366 hdforce-1.0.1/hdforce/GetGroups.py
+-rw-r--r--   0        0        0     4711 2024-05-07 03:52:23.121004 hdforce-1.0.1/hdforce/GetMetrics.py
+-rw-r--r--   0        0        0     4235 2024-05-07 03:52:23.122655 hdforce-1.0.1/hdforce/GetTags.py
+-rw-r--r--   0        0        0     4188 2024-05-07 03:52:23.122655 hdforce-1.0.1/hdforce/GetTeams.py
+-rw-r--r--   0        0        0     6165 2024-05-07 03:52:23.125197 hdforce-1.0.1/hdforce/GetTests.py
+-rw-r--r--   0        0        0     6751 2024-05-07 03:52:23.125702 hdforce-1.0.1/hdforce/GetTestsAth.py
+-rw-r--r--   0        0        0     6656 2024-05-07 03:52:23.128636 hdforce-1.0.1/hdforce/GetTestsGroup.py
+-rw-r--r--   0        0        0     6765 2024-05-07 03:52:23.129871 hdforce-1.0.1/hdforce/GetTestsTeam.py
+-rw-r--r--   0        0        0     7722 2024-05-07 03:52:23.131247 hdforce-1.0.1/hdforce/GetTestsType.py
+-rw-r--r--   0        0        0     4111 2024-05-07 03:52:23.133558 hdforce-1.0.1/hdforce/GetTypes.py
+-rw-r--r--   0        0        0     1968 2024-05-07 03:52:23.133558 hdforce-1.0.1/hdforce/LoggerConfig.py
+-rw-r--r--   0        0        0    10963 2024-05-07 03:52:23.137952 hdforce-1.0.1/hdforce/utils.py
+-rw-r--r--   0        0        0     1072 2024-05-07 03:52:23.059561 hdforce-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1101 2024-05-07 06:27:25.831900 hdforce-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11799 2024-05-07 06:05:58.756211 hdforce-1.0.1/README.md
+-rw-r--r--   0        0        0    12764 1970-01-01 00:00:00.000000 hdforce-1.0.1/PKG-INFO
```

### Comparing `hdforce-1.0.0/hdforce/__init__.py` & `hdforce-1.0.1/hdforce/__init__.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/AuthManager.py` & `hdforce-1.0.1/hdforce/AuthManager.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetAthletes.py` & `hdforce-1.0.1/hdforce/GetAthletes.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetForceTime.py` & `hdforce-1.0.1/hdforce/GetForceTime.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetGroups.py` & `hdforce-1.0.1/hdforce/GetGroups.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetMetrics.py` & `hdforce-1.0.1/hdforce/GetMetrics.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTags.py` & `hdforce-1.0.1/hdforce/GetTags.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTeams.py` & `hdforce-1.0.1/hdforce/GetTeams.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTests.py` & `hdforce-1.0.1/hdforce/GetTests.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTestsAth.py` & `hdforce-1.0.1/hdforce/GetTestsAth.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTestsGroup.py` & `hdforce-1.0.1/hdforce/GetTestsGroup.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTestsTeam.py` & `hdforce-1.0.1/hdforce/GetTestsTeam.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTestsType.py` & `hdforce-1.0.1/hdforce/GetTestsType.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/GetTypes.py` & `hdforce-1.0.1/hdforce/GetTypes.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/LoggerConfig.py` & `hdforce-1.0.1/hdforce/LoggerConfig.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/hdforce/utils.py` & `hdforce-1.0.1/hdforce/utils.py`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/LICENSE.txt` & `hdforce-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdforce-1.0.0/pyproject.toml` & `hdforce-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "hdforce"
-version= "1.0.0"
+version= "1.0.01"
 description = "Get your data from the Hawkin Dynamics API"
 authors = ["laureng-hd <lauren@hawkindynamics.com>"]
 readme = "README.md"
 keywords = ["hawkin", "force plates", "sports science"]
 homepage = "https://www.hawkindynamics.com/"
 repository = "https://github.com/HawkinDynamics/hawkinPy"
-documentation = "https://silver-adventure-22j19qq.pages.github.io/"
+documentation = "https://hawkindynamics.github.io/hawkinPy/"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `hdforce-1.0.0/README.md` & `hdforce-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # HDFORCE <img src="docs/img/hdlogo_sm.png" align="right" alt="" width="120" />
 
 **Get your data from the Hawkin Dynamics API**
 
 <!-- badges: start -->
-![GitHub Release](https://img.shields.io/github/v/release/HawkinDynamics/hawkinPy)
-[![Test Py Versions and OS](https://github.com/HawkinDynamics/hawkinPy/actions/workflows/push-test.yml/badge.svg?branch=dev_env)](https://github.com/HawkinDynamics/hawkinPy/actions/workflows/push-test.yml)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/HawkinDynamics/hawkinPy/dev_env)
+![Static Badge](https://img.shields.io/badge/release-v1.0.01-blue?link=https%3A%2F%2Fsilver-adventure-22j19qq.pages.github.io%2F)
+![Static Badge](https://img.shields.io/badge/OS_and_Py_Version_Tests-pass-success)
+![Static Badge](https://img.shields.io/badge/last_commit-2024--05--06-blue)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![lifecycle](https://img.shields.io/badge/lifecycle-stable-green.svg)](https://www.tidyverse.org/lifecycle/#stable)
 [![license](https://img.shields.io/badge/license-MIT%20+%20file%20LICENSE-lightgrey.svg)](https://choosealicense.com/)
 <!-- badges: end -->
 
 ## How To Use The HDFORCE Package
```

### Comparing `hdforce-1.0.0/PKG-INFO` & `hdforce-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdforce
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get your data from the Hawkin Dynamics API
 Home-page: https://www.hawkindynamics.com/
 Keywords: hawkin,force plates,sports science
 Author: laureng-hd
 Author-email: lauren@hawkindynamics.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,26 +17,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: flake8 (>=7.0.0,<8.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://silver-adventure-22j19qq.pages.github.io/
+Project-URL: Documentation, https://hawkindynamics.github.io/hawkinPy/
 Project-URL: Repository, https://github.com/HawkinDynamics/hawkinPy
 Description-Content-Type: text/markdown
 
 # HDFORCE <img src="docs/img/hdlogo_sm.png" align="right" alt="" width="120" />
 
 **Get your data from the Hawkin Dynamics API**
 
 <!-- badges: start -->
-![GitHub Release](https://img.shields.io/github/v/release/HawkinDynamics/hawkinPy)
-[![Test Py Versions and OS](https://github.com/HawkinDynamics/hawkinPy/actions/workflows/push-test.yml/badge.svg?branch=dev_env)](https://github.com/HawkinDynamics/hawkinPy/actions/workflows/push-test.yml)
-![GitHub last commit (branch)](https://img.shields.io/github/last-commit/HawkinDynamics/hawkinPy/dev_env)
+![Static Badge](https://img.shields.io/badge/release-v1.0.01-blue?link=https%3A%2F%2Fsilver-adventure-22j19qq.pages.github.io%2F)
+![Static Badge](https://img.shields.io/badge/OS_and_Py_Version_Tests-pass-success)
+![Static Badge](https://img.shields.io/badge/last_commit-2024--05--06-blue)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![lifecycle](https://img.shields.io/badge/lifecycle-stable-green.svg)](https://www.tidyverse.org/lifecycle/#stable)
 [![license](https://img.shields.io/badge/license-MIT%20+%20file%20LICENSE-lightgrey.svg)](https://choosealicense.com/)
 <!-- badges: end -->
 
 ## How To Use The HDFORCE Package
```

