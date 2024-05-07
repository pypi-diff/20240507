# Comparing `tmp/airbyte_source_zendesk_support-2.6.2.tar.gz` & `tmp/airbyte_source_zendesk_support-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_support-2.6.2.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_support-2.6.3.tar", max compression
```

## Comparing `airbyte_source_zendesk_support-2.6.2.tar` & `airbyte_source_zendesk_support-2.6.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     4663 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/README.md
--rw-r--r--   0        0        0      832 2024-05-02 13:37:53.044599 airbyte_source_zendesk_support-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/__init__.py
--rw-r--r--   0        0        0     3294 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/components.py
--rw-r--r--   0        0        0    19960 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/manifest.yaml
--rw-r--r--   0        0        0      255 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/run.py
--rw-r--r--   0        0        0      392 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/account_attributes.json
--rw-r--r--   0        0        0     1064 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/article_comments.json
--rw-r--r--   0        0        0     1714 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/articles.json
--rw-r--r--   0        0        0     1625 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/attribute_definitions.json
--rw-r--r--   0        0        0      877 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/audit_logs.json
--rw-r--r--   0        0        0     1068 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/brands.json
--rw-r--r--   0        0        0     5246 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/custom_roles.json
--rw-r--r--   0        0        0      682 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/deleted_tickets.json
--rw-r--r--   0        0        0      514 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/group_memberships.json
--rw-r--r--   0        0        0      630 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/groups.json
--rw-r--r--   0        0        0     1423 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/macros.json
--rw-r--r--   0        0        0     1284 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/organization_fields.json
--rw-r--r--   0        0        0      651 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/organization_memberships.json
--rw-r--r--   0        0        0     1210 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/organizations.json
--rw-r--r--   0        0        0     1004 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/post_comments.json
--rw-r--r--   0        0        0     1595 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/posts.json
--rw-r--r--   0        0        0      801 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0      708 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/schedules.json
--rw-r--r--   0        0        0     1958 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/attachments.json
--rw-r--r--   0        0        0     1835 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/metadata.json
--rw-r--r--   0        0        0     4521 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/tickets.json
--rw-r--r--   0        0        0     1617 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/via.json
--rw-r--r--   0        0        0     2707 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/via_channel.json
--rw-r--r--   0        0        0     1929 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/sla_policies.json
--rw-r--r--   0        0        0      165 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/tags.json
--rw-r--r--   0        0        0     2114 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_activities.json
--rw-r--r--   0        0        0    17835 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_audits.json
--rw-r--r--   0        0        0     1151 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_comments.json
--rw-r--r--   0        0        0     2335 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_fields.json
--rw-r--r--   0        0        0     1359 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_forms.json
--rw-r--r--   0        0        0      394 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_metric_events.json
--rw-r--r--   0        0        0     3616 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_metrics.json
--rw-r--r--   0        0        0      512 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_skips.json
--rw-r--r--   0        0        0       27 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/tickets.json
--rw-r--r--   0        0        0      902 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/topics.json
--rw-r--r--   0        0        0     1054 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/user_fields.json
--rw-r--r--   0        0        0     4496 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/users.json
--rw-r--r--   0        0        0      647 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/votes.json
--rw-r--r--   0        0        0     7876 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/source.py
--rw-r--r--   0        0        0     5975 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/spec.json
--rw-r--r--   0        0        0    39231 2024-05-02 13:04:26.000000 airbyte_source_zendesk_support-2.6.2/source_zendesk_support/streams.py
--rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4663 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/README.md
+-rw-r--r--   0        0        0      836 2024-05-07 13:34:03.014973 airbyte_source_zendesk_support-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/__init__.py
+-rw-r--r--   0        0        0     3294 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/components.py
+-rw-r--r--   0        0        0    19960 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/manifest.yaml
+-rw-r--r--   0        0        0      255 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/run.py
+-rw-r--r--   0        0        0      798 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/account_attributes.json
+-rw-r--r--   0        0        0     2103 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/article_comments.json
+-rw-r--r--   0        0        0     3577 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/articles.json
+-rw-r--r--   0        0        0     3046 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/attribute_definitions.json
+-rw-r--r--   0        0        0     1741 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/audit_logs.json
+-rw-r--r--   0        0        0     2061 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/brands.json
+-rw-r--r--   0        0        0     9569 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/custom_roles.json
+-rw-r--r--   0        0        0     1211 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/deleted_tickets.json
+-rw-r--r--   0        0        0     1098 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/group_memberships.json
+-rw-r--r--   0        0        0     1211 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/groups.json
+-rw-r--r--   0        0        0     2642 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/macros.json
+-rw-r--r--   0        0        0     2659 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/organization_fields.json
+-rw-r--r--   0        0        0     1453 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/organization_memberships.json
+-rw-r--r--   0        0        0     2262 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/organizations.json
+-rw-r--r--   0        0        0     1978 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/post_comments.json
+-rw-r--r--   0        0        0     3315 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/posts.json
+-rw-r--r--   0        0        0     1843 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0     1239 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/schedules.json
+-rw-r--r--   0        0        0     1958 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/attachments.json
+-rw-r--r--   0        0        0     1835 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/metadata.json
+-rw-r--r--   0        0        0     4521 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/tickets.json
+-rw-r--r--   0        0        0     1617 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/via.json
+-rw-r--r--   0        0        0     2707 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/via_channel.json
+-rw-r--r--   0        0        0     3655 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/sla_policies.json
+-rw-r--r--   0        0        0      320 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/tags.json
+-rw-r--r--   0        0        0     2114 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_activities.json
+-rw-r--r--   0        0        0    29608 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_audits.json
+-rw-r--r--   0        0        0     2495 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_comments.json
+-rw-r--r--   0        0        0     4685 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     2644 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_forms.json
+-rw-r--r--   0        0        0      855 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_metric_events.json
+-rw-r--r--   0        0        0     7095 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_metrics.json
+-rw-r--r--   0        0        0     1013 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_skips.json
+-rw-r--r--   0        0        0       27 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/tickets.json
+-rw-r--r--   0        0        0     1735 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/topics.json
+-rw-r--r--   0        0        0     2182 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/user_fields.json
+-rw-r--r--   0        0        0     8484 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/users.json
+-rw-r--r--   0        0        0     1170 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/votes.json
+-rw-r--r--   0        0        0     7876 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/source.py
+-rw-r--r--   0        0        0     5975 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/spec.json
+-rw-r--r--   0        0        0    39231 2024-05-07 10:08:07.000000 airbyte_source_zendesk_support-2.6.3/source_zendesk_support/streams.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.3/PKG-INFO
```

### Comparing `airbyte_source_zendesk_support-2.6.2/README.md` & `airbyte_source_zendesk_support-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/pyproject.toml` & `airbyte_source_zendesk_support-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.6.2"
+version = "2.6.3"
 name = "airbyte-source-zendesk-support"
 description = "Source implementation for Zendesk Support."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_zendesk_support" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.81.4"
 pytz = "==2024.1"
 
 [tool.poetry.scripts]
 source-zendesk-support = "source_zendesk_support.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1"
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/__init__.py` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/components.py` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/manifest.yaml` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/article_comments.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/group_memberships.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3982843137254902%*

 * *Differences: {"'properties'": "{'created_at': {'description': 'Timestamp indicating when the group membership "*

 * *                 "was created.'}, 'id': {'description': 'The unique identifier of the group "*

 * *                 "membership.'}, 'updated_at': {'description': 'Timestamp indicating when the "*

 * *                 "group membership was last updated.'}, 'url': {'description': 'URL pointing to "*

 * *                 "the group membership resource.'}, 'default': OrderedDict([('description', 'Flag "*

 * *                 "indicat […]*

```diff
@@ -1,97 +1,59 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "author_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "body": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "created_at": {
+            "description": "Timestamp indicating when the group membership was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "html_url": {
+        "default": {
+            "description": "Flag indicating if this group membership is the default one.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "id": {
+        "group_id": {
+            "description": "The unique identifier of the group this membership belongs to.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "locale": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "non_author_editor_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "non_author_updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "source_id": {
+        "id": {
+            "description": "The unique identifier of the group membership.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "source_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "updated_at": {
+            "description": "Timestamp indicating when the group membership was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "url": {
+            "description": "URL pointing to the group membership resource.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "vote_count": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "vote_sum": {
+        "user_id": {
+            "description": "The unique identifier of the user associated with this group membership.",
             "type": [
                 "null",
                 "integer"
             ]
         }
     },
-    "title": "Post Comments",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/articles.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/attachments.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.13333333333333333%*

 * *Differences: {"'items'": "OrderedDict([('properties', OrderedDict([('id', OrderedDict([('type', ['null', "*

 * *            "'integer'])])), ('size', OrderedDict([('type', ['null', 'integer'])])), ('url', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('malware_scan_result', "*

 * *            "OrderedDict([('type', ['null', 'string'])])), ('inline', OrderedDict([('type', "*

 * *            "['null', 'boolean'])])), ('deleted', OrderedDict([('type', ['null', 'boolean'])])), "*

 * *            "('malware_access_override', Orde […]*

```diff
@@ -1,163 +1,166 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
-    "properties": {
-        "author_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "body": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "comments_disabled": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "content_tag_ids": {
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "created_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "draft": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "edited_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "html_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "label_names": {
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "locale": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "outdated": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "outdated_locales": {
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "permission_group_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "position": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "promoted": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "section_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "source_locale": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "user_segment_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "vote_count": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "vote_sum": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        }
+    "items": {
+        "properties": {
+            "content_type": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "content_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "deleted": {
+                "type": [
+                    "null",
+                    "boolean"
+                ]
+            },
+            "file_name": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "height": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "id": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "inline": {
+                "type": [
+                    "null",
+                    "boolean"
+                ]
+            },
+            "malware_access_override": {
+                "type": [
+                    "null",
+                    "boolean"
+                ]
+            },
+            "malware_scan_result": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "mapped_content_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "size": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "thumbnails": {
+                "items": {
+                    "properties": {
+                        "content_type": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "content_url": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "file_name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "height": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "id": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "inline": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "mapped_content_url": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "size": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "url": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "width": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
+            "url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "width": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            }
+        },
+        "type": [
+            "null",
+            "object"
+        ]
     },
-    "title": "Articles",
     "type": [
         "null",
-        "object"
+        "array"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/attribute_definitions.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/metadata.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('custom', OrderedDict([('type', ['null', 'object']), "*

 * *                 "('properties', OrderedDict()), ('additionalProperties', True)])), ('trusted', "*

 * *                 "OrderedDict([('type', ['null', 'boolean'])])), ('notifications_suppressed_for', "*

 * *                 "OrderedDict([('type', ['null', 'array']), ('items', OrderedDict([('type', "*

 * *                 "['null', 'integer'])]))])), ('flags_options', OrderedDict([('type', ['null', "*

 * *                 "'object' […]*

```diff
@@ -1,143 +1,152 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "condition": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "confition": {
+        "custom": {
+            "additionalProperties": true,
+            "properties": {},
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "group": {
+        "flags": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "metadata": {
-            "additionalProperties": true,
+        "flags_options": {
             "properties": {
-                "collection_key": {
+                "11": {
+                    "properties": {
+                        "message": {
+                            "properties": {
+                                "user": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "trusted": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "object"
                     ]
                 },
-                "item_key": {
+                "2": {
+                    "properties": {
+                        "trusted": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "object"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
-        "nullable": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "operators": {
+        "notifications_suppressed_for": {
             "items": {
-                "properties": {
-                    "terminal": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "title": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "value": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
                 "type": [
                     "null",
-                    "object"
+                    "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "repeatable": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "subject": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
+        "system": {
+            "properties": {
+                "client": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "ip_address": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "json_email_identifier": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "latitude": {
+                    "type": [
+                        "null",
+                        "number"
+                    ]
+                },
+                "location": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "longitude": {
+                    "type": [
+                        "null",
+                        "number"
+                    ]
+                },
+                "message_id": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "raw_email_identifier": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "values": {
-            "items": {
-                "properties": {
-                    "enabled": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "title": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "value": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "trusted": {
             "type": [
                 "null",
-                "array"
+                "boolean"
             ]
         }
     },
-    "title": "Attribute Definitions",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/group_memberships.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/account_attributes.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8463541666666666%*

 * *Differences: {"'properties'": "{'url': {'description': 'The URL that can be used to access the account "*

 * *                 "attribute.'}, 'updated_at': {'description': 'The timestamp indicating when the "*

 * *                 "account attribute was last updated.'}, 'created_at': {'description': 'The "*

 * *                 "timestamp indicating when the account attribute was created.'}, 'id': {'type': "*

 * *                 "{insert: [(1, 'string')], delete: [1]}, 'description': 'The unique identifier "*

 * *                 "for the acco […]*

```diff
@@ -1,52 +1,45 @@
 {
     "properties": {
         "created_at": {
+            "description": "The timestamp indicating when the account attribute was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "group_id": {
+        "id": {
+            "description": "The unique identifier for the account attribute.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "id": {
+        "name": {
+            "description": "The name or label of the account attribute.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "updated_at": {
+            "description": "The timestamp indicating when the account attribute was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "url": {
+            "description": "The URL that can be used to access the account attribute.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "user_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/groups.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/votes.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.40544871794871795%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'created_at': {'description': 'Timestamp when the vote was created'}, 'url': "*

 * *                 "{'description': 'URL of the resource related to the vote'}, 'updated_at': "*

 * *                 "{'description': 'Timestamp when the vote was last updated'}, 'id': "*

 * *                 "{'description': 'Unique identifier for the vote'}, 'item_id': "*

 * *                 "OrderedDict([('description', 'Identifier of the item that was voted on'), […]*

```diff
@@ -1,64 +1,68 @@
 {
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "created_at": {
+            "description": "Timestamp when the vote was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default": {
+        "id": {
+            "description": "Unique identifier for the vote",
             "type": [
                 "null",
-                "boolean"
+                "integer"
             ]
         },
-        "deleted": {
+        "item_id": {
+            "description": "Identifier of the item that was voted on",
             "type": [
                 "null",
-                "boolean"
+                "integer"
             ]
         },
-        "description": {
+        "item_type": {
+            "description": "Type of the item that was voted on (e.g., ticket, article)",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "is_public": {
+        "updated_at": {
+            "description": "Timestamp when the vote was last updated",
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "name": {
+        "url": {
+            "description": "URL of the resource related to the vote",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "user_id": {
+            "description": "Unique identifier of the user who voted",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "url": {
+        "value": {
+            "description": "Value of the vote (e.g., upvote, downvote)",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
+    "title": "Votes",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/macros.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/via.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('channel', OrderedDict([('type', ['null', 'string'])])), "*

 * *                 "('source', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('from', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('ticket_ids', OrderedDict([('type', ['null', 'array']), ('items', "*

 * *                 "OrderedDict([('type', ['null', 'integer'])]))])), ('subject', "*

 * *                 "OrderedDict([('type',  […]*

```diff
@@ -1,130 +1,128 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "actions": {
-            "items": {
-                "properties": {
-                    "field": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "value": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "created_at": {
-            "format": "date-time",
+        "channel": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "description": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "position": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "raw_title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "restriction": {
+        "source": {
             "properties": {
-                "id": {
+                "from": {
+                    "properties": {
+                        "address": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "channel": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "deleted": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "id": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "original_recipients": {
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "type": [
+                                "null",
+                                "array"
+                            ]
+                        },
+                        "subject": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "ticket_id": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "ticket_ids": {
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "type": [
+                                "null",
+                                "array"
+                            ]
+                        },
+                        "title": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "integer"
+                        "object"
                     ]
                 },
-                "ids": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
+                "rel": {
                     "type": [
                         "null",
-                        "array"
+                        "string"
                     ]
                 },
-                "type": {
+                "to": {
+                    "properties": {
+                        "address": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "object"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
-        },
-        "title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "url": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
-    "title": "Macros",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/organization_fields.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/groups.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.39725378787878785%*

 * *Differences: {"'properties'": "{'created_at': {'description': 'The date and time when the group was created.'}, "*

 * *                 "'description': {'description': 'The description or details about the group.'}, "*

 * *                 "'id': {'description': 'The unique identifier of the group.'}, 'updated_at': "*

 * *                 "{'description': 'The date and time when the group was last updated.'}, 'url': "*

 * *                 "{'description': 'The URL of the group.'}, 'name': OrderedDict([('description', "*

 * *                 "' […]*

```diff
@@ -1,120 +1,73 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "created_at": {
+            "description": "The date and time when the group was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "custom_field_options": {
+        "default": {
+            "description": "Indicates if the group is set as the default group.",
             "type": [
                 "null",
-                "array"
-            ]
-        },
-        "description": {
-            "type": [
-                "null",
-                "string"
+                "boolean"
             ]
         },
-        "id": {
+        "deleted": {
+            "description": "Indicates if the group has been deleted.",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "key": {
+        "description": {
+            "description": "The description or details about the group.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "position": {
+        "id": {
+            "description": "The unique identifier of the group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "raw_description": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "raw_title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "regexp_for_validation": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "relationship_filter": {
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "relationship_target_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "system": {
+        "is_public": {
+            "description": "Indicates whether the group is public or private.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "tag": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
+        "name": {
+            "description": "The name of the group.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the group was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "url": {
+            "description": "The URL of the group.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "title": "Ticket Activities",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/organizations.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/schedules.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7965686274509804%*

 * *Differences: {"'properties'": "{'created_at': {'description': 'The date and time when the schedule was "*

 * *                 "created'}, 'updated_at': {'description': 'The date and time when the schedule "*

 * *                 "was last updated'}, 'name': {'description': 'The name of the schedule'}, 'id': "*

 * *                 "{'description': 'The unique identifier for the schedule'}, 'intervals': "*

 * *                 "OrderedDict([('description', 'List of time intervals within the schedule'), "*

 * *                 "('type', ['null', […]*

```diff
@@ -1,115 +1,74 @@
 {
     "properties": {
         "created_at": {
+            "description": "The date and time when the schedule was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deleted_at": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "details": {
+        "id": {
+            "description": "The unique identifier for the schedule",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "domain_names": {
+        "intervals": {
+            "description": "List of time intervals within the schedule",
             "items": {
+                "properties": {
+                    "end_time": {
+                        "description": "The end time of a specific interval",
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "start_time": {
+                        "description": "The start time of a specific interval",
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    }
+                },
                 "type": [
                     "null",
-                    "string"
+                    "object"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "external_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "group_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "name": {
+            "description": "The name of the schedule",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "notes": {
+        "time_zone": {
+            "description": "The time zone in which the schedule operates",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "organization_fields": {
-            "additionalProperties": true,
-            "properties": {},
-            "type": [
-                "null",
-                "object"
-            ]
-        },
-        "shared_comments": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "shared_tickets": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "tags": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "updated_at": {
+            "description": "The date and time when the schedule was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "url": {
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

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/posts.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/satisfaction_ratings.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.26284722222222223%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}, 'description': 'The "*

 * *                 "unique identifier of the satisfaction rating entry.'}, 'created_at': "*

 * *                 "{'description': 'The date and time when the satisfaction rating was created.'}, "*

 * *                 "'url': {'description': 'The URL to access the details of the satisfaction "*

 * *                 "rating.'}, 'updated_at': {'description': 'The date and time when the "*

 * *                 "satisfaction rating was l […]*

```diff
@@ -1,151 +1,91 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "author_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "closed": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "comment_count": {
+        "assignee_id": {
+            "description": "The unique identifier of the user assigned to the ticket.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "content_tag_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "number"
-                ]
-            },
+        "comment": {
+            "description": "The feedback comment provided by the requester.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
         "created_at": {
+            "description": "The date and time when the satisfaction rating was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "description": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "details": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "featured": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "follower_count": {
+        "group_id": {
+            "description": "The unique identifier of the group associated with the ticket.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "frozen": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "html_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "non_author_editor_id": {
+            "description": "The unique identifier of the satisfaction rating entry.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "non_author_updated_at": {
-            "format": "date-time",
+        "reason": {
+            "description": "The reason selected by the requester for the satisfaction rating.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "pinned": {
+        "reason_id": {
+            "description": "The unique identifier of the selected satisfaction rating reason.",
             "type": [
                 "null",
-                "boolean"
+                "integer"
             ]
         },
-        "status": {
+        "requester_id": {
+            "description": "The unique identifier of the requester who provided the rating.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "title": {
+        "score": {
+            "description": "The satisfaction score given by the requester (usually a numeric value).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "topic_id": {
+        "ticket_id": {
+            "description": "The unique identifier of the ticket associated with the satisfaction rating.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the satisfaction rating was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "url": {
+            "description": "The URL to access the details of the satisfaction rating.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "vote_count": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "vote_sum": {
-            "type": [
-                "null",
-                "integer"
-            ]
         }
     },
-    "title": "Posts",
-    "type": [
-        "null",
-        "object"
-    ]
+    "type": "object"
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/attachments.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/via_channel.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2222222222222222%*

 * *Differences: {"'properties'": "OrderedDict([('channel', OrderedDict([('type', ['null', 'string'])])), "*

 * *                 "('source', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('from', OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                 "OrderedDict([('name', OrderedDict([('type', ['null', 'string'])])), ('address', "*

 * *                 "OrderedDict([('type', ['null', 'string'])])), ('original_recipients', "*

 * *                 "OrderedDict([('type', [' […]*

```diff
@@ -1,166 +1,206 @@
 {
-    "items": {
-        "properties": {
-            "content_type": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "content_url": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "deleted": {
-                "type": [
-                    "null",
-                    "boolean"
-                ]
-            },
-            "file_name": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "height": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "id": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "inline": {
-                "type": [
-                    "null",
-                    "boolean"
-                ]
-            },
-            "malware_access_override": {
-                "type": [
-                    "null",
-                    "boolean"
-                ]
-            },
-            "malware_scan_result": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "mapped_content_url": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "size": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "thumbnails": {
-                "items": {
+    "properties": {
+        "channel": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "source": {
+            "properties": {
+                "from": {
                     "properties": {
-                        "content_type": {
+                        "address": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "content_url": {
+                        "channel": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "file_name": {
+                        "deleted": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "facebook_id": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "height": {
+                        "formatted_phone": {
                             "type": [
                                 "null",
-                                "integer"
+                                "string"
                             ]
                         },
                         "id": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
                         },
-                        "inline": {
+                        "name": {
                             "type": [
                                 "null",
-                                "boolean"
+                                "string"
+                            ]
+                        },
+                        "original_recipients": {
+                            "items": {
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "type": [
+                                "null",
+                                "array"
+                            ]
+                        },
+                        "phone": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "profile_url": {
+                            "type": [
+                                "null",
+                                "string"
                             ]
                         },
-                        "mapped_content_url": {
+                        "revision_id": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "subject": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "size": {
+                        "ticket_id": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
                         },
-                        "url": {
+                        "title": {
                             "type": [
                                 "null",
                                 "string"
                             ]
                         },
-                        "width": {
+                        "topic_id": {
                             "type": [
                                 "null",
                                 "integer"
                             ]
+                        },
+                        "topic_name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "username": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
                         }
                     },
                     "type": [
                         "null",
                         "object"
                     ]
                 },
-                "type": [
-                    "null",
-                    "array"
-                ]
-            },
-            "url": {
-                "type": [
-                    "null",
-                    "string"
-                ]
+                "rel": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "to": {
+                    "properties": {
+                        "address": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "brand_id": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "email_ccs": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "facebook_id": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "formatted_phone": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "name": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "phone": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "profile_url": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "username": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
             },
-            "width": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            }
-        },
-        "type": [
-            "null",
-            "object"
-        ]
+            "type": [
+                "null",
+                "object"
+            ]
+        }
     },
     "type": [
         "null",
-        "array"
+        "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/tickets.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/shared/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/shared/via_channel.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/posts.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{replace: OrderedDict([('author_id', OrderedDict([('description', 'The unique "*

 * *                 "identifier of the author of the post.'), ('type', ['null', 'number'])])), "*

 * *                 "('closed', OrderedDict([('description', 'Indicates whether the post is closed or "*

 * *                 "open for further comments.'), ('type', ['null', 'boolean'])])), "*

 * *                 "('comment_count', OrderedDict([('description', 'The total […]*

```diff
@@ -1,206 +1,173 @@
 {
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "channel": {
+        "author_id": {
+            "description": "The unique identifier of the author of the post.",
             "type": [
                 "null",
-                "string"
+                "number"
+            ]
+        },
+        "closed": {
+            "description": "Indicates whether the post is closed or open for further comments.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "comment_count": {
+            "description": "The total number of comments on the post.",
+            "type": [
+                "null",
+                "integer"
             ]
         },
-        "source": {
-            "properties": {
-                "from": {
-                    "properties": {
-                        "address": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "channel": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "deleted": {
-                            "type": [
-                                "null",
-                                "boolean"
-                            ]
-                        },
-                        "facebook_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "formatted_phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "id": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "original_recipients": {
-                            "items": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "type": [
-                                "null",
-                                "array"
-                            ]
-                        },
-                        "phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "profile_url": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "revision_id": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "subject": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "ticket_id": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "title": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "topic_id": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "topic_name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "username": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "rel": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "to": {
-                    "properties": {
-                        "address": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "brand_id": {
-                            "type": [
-                                "null",
-                                "integer"
-                            ]
-                        },
-                        "email_ccs": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "facebook_id": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "formatted_phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "name": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "phone": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "profile_url": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        },
-                        "username": {
-                            "type": [
-                                "null",
-                                "string"
-                            ]
-                        }
-                    },
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                }
+        "content_tag_ids": {
+            "description": "Array containing unique identifiers of tags associated with the post.",
+            "items": {
+                "type": [
+                    "null",
+                    "number"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
+            ]
+        },
+        "created_at": {
+            "description": "The date and time when the post was created.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "description": {
+            "description": "A brief summary or overview of the post content.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "details": {
+            "description": "Additional details or content of the post.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "featured": {
+            "description": "Indicates whether the post is featured or not.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "follower_count": {
+            "description": "The number of users following the post for updates.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "frozen": {
+            "description": "Indicates whether the post content is frozen or editable.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "html_url": {
+            "description": "The URL that directs to the HTML version of the post.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "id": {
+            "description": "The unique identifier of the post.",
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "non_author_editor_id": {
+            "description": "The unique identifier of a user who is not the author but edited the post.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "non_author_updated_at": {
+            "description": "The date and time when a non-author user last updated the post.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "pinned": {
+            "description": "Indicates if the post is pinned to stay on top of the list.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "status": {
+            "description": "The current status of the post, such as 'open', 'solved', 'archived', etc.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "title": {
+            "description": "The title or headline of the post.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "topic_id": {
+            "description": "The identifier of the topic under which the post belongs.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "updated_at": {
+            "description": "The date and time of the last update made to the post.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "url": {
+            "description": "The URL that points to the post details.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "vote_count": {
+            "description": "The total count of votes the post has received.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "vote_sum": {
+            "description": "The sum of all votes received considering both upvotes and downvotes.",
+            "type": [
+                "null",
+                "integer"
             ]
         }
     },
+    "title": "Posts",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_activities.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_forms.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/topics.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7744565217391304%*

 * *Differences: {"'properties'": "{'created_at': {'description': 'The date and time when this topic was "*

 * *                 "created.'}, 'name': {'description': 'The name/title of the topic.'}, 'position': "*

 * *                 "{'type': {insert: [(1, 'number')], delete: [1]}, 'description': 'The order "*

 * *                 "position of this topic relative to others.'}, 'updated_at': {'description': 'The "*

 * *                 "date and time when this topic was last updated.'}, 'url': {'description': 'The "*

 * *                 "URL of t […]*

```diff
@@ -1,126 +1,96 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "active": {
+        "community_id": {
+            "description": "The unique identifier of the community to which this topic belongs.",
             "type": [
                 "null",
-                "boolean"
-            ]
-        },
-        "agent_conditions": {
-            "type": [
-                "null",
-                "array"
+                "integer"
             ]
         },
         "created_at": {
+            "description": "The date and time when this topic was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "default": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "display_name": {
+        "description": {
+            "description": "The textual description of the topic.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "end_user_conditions": {
+        "follower_count": {
+            "description": "The count of users following this topic.",
             "type": [
                 "null",
-                "array"
+                "number"
             ]
         },
-        "end_user_visible": {
+        "html_url": {
+            "description": "The URL of the topic in HTML format.",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "id": {
+            "description": "The unique identifier of the topic.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "in_all_brands": {
+        "manageable_by": {
+            "description": "The user or group who can manage this topic.",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "name": {
+            "description": "The name/title of the topic.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "position": {
+            "description": "The order position of this topic relative to others.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "raw_display_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "raw_name": {
+        "updated_at": {
+            "description": "The date and time when this topic was last updated.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "restricted_brand_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "ticket_field_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "updated_at": {
-            "format": "date-time",
+        "url": {
+            "description": "The URL of the topic in API format.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "url": {
+        "user_segment_id": {
+            "description": "The identifier of the user segment associated with this topic.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         }
     },
-    "title": "Ticket Forms",
+    "title": "Topics",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/ticket_skips.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_metric_events.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7840909090909091%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the ticket metric event'}, "*

 * *                 "'ticket_id': {'description': 'Unique identifier for the ticket associated with "*

 * *                 "the metric event'}, 'metric': OrderedDict([('description', 'Type of metric being "*

 * *                 "tracked for the ticket'), ('type', ['null', 'string'])]), 'time': "*

 * *                 "OrderedDict([('description', 'Timestamp when the metric event occurred'), "*

 * *                 "('type', ['null', 'st […]*

```diff
@@ -1,48 +1,49 @@
 {
     "properties": {
-        "created_at": {
-            "format": "date-time",
+        "id": {
+            "description": "Unique identifier for the ticket metric event",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "id": {
+        "instance_id": {
+            "description": "Unique identifier for the specific instance of the metric event",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "reason": {
+        "metric": {
+            "description": "Type of metric being tracked for the ticket",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ticket": {
-            "$ref": "tickets.json"
-        },
         "ticket_id": {
+            "description": "Unique identifier for the ticket associated with the metric event",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "updated_at": {
-            "format": "date-time",
+        "time": {
+            "description": "Timestamp when the metric event occurred",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "user_id": {
+        "type": {
+            "description": "Type of metric event (e.g., update, change, escalation)",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/schemas/topics.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/schemas/ticket_skips.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.39322916666666663%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}, 'description': 'Unique "*

 * *                 "identifier for the ticket skip entry'}, 'created_at': {'description': 'The "*

 * *                 "timestamp when the ticket skip entry was created'}, 'updated_at': "*

 * *                 "{'description': 'The timestamp when the ticket skip entry was last updated'}, "*

 * *                 "'reason': OrderedDict([('description', 'The reason for skipping the ticket'), "*

 * *                 "('type', ['null', […]*

```diff
@@ -1,84 +1,56 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "community_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "created_at": {
+            "description": "The timestamp when the ticket skip entry was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "description": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "follower_count": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "html_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "id": {
+            "description": "Unique identifier for the ticket skip entry",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "manageable_by": {
+        "reason": {
+            "description": "The reason for skipping the ticket",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
+        "ticket": {
+            "$ref": "tickets.json",
+            "description": "Information related to the skipped ticket"
         },
-        "position": {
+        "ticket_id": {
+            "description": "The unique identifier of the skipped ticket",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "updated_at": {
+            "description": "The timestamp when the ticket skip entry was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "url": {
+        "user_id": {
+            "description": "The unique identifier of the user who skipped the ticket",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "user_segment_id": {
-            "type": [
-                "null",
-                "number"
+                "integer"
             ]
         }
     },
-    "title": "Topics",
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/source.py` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/spec.json` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/source_zendesk_support/streams.py` & `airbyte_source_zendesk_support-2.6.3/source_zendesk_support/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.2/PKG-INFO` & `airbyte_source_zendesk_support-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-support
-Version: 2.6.2
+Version: 2.6.3
 Summary: Source implementation for Zendesk Support.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.81.4)
 Requires-Dist: pytz (==2024.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zendesk-support
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Zendesk-Support source connector
```

