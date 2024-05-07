# Comparing `tmp/airbyte_source_google_ads-3.4.1.tar.gz` & `tmp/airbyte_source_google_ads-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_ads-3.4.1.tar", max compression
+gzip compressed data, was "airbyte_source_google_ads-3.4.2.tar", max compression
```

## Comparing `airbyte_source_google_ads-3.4.1.tar` & `airbyte_source_google_ads-3.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     4573 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/README.md
--rw-r--r--   0        0        0      833 2024-04-08 13:34:35.362123 airbyte_source_google_ads-3.4.1/pyproject.toml
--rw-r--r--   0        0        0     1201 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/__init__.py
--rw-r--r--   0        0        0     4834 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/config_migrations.py
--rw-r--r--   0        0        0     4251 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/custom_query_stream.py
--rw-r--r--   0        0        0     9407 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/google_ads.py
--rw-r--r--   0        0        0     1078 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/models.py
--rw-r--r--   0        0        0      360 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/run.py
--rw-r--r--   0        0        0     4497 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/account_performance_report.json
--rw-r--r--   0        0        0     2589 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group.json
--rw-r--r--   0        0        0    14530 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_ad.json
--rw-r--r--   0        0        0      578 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_ad_label.json
--rw-r--r--   0        0        0    12841 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_ad_legacy.json
--rw-r--r--   0        0        0     2914 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_bidding_strategy.json
--rw-r--r--   0        0        0     6679 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_criterion.json
--rw-r--r--   0        0        0      565 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_criterion_label.json
--rw-r--r--   0        0        0      501 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_label.json
--rw-r--r--   0        0        0     2927 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_listing_group_criterion.json
--rw-r--r--   0        0        0      692 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/audience.json
--rw-r--r--   0        0        0     8785 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign.json
--rw-r--r--   0        0        0     2976 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign_bidding_strategy.json
--rw-r--r--   0        0        0     4268 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign_budget.json
--rw-r--r--   0        0        0      906 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign_criterion.json
--rw-r--r--   0        0        0      501 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign_label.json
--rw-r--r--   0        0        0      583 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/change_status.json
--rw-r--r--   0        0        0     1342 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/click_view.json
--rw-r--r--   0        0        0     1965 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/customer.json
--rw-r--r--   0        0        0      544 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/customer_client.json
--rw-r--r--   0        0        0      384 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/customer_label.json
--rw-r--r--   0        0        0     6505 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/display_keyword_view.json
--rw-r--r--   0        0        0      553 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/geographic_view.json
--rw-r--r--   0        0        0     2150 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/keyword_view.json
--rw-r--r--   0        0        0      574 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/label.json
--rw-r--r--   0        0        0     1878 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/service_accounts.json
--rw-r--r--   0        0        0     4499 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/shopping_performance_view.json
--rw-r--r--   0        0        0     6513 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/topic_view.json
--rw-r--r--   0        0        0      706 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/user_interest.json
--rw-r--r--   0        0        0     3529 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/schemas/user_location_view.json
--rw-r--r--   0        0        0    12007 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/source.py
--rw-r--r--   0        0        0     7810 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/spec.json
--rw-r--r--   0        0        0    37661 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/streams.py
--rw-r--r--   0        0        0    21368 2024-04-08 12:42:51.000000 airbyte_source_google_ads-3.4.1/source_google_ads/utils.py
--rw-r--r--   0        0        0     5358 1970-01-01 00:00:00.000000 airbyte_source_google_ads-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4573 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/README.md
+-rw-r--r--   0        0        0      837 2024-05-07 12:21:59.569654 airbyte_source_google_ads-3.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1201 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/__init__.py
+-rw-r--r--   0        0        0     4834 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/config_migrations.py
+-rw-r--r--   0        0        0     4251 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/custom_query_stream.py
+-rw-r--r--   0        0        0     9407 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/google_ads.py
+-rw-r--r--   0        0        0     1078 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/models.py
+-rw-r--r--   0        0        0      360 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/run.py
+-rw-r--r--   0        0        0     7841 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/account_performance_report.json
+-rw-r--r--   0        0        0     4764 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group.json
+-rw-r--r--   0        0        0    23470 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_ad.json
+-rw-r--r--   0        0        0     1121 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_ad_label.json
+-rw-r--r--   0        0        0    21748 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_ad_legacy.json
+-rw-r--r--   0        0        0     5444 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_bidding_strategy.json
+-rw-r--r--   0        0        0    12187 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_criterion.json
+-rw-r--r--   0        0        0     1031 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_criterion_label.json
+-rw-r--r--   0        0        0      851 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_label.json
+-rw-r--r--   0        0        0     5322 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_listing_group_criterion.json
+-rw-r--r--   0        0        0     1493 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/audience.json
+-rw-r--r--   0        0        0    16096 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/campaign.json
+-rw-r--r--   0        0        0     5671 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/campaign_bidding_strategy.json
+-rw-r--r--   0        0        0     8151 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/campaign_budget.json
+-rw-r--r--   0        0        0     1691 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/campaign_criterion.json
+-rw-r--r--   0        0        0      882 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/campaign_label.json
+-rw-r--r--   0        0        0     1017 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/change_status.json
+-rw-r--r--   0        0        0     2507 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/click_view.json
+-rw-r--r--   0        0        0     3572 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/customer.json
+-rw-r--r--   0        0        0      984 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/customer_client.json
+-rw-r--r--   0        0        0      778 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/customer_label.json
+-rw-r--r--   0        0        0    11041 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/display_keyword_view.json
+-rw-r--r--   0        0        0     1087 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/geographic_view.json
+-rw-r--r--   0        0        0     4225 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/keyword_view.json
+-rw-r--r--   0        0        0     1024 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/label.json
+-rw-r--r--   0        0        0     3485 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/service_accounts.json
+-rw-r--r--   0        0        0     7683 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/shopping_performance_view.json
+-rw-r--r--   0        0        0    12149 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/topic_view.json
+-rw-r--r--   0        0        0     1190 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/user_interest.json
+-rw-r--r--   0        0        0     6435 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/schemas/user_location_view.json
+-rw-r--r--   0        0        0    12007 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/source.py
+-rw-r--r--   0        0        0     7810 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/spec.json
+-rw-r--r--   0        0        0    37661 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/streams.py
+-rw-r--r--   0        0        0    21368 2024-05-07 10:15:59.000000 airbyte_source_google_ads-3.4.2/source_google_ads/utils.py
+-rw-r--r--   0        0        0     5360 1970-01-01 00:00:00.000000 airbyte_source_google_ads-3.4.2/PKG-INFO
```

### Comparing `airbyte_source_google_ads-3.4.1/README.md` & `airbyte_source_google_ads-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/pyproject.toml` & `airbyte_source_google_ads-3.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.4.1"
+version = "3.4.2"
 name = "airbyte-source-google-ads"
 description = "Source implementation for Google Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
@@ -20,15 +20,15 @@
     { include = "source_google_ads" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 google-ads = "==22.1.0"
 protobuf = "==4.25.2"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-google-ads = "source_google_ads.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.12.0"
 requests-mock = "^1.11.0"
```

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/__init__.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/config_migrations.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/custom_query_stream.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/custom_query_stream.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/google_ads.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/google_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/models.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/models.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_ad_label.json` & `airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_label.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'properties'": "{'ad_group.id': {'description': 'The unique identifier of the ad group.'}, "*

 * *                 "'label.name': {'description': 'The name of the label.'}, 'label.resource_name': "*

 * *                 "{'description': 'The resource name of the label.'}, 'label.id': {'description': "*

 * *                 "'The unique identifier of the label.'}, 'ad_group.resource_name': "*

 * *                 "OrderedDict([('description', 'The resource name of the ad group.'), ('type', "*

 * *                 "['null', 'string […]*

```diff
@@ -1,47 +1,47 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "ad_group.id": {
+            "description": "The unique identifier of the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "ad_group_ad.ad.id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "ad_group_ad.ad.resource_name": {
+        "ad_group.resource_name": {
+            "description": "The resource name of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ad_group_ad_label.resource_name": {
+        "ad_group_label.resource_name": {
+            "description": "The resource name of the ad group label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.id": {
+            "description": "The unique identifier of the label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "label.name": {
+            "description": "The name of the label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.resource_name": {
+            "description": "The resource name of the label.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/schemas/ad_group_criterion_label.json` & `airbyte_source_google_ads-3.4.2/source_google_ads/schemas/ad_group_criterion_label.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'properties'": "{'ad_group.id': {'description': 'The ID of the ad group to which the criterion "*

 * *                 "label belongs.'}, 'label.id': {'description': 'The ID of the label assigned to "*

 * *                 "the ad group criterion.'}, 'ad_group_criterion_label.ad_group_criterion': "*

 * *                 "{'description': 'The ad group criterion to which the label is applied.'}, "*

 * *                 "'ad_group_criterion_label.label': {'description': 'The label assigned to the ad "*

 * *                 "group cr […]*

```diff
@@ -1,41 +1,47 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "ad_group.id": {
+            "description": "The ID of the ad group to which the criterion label belongs.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ad_group_criterion.criterion_id": {
+            "description": "The ID of the criterion associated with the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ad_group_criterion_label.ad_group_criterion": {
+            "description": "The ad group criterion to which the label is applied.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "ad_group_criterion_label.label": {
+            "description": "The label assigned to the ad group criterion.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "ad_group_criterion_label.resource_name": {
+            "description": "The resource name of the ad group criterion label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.id": {
+            "description": "The ID of the label assigned to the ad group criterion.",
             "type": [
                 "null",
                 "integer"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/schemas/campaign_bidding_strategy.json` & `airbyte_source_google_ads-3.4.2/source_google_ads/schemas/click_view.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8421717171717171%*

 * *Differences: {"'properties'": "{'customer.id': {'description': 'The unique identifier for the customer "*

 * *                 "account.'}, 'campaign.id': {'description': 'The unique identifier for the "*

 * *                 "campaign.'}, 'segments.date': {'description': 'The date when the click "*

 * *                 "occurred.'}, 'ad_group.name': OrderedDict([('description', 'The name of the ad "*

 * *                 "group.'), ('type', ['null', 'string'])]), 'click_view.gclid': "*

 * *                 "OrderedDict([('description', 'The Go […]*

```diff
@@ -1,191 +1,117 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "bidding_strategy.aligned_campaign_budget_id": {
+        "ad_group.id": {
+            "description": "The unique identifier for the ad group.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "bidding_strategy.campaign_count": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.currency_code": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "bidding_strategy.effective_currency_code": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "bidding_strategy.enhanced_cpc": {
+        "ad_group.name": {
+            "description": "The name of the ad group.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bidding_strategy.id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.maximize_conversion_value.cpc_bid_ceiling_micros": {
+        "campaign.id": {
+            "description": "The unique identifier for the campaign.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "bidding_strategy.maximize_conversion_value.cpc_bid_floor_micros": {
+        "campaign.name": {
+            "description": "The name of the campaign.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "bidding_strategy.maximize_conversion_value.target_roas": {
+        "campaign.network_settings.target_content_network": {
+            "description": "Boolean indicating if the campaign is targeting the content network.",
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "bidding_strategy.maximize_conversions.cpc_bid_ceiling_micros": {
+        "campaign.network_settings.target_google_search": {
+            "description": "Boolean indicating if the campaign is targeting Google search.",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "bidding_strategy.maximize_conversions.cpc_bid_floor_micros": {
+        "campaign.network_settings.target_partner_search_network": {
+            "description": "Boolean indicating if the campaign is targeting partner search network.",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "bidding_strategy.maximize_conversions.target_cpa_micros": {
+        "campaign.network_settings.target_search_network": {
+            "description": "Boolean indicating if the campaign is targeting search network.",
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "bidding_strategy.name": {
+        "click_view.ad_group_ad": {
+            "description": "Details of the ad in the ad group that was clicked.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bidding_strategy.non_removed_campaign_count": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.resource_name": {
+        "click_view.gclid": {
+            "description": "The Google Click Identifier for tracking purposes.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bidding_strategy.status": {
+        "click_view.keyword": {
+            "description": "The keyword that triggered the ad click.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bidding_strategy.target_cpa.cpc_bid_ceiling_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_cpa.cpc_bid_floor_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_cpa.target_cpa_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_impression_share.cpc_bid_ceiling_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_impression_share.location": {
+        "click_view.keyword_info.match_type": {
+            "description": "The match type of the keyword triggering the ad click.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "bidding_strategy.target_impression_share.location_fraction_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_roas.cpc_bid_ceiling_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_roas.cpc_bid_floor_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_roas.target_roas": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "bidding_strategy.target_spend.cpc_bid_ceiling_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.target_spend.target_spend_micros": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "bidding_strategy.type": {
+        "click_view.keyword_info.text": {
+            "description": "The text of the keyword that triggered the ad click.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "campaign.id": {
+        "customer.id": {
+            "description": "The unique identifier for the customer account.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "customer.id": {
+        "segments.ad_network_type": {
+            "description": "Type of ad network where the click originated.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "segments.date": {
+            "description": "The date when the click occurred.",
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/schemas/label.json` & `airbyte_source_google_ads-3.4.2/source_google_ads/schemas/label.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'properties'": "{'customer.id': {'description': 'The unique identifier of the customer "*

 * *                 "associated with the label.'}, 'label.id': {'description': 'The unique identifier "*

 * *                 "of the label.'}, 'label.name': {'description': 'The name associated with the "*

 * *                 "label.'}, 'label.resource_name': {'description': 'The resource name of the "*

 * *                 "label.'}, 'label.status': {'description': 'The status of the label.'}, "*

 * *                 "'label.text_label.b […]*

```diff
@@ -1,47 +1,54 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "customer.id": {
+            "description": "The unique identifier of the customer associated with the label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "label.id": {
+            "description": "The unique identifier of the label.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "label.name": {
+            "description": "The name associated with the label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.resource_name": {
+            "description": "The resource name of the label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.status": {
+            "description": "The status of the label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.text_label.background_color": {
+            "description": "The background color of the text label.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "label.text_label.description": {
+            "description": "The description associated with the text label.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/source.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/spec.json` & `airbyte_source_google_ads-3.4.2/source_google_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/streams.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/source_google_ads/utils.py` & `airbyte_source_google_ads-3.4.2/source_google_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_ads-3.4.1/PKG-INFO` & `airbyte_source_google_ads-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-ads
-Version: 3.4.1
+Version: 3.4.2
 Summary: Source implementation for Google Ads.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Requires-Dist: google-ads (==22.1.0)
 Requires-Dist: protobuf (==4.25.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/google-ads
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Google-Ads source connector
```

