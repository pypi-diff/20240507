# Comparing `tmp/gaarf-exporter-0.7.0.dev2.tar.gz` & `tmp/gaarf-exporter-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaarf-exporter-0.7.0.dev2.tar", last modified: Sun Mar 24 07:24:41 2024, max compression
+gzip compressed data, was "gaarf-exporter-0.7.0rc1.tar", last modified: Mon Mar 25 13:31:25 2024, max compression
```

## Comparing `gaarf-exporter-0.7.0.dev2.tar` & `gaarf-exporter-0.7.0rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-24 07:24:41.373604 gaarf-exporter-0.7.0.dev2/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5744 2024-03-24 07:24:41.373604 gaarf-exporter-0.7.0.dev2/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5270 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-24 07:24:41.369604 gaarf-exporter-0.7.0.dev2/gaarf_exporter/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1287 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/alert.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/alert_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1971 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/bootstrap.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    28882 2024-03-24 05:05:19.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3687 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7548 2024-03-24 07:22:06.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/main.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2799 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      908 2024-03-15 19:34:24.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/search_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8745 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter/util.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-24 07:24:41.369604 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5744 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      775 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-03-24 07:24:41.000000 gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-03-24 07:24:41.373604 gaarf-exporter-0.7.0.dev2/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1557 2024-03-24 07:24:18.000000 gaarf-exporter-0.7.0.dev2/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-24 07:24:41.373604 gaarf-exporter-0.7.0.dev2/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0.dev2/tests/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3950 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/conftest.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_alerts.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2670 2024-03-21 10:06:54.000000 gaarf-exporter-0.7.0.dev2/tests/test_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2349 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_query_element.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    12589 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0.dev2/tests/test_util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5742 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5270 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/gaarf_exporter/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1287 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/alert.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/alert_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1971 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/bootstrap.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    28882 2024-03-24 05:05:19.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3687 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/config.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7548 2024-03-24 07:22:06.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/main.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2799 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      908 2024-03-15 19:34:24.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/search_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8745 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter/util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5742 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      775 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-03-25 13:31:25.000000 gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1556 2024-03-25 13:18:51.000000 gaarf-exporter-0.7.0rc1/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-03-25 13:31:25.391427 gaarf-exporter-0.7.0rc1/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.0rc1/tests/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3950 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/conftest.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_alerts.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2670 2024-03-21 10:06:54.000000 gaarf-exporter-0.7.0rc1/tests/test_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2349 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_config.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_query_element.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    12589 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.0rc1/tests/test_util.py
```

### Comparing `gaarf-exporter-0.7.0.dev2/PKG-INFO` & `gaarf-exporter-0.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 0.7.0.dev2
+Version: 0.7.0rc1
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
```

### Comparing `gaarf-exporter-0.7.0.dev2/README.md` & `gaarf-exporter-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/alert.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/alert.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/alert_elements.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/alert_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/bootstrap.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/collectors.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/collectors.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/config.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/config.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/exporter.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/main.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/main.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/query_elements.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/search_collectors.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/search_collectors.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/target.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/target.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter/util.py` & `gaarf-exporter-0.7.0rc1/gaarf_exporter/util.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/PKG-INFO` & `gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 0.7.0.dev2
+Version: 0.7.0rc1
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
```

### Comparing `gaarf-exporter-0.7.0.dev2/gaarf_exporter.egg-info/SOURCES.txt` & `gaarf-exporter-0.7.0rc1/gaarf_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/setup.py` & `gaarf-exporter-0.7.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
 setup(
   name='gaarf-exporter',
-  version='0.7.0.dev2',
+  version='0.7.0.rc1',
   long_description=README,
   long_description_content_type='text/markdown',
   author='Google Inc. (gTech gPS CSE team)',
   author_email='no-reply@google.com',
   license='Apache 2.0',
   classifiers=[
     'Programming Language :: Python :: 3',
```

### Comparing `gaarf-exporter-0.7.0.dev2/tests/conftest.py` & `gaarf-exporter-0.7.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_alerts.py` & `gaarf-exporter-0.7.0rc1/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_collectors.py` & `gaarf-exporter-0.7.0rc1/tests/test_collectors.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_config.py` & `gaarf-exporter-0.7.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_exporter.py` & `gaarf-exporter-0.7.0rc1/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_query_element.py` & `gaarf-exporter-0.7.0rc1/tests/test_query_element.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_target.py` & `gaarf-exporter-0.7.0rc1/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.0.dev2/tests/test_util.py` & `gaarf-exporter-0.7.0rc1/tests/test_util.py`

 * *Files identical despite different names*

