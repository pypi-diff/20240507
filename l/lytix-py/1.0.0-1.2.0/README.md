# Comparing `tmp/lytix_py-1.0.0.tar.gz` & `tmp/lytix_py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.0.0.tar", last modified: Sun May  5 22:04:52 2024, max compression
+gzip compressed data, was "lytix_py-1.2.0.tar", last modified: Tue May  7 21:46:28 2024, max compression
```

## Comparing `lytix_py-1.0.0.tar` & `lytix_py-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:04:52.774834 lytix_py-1.0.0/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.0.0/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-05 22:04:52.774643 lytix_py-1.0.0/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.0.0/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-05 22:04:49.000000 lytix_py-1.0.0/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-05 22:04:52.774873 lytix_py-1.0.0/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:04:52.772371 lytix_py-1.0.0/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:04:52.773326 lytix_py-1.0.0/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:04:52.774105 lytix_py-1.0.0/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1335 2024-05-05 22:00:04.000000 lytix_py-1.0.0/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:00:47.000000 lytix_py-1.0.0/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      403 2024-05-05 21:48:37.000000 lytix_py-1.0.0/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-05 22:04:52.774428 lytix_py-1.0.0/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-05 22:04:52.000000 lytix_py-1.0.0/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      311 2024-05-05 22:04:52.000000 lytix_py-1.0.0/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-05 22:04:52.000000 lytix_py-1.0.0/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-05 22:04:52.000000 lytix_py-1.0.0/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-05 22:04:52.000000 lytix_py-1.0.0/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.094629 lytix_py-1.2.0/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.2.0/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-07 21:46:28.094431 lytix_py-1.2.0/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.2.0/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-07 21:15:12.000000 lytix_py-1.2.0/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-07 21:46:28.094682 lytix_py-1.2.0/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.092205 lytix_py-1.2.0/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.093049 lytix_py-1.2.0/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.093870 lytix_py-1.2.0/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.2.0/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.094015 lytix_py-1.2.0/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1826 2024-05-07 21:14:13.000000 lytix_py-1.2.0/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      102 2024-05-07 21:15:04.000000 lytix_py-1.2.0/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      403 2024-05-05 21:48:37.000000 lytix_py-1.2.0/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-07 21:46:28.094206 lytix_py-1.2.0/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-07 21:46:28.000000 lytix_py-1.2.0/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-07 21:46:28.000000 lytix_py-1.2.0/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-07 21:46:28.000000 lytix_py-1.2.0/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-07 21:46:28.000000 lytix_py-1.2.0/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-07 21:46:28.000000 lytix_py-1.2.0/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.0.0/LICENSE.md` & `lytix_py-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.0.0/PKG-INFO` & `lytix_py-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.0.0
+Version: 1.2.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.0.0/pyproject.toml` & `lytix_py-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.0.0"
+version = "1.2.0"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.0.0/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.2.0/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from lytix_py.envVars import LX_API_KEY, LX_BASE_URL
 import os.path
 
 """
  Main class to collect and report metrics
  back to HQ
 """
-class MetricCollector:
+class _MetricCollector:
     _apiKey: str = None
     _baseURL: str = None
     # _logger: str = None
 
     def __init__(self):
         self._apiKey = LX_API_KEY
         self._baseURL = urljoin(LX_BASE_URL, "/v1/metrics")
@@ -39,7 +39,24 @@
             metricMetadata = {}
         body = {
             "metricName": metricName,
             "metricValue": metricValue,
             "metadata": metricMetadata
         }
         self._sendPostRequest("increment", body)
+
+    """
+    Capture a model input/output
+    """
+    def captureModelIO(self, modelName: str, userInput: str, modelOutput: str, metricMetadata: dict = None):
+        if metricMetadata is None:
+            metricMetadata = {}
+        body = {
+            "modelName": modelName,
+            "userInput": userInput,
+            "modelOutput": modelOutput,
+            "metadata": metricMetadata
+        }
+        self._sendPostRequest("modelIO", body)
+
+MetricCollector = _MetricCollector()
+
```

### Comparing `lytix_py-1.0.0/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.2.0/src/lytix_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.0.0
+Version: 1.2.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

