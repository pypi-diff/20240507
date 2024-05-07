# Comparing `tmp/airbyte_source_google_search_console-1.4.0.tar.gz` & `tmp/airbyte_source_google_search_console-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_search_console-1.4.0.tar", max compression
+gzip compressed data, was "airbyte_source_google_search_console-1.4.2.tar", max compression
```

## Comparing `airbyte_source_google_search_console-1.4.0.tar` & `airbyte_source_google_search_console-1.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     4771 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/README.md
--rw-r--r--   0        0        0      926 2024-03-21 02:21:29.056524 airbyte_source_google_search_console-1.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     1191 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/__init__.py
--rw-r--r--   0        0        0     4134 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/config_migrations.py
--rw-r--r--   0        0        0     1097 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/exceptions.py
--rwxr-xr-x   0        0        0      462 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/run.py
--rwxr-xr-x   0        0        0      804 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_all_fields.json
--rwxr-xr-x   0        0        0      639 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_by_country.json
--rwxr-xr-x   0        0        0      582 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_by_date.json
--rwxr-xr-x   0        0        0      638 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_by_device.json
--rwxr-xr-x   0        0        0      636 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_by_page.json
--rwxr-xr-x   0        0        0      637 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_by_query.json
--rwxr-xr-x   0        0        0      837 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_keyword_page_report.json
--rwxr-xr-x   0        0        0      783 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json
--rwxr-xr-x   0        0        0      783 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json
--rwxr-xr-x   0        0        0      782 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_page_report.json
--rwxr-xr-x   0        0        0      728 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_site_report_by_page.json
--rwxr-xr-x   0        0        0      728 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/search_analytics_site_report_by_site.json
--rwxr-xr-x   0        0        0      990 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/sitemaps.json
--rwxr-xr-x   0        0        0      223 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/sites.json
--rwxr-xr-x   0        0        0     1225 2024-03-21 01:47:20.481994 airbyte_source_google_search_console-1.4.0/source_google_search_console/service_account_authenticator.py
--rwxr-xr-x   0        0        0    10013 2024-03-21 01:47:20.485994 airbyte_source_google_search_console-1.4.0/source_google_search_console/source.py
--rwxr-xr-x   0        0        0     8470 2024-03-21 01:47:20.485994 airbyte_source_google_search_console-1.4.0/source_google_search_console/spec.json
--rwxr-xr-x   0        0        0    18404 2024-03-21 01:47:20.485994 airbyte_source_google_search_console-1.4.0/source_google_search_console/streams.py
--rw-r--r--   0        0        0     5607 1970-01-01 00:00:00.000000 airbyte_source_google_search_console-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     4771 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/README.md
+-rw-r--r--   0        0        0      930 2024-05-07 12:21:58.536642 airbyte_source_google_search_console-1.4.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1191 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/__init__.py
+-rw-r--r--   0        0        0     4134 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/config_migrations.py
+-rw-r--r--   0        0        0     1097 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/exceptions.py
+-rwxr-xr-x   0        0        0      462 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/run.py
+-rw-r--r--   0        0        0     1729 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_all_fields.json
+-rw-r--r--   0        0        0     1491 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_country.json
+-rw-r--r--   0        0        0     1388 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_date.json
+-rw-r--r--   0        0        0     1525 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_device.json
+-rw-r--r--   0        0        0     1473 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_page.json
+-rw-r--r--   0        0        0     1439 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_by_query.json
+-rw-r--r--   0        0        0     1681 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_page_report.json
+-rw-r--r--   0        0        0     1626 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_page.json
+-rw-r--r--   0        0        0     1755 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_keyword_site_report_by_site.json
+-rw-r--r--   0        0        0     1776 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_page_report.json
+-rw-r--r--   0        0        0     1515 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_page.json
+-rw-r--r--   0        0        0     1408 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/search_analytics_site_report_by_site.json
+-rw-r--r--   0        0        0     1775 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sitemaps.json
+-rw-r--r--   0        0        0      383 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sites.json
+-rwxr-xr-x   0        0        0     1225 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/service_account_authenticator.py
+-rwxr-xr-x   0        0        0    10013 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/source.py
+-rwxr-xr-x   0        0        0     8470 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/spec.json
+-rwxr-xr-x   0        0        0    18404 2024-05-07 10:16:14.000000 airbyte_source_google_search_console-1.4.2/source_google_search_console/streams.py
+-rw-r--r--   0        0        0     5609 1970-01-01 00:00:00.000000 airbyte_source_google_search_console-1.4.2/PKG-INFO
```

### Comparing `airbyte_source_google_search_console-1.4.0/README.md` & `airbyte_source_google_search_console-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/__init__.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/config_migrations.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/exceptions.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/schemas/sitemaps.json` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/schemas/sitemaps.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9628665123456791%*

 * *Differences: {"'properties'": "{'path': {'description': 'Path to the sitemap file'}, 'lastSubmitted': "*

 * *                 "{'description': 'Timestamp when the sitemap was last submitted'}, 'isPending': "*

 * *                 "{'description': 'Flag indicating if the sitemap is pending for processing'}, "*

 * *                 "'isSitemapsIndex': {'description': 'Flag indicating if the data represents a "*

 * *                 "sitemap index'}, 'type': {'description': 'Type of the sitemap'}, "*

 * *                 "'lastDownloaded': {'descr […]*

```diff
@@ -1,81 +1,93 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "contents": {
+            "description": "Data related to the sitemap contents",
             "items": {
                 "properties": {
                     "indexed": {
+                        "description": "Number of indexed sitemap URLs",
                         "type": [
                             "null",
                             "string"
                         ]
                     },
                     "submitted": {
+                        "description": "Number of submitted sitemap URLs",
                         "type": [
                             "null",
                             "string"
                         ]
                     },
                     "type": {
+                        "description": "Type of the sitemap content",
                         "type": [
                             "null",
                             "string"
                         ]
                     }
                 },
                 "type": "object"
             },
             "type": "array"
         },
         "errors": {
+            "description": "Errors encountered while processing the sitemaps",
             "type": [
                 "null",
                 "string"
             ]
         },
         "isPending": {
+            "description": "Flag indicating if the sitemap is pending for processing",
             "type": [
                 "null",
                 "boolean"
             ]
         },
         "isSitemapsIndex": {
+            "description": "Flag indicating if the data represents a sitemap index",
             "type": [
                 "null",
                 "boolean"
             ]
         },
         "lastDownloaded": {
+            "description": "Timestamp when the sitemap was last downloaded",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "lastSubmitted": {
+            "description": "Timestamp when the sitemap was last submitted",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "path": {
+            "description": "Path to the sitemap file",
             "type": [
                 "null",
                 "string"
             ]
         },
         "type": {
+            "description": "Type of the sitemap",
             "type": [
                 "null",
                 "string"
             ]
         },
         "warnings": {
+            "description": "Warnings encountered while processing the sitemaps",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/service_account_authenticator.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/service_account_authenticator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/source.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/spec.json` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/source_google_search_console/streams.py` & `airbyte_source_google_search_console-1.4.2/source_google_search_console/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_search_console-1.4.0/PKG-INFO` & `airbyte_source_google_search_console-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-search-console
-Version: 1.4.0
+Version: 1.4.2
 Summary: Source implementation for Google Search Console.
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
 Requires-Dist: google-api-python-client (==2.105.0)
 Requires-Dist: google-auth (==2.23.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/google-search-console
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Google-Search-Console source connector
```

