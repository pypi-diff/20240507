# Comparing `tmp/airbyte_source_instagram-3.0.5.tar.gz` & `tmp/airbyte_source_instagram-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_instagram-3.0.5.tar", max compression
+gzip compressed data, was "airbyte_source_instagram-3.0.7.tar", max compression
```

## Comparing `airbyte_source_instagram-3.0.5.tar` & `airbyte_source_instagram-3.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4550 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/README.md
--rw-r--r--   0        0        0      814 2024-03-20 18:33:13.346905 airbyte_source_instagram-3.0.5/pyproject.toml
--rw-r--r--   0        0        0       67 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/__init__.py
--rw-r--r--   0        0        0     4887 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/api.py
--rw-r--r--   0        0        0     3281 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/common.py
--rw-r--r--   0        0        0      239 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/run.py
--rw-r--r--   0        0        0     2357 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/media.json
--rw-r--r--   0        0        0      909 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/media_insights.json
--rw-r--r--   0        0        0     1108 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/stories.json
--rw-r--r--   0        0        0      399 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/story_insights.json
--rw-r--r--   0        0        0     1218 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/user_insights.json
--rw-r--r--   0        0        0      341 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/user_lifetime_insights.json
--rw-r--r--   0        0        0      699 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/schemas/users.json
--rw-r--r--   0        0        0     5683 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/source.py
--rw-r--r--   0        0        0    21534 2024-03-20 18:29:21.265722 airbyte_source_instagram-3.0.5/source_instagram/streams.py
--rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 airbyte_source_instagram-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     4550 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/README.md
+-rw-r--r--   0        0        0      818 2024-05-07 12:25:04.958446 airbyte_source_instagram-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/__init__.py
+-rw-r--r--   0        0        0     4887 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/api.py
+-rw-r--r--   0        0        0     3281 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/common.py
+-rw-r--r--   0        0        0      239 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/run.py
+-rw-r--r--   0        0        0     4924 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/media.json
+-rw-r--r--   0        0        0     2012 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/media_insights.json
+-rw-r--r--   0        0        0     2093 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/stories.json
+-rw-r--r--   0        0        0      907 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/story_insights.json
+-rw-r--r--   0        0        0     2566 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/user_insights.json
+-rw-r--r--   0        0        0      791 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/user_lifetime_insights.json
+-rw-r--r--   0        0        0     1591 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/schemas/users.json
+-rw-r--r--   0        0        0     5683 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/source.py
+-rw-r--r--   0        0        0    21534 2024-05-07 10:34:10.000000 airbyte_source_instagram-3.0.7/source_instagram/streams.py
+-rw-r--r--   0        0        0     5348 1970-01-01 00:00:00.000000 airbyte_source_instagram-3.0.7/PKG-INFO
```

### Comparing `airbyte_source_instagram-3.0.5/README.md` & `airbyte_source_instagram-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_instagram-3.0.5/pyproject.toml` & `airbyte_source_instagram-3.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.5"
+version = "3.0.7"
 name = "airbyte-source-instagram"
 description = "Source implementation for Instagram."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -19,15 +19,15 @@
 packages = [
     { include = "source_instagram" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 facebook-business = "==18.0.5"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 cached-property = "==1.5.2"
 
 [tool.poetry.scripts]
 source-instagram = "source_instagram.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
```

### Comparing `airbyte_source_instagram-3.0.5/source_instagram/api.py` & `airbyte_source_instagram-3.0.7/source_instagram/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_instagram-3.0.5/source_instagram/common.py` & `airbyte_source_instagram-3.0.7/source_instagram/common.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_instagram-3.0.5/source_instagram/schemas/media.json` & `airbyte_source_instagram-3.0.7/source_instagram/schemas/media_insights.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7693965517241379%*

 * *Differences: {"'properties'": "{'business_account_id': {'description': 'The unique identifier of the Instagram "*

 * *                 "business account associated with the media.'}, 'page_id': {'description': 'The "*

 * *                 "unique identifier of the Instagram page where the media is posted.'}, 'id': "*

 * *                 "{'description': 'The unique identifier of the media.'}, "*

 * *                 "'ig_reels_avg_watch_time': OrderedDict([('description', 'The average watch time "*

 * *                 "of Instagram Reels vide […]*

```diff
@@ -1,198 +1,103 @@
 {
     "properties": {
         "business_account_id": {
+            "description": "The unique identifier of the Instagram business account associated with the media.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "caption": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "children": {
-            "items": {
-                "properties": {
-                    "id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "ig_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "media_type": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "media_url": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "owner": {
-                        "properties": {
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "permalink": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "shortcode": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "thumbnail_url": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "timestamp": {
-                        "airbyte_type": "timestamp_with_timezone",
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "username": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": "object"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "comments_count": {
+        "comments": {
+            "description": "The number of comments received on the media.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "id": {
+            "description": "The unique identifier of the media.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ig_id": {
+        "ig_reels_avg_watch_time": {
+            "description": "The average watch time of Instagram Reels videos in seconds.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "is_comment_enabled": {
+        "ig_reels_video_view_total_time": {
+            "description": "The total watch time of Instagram Reels videos in seconds.",
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "like_count": {
+        "impressions": {
+            "description": "The number of times the media has been displayed to users.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "media_product_type": {
+        "likes": {
+            "description": "The number of likes received on the media.",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "media_type": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
-        "media_url": {
+        "page_id": {
+            "description": "The unique identifier of the Instagram page where the media is posted.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "owner": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "plays": {
+            "description": "The number of times the media has been played.",
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "page_id": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
-        "permalink": {
+        "reach": {
+            "description": "The number of unique users who have seen the media.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "shortcode": {
+        "saved": {
+            "description": "The number of times users have saved the media.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "thumbnail_url": {
+        "shares": {
+            "description": "The number of times the media has been shared.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "timestamp": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "total_interactions": {
+            "description": "The total number of interactions (likes, comments, shares) on the media.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "username": {
+        "video_views": {
+            "description": "The total number of views on video media.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_instagram-3.0.5/source_instagram/source.py` & `airbyte_source_instagram-3.0.7/source_instagram/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_instagram-3.0.5/source_instagram/streams.py` & `airbyte_source_instagram-3.0.7/source_instagram/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_instagram-3.0.5/PKG-INFO` & `airbyte_source_instagram-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-instagram
-Version: 3.0.5
+Version: 3.0.7
 Summary: Source implementation for Instagram.
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
 Requires-Dist: cached-property (==1.5.2)
 Requires-Dist: facebook-business (==18.0.5)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/instagram
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Instagram source connector
```

