# Comparing `tmp/access_nri_intake-0.1.2.tar.gz` & `tmp/access_nri_intake-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.1.2.tar", last modified: Sun Mar 31 00:52:38 2024, max compression
+gzip compressed data, was "access_nri_intake-0.1.3.tar", last modified: Tue May  7 01:59:40 2024, max compression
```

## Comparing `access_nri_intake-0.1.2.tar` & `access_nri_intake-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.103591 access_nri_intake-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.103591 access_nri_intake-0.1.2/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.103591 access_nri_intake-0.1.2/src/access_nri_intake/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/catalog/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/catalog/translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/src/access_nri_intake/data/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/data/catalog.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/src/access_nri_intake/source/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/source/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/source/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-31 00:52:38.000000 access_nri_intake-0.1.2/src/access_nri_intake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:52:38.107591 access_nri_intake-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_source_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    83751 2024-03-31 00:52:30.000000 access_nri_intake-0.1.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.632588 access_nri_intake-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.636587 access_nri_intake-0.1.3/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.636587 access_nri_intake-0.1.3/src/access_nri_intake/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/catalog/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/catalog/translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.636587 access_nri_intake-0.1.3/src/access_nri_intake/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/data/catalog.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.636587 access_nri_intake-0.1.3/src/access_nri_intake/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/source/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/source/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 01:59:40.000000 access_nri_intake-0.1.3/src/access_nri_intake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:59:40.640587 access_nri_intake-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_source_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83751 2024-05-07 01:59:31.000000 access_nri_intake-0.1.3/versioneer.py
```

### Comparing `access_nri_intake-0.1.2/LICENSE` & `access_nri_intake-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/PKG-INFO` & `access_nri_intake-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.1.2
+Version: 0.1.3
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.1.2/README.rst` & `access_nri_intake-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/pyproject.toml` & `access_nri_intake-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/catalog/__init__.py` & `access_nri_intake-0.1.3/src/access_nri_intake/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/catalog/manager.py` & `access_nri_intake-0.1.3/src/access_nri_intake/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/catalog/translators.py` & `access_nri_intake-0.1.3/src/access_nri_intake/catalog/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/cli.py` & `access_nri_intake-0.1.3/src/access_nri_intake/cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/data/catalog.yaml` & `access_nri_intake-0.1.3/src/access_nri_intake/data/catalog.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     description: ACCESS-NRI intake catalog
     driver: intake_dataframe_catalog.core.DfFileCatalog
     metadata:
       storage: gdata/al33+gdata/cj50+gdata/dk92+gdata/fs38+gdata/ik11+gdata/oi10+gdata/p73+gdata/rr3+gdata/xp65
       version: '{{version}}'
     parameters:
       version:
-        default: v0.1.2
+        default: v0.1.3
         description: Catalog version
         type: str
```

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/source/__init__.py` & `access_nri_intake-0.1.3/src/access_nri_intake/source/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/source/builders.py` & `access_nri_intake-0.1.3/src/access_nri_intake/source/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/source/utils.py` & `access_nri_intake-0.1.3/src/access_nri_intake/source/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake/utils.py` & `access_nri_intake-0.1.3/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.1.3/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.1.2
+Version: 0.1.3
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `access_nri_intake-0.1.2/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.1.3/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_builders.py` & `access_nri_intake-0.1.3/tests/test_builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_cli.py` & `access_nri_intake-0.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_manager.py` & `access_nri_intake-0.1.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_source_utils.py` & `access_nri_intake-0.1.3/tests/test_source_utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_translators.py` & `access_nri_intake-0.1.3/tests/test_translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/tests/test_utils.py` & `access_nri_intake-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.1.2/versioneer.py` & `access_nri_intake-0.1.3/versioneer.py`

 * *Files identical despite different names*

