# Comparing `tmp/mlpro_int_river-0.1.5.tar.gz` & `tmp/mlpro_int_river-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_int_river-0.1.5.tar", last modified: Thu Apr 18 18:16:13 2024, max compression
+gzip compressed data, was "mlpro_int_river-0.1.6.tar", last modified: Tue May  7 18:25:12 2024, max compression
```

## Comparing `mlpro_int_river-0.1.5.tar` & `mlpro_int_river-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.597025 mlpro_int_river-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.597025 mlpro_int_river-0.1.5/src/mlpro_int_river/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/anomalydetectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    41611 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/clusteranalyzers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 18:16:13.000000 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-18 18:16:13.000000 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:16:13.000000 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 18:16:13.000000 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 18:16:13.000000 mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:16:13.601025 mlpro_int_river-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-18 18:16:09.000000 mlpro_int_river-0.1.5/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.013559 mlpro_int_river-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.013559 mlpro_int_river-0.1.6/src/mlpro_int_river/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/anomalydetectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/clustream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/dbstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/denstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/clusteranalyzers/streamkmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-07 18:25:12.000000 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 18:25:12.000000 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:25:12.000000 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 18:25:12.000000 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 18:25:12.000000 mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:25:12.017559 mlpro_int_river-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-07 18:25:07.000000 mlpro_int_river-0.1.6/test/test_examples.py
```

### Comparing `mlpro_int_river-0.1.5/LICENSE` & `mlpro_int_river-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro_int_river-0.1.5/PKG-INFO` & `mlpro_int_river-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-river
-Version: 0.1.5
+Version: 0.1.6
 Summary: MLPro: Integration River
 Home-page: https://mlpro-int-river.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-river.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.2; extra == "full"
 Requires-Dist: river>=0.21.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-river/badge/?version=latest)](https://mlpro-int-river.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-river.svg)](https://badge.fury.io/py/mlpro-int-river)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-river/mlpro-int-river/badges/version.svg)](https://anaconda.org/mlpro-int-river/mlpro)
```

### Comparing `mlpro_int_river-0.1.5/README.md` & `mlpro_int_river-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mlpro_int_river-0.1.5/setup.cfg` & `mlpro_int_river-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-river
-version = 0.1.5
+version = 0.1.6
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration River
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-river.readthedocs.io
 project_urls = 
@@ -22,14 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	mlpro[full]>=1.4.0
+	mlpro[full]>=1.4.2
 	river>=0.21.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/anomalydetectors.py` & `mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/anomalydetectors.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/basics.py` & `mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro_int_river-0.1.5/src/mlpro_int_river/wrappers/streams.py` & `mlpro_int_river-0.1.6/src/mlpro_int_river/wrappers/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## -------------------------------------------------------------------------------------------------
-## -- Project : MLPro - A Synoptic Framework for Standardized Machine Learning Tasks
-## -- Package : mlpro.wrappers.river
+## -- Project : MLPro - The integrative middleware framework for standardized machine learning
+## -- Package : mlpro_int_river.wrappers
 ## -- Module  : streams.py
 ## -------------------------------------------------------------------------------------------------
 ## -- History :
 ## -- yyyy-mm-dd  Ver.      Auth.    Description
 ## -- 2022-06-14  0.0.0     LSB      Creation
 ## -- 2022-06-14  1.0.0     LSB      Release of first version
 ## -- 2022-06-18  1.0.1     LSB      Stream names as Stream ids
```

### Comparing `mlpro_int_river-0.1.5/src/mlpro_int_river.egg-info/PKG-INFO` & `mlpro_int_river-0.1.6/src/mlpro_int_river.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mlpro-int-river
-Version: 0.1.5
+Version: 0.1.6
 Summary: MLPro: Integration River
 Home-page: https://mlpro-int-river.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-river.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.2; extra == "full"
 Requires-Dist: river>=0.21.0; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-River/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-river/badge/?version=latest)](https://mlpro-int-river.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-river.svg)](https://badge.fury.io/py/mlpro-int-river)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-river/mlpro-int-river/badges/version.svg)](https://anaconda.org/mlpro-int-river/mlpro)
```

### Comparing `mlpro_int_river-0.1.5/test/test_examples.py` & `mlpro_int_river-0.1.6/test/test_examples.py`

 * *Files identical despite different names*

