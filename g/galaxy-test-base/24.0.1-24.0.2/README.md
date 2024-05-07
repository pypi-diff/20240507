# Comparing `tmp/galaxy_test_base-24.0.1.tar.gz` & `tmp/galaxy_test_base-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_test_base-24.0.1.tar", last modified: Thu May  2 13:48:46 2024, max compression
+gzip compressed data, was "galaxy_test_base-24.0.2.tar", last modified: Tue May  7 14:33:52 2024, max compression
```

## Comparing `galaxy_test_base-24.0.1.tar` & `galaxy_test_base-24.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.049886 galaxy_test_base-24.0.1/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.053886 galaxy_test_base-24.0.1/galaxy_test/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api_asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/galaxy_test/base/data/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/minimal_tool_no_id.json
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_2.ga
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_batch.ga
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_matching_lists.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_missing_tool.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_pause.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity.ga
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_two_random_lines.ga
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_validation_1.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_input_tags.ga
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   135637 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/populators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/rules_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/uses_shed_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/base/workflow_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:48:46.000000 galaxy_test_base-24.0.1/galaxy_test_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 13:48:46.057886 galaxy_test_base-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_test_base-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:52.004832 galaxy_test_base-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_test_base-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-07 14:33:52.004832 galaxy_test_base-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:51.996832 galaxy_test_base-24.0.2/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:52.000832 galaxy_test_base-24.0.2/galaxy_test/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/api_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:52.000832 galaxy_test_base-24.0.2/galaxy_test/base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/minimal_tool_no_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_2.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_batch.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_matching_lists.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_missing_tool.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_topoambigouity.ga
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_two_random_lines.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_validation_1.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_with_input_tags.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_with_runtime_input.ga
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135637 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/rules_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/uses_shed_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/base/workflow_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:52.004832 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-07 14:33:51.000000 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-07 14:33:51.000000 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:33:51.000000 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 14:33:51.000000 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 14:33:51.000000 galaxy_test_base-24.0.2/galaxy_test_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-07 14:33:52.004832 galaxy_test_base-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_test_base-24.0.2/test-requirements.txt
```

### Comparing `galaxy_test_base-24.0.1/HISTORY.rst` & `galaxy_test_base-24.0.2/HISTORY.rst`

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

### Comparing `galaxy_test_base-24.0.1/LICENSE` & `galaxy_test_base-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/PKG-INFO` & `galaxy_test_base-24.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,14 +51,20 @@
 
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

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/api.py` & `galaxy_test_base-24.0.2/galaxy_test/base/api.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/api_asserts.py` & `galaxy_test_base-24.0.2/galaxy_test/base/api_asserts.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/api_util.py` & `galaxy_test_base-24.0.2/galaxy_test/base/api_util.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_subworkflow_with_integer_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_1.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_2.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_2.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_batch.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_batch.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_map_reduce_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_matching_lists.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_matching_lists.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_missing_tool.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_missing_tool.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_pause.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_topoambigouity.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_two_random_lines.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_two_random_lines.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_validation_1.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_validation_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_input_tags.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_with_input_tags.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga` & `galaxy_test_base-24.0.2/galaxy_test/base/data/test_workflow_with_runtime_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/decorators.py` & `galaxy_test_base-24.0.2/galaxy_test/base/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/env.py` & `galaxy_test_base-24.0.2/galaxy_test/base/env.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/interactor.py` & `galaxy_test_base-24.0.2/galaxy_test/base/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/json_schema_utils.py` & `galaxy_test_base-24.0.2/galaxy_test/base/json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/populators.py` & `galaxy_test_base-24.0.2/galaxy_test/base/populators.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/rules_test_data.py` & `galaxy_test_base-24.0.2/galaxy_test/base/rules_test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/testcase.py` & `galaxy_test_base-24.0.2/galaxy_test/base/testcase.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/uses_shed_api.py` & `galaxy_test_base-24.0.2/galaxy_test/base/uses_shed_api.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test/base/workflow_fixtures.py` & `galaxy_test_base-24.0.2/galaxy_test/base/workflow_fixtures.py`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/galaxy_test_base.egg-info/PKG-INFO` & `galaxy_test_base-24.0.2/galaxy_test_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,14 +51,20 @@
 
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

### Comparing `galaxy_test_base-24.0.1/galaxy_test_base.egg-info/SOURCES.txt` & `galaxy_test_base-24.0.2/galaxy_test_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_test_base-24.0.1/setup.cfg` & `galaxy_test_base-24.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-base
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-tool-util
 	galaxy-util
 	bioblend
```

