# Comparing `tmp/galaxy_job_metrics-24.0.1.tar.gz` & `tmp/galaxy_job_metrics-24.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy_job_metrics-24.0.1.tar", last modified: Thu May  2 13:47:30 2024, max compression
+gzip compressed data, was "galaxy_job_metrics-24.0.2.tar", last modified: Tue May  7 14:32:35 2024, max compression
```

## Comparing `galaxy_job_metrics-24.0.1.tar` & `galaxy_job_metrics-24.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:30.909470 galaxy_job_metrics-24.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-02 13:47:30.909470 galaxy_job_metrics-24.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:30.905470 galaxy_job_metrics-24.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:30.905470 galaxy_job_metrics-24.0.1/galaxy/job_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:30.905470 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/meminfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/uname.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/job_metrics/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:30.909470 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-02 13:47:30.000000 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-02 13:47:30.000000 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:30.000000 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:47:30.000000 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:30.000000 galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-02 13:47:30.909470 galaxy_job_metrics-24.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_job_metrics-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:35.661323 galaxy_job_metrics-24.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-07 14:31:49.000000 galaxy_job_metrics-24.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 14:32:35.661323 galaxy_job_metrics-24.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:35.657323 galaxy_job_metrics-24.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:35.657323 galaxy_job_metrics-24.0.2/galaxy/job_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:35.661323 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/meminfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/uname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/job_metrics/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:32:35.661323 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 14:32:35.000000 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-07 14:32:35.000000 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:32:35.000000 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 14:32:35.000000 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:32:35.000000 galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 14:32:35.661323 galaxy_job_metrics-24.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:31:50.000000 galaxy_job_metrics-24.0.2/test-requirements.txt
```

### Comparing `galaxy_job_metrics-24.0.1/HISTORY.rst` & `galaxy_job_metrics-24.0.2/HISTORY.rst`

 * *Files 2% similar despite different names*

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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_job_metrics-24.0.1/LICENSE` & `galaxy_job_metrics-24.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/PKG-INFO` & `galaxy_job_metrics-24.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/__init__.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/formatting.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/formatting.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/__init__.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/cgroup.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/cgroup.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/core.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/core.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/env.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/env.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/hostname.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/hostname.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/meminfo.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/meminfo.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy/job_metrics/instrumenters/uname.py` & `galaxy_job_metrics-24.0.2/galaxy/job_metrics/instrumenters/uname.py`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/PKG-INFO` & `galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 24.0.1
+Version: 24.0.2
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
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
 
 No recorded changes since last release
 
 -------------------
 24.0.0 (2024-04-02)
```

### Comparing `galaxy_job_metrics-24.0.1/galaxy_job_metrics.egg-info/SOURCES.txt` & `galaxy_job_metrics-24.0.2/galaxy_job_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy_job_metrics-24.0.1/setup.cfg` & `galaxy_job_metrics-24.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-metrics
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.1
+version = 24.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 packages = find:
 python_requires = >=3.7
```

