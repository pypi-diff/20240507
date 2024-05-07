# Comparing `tmp/airbyte_source_zendesk_talk-0.2.0.tar.gz` & `tmp/airbyte_source_zendesk_talk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_talk-0.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_talk-0.2.1.tar", max compression
```

## Comparing `airbyte_source_zendesk_talk-0.2.0.tar` & `airbyte_source_zendesk_talk-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4609 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/README.md
--rw-r--r--   0        0        0      773 2024-03-29 18:36:53.739496 airbyte_source_zendesk_talk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      132 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/__init__.py
--rw-r--r--   0        0        0      246 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/run.py
--rw-r--r--   0        0        0     1779 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/account_overview.json
--rw-r--r--   0        0        0      614 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/addresses.json
--rw-r--r--   0        0        0     1742 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/agents_activity.json
--rw-r--r--   0        0        0     1654 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/agents_overview.json
--rw-r--r--   0        0        0     1685 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/call_legs.json
--rw-r--r--   0        0        0     2728 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/calls.json
--rw-r--r--   0        0        0      570 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/current_queue_activity.json
--rw-r--r--   0        0        0      208 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/greeting_categories.json
--rw-r--r--   0        0        0     1000 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/greetings.json
--rw-r--r--   0        0        0      385 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/ivr_menus.json
--rw-r--r--   0        0        0      628 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/ivr_routes.json
--rw-r--r--   0        0        0     1829 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/ivrs.json
--rw-r--r--   0        0        0     2251 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/phone_numbers.json
--rw-r--r--   0        0        0     2939 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/source.py
--rw-r--r--   0        0        0     4827 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/spec.json
--rw-r--r--   0        0        0    11179 2024-03-29 17:25:06.000000 airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/streams.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 airbyte_source_zendesk_talk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4609 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/README.md
+-rw-r--r--   0        0        0      777 2024-05-07 13:35:03.082929 airbyte_source_zendesk_talk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/run.py
+-rw-r--r--   0        0        0     3487 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/account_overview.json
+-rw-r--r--   0        0        0     1180 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/addresses.json
+-rw-r--r--   0        0        0     3514 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/agents_activity.json
+-rw-r--r--   0        0        0     3269 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/agents_overview.json
+-rw-r--r--   0        0        0     3573 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/call_legs.json
+-rw-r--r--   0        0        0     5438 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/calls.json
+-rw-r--r--   0        0        0     1401 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/current_queue_activity.json
+-rw-r--r--   0        0        0      332 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/greeting_categories.json
+-rw-r--r--   0        0        0     1953 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/greetings.json
+-rw-r--r--   0        0        0      727 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/ivr_menus.json
+-rw-r--r--   0        0        0     1337 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/ivr_routes.json
+-rw-r--r--   0        0        0     3394 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/ivrs.json
+-rw-r--r--   0        0        0     4444 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/phone_numbers.json
+-rw-r--r--   0        0        0     2939 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/source.py
+-rw-r--r--   0        0        0     4827 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/spec.json
+-rw-r--r--   0        0        0    11179 2024-05-07 10:06:52.000000 airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/streams.py
+-rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 airbyte_source_zendesk_talk-0.2.1/PKG-INFO
```

### Comparing `airbyte_source_zendesk_talk-0.2.0/README.md` & `airbyte_source_zendesk_talk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_talk-0.2.0/pyproject.toml` & `airbyte_source_zendesk_talk-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.0"
+version = "0.2.1"
 name = "airbyte-source-zendesk-talk"
 description = "Source implementation for Zendesk Talk."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_zendesk_talk" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-zendesk-talk = "source_zendesk_talk.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6"
```

### Comparing `airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/agents_overview.json` & `airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/greetings.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('active', OrderedDict([('description', 'Indicates if the "*

 * *                 "greeting is currently active or not'), ('type', ['null', 'boolean'])])), "*

 * *                 "('audio_name', OrderedDict([('description', 'Name of the audio file for the "*

 * *                 "greeting'), ('type', ['null', 'string'])])), ('audio_url', "*

 * *                 "OrderedDict([('description', 'URL to access the audio file for the greeting'), "*

 * *                 "('type', ['null', 'string' […]*

```diff
@@ -1,134 +1,110 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "average_accepted_transfers": {
+        "active": {
+            "description": "Indicates if the greeting is currently active or not",
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "average_available_time": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_away_time": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_calls_accepted": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_calls_denied": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_calls_missed": {
-            "type": [
-                "null",
-                "integer"
+                "boolean"
             ]
         },
-        "average_calls_put_on_hold": {
+        "audio_name": {
+            "description": "Name of the audio file for the greeting",
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "average_hold_time": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_online_time": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "average_started_transfers": {
-            "type": [
-                "null",
-                "integer"
+                "string"
             ]
         },
-        "average_talk_time": {
+        "audio_url": {
+            "description": "URL to access the audio file for the greeting",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "average_wrap_up_time": {
+        "category_id": {
+            "description": "ID of the category to which the greeting belongs",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "current_timestamp": {
-            "type": "integer"
-        },
-        "total_accepted_transfers": {
+        "default": {
+            "description": "Indicates if the greeting is set as the default",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "total_calls_accepted": {
+        "default_lang": {
+            "description": "Default language for the greeting",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "total_calls_denied": {
+        "has_sub_settings": {
+            "description": "Indicates if the greeting has sub settings or not",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "total_calls_missed": {
+        "id": {
+            "description": "Unique identifier for the greeting",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "total_calls_put_on_hold": {
+        "ivr_ids": {
+            "description": "List of IVR IDs associated with the greeting",
+            "items": {
+                "description": "IVR ID",
+                "type": [
+                    "string",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
-        "total_hold_time": {
+        "name": {
+            "description": "Name of the greeting",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "total_started_transfers": {
+        "pending": {
+            "description": "Indicates if the greeting is pending for approval",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "total_talk_time": {
+        "phone_number_ids": {
+            "description": "List of phone number IDs linked to the greeting",
+            "items": {
+                "description": "Phone number ID",
+                "type": [
+                    "string",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
-        "total_wrap_up_time": {
+        "upload_id": {
+            "description": "ID of the uploaded audio file for the greeting",
             "type": [
                 "null",
                 "integer"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/schemas/ivr_routes.json` & `airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/schemas/ivr_menus.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8541666666666666%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the IVR menu.'}, 'ivr_id': "*

 * *                 "{'description': 'The ID of the IVR associated with this menu.'}, 'default': "*

 * *                 "OrderedDict([('description', 'The default action or response for this IVR "*

 * *                 "menu.'), ('type', ['null', 'boolean'])]), 'greeting_id': "*

 * *                 "OrderedDict([('description', 'The ID of the greeting message associated with "*

 * *                 "this IVR menu.'), ('type', ['null' […]*

```diff
@@ -1,60 +1,41 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "action": {
+        "default": {
+            "description": "The default action or response for this IVR menu.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "greeting": {
+        "greeting_id": {
+            "description": "The ID of the greeting message associated with this IVR menu.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
         "id": {
+            "description": "The unique identifier of the IVR menu.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ivr_id": {
+            "description": "The ID of the IVR associated with this menu.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "ivr_menu_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "keypress": {
+        "name": {
+            "description": "The name of the IVR menu.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "option_text": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "options": {
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "overflow_options": {
-            "type": [
-                "null",
-                "array"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/source.py` & `airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/spec.json` & `airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_talk-0.2.0/source_zendesk_talk/streams.py` & `airbyte_source_zendesk_talk-0.2.1/source_zendesk_talk/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_talk-0.2.0/PKG-INFO` & `airbyte_source_zendesk_talk-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-talk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Source implementation for Zendesk Talk.
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
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zendesk-talk
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Zendesk-Talk source connector
```

