# Comparing `tmp/airbyte_source_linkedin_ads-2.1.0.tar.gz` & `tmp/airbyte_source_linkedin_ads-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_linkedin_ads-2.1.0.tar", max compression
+gzip compressed data, was "airbyte_source_linkedin_ads-2.1.1.tar", max compression
```

## Comparing `airbyte_source_linkedin_ads-2.1.0.tar` & `airbyte_source_linkedin_ads-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4604 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/README.md
--rw-r--r--   0        0        0      776 2024-05-02 12:06:29.258237 airbyte_source_linkedin_ads-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1179 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/__init__.py
--rw-r--r--   0        0        0    15085 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/analytics_streams.py
--rw-r--r--   0        0        0      246 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/run.py
--rw-r--r--   0        0        0      512 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/account_users.json
--rw-r--r--   0        0        0     1405 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/accounts.json
--rw-r--r--   0        0        0     7113 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/ad_analytics.json
--rw-r--r--   0        0        0     1399 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaign_groups.json
--rw-r--r--   0        0        0     4731 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaigns.json
--rw-r--r--   0        0        0     1511 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/conversions.json
--rw-r--r--   0        0        0     1404 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/creatives.json
--rw-r--r--   0        0        0     5505 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/source.py
--rw-r--r--   0        0        0     6880 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/spec.json
--rw-r--r--   0        0        0    18463 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/streams.py
--rw-r--r--   0        0        0    11728 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/utils.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4604 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/README.md
+-rw-r--r--   0        0        0      776 2024-05-07 10:41:53.323349 airbyte_source_linkedin_ads-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1179 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/__init__.py
+-rw-r--r--   0        0        0    15085 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/analytics_streams.py
+-rw-r--r--   0        0        0      246 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/run.py
+-rw-r--r--   0        0        0      512 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/account_users.json
+-rw-r--r--   0        0        0     1405 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/accounts.json
+-rw-r--r--   0        0        0     7113 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/ad_analytics.json
+-rw-r--r--   0        0        0     1399 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/campaign_groups.json
+-rw-r--r--   0        0        0     4731 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/campaigns.json
+-rw-r--r--   0        0        0     1511 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/conversions.json
+-rw-r--r--   0        0        0     1404 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/creatives.json
+-rw-r--r--   0        0        0     5505 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/source.py
+-rw-r--r--   0        0        0     6880 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/spec.json
+-rw-r--r--   0        0        0    18927 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/streams.py
+-rw-r--r--   0        0        0    11728 2024-05-07 10:11:05.000000 airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/utils.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-2.1.1/PKG-INFO
```

### Comparing `airbyte_source_linkedin_ads-2.1.0/README.md` & `airbyte_source_linkedin_ads-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/pyproject.toml` & `airbyte_source_linkedin_ads-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.0"
+version = "2.1.1"
 name = "airbyte-source-linkedin-ads"
 description = "Source implementation for Linkedin Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/__init__.py` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/analytics_streams.py` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/analytics_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/account_users.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/accounts.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/ad_analytics.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/ad_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaign_groups.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaigns.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/conversions.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/conversions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/creatives.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/source.py` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/spec.json` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/streams.py` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Iterable, Mapping, MutableMapping, Optional
-from urllib.parse import urlencode
+from urllib.parse import quote, urlencode
 
 import pendulum
 import requests
 from airbyte_cdk.sources.streams.http import HttpStream
 from airbyte_cdk.sources.utils.transform import TransformConfig, TypeTransformer
 
 from .utils import get_parent_stream_values, transform_data
@@ -179,20 +179,27 @@
         stream_slice: Mapping[str, Any] = None,
         next_page_token: Mapping[str, Any] = None,
     ) -> MutableMapping[str, Any]:
         """
         Override request_params() to have the ability to accept the specific account_ids from user's configuration.
         If we have list of account_ids, we need to make sure that the request_params are encoded correctly,
         We will get HTTP Error 500, if we use standard requests.urlencode methods to parse parameters,
-        so the urlencode(..., safe=":(),") is used instead, to keep the values as they are.
+        so the urlencode(..., safe=":(),%") is used instead, to keep the values as they are.
         """
         params = super().request_params(stream_state, stream_slice, next_page_token)
         if self.accounts:
-            params["search"] = f"(id:(values:List({self.accounts})))"
-        return urlencode(params, safe="():,%")
+            # Construct the URN for each account ID
+            accounts = [f"urn:li:sponsoredAccount:{account_id}" for account_id in self.config.get("account_ids")]
+
+            # Join the URNs into a single string, separated by commas, and URL encode only this part
+            encoded_accounts = quote(",".join(accounts), safe=",")
+
+            # Insert the encoded account IDs into the overall structure, keeping colons and parentheses outside safe
+            params["search"] = f"(id:(values:List({encoded_accounts})))"
+        return urlencode(params, safe=":(),%")
 
 
 class IncrementalLinkedinAdsStream(LinkedinAdsStream):
     cursor_field = "lastModified"
 
     @property
     def primary_slice_key(self) -> str:
```

### Comparing `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/utils.py` & `airbyte_source_linkedin_ads-2.1.1/source_linkedin_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.1.0/PKG-INFO` & `airbyte_source_linkedin_ads-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-linkedin-ads
-Version: 2.1.0
+Version: 2.1.1
 Summary: Source implementation for Linkedin Ads.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

