# Comparing `tmp/airbyte_source_surveymonkey-0.3.0.tar.gz` & `tmp/airbyte_source_surveymonkey-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_surveymonkey-0.3.0.tar", max compression
+gzip compressed data, was "airbyte_source_surveymonkey-0.3.1.tar", max compression
```

## Comparing `airbyte_source_surveymonkey-0.3.0.tar` & `airbyte_source_surveymonkey-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4609 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/README.md
--rw-r--r--   0        0        0      818 2024-04-01 21:13:51.251355 airbyte_source_surveymonkey-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1244 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/components.py
--rw-r--r--   0        0        0     2620 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/config_migrations.py
--rw-r--r--   0        0        0    15740 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/manifest.yaml
--rw-r--r--   0        0        0      347 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/run.py
--rw-r--r--   0        0        0     1869 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/collectors.json
--rw-r--r--   0        0        0      352 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_collectors.json
--rw-r--r--   0        0        0      320 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_ids.json
--rw-r--r--   0        0        0      447 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_pages.json
--rw-r--r--   0        0        0     2700 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_questions.json
--rw-r--r--   0        0        0     2515 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_responses.json
--rw-r--r--   0        0        0     1791 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/surveys.json
--rw-r--r--   0        0        0     2344 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/source.py
--rw-r--r--   0        0        0     8428 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/streams.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4609 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/README.md
+-rw-r--r--   0        0        0      822 2024-05-07 12:32:06.325868 airbyte_source_surveymonkey-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1244 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/components.py
+-rw-r--r--   0        0        0     2620 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/config_migrations.py
+-rw-r--r--   0        0        0    15740 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/manifest.yaml
+-rw-r--r--   0        0        0      347 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/run.py
+-rw-r--r--   0        0        0     3791 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/collectors.json
+-rw-r--r--   0        0        0      660 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_collectors.json
+-rw-r--r--   0        0        0      588 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_ids.json
+-rw-r--r--   0        0        0      815 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_pages.json
+-rw-r--r--   0        0        0     4871 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_questions.json
+-rw-r--r--   0        0        0     4641 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_responses.json
+-rw-r--r--   0        0        0     3390 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/surveys.json
+-rw-r--r--   0        0        0     2344 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/source.py
+-rw-r--r--   0        0        0     8428 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/streams.py
+-rw-r--r--   0        0        0     5397 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.1/PKG-INFO
```

### Comparing `airbyte_source_surveymonkey-0.3.0/README.md` & `airbyte_source_surveymonkey-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/pyproject.toml` & `airbyte_source_surveymonkey-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.0"
+version = "0.3.1"
 name = "airbyte-source-surveymonkey"
 description = "Source implementation for Surveymonkey."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_surveymonkey" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 vcrpy = "==4.1.1"
 urllib3 = "==1.26.18"
 
 [tool.poetry.scripts]
 source-surveymonkey = "source_surveymonkey.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/__init__.py` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/components.py` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/config_migrations.py` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/manifest.yaml` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/source.py` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/streams.py` & `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.0/PKG-INFO` & `airbyte_source_surveymonkey-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-surveymonkey
-Version: 0.3.0
+Version: 0.3.1
 Summary: Source implementation for Surveymonkey.
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
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Requires-Dist: urllib3 (==1.26.18)
 Requires-Dist: vcrpy (==4.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/surveymonkey
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Surveymonkey source connector
```

