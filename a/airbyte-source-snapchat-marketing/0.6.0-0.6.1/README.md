# Comparing `tmp/airbyte_source_snapchat_marketing-0.6.0.tar.gz` & `tmp/airbyte_source_snapchat_marketing-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_snapchat_marketing-0.6.0.tar", max compression
+gzip compressed data, was "airbyte_source_snapchat_marketing-0.6.1.tar", max compression
```

## Comparing `airbyte_source_snapchat_marketing-0.6.0.tar` & `airbyte_source_snapchat_marketing-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4712 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/README.md
--rw-r--r--   0        0        0      811 2024-04-10 08:57:27.640394 airbyte_source_snapchat_marketing-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1156 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/__init__.py
--rw-r--r--   0        0        0      264 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/run.py
--rw-r--r--   0        0        0     1236 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adaccounts.json
--rw-r--r--   0        0        0      893 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/ads.json
--rw-r--r--   0        0        0     4855 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adsquads.json
--rw-r--r--   0        0        0     5087 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/basic_stats.json
--rw-r--r--   0        0        0      767 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0     1829 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/creatives.json
--rw-r--r--   0        0        0     1175 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/media.json
--rw-r--r--   0        0        0     1600 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/organizations.json
--rw-r--r--   0        0        0      980 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/segments.json
--rw-r--r--   0        0        0    31941 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/source.py
--rw-r--r--   0        0        0     3503 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/spec.json
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4712 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/README.md
+-rw-r--r--   0        0        0      815 2024-05-07 12:32:32.839530 airbyte_source_snapchat_marketing-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1156 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/__init__.py
+-rw-r--r--   0        0        0      264 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/run.py
+-rw-r--r--   0        0        0     2621 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adaccounts.json
+-rw-r--r--   0        0        0     1656 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/ads.json
+-rw-r--r--   0        0        0     8945 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/adsquads.json
+-rw-r--r--   0        0        0     9688 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/basic_stats.json
+-rw-r--r--   0        0        0     1659 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     3783 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/creatives.json
+-rw-r--r--   0        0        0     2391 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/media.json
+-rw-r--r--   0        0        0     3489 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/organizations.json
+-rw-r--r--   0        0        0     2062 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/segments.json
+-rw-r--r--   0        0        0    31941 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/source.py
+-rw-r--r--   0        0        0     3503 2024-05-07 10:59:11.000000 airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/spec.json
+-rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.6.1/PKG-INFO
```

### Comparing `airbyte_source_snapchat_marketing-0.6.0/README.md` & `airbyte_source_snapchat_marketing-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.0/pyproject.toml` & `airbyte_source_snapchat_marketing-0.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.6.0"
+version = "0.6.1"
 name = "airbyte-source-snapchat-marketing"
 description = "Source implementation for Snapchat Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_snapchat_marketing" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-snapchat-marketing = "source_snapchat_marketing.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
 pytest = "^6.1"
```

### Comparing `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/__init__.py` & `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/organizations.json` & `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/schemas/segments.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7734375%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the segment'}, 'updated_at': "*

 * *                 "{'description': 'The date and time when the segment was last updated'}, "*

 * *                 "'created_at': {'description': 'The date and time when the segment was created'}, "*

 * *                 "'name': {'description': 'Name or title of the segment'}, 'ad_account_id': "*

 * *                 "OrderedDict([('description', 'The unique identifier for the ad account "*

 * *                 "associated with the s […]*

```diff
@@ -1,154 +1,112 @@
 {
     "properties": {
-        "accepted_term_version": {
+        "ad_account_id": {
+            "description": "The unique identifier for the ad account associated with the segment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "address_line_1": {
+        "approximate_number_users": {
+            "description": "Approximate number of users within the segment",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "administrative_district_level_1": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "configuration_settings": {
-            "properties": {
-                "notifications_enabled": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "contact_email": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
-        "contact_name": {
+        "created_at": {
+            "description": "The date and time when the segment was created",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "contact_phone": {
+        "description": {
+            "description": "Brief description of the segment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "contact_phone_optin": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "country": {
+        "id": {
+            "description": "Unique identifier for the segment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "createdByCaller": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "created_at": {
+        "name": {
+            "description": "Name or title of the segment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "organization_id": {
+            "description": "Unique identifier for the organization to which the segment belongs",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "locality": {
+        "retention_in_days": {
+            "description": "Number of days for which the segment data is retained",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "my_display_name": {
+        "source_type": {
+            "description": "Type of the source data used to create the segment",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "my_invited_email": {
+        "status": {
+            "description": "Current status of the segment (e.g., active, inactive)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "my_member_id": {
+        "targetable_status": {
+            "description": "Status indicating whether the segment can be targeted in marketing campaigns",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
+        "updated_at": {
+            "description": "The date and time when the segment was last updated",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "postal_code": {
+        "upload_status": {
+            "description": "Status of the segment upload process (e.g., pending, completed)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "roles": {
+        "visible_to": {
+            "description": "Visibility setting for the segment, determining who can access it",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
-        },
-        "state": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "updated_at": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/source.py` & `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/spec.json` & `airbyte_source_snapchat_marketing-0.6.1/source_snapchat_marketing/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.6.0/PKG-INFO` & `airbyte_source_snapchat_marketing-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-snapchat-marketing
-Version: 0.6.0
+Version: 0.6.1
 Summary: Source implementation for Snapchat Marketing.
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
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/snapchat-marketing
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Snapchat-Marketing source connector
```

