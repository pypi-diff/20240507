# Comparing `tmp/airbyte_source_amplitude-0.3.7.tar.gz` & `tmp/airbyte_source_amplitude-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_amplitude-0.3.7.tar", max compression
+gzip compressed data, was "airbyte_source_amplitude-0.3.8.tar", max compression
```

## Comparing `airbyte_source_amplitude-0.3.7.tar` & `airbyte_source_amplitude-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4550 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/README.md
--rw-r--r--   0        0        0      763 2024-02-12 12:56:43.973142 airbyte_source_amplitude-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      130 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/__init__.py
--rw-r--r--   0        0        0     4554 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/components.py
--rw-r--r--   0        0        0     4244 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/manifest.yaml
--rw-r--r--   0        0        0      239 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/run.py
--rw-r--r--   0        0        0      240 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/schemas/active_users.json
--rw-r--r--   0        0        0      345 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/schemas/annotations.json
--rw-r--r--   0        0        0      241 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/schemas/average_session_length.json
--rw-r--r--   0        0        0     1837 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/schemas/cohorts.json
--rw-r--r--   0        0        0     3913 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/schemas/events.json
--rw-r--r--   0        0        0     1595 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/source.py
--rw-r--r--   0        0        0     1836 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/spec.yaml
--rw-r--r--   0        0        0     8061 2024-02-12 12:10:14.000000 airbyte_source_amplitude-0.3.7/source_amplitude/streams.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 airbyte_source_amplitude-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     4550 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/README.md
+-rw-r--r--   0        0        0      757 2024-03-12 19:14:47.042841 airbyte_source_amplitude-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/components.py
+-rw-r--r--   0        0        0     4244 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/run.py
+-rw-r--r--   0        0        0      240 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/schemas/active_users.json
+-rw-r--r--   0        0        0      345 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/schemas/annotations.json
+-rw-r--r--   0        0        0      241 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/schemas/average_session_length.json
+-rw-r--r--   0        0        0     1837 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/schemas/cohorts.json
+-rw-r--r--   0        0        0     3913 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/schemas/events.json
+-rw-r--r--   0        0        0     1595 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/source.py
+-rw-r--r--   0        0        0     1836 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/spec.yaml
+-rw-r--r--   0        0        0     8061 2024-03-12 16:19:19.000000 airbyte_source_amplitude-0.3.8/source_amplitude/streams.py
+-rw-r--r--   0        0        0     5261 1970-01-01 00:00:00.000000 airbyte_source_amplitude-0.3.8/PKG-INFO
```

### Comparing `airbyte_source_amplitude-0.3.7/README.md` & `airbyte_source_amplitude-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/pyproject.toml` & `airbyte_source_amplitude-0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.7"
+version = "0.3.8"
 name = "airbyte-source-amplitude"
 description = "Source implementation for Amplitude."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_amplitude" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "==0.52.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-amplitude = "source_amplitude.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/components.py` & `airbyte_source_amplitude-0.3.8/source_amplitude/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/manifest.yaml` & `airbyte_source_amplitude-0.3.8/source_amplitude/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/schemas/cohorts.json` & `airbyte_source_amplitude-0.3.8/source_amplitude/schemas/cohorts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/schemas/events.json` & `airbyte_source_amplitude-0.3.8/source_amplitude/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/source.py` & `airbyte_source_amplitude-0.3.8/source_amplitude/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/spec.yaml` & `airbyte_source_amplitude-0.3.8/source_amplitude/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/source_amplitude/streams.py` & `airbyte_source_amplitude-0.3.8/source_amplitude/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amplitude-0.3.7/PKG-INFO` & `airbyte_source_amplitude-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-amplitude
-Version: 0.3.7
+Version: 0.3.8
 Summary: Source implementation for Amplitude.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.52.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/amplitude
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Amplitude source connector
```

