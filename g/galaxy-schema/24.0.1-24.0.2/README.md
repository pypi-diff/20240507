# Comparing `tmp/galaxy_schema-24.0.1.tar.gz` & `tmp/galaxy_schema-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_schema-24.0.1.tar", last modified: Thu May  2 13:47:57 2024, max compression
+gzip compressed data, was "galaxy_schema-24.0.2.tar", last modified: Tue May  7 14:33:03 2024, max compression
```

## Comparing `galaxy_schema-24.0.1.tar` & `galaxy_schema-24.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.925628 galaxy_schema-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.929628 galaxy_schema-24.0.1/galaxy/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/bco/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/description_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/error_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/execution_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/io_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/parametric_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/provenance_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/usability_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/bco/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/drs/
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)   118022 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflow/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/galaxy/schema/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/galaxy_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:57.000000 galaxy_schema-24.0.1/galaxy_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-02 13:47:57.933628 galaxy_schema-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_schema-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_schema-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.097161 galaxy_schema-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/galaxy/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/galaxy/schema/bco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/description_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/error_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/execution_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/io_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/parametric_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/provenance_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/usability_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/bco/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/galaxy/schema/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118022 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/galaxy/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/workflow/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/galaxy/schema/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/galaxy_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-07 14:33:03.000000 galaxy_schema-24.0.2/galaxy_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-07 14:33:03.000000 galaxy_schema-24.0.2/galaxy_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:33:03.000000 galaxy_schema-24.0.2/galaxy_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 14:33:03.000000 galaxy_schema-24.0.2/galaxy_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:33:03.000000 galaxy_schema-24.0.2/galaxy_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-07 14:33:03.101161 galaxy_schema-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_schema-24.0.2/test-requirements.txt
```

### Comparing `galaxy_schema-24.0.1/HISTORY.rst` & `galaxy_schema-24.0.2/HISTORY.rst`

 * *Files 4% similar despite different names*

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

### Comparing `galaxy_schema-24.0.1/LICENSE` & `galaxy_schema-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/PKG-INFO` & `galaxy_schema-24.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-schema
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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

### Comparing `galaxy_schema-24.0.1/galaxy/schema/__init__.py` & `galaxy_schema-24.0.2/galaxy/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/__init__.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/description_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/description_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/error_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/error_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/execution_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/execution_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/io_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/io_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/parametric_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/parametric_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/provenance_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/provenance_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/usability_domain.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/usability_domain.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/bco/util.py` & `galaxy_schema-24.0.2/galaxy/schema/bco/util.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/cloud.py` & `galaxy_schema-24.0.2/galaxy/schema/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/drs/__init__.py` & `galaxy_schema-24.0.2/galaxy/schema/drs/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/fetch_data.py` & `galaxy_schema-24.0.2/galaxy/schema/fetch_data.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/fields.py` & `galaxy_schema-24.0.2/galaxy/schema/fields.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/groups.py` & `galaxy_schema-24.0.2/galaxy/schema/groups.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/help.py` & `galaxy_schema-24.0.2/galaxy/schema/help.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/history.py` & `galaxy_schema-24.0.2/galaxy/schema/history.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/invocation.py` & `galaxy_schema-24.0.2/galaxy/schema/invocation.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/item_tags.py` & `galaxy_schema-24.0.2/galaxy/schema/item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/jobs.py` & `galaxy_schema-24.0.2/galaxy/schema/jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/notifications.py` & `galaxy_schema-24.0.2/galaxy/schema/notifications.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/remote_files.py` & `galaxy_schema-24.0.2/galaxy/schema/remote_files.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/schema.py` & `galaxy_schema-24.0.2/galaxy/schema/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/storage_cleaner.py` & `galaxy_schema-24.0.2/galaxy/schema/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/tasks.py` & `galaxy_schema-24.0.2/galaxy/schema/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/types.py` & `galaxy_schema-24.0.2/galaxy/schema/types.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/visualization.py` & `galaxy_schema-24.0.2/galaxy/schema/visualization.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/workflow/comments.py` & `galaxy_schema-24.0.2/galaxy/schema/workflow/comments.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy/schema/workflows.py` & `galaxy_schema-24.0.2/galaxy/schema/workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/galaxy_schema.egg-info/PKG-INFO` & `galaxy_schema-24.0.2/galaxy_schema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-schema
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,20 @@
 
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

### Comparing `galaxy_schema-24.0.1/galaxy_schema.egg-info/SOURCES.txt` & `galaxy_schema-24.0.2/galaxy_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_schema-24.0.1/setup.cfg` & `galaxy_schema-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-schema
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	pydantic[email]>=2,!=2.6.0,!=2.6.1
 packages = find:
```

