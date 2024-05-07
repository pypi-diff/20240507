# Comparing `tmp/zyte-spider-templates-0.7.1.tar.gz` & `tmp/zyte_spider_templates-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-spider-templates-0.7.1.tar", last modified: Thu Feb 22 20:58:04 2024, max compression
+gzip compressed data, was "zyte_spider_templates-0.7.2.tar", last modified: Tue May  7 19:41:23 2024, max compression
```

## Comparing `zyte-spider-templates-0.7.1.tar` & `zyte_spider_templates-0.7.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.798798 zyte-spider-templates-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.798798 zyte-spider-templates-0.7.1/tests/pages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/pages/test_product_navigation_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)    22706 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/test_ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/test_middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/zyte_spider_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/_geolocations.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/middlewares.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/zyte_spider_templates/page_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/page_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/page_objects/product_navigation_heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/zyte_spider_templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/pages/product_navigation_heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/zyte_spider_templates/spiders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/spiders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/spiders/ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-22 20:57:48.000000 zyte-spider-templates-0.7.1/zyte_spider_templates/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:58:04.802798 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-22 20:58:04.000000 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-22 20:58:04.000000 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 20:58:04.000000 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-22 20:58:04.000000 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-22 20:58:04.000000 zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.162784 zyte_spider_templates-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.162784 zyte_spider_templates-0.7.2/tests/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/pages/test_product_navigation_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23412 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/test_ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/test_middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.162784 zyte_spider_templates-0.7.2/zyte_spider_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/_geolocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/middlewares.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.162784 zyte_spider_templates-0.7.2/zyte_spider_templates/page_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/page_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/page_objects/product_navigation_heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/zyte_spider_templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/pages/product_navigation_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/zyte_spider_templates/spiders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/spiders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/spiders/ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 19:41:19.000000 zyte_spider_templates-0.7.2/zyte_spider_templates/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:41:23.166784 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-07 19:41:23.000000 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-07 19:41:23.000000 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:41:23.000000 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 19:41:23.000000 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 19:41:23.000000 zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/top_level.txt
```

### Comparing `zyte-spider-templates-0.7.1/LICENSE` & `zyte_spider_templates-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/PKG-INFO` & `zyte_spider_templates-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-spider-templates
-Version: 0.7.1
+Version: 0.7.2
 Summary: Spider templates for automatic crawlers.
 Home-page: https://github.com/zytedata/zyte-spider-templates
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-spider-templates-0.7.1/README.rst` & `zyte_spider_templates-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/setup.py` & `zyte_spider_templates-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="zyte-spider-templates",
-    version="0.7.1",
+    version="0.7.2",
     description="Spider templates for automatic crawlers.",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="info@zyte.com",
     url="https://github.com/zytedata/zyte-spider-templates",
     packages=find_packages(),
```

### Comparing `zyte-spider-templates-0.7.1/tests/__init__.py` & `zyte_spider_templates-0.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/tests/pages/test_product_navigation_heuristics.py` & `zyte_spider_templates-0.7.2/tests/pages/test_product_navigation_heuristics.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/tests/test_ecommerce.py` & `zyte_spider_templates-0.7.2/tests/test_ecommerce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import re
 from unittest.mock import MagicMock, call
 
 import pytest
 import scrapy
 from pydantic import ValidationError
@@ -344,119 +345,139 @@
         crawler = get_crawler(settings=settings)
         spider = EcommerceSpider.from_crawler(crawler, **kwargs, **base_kwargs)
         getter = getattr(crawler.settings, getter_name)
         assert getter(setting) == new_setting_value
         assert spider.allowed_domains == ["example.com"]
 
 
+def assertEqualJson(actual, expected):
+    """Compare the JSON representation of 2 Python objects.
+
+    This allows to take into account things like the order of key-value pairs
+    in dictionaries, which would not be taken into account when comparing
+    dictionaries directly.
+
+    It also generates a better diff in pytest output when enums are involved,
+    e.g. geolocation values.
+    """
+    actual_json = json.dumps(actual, indent=2)
+    expected_json = json.dumps(expected, indent=2)
+    assert actual_json == expected_json
+
+
 def test_metadata():
-    metadata = get_spider_metadata(EcommerceSpider, normalize=True)
-    assert metadata == {
+    actual_metadata = get_spider_metadata(EcommerceSpider, normalize=True)
+    expected_metadata = {
         "template": True,
         "title": "E-commerce",
         "description": "Template for spiders that extract product data from e-commerce websites.",
         "param_schema": {
             "properties": {
-                "crawl_strategy": {
-                    "default": "full",
-                    "title": "Crawl strategy",
-                    "description": "Determines how the start URL and follow-up URLs are crawled.",
-                    "type": "string",
-                    "enum": ["full", "navigation", "pagination_only"],
-                    "enumMeta": {
-                        "full": {
-                            "description": "Follow most links within the domain of URL in an attempt to discover and extract as many products as possible.",
-                            "title": "Full",
-                        },
-                        "navigation": {
-                            "description": (
-                                "Follow pagination, subcategories, and "
-                                "product detail pages. Pagination Only is a "
-                                "better choice if the target URL does not "
-                                "have subcategories, or if Zyte API is "
-                                "misidentifying some URLs as subcategories."
-                            ),
-                            "title": "Navigation",
-                        },
-                        "pagination_only": {
-                            "description": (
-                                "Follow pagination and product detail pages. Subcategory links are ignored."
-                            ),
-                            "title": "Pagination Only",
-                        },
-                    },
-                },
-                "extract_from": {
-                    "anyOf": [{"type": "string"}, {"type": "null"}],
-                    "default": None,
-                    "title": "Extraction source",
+                "url": {
                     "description": (
-                        "Whether to perform extraction using a browser request "
-                        "(browserHtml) or an HTTP request (httpResponseBody)."
+                        "Initial URL for the crawl. Enter the full URL including http(s), "
+                        "you can copy and paste it from your browser. Example: https://toscrape.com/"
                     ),
-                    "enum": ["httpResponseBody", "browserHtml"],
-                    "enumMeta": {
-                        "httpResponseBody": {
-                            "title": "httpResponseBody",
-                            "description": "Use HTTP responses. Cost-efficient and fast extraction method, which works well on many websites.",
-                        },
-                        "browserHtml": {
-                            "title": "browserHtml",
-                            "description": "Use browser rendering. Often provides the best quality.",
-                        },
-                    },
+                    "pattern": r"^https?://[^:/\s]+(:\d{1,5})?(/[^\s]*)*(#[^\s]*)?$",
+                    "title": "URL",
+                    "type": "string",
                 },
                 "geolocation": {
                     "anyOf": [
                         {"type": "string"},
                         {"type": "null"},
                     ],
                     "default": None,
-                    "title": "Geolocation",
-                    "description": "ISO 3166-1 alpha-2 2-character string specified in "
-                    "https://docs.zyte.com/zyte-api/usage/reference.html#operation/extract/request/geolocation.",
-                    "enum": list(
-                        sorted(GEOLOCATION_OPTIONS, key=GEOLOCATION_OPTIONS.__getitem__)
+                    "description": (
+                        "ISO 3166-1 alpha-2 2-character string specified in "
+                        "https://docs.zyte.com/zyte-api/usage/reference.html"
+                        "#operation/extract/request/geolocation."
                     ),
                     "enumMeta": {
                         code: {
                             "title": GEOLOCATION_OPTIONS_WITH_CODE[code],
                         }
-                        for code in Geolocation
+                        for code in sorted(Geolocation)
                     },
+                    "title": "Geolocation",
+                    "enum": list(
+                        sorted(GEOLOCATION_OPTIONS, key=GEOLOCATION_OPTIONS.__getitem__)
+                    ),
                 },
                 "max_requests": {
                     "anyOf": [{"type": "integer"}, {"type": "null"}],
                     "default": 100,
-                    "title": "Max Requests",
                     "description": (
                         "The maximum number of Zyte API requests allowed for the crawl.\n"
                         "\n"
                         "Requests with error responses that cannot be retried or exceed "
                         "their retry limit also count here, but they incur in no costs "
                         "and do not increase the request count in Scrapy Cloud."
                     ),
+                    "title": "Max Requests",
                     "widget": "request-limit",
                 },
-                "url": {
-                    "type": "string",
-                    "title": "URL",
+                "extract_from": {
+                    "anyOf": [{"type": "string"}, {"type": "null"}],
+                    "default": None,
                     "description": (
-                        "Initial URL for the crawl. Enter the full URL including http(s), "
-                        "you can copy and paste it from your browser. Example: https://toscrape.com/"
+                        "Whether to perform extraction using a browser request "
+                        "(browserHtml) or an HTTP request (httpResponseBody)."
                     ),
-                    "pattern": r"^https?://[^:/\s]+(:\d{1,5})?(/[^\s]*)*(#[^\s]*)?$",
+                    "enumMeta": {
+                        "browserHtml": {
+                            "description": "Use browser rendering. Often provides the best quality.",
+                            "title": "browserHtml",
+                        },
+                        "httpResponseBody": {
+                            "description": "Use HTTP responses. Cost-efficient and fast extraction method, which works well on many websites.",
+                            "title": "httpResponseBody",
+                        },
+                    },
+                    "title": "Extraction source",
+                    "enum": ["httpResponseBody", "browserHtml"],
+                },
+                "crawl_strategy": {
+                    "default": "full",
+                    "description": "Determines how the start URL and follow-up URLs are crawled.",
+                    "enumMeta": {
+                        "full": {
+                            "description": "Follow most links within the domain of URL in an attempt to discover and extract as many products as possible.",
+                            "title": "Full",
+                        },
+                        "navigation": {
+                            "description": (
+                                "Follow pagination, subcategories, and "
+                                "product detail pages. Pagination Only is a "
+                                "better choice if the target URL does not "
+                                "have subcategories, or if Zyte API is "
+                                "misidentifying some URLs as subcategories."
+                            ),
+                            "title": "Navigation",
+                        },
+                        "pagination_only": {
+                            "description": (
+                                "Follow pagination and product detail pages. Subcategory links are ignored."
+                            ),
+                            "title": "Pagination Only",
+                        },
+                    },
+                    "title": "Crawl strategy",
+                    "enum": ["full", "navigation", "pagination_only"],
+                    "type": "string",
                 },
             },
             "required": ["url"],
             "title": "EcommerceSpiderParams",
             "type": "object",
         },
     }
-    geolocation = metadata["param_schema"]["properties"]["geolocation"]
+    assertEqualJson(actual_metadata, expected_metadata)
+
+    geolocation = actual_metadata["param_schema"]["properties"]["geolocation"]
     assert geolocation["enum"][0] == "AF"
     assert geolocation["enumMeta"]["UY"] == {"title": "Uruguay (UY)"}
     assert set(geolocation["enum"]) == set(geolocation["enumMeta"])
 
 
 @pytest.mark.parametrize(
     "valid,url",
```

### Comparing `zyte-spider-templates-0.7.1/tests/test_heuristics.py` & `zyte_spider_templates-0.7.2/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/tests/test_middlewares.py` & `zyte_spider_templates-0.7.2/tests/test_middlewares.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/tests/test_utils.py` & `zyte_spider_templates-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates/_geolocations.py` & `zyte_spider_templates-0.7.2/zyte_spider_templates/_geolocations.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates/heuristics.py` & `zyte_spider_templates-0.7.2/zyte_spider_templates/heuristics.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates/middlewares.py` & `zyte_spider_templates-0.7.2/zyte_spider_templates/middlewares.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates/pages/product_navigation_heuristics.py` & `zyte_spider_templates-0.7.2/zyte_spider_templates/pages/product_navigation_heuristics.py`

 * *Files identical despite different names*

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates/spiders/ecommerce.py` & `zyte_spider_templates-0.7.2/zyte_spider_templates/spiders/ecommerce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from enum import Enum
 from typing import Any, Callable, Dict, Iterable, Optional, Union
 
 import scrapy
-from pydantic import Field
+from pydantic import BaseModel, Field
 from scrapy import Request
 from scrapy.crawler import Crawler
 from scrapy_poet import DummyResponse
 from scrapy_spider_metadata import Args
 from zyte_common_items import ProbabilityRequest, Product, ProductNavigation
 
-from zyte_spider_templates.documentation import document_enum
 from zyte_spider_templates.spiders.base import (
     ARG_SETTING_PRIORITY,
     BaseSpider,
     BaseSpiderParams,
 )
 from zyte_spider_templates.utils import get_domain
 
+from ..documentation import document_enum
+
 
 @document_enum
 class EcommerceCrawlStrategy(str, Enum):
     full: str = "full"
     """Follow most links within the domain of URL in an attempt to discover and
     extract as many products as possible."""
 
@@ -32,15 +33,15 @@
     """
 
     pagination_only: str = "pagination_only"
     """Follow pagination and product detail pages. Subcategory links are
     ignored."""
 
 
-class EcommerceSpiderParams(BaseSpiderParams):
+class EcommerceCrawlStrategyParam(BaseModel):
     crawl_strategy: EcommerceCrawlStrategy = Field(
         title="Crawl strategy",
         description="Determines how the start URL and follow-up URLs are crawled.",
         default=EcommerceCrawlStrategy.full,
         json_schema_extra={
             "enumMeta": {
                 EcommerceCrawlStrategy.full: {
@@ -63,14 +64,18 @@
                     ),
                 },
             },
         },
     )
 
 
+class EcommerceSpiderParams(EcommerceCrawlStrategyParam, BaseSpiderParams):
+    pass
+
+
 class EcommerceSpider(Args[EcommerceSpiderParams], BaseSpider):
     """Yield products from an e-commerce website.
 
     See :class:`~zyte_spider_templates.spiders.ecommerce.EcommerceSpiderParams`
     for supported parameters.
 
     .. seealso:: :ref:`e-commerce`.
```

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/PKG-INFO` & `zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-spider-templates
-Version: 0.7.1
+Version: 0.7.2
 Summary: Spider templates for automatic crawlers.
 Home-page: https://github.com/zytedata/zyte-spider-templates
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-spider-templates-0.7.1/zyte_spider_templates.egg-info/SOURCES.txt` & `zyte_spider_templates-0.7.2/zyte_spider_templates.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 tests/pages/__init__.py
 tests/pages/test_product_navigation_heuristics.py
 zyte_spider_templates/__init__.py
 zyte_spider_templates/_geolocations.py
 zyte_spider_templates/documentation.py
 zyte_spider_templates/heuristics.py
 zyte_spider_templates/middlewares.py
+zyte_spider_templates/params.py
 zyte_spider_templates/utils.py
 zyte_spider_templates.egg-info/PKG-INFO
 zyte_spider_templates.egg-info/SOURCES.txt
 zyte_spider_templates.egg-info/dependency_links.txt
 zyte_spider_templates.egg-info/requires.txt
 zyte_spider_templates.egg-info/top_level.txt
 zyte_spider_templates/page_objects/__init__.py
```

