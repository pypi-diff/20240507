# Comparing `tmp/airbyte_source_typeform-1.2.7.tar.gz` & `tmp/airbyte_source_typeform-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_typeform-1.2.7.tar", max compression
+gzip compressed data, was "airbyte_source_typeform-1.2.8.tar", max compression
```

## Comparing `airbyte_source_typeform-1.2.7.tar` & `airbyte_source_typeform-1.2.8.tar`

### file list

```diff
@@ -1,14 +1,8 @@
--rw-r--r--   0        0        0     4532 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/README.md
--rw-r--r--   0        0        0      751 2024-05-02 16:02:20.843582 airbyte_source_typeform-1.2.7/pyproject.toml
--rw-r--r--   0        0        0      128 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/__init__.py
--rw-r--r--   0        0        0     1604 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/components.py
--rw-r--r--   0        0        0    10424 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/run.py
--rw-r--r--   0        0        0    16449 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/forms.json
--rw-r--r--   0        0        0      557 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/images.json
--rw-r--r--   0        0        0     3970 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/responses.json
--rw-r--r--   0        0        0     1754 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/themes.json
--rw-r--r--   0        0        0      555 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/webhooks.json
--rw-r--r--   0        0        0      750 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/schemas/workspaces.json
--rw-r--r--   0        0        0      477 2024-05-02 14:37:40.000000 airbyte_source_typeform-1.2.7/source_typeform/source.py
--rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 airbyte_source_typeform-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     4532 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/README.md
+-rw-r--r--   0        0        0      755 2024-05-07 13:33:52.112189 airbyte_source_typeform-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/source_typeform/__init__.py
+-rw-r--r--   0        0        0     1604 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/source_typeform/components.py
+-rw-r--r--   0        0        0    58456 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/source_typeform/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/source_typeform/run.py
+-rw-r--r--   0        0        0      477 2024-05-07 10:08:25.000000 airbyte_source_typeform-1.2.8/source_typeform/source.py
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_typeform-1.2.8/PKG-INFO
```

### Comparing `airbyte_source_typeform-1.2.7/README.md` & `airbyte_source_typeform-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_typeform-1.2.7/pyproject.toml` & `airbyte_source_typeform-1.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.2.7"
+version = "1.2.8"
 name = "airbyte-source-typeform"
 description = "Source implementation for Typeform."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_typeform" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.85.0"
 
 [tool.poetry.scripts]
 source-typeform = "source_typeform.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_typeform-1.2.7/source_typeform/components.py` & `airbyte_source_typeform-1.2.8/source_typeform/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_typeform-1.2.7/PKG-INFO` & `airbyte_source_typeform-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-typeform
-Version: 1.2.7
+Version: 1.2.8
 Summary: Source implementation for Typeform.
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
+Requires-Dist: airbyte-cdk (==0.85.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/typeform
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Typeform source connector
```

