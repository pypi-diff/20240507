# Comparing `tmp/movva_tools-1.1.0.tar.gz` & `tmp/movva_tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movva_tools-1.1.0.tar", max compression
+gzip compressed data, was "movva_tools-1.2.0.tar", max compression
```

## Comparing `movva_tools-1.1.0.tar` & `movva_tools-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-1.1.0/README.md
--rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-1.1.0/movva_tools/__init__.py
--rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-1.1.0/movva_tools/base_exception.py
--rw-r--r--   0        0        0     3303 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/constants.py
--rw-r--r--   0        0        0     2631 2023-09-28 15:15:46.604573 movva_tools-1.1.0/movva_tools/databases.py
--rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/decorators.py
--rw-r--r--   0        0        0     1996 2023-11-16 13:16:58.036191 movva_tools-1.1.0/movva_tools/examples/copy_flow_example.py
--rw-r--r--   0        0        0     1676 2023-11-16 13:18:08.634409 movva_tools-1.1.0/movva_tools/examples/import_contacts_example.py
--rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-1.1.0/movva_tools/exceptions.py
--rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-1.1.0/movva_tools/import_contacts.py
--rw-r--r--   0        0        0       97 2023-11-16 13:15:48.286193 movva_tools-1.1.0/movva_tools/integrations/__init__.py
--rw-r--r--   0        0        0    10101 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/integrations/google_integration.py
--rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-1.1.0/movva_tools/models/__init__.py
--rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/models/api_token_model.py
--rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/models/campaign_models.py
--rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/models/channel_models.py
--rw-r--r--   0        0        0     2284 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/models/contacts_models.py
--rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/models/flow_models.py
--rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-1.1.0/movva_tools/models/messages_models.py
--rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-1.1.0/movva_tools/models/organization_models.py
--rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-1.1.0/movva_tools/models/user_models.py
--rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/notifications/__init__.py
--rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/notifications/slack.py
--rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-1.1.0/movva_tools/parsers.py
--rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/serializers/__init__.py
--rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/serializers/base_serializer.py
--rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-1.1.0/movva_tools/serializers/campaign_event_serializer.py
--rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-1.1.0/movva_tools/serializers/campaign_serializer.py
--rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-1.1.0/movva_tools/serializers/contact_group_serializer.py
--rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-1.1.0/movva_tools/serializers/flow_revision_serializer.py
--rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-1.1.0/movva_tools/serializers/flow_serializer.py
--rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-1.1.0/movva_tools/serializers/organization_serializer.py
--rw-r--r--   0        0        0      658 2023-11-30 17:04:20.189985 movva_tools-1.1.0/movva_tools/services/__init__.py
--rw-r--r--   0        0        0     1171 2023-11-16 13:18:15.450249 movva_tools-1.1.0/movva_tools/services/api_token_service.py
--rw-r--r--   0        0        0      920 2023-09-28 16:12:52.612769 movva_tools-1.1.0/movva_tools/services/base_service.py
--rw-r--r--   0        0        0     4644 2023-11-16 13:18:26.202000 movva_tools-1.1.0/movva_tools/services/campaign_service.py
--rw-r--r--   0        0        0     1573 2023-11-16 13:15:42.558369 movva_tools-1.1.0/movva_tools/services/channel_service.py
--rw-r--r--   0        0        0     2004 2023-11-16 13:15:45.006294 movva_tools-1.1.0/movva_tools/services/contacts_service.py
--rw-r--r--   0        0        0    23957 2023-11-30 16:39:12.101496 movva_tools-1.1.0/movva_tools/services/flow_service.py
--rw-r--r--   0        0        0     1325 2023-11-30 17:59:19.280252 movva_tools-1.1.0/movva_tools/services/messages_service.py
--rw-r--r--   0        0        0      986 2023-11-16 13:16:59.992139 movva_tools-1.1.0/movva_tools/services/organization_service.py
--rw-r--r--   0        0        0      739 2023-11-16 13:18:13.646291 movva_tools-1.1.0/movva_tools/services/user_service.py
--rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-1.1.0/movva_tools/utils.py
--rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-1.1.0/movva_tools/validators.py
--rw-r--r--   0        0        0      919 2023-11-30 18:26:10.818340 movva_tools-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 movva_tools-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-09-28 10:29:10.291654 movva_tools-1.2.0/README.md
+-rw-r--r--   0        0        0      175 2023-11-30 17:04:01.622621 movva_tools-1.2.0/movva_tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-09-28 10:29:10.291654 movva_tools-1.2.0/movva_tools/base_exception.py
+-rw-r--r--   0        0        0     3303 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/constants.py
+-rw-r--r--   0        0        0     2631 2023-09-28 15:15:46.604573 movva_tools-1.2.0/movva_tools/databases.py
+-rw-r--r--   0        0        0      637 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/decorators.py
+-rw-r--r--   0        0        0     1996 2023-11-16 13:16:58.036191 movva_tools-1.2.0/movva_tools/examples/copy_flow_example.py
+-rw-r--r--   0        0        0     1676 2023-11-16 13:18:08.634409 movva_tools-1.2.0/movva_tools/examples/import_contacts_example.py
+-rw-r--r--   0        0        0     1641 2023-10-13 15:28:13.270038 movva_tools-1.2.0/movva_tools/exceptions.py
+-rw-r--r--   0        0        0     8910 2023-09-28 15:44:14.538563 movva_tools-1.2.0/movva_tools/import_contacts.py
+-rw-r--r--   0        0        0       97 2023-11-16 13:15:48.286193 movva_tools-1.2.0/movva_tools/integrations/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-07 19:01:49.033794 movva_tools-1.2.0/movva_tools/integrations/google_drive.py
+-rw-r--r--   0        0        0    10101 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/integrations/google_integration.py
+-rw-r--r--   0        0        0      848 2023-11-30 16:38:20.085932 movva_tools-1.2.0/movva_tools/models/__init__.py
+-rw-r--r--   0        0        0      490 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/api_token_model.py
+-rw-r--r--   0        0        0     2507 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/campaign_models.py
+-rw-r--r--   0        0        0     2014 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/channel_models.py
+-rw-r--r--   0        0        0     3363 2024-05-06 12:45:47.658291 movva_tools-1.2.0/movva_tools/models/contacts_models.py
+-rw-r--r--   0        0        0     9630 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/models/flow_models.py
+-rw-r--r--   0        0        0     1348 2023-11-30 17:53:45.673645 movva_tools-1.2.0/movva_tools/models/messages_models.py
+-rw-r--r--   0        0        0     1369 2023-09-28 15:17:44.535564 movva_tools-1.2.0/movva_tools/models/organization_models.py
+-rw-r--r--   0        0        0      638 2023-09-28 15:17:43.643571 movva_tools-1.2.0/movva_tools/models/user_models.py
+-rw-r--r--   0        0        0       76 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/notifications/__init__.py
+-rw-r--r--   0        0        0     5710 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/notifications/slack.py
+-rw-r--r--   0        0        0     1362 2023-09-28 10:29:10.291654 movva_tools-1.2.0/movva_tools/parsers.py
+-rw-r--r--   0        0        0      479 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/serializers/__init__.py
+-rw-r--r--   0        0        0      205 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/serializers/base_serializer.py
+-rw-r--r--   0        0        0     1340 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/campaign_event_serializer.py
+-rw-r--r--   0        0        0      469 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/campaign_serializer.py
+-rw-r--r--   0        0        0      427 2023-11-16 13:02:39.312774 movva_tools-1.2.0/movva_tools/serializers/contact_group_serializer.py
+-rw-r--r--   0        0        0      432 2023-11-16 13:18:23.218068 movva_tools-1.2.0/movva_tools/serializers/flow_revision_serializer.py
+-rw-r--r--   0        0        0      453 2023-11-16 13:18:24.762033 movva_tools-1.2.0/movva_tools/serializers/flow_serializer.py
+-rw-r--r--   0        0        0      422 2023-11-16 13:02:39.308774 movva_tools-1.2.0/movva_tools/serializers/organization_serializer.py
+-rw-r--r--   0        0        0      658 2023-11-30 17:04:20.189985 movva_tools-1.2.0/movva_tools/services/__init__.py
+-rw-r--r--   0        0        0     1205 2024-05-06 12:19:06.870867 movva_tools-1.2.0/movva_tools/services/api_token_service.py
+-rw-r--r--   0        0        0      920 2023-09-28 16:12:52.612769 movva_tools-1.2.0/movva_tools/services/base_service.py
+-rw-r--r--   0        0        0     4644 2023-11-16 13:18:26.202000 movva_tools-1.2.0/movva_tools/services/campaign_service.py
+-rw-r--r--   0        0        0     1573 2023-11-16 13:15:42.558369 movva_tools-1.2.0/movva_tools/services/channel_service.py
+-rw-r--r--   0        0        0     4044 2024-05-06 14:18:16.752989 movva_tools-1.2.0/movva_tools/services/contacts_service.py
+-rw-r--r--   0        0        0    23957 2023-11-30 16:39:12.101496 movva_tools-1.2.0/movva_tools/services/flow_service.py
+-rw-r--r--   0        0        0     3007 2024-05-06 18:33:02.915329 movva_tools-1.2.0/movva_tools/services/messages_service.py
+-rw-r--r--   0        0        0      986 2023-11-16 13:16:59.992139 movva_tools-1.2.0/movva_tools/services/organization_service.py
+-rw-r--r--   0        0        0      739 2023-11-16 13:18:13.646291 movva_tools-1.2.0/movva_tools/services/user_service.py
+-rw-r--r--   0        0        0     1818 2023-11-16 12:54:55.447688 movva_tools-1.2.0/movva_tools/utils.py
+-rw-r--r--   0        0        0      982 2023-09-28 16:52:41.474439 movva_tools-1.2.0/movva_tools/validators.py
+-rw-r--r--   0        0        0      919 2024-05-07 19:15:06.058737 movva_tools-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 movva_tools-1.2.0/PKG-INFO
```

### Comparing `movva_tools-1.1.0/movva_tools/constants.py` & `movva_tools-1.2.0/movva_tools/constants.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/databases.py` & `movva_tools-1.2.0/movva_tools/databases.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/decorators.py` & `movva_tools-1.2.0/movva_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/examples/copy_flow_example.py` & `movva_tools-1.2.0/movva_tools/examples/copy_flow_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/examples/import_contacts_example.py` & `movva_tools-1.2.0/movva_tools/examples/import_contacts_example.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/exceptions.py` & `movva_tools-1.2.0/movva_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/import_contacts.py` & `movva_tools-1.2.0/movva_tools/import_contacts.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/integrations/google_integration.py` & `movva_tools-1.2.0/movva_tools/integrations/google_integration.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/__init__.py` & `movva_tools-1.2.0/movva_tools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/campaign_models.py` & `movva_tools-1.2.0/movva_tools/models/campaign_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/channel_models.py` & `movva_tools-1.2.0/movva_tools/models/channel_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/flow_models.py` & `movva_tools-1.2.0/movva_tools/models/flow_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/messages_models.py` & `movva_tools-1.2.0/movva_tools/models/messages_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/organization_models.py` & `movva_tools-1.2.0/movva_tools/models/organization_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/models/user_models.py` & `movva_tools-1.2.0/movva_tools/models/user_models.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/notifications/slack.py` & `movva_tools-1.2.0/movva_tools/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/parsers.py` & `movva_tools-1.2.0/movva_tools/parsers.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/serializers/campaign_event_serializer.py` & `movva_tools-1.2.0/movva_tools/serializers/campaign_event_serializer.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/__init__.py` & `movva_tools-1.2.0/movva_tools/services/__init__.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/api_token_service.py` & `movva_tools-1.2.0/movva_tools/services/api_token_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
 from movva_tools.models.api_token_model import RapidProApiToken
 
 from movva_tools.services.base_service import BaseService
 from temba_client.v2 import TembaClient
 
 from movva_tools.exceptions import (
     ObjectDoesNotExistException
 )
 
 
 class APITokenService(BaseService):
 
-    def __init__(self, db_connection=None) -> None:
+    def __init__(self, rapidpro_url, db_connection=None) -> None:
 
         super().__init__(db_connection)
 
         # model table entities
         self.APIToken = RapidProApiToken
+        self._rapidpro_url = rapidpro_url
 
     def get_token_by_org_id(self, org_id):
 
         api_token = self.db_connection.session.query(
             self.APIToken
         ).filter_by(
             is_active=True,
@@ -33,14 +33,14 @@
             raise ObjectDoesNotExistException(
                 dababase_object=self.APIToken
             )
 
     def rapidpro_api_client(self, token):
         try:
             return TembaClient(
-                host=os.environ.get('RAPIDPRO_URL'),
+                host=self._rapidpro_url,
                 token=token
             )
         except Exception:
             raise Exception(
                 'Não foi possível estabelecer conexão com o RapidPro.'
             )
```

### Comparing `movva_tools-1.1.0/movva_tools/services/base_service.py` & `movva_tools-1.2.0/movva_tools/services/base_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/campaign_service.py` & `movva_tools-1.2.0/movva_tools/services/campaign_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/channel_service.py` & `movva_tools-1.2.0/movva_tools/services/channel_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/flow_service.py` & `movva_tools-1.2.0/movva_tools/services/flow_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/organization_service.py` & `movva_tools-1.2.0/movva_tools/services/organization_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/services/user_service.py` & `movva_tools-1.2.0/movva_tools/services/user_service.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/utils.py` & `movva_tools-1.2.0/movva_tools/utils.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/movva_tools/validators.py` & `movva_tools-1.2.0/movva_tools/validators.py`

 * *Files identical despite different names*

### Comparing `movva_tools-1.1.0/pyproject.toml` & `movva_tools-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "movva_tools"
-version = "1.1.0"
+version = "1.2.0"
 description = "Package that contains integrations and tools to use in issues of Movva organization."
 authors = ["WillamesCampos <willwjccampos@gmail.com>"]
 readme = "README.md"
 packages = [{include = "movva_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `movva_tools-1.1.0/PKG-INFO` & `movva_tools-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movva_tools
-Version: 1.1.0
+Version: 1.2.0
 Summary: Package that contains integrations and tools to use in issues of Movva organization.
 Author: WillamesCampos
 Author-email: willwjccampos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

