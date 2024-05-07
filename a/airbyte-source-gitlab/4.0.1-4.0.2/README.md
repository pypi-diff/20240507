# Comparing `tmp/airbyte_source_gitlab-4.0.1.tar.gz` & `tmp/airbyte_source_gitlab-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_gitlab-4.0.1.tar", max compression
+gzip compressed data, was "airbyte_source_gitlab-4.0.2.tar", max compression
```

## Comparing `airbyte_source_gitlab-4.0.1.tar` & `airbyte_source_gitlab-4.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     4501 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/README.md
--rw-r--r--   0        0        0      758 2024-04-23 16:20:49.970526 airbyte_source_gitlab-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/__init__.py
--rw-r--r--   0        0        0     2054 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/components/partition_routers.py
--rw-r--r--   0        0        0     3816 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/config_migrations.py
--rw-r--r--   0        0        0    20615 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/manifest.yaml
--rw-r--r--   0        0        0      403 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/run.py
--rw-r--r--   0        0        0      800 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/branches.json
--rw-r--r--   0        0        0     1676 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/commits.json
--rw-r--r--   0        0        0     5084 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/deployments.json
--rw-r--r--   0        0        0     5472 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/epic_issues.json
--rw-r--r--   0        0        0     2790 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/epics.json
--rw-r--r--   0        0        0     1687 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/group_issue_boards.json
--rw-r--r--   0        0        0      785 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/group_labels.json
--rw-r--r--   0        0        0     1261 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/group_members.json
--rw-r--r--   0        0        0      898 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/group_milestones.json
--rw-r--r--   0        0        0     4148 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/groups.json
--rw-r--r--   0        0        0     6304 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/issues.json
--rw-r--r--   0        0        0     2275 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/jobs.json
--rw-r--r--   0        0        0     1744 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/merge_request_commits.json
--rw-r--r--   0        0        0     4388 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/merge_requests.json
--rw-r--r--   0        0        0      777 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/pipelines.json
--rw-r--r--   0        0        0     2041 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/pipelines_extended.json
--rw-r--r--   0        0        0      913 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/project_labels.json
--rw-r--r--   0        0        0     1263 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/project_members.json
--rw-r--r--   0        0        0      900 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/project_milestones.json
--rw-r--r--   0        0        0    12131 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/projects.json
--rw-r--r--   0        0        0     1781 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/releases.json
--rw-r--r--   0        0        0      771 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/tags.json
--rw-r--r--   0        0        0      496 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/schemas/users.json
--rw-r--r--   0        0        0     1093 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/source.py
--rw-r--r--   0        0        0     6132 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/spec.json
--rw-r--r--   0        0        0      456 2024-04-23 15:36:48.000000 airbyte_source_gitlab-4.0.1/source_gitlab/utils.py
--rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 airbyte_source_gitlab-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4501 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/README.md
+-rw-r--r--   0        0        0      762 2024-05-07 12:21:48.136633 airbyte_source_gitlab-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/__init__.py
+-rw-r--r--   0        0        0     2054 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/components/partition_routers.py
+-rw-r--r--   0        0        0     3816 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/config_migrations.py
+-rw-r--r--   0        0        0    20615 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/manifest.yaml
+-rw-r--r--   0        0        0      403 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/run.py
+-rw-r--r--   0        0        0     1654 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/branches.json
+-rw-r--r--   0        0        0     3310 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/commits.json
+-rw-r--r--   0        0        0     9049 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/deployments.json
+-rw-r--r--   0        0        0     8831 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/epic_issues.json
+-rw-r--r--   0        0        0     5040 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/epics.json
+-rw-r--r--   0        0        0     3173 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/group_issue_boards.json
+-rw-r--r--   0        0        0     1627 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/group_labels.json
+-rw-r--r--   0        0        0     1261 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/group_members.json
+-rw-r--r--   0        0        0     1765 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/group_milestones.json
+-rw-r--r--   0        0        0     7472 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/groups.json
+-rw-r--r--   0        0        0    11629 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/issues.json
+-rw-r--r--   0        0        0     4326 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/jobs.json
+-rw-r--r--   0        0        0     3256 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/merge_request_commits.json
+-rw-r--r--   0        0        0     8440 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/merge_requests.json
+-rw-r--r--   0        0        0     1590 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/pipelines.json
+-rw-r--r--   0        0        0     4119 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/pipelines_extended.json
+-rw-r--r--   0        0        0     2089 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/project_labels.json
+-rw-r--r--   0        0        0     1263 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/project_members.json
+-rw-r--r--   0        0        0     1761 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/project_milestones.json
+-rw-r--r--   0        0        0    21255 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/projects.json
+-rw-r--r--   0        0        0     3144 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/releases.json
+-rw-r--r--   0        0        0     1439 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/tags.json
+-rw-r--r--   0        0        0      964 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/schemas/users.json
+-rw-r--r--   0        0        0     1093 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/source.py
+-rw-r--r--   0        0        0     6132 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/spec.json
+-rw-r--r--   0        0        0      456 2024-05-07 10:14:52.000000 airbyte_source_gitlab-4.0.2/source_gitlab/utils.py
+-rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 airbyte_source_gitlab-4.0.2/PKG-INFO
```

### Comparing `airbyte_source_gitlab-4.0.1/README.md` & `airbyte_source_gitlab-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/pyproject.toml` & `airbyte_source_gitlab-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.0.1"
+version = "4.0.2"
 name = "airbyte-source-gitlab"
 description = "Source implementation for GitLab."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_gitlab" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 vcrpy = "==4.1.1"
 
 [tool.poetry.scripts]
 source-gitlab = "source_gitlab.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.12.0"
```

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/__init__.py` & `airbyte_source_gitlab-4.0.2/source_gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/components/partition_routers.py` & `airbyte_source_gitlab-4.0.2/source_gitlab/components/partition_routers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/config_migrations.py` & `airbyte_source_gitlab-4.0.2/source_gitlab/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/manifest.yaml` & `airbyte_source_gitlab-4.0.2/source_gitlab/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/schemas/commits.json` & `airbyte_source_gitlab-4.0.2/source_gitlab/schemas/group_members.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8508230452674898%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'group_id': "*

 * *                 "OrderedDict([('type', ['null', 'integer'])]), 'name': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'username': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'state': OrderedDict([('type', ['null', 'string'])]), 'membership_state': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'avatar_url': OrderedDict([('type', "*

 * *                 "['null', 'str […]*

```diff
@@ -1,147 +1,114 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "author_email": {
+        "access_level": {
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "author_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "authored_date": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "committed_date": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "committer_email": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
-        "committer_name": {
+        "avatar_url": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "created_at": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "extended_trailers": {
-            "properties": {
-                "Cc": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                }
+        "created_by": {
+            "avatar_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
-            "type": [
-                "null",
-                "object"
-            ]
+            "id": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "name": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "state": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "username": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "web_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            }
         },
-        "id": {
+        "expires_at": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "message": {
+        "group_id": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "parent_ids": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "id": {
             "type": [
                 "null",
-                "array"
+                "integer"
             ]
         },
-        "project_id": {
+        "locked": {
             "type": [
                 "null",
-                "integer"
+                "boolean"
             ]
         },
-        "short_id": {
+        "membership_state": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "stats": {
-            "properties": {
-                "additions": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "deletions": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "total": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
-            },
+        "name": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "title": {
+        "state": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "trailers": {
+        "username": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
         "web_url": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/schemas/epics.json` & `airbyte_source_gitlab-4.0.2/source_gitlab/schemas/releases.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8469267139479905%*

 * *Differences: {"'properties'": "{'description': {'description': 'Description of the release'}, 'author': "*

 * *                 "{'description': 'Name of the author of the release'}, 'author_id': "*

 * *                 "{'description': 'ID of the author of the release'}, 'created_at': "*

 * *                 "{'description': 'Date and time when the release was created'}, '_links': "*

 * *                 "{'description': 'Links related to the releases data', delete: ['properties']}, "*

 * *                 "'name': OrderedDict([('description', […]*

```diff
@@ -1,251 +1,171 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
         "_links": {
+            "description": "Links related to the releases data",
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "assets": {
+            "description": "Information about assets related to the release",
             "properties": {
-                "epic_issues": {
+                "count": {
+                    "description": "Number of assets in the release",
                     "type": [
                         "null",
-                        "string"
+                        "integer"
                     ]
                 },
-                "group": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
+                "links": {
+                    "description": "Links related to the assets",
+                    "type": "array"
                 },
-                "parent": {
+                "sources": {
+                    "description": "List of sources for the assets",
+                    "items": {
+                        "properties": {
+                            "format": {
+                                "description": "Format of the asset",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            },
+                            "url": {
+                                "description": "URL of the asset file",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
+                        "type": "object"
+                    },
                     "type": [
                         "null",
-                        "string"
-                    ]
-                },
-                "self": {
-                    "type": [
-                        "null",
-                        "string"
+                        "array"
                     ]
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
         },
         "author": {
             "additionalProperties": true,
+            "description": "Name of the author of the release",
             "type": [
                 "null",
                 "object"
             ]
         },
         "author_id": {
+            "description": "ID of the author of the release",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "closed_at": {
-            "format": "date-time",
+        "commit": {
+            "additionalProperties": true,
+            "description": "Commit details related to the release",
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "color": {
+        "commit_id": {
+            "description": "ID of the commit related to the release",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "confidential": {
+        "commit_path": {
+            "description": "Path to the commit related to the release",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "created_at": {
+            "description": "Date and time when the release was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "description": {
+            "description": "Description of the release",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "downvotes": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "due_date": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "due_date_fixed": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "due_date_from_inherited_source": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "due_date_from_milestones": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "due_date_is_fixed": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "end_date": {
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
-        "iid": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "labels": {
+        "evidences": {
+            "description": "Any evidences associated with the release",
             "type": [
                 "null",
                 "array"
             ]
         },
-        "parent_id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "parent_iid": {
+        "milestones": {
+            "description": "List of milestones related to the release",
+            "items": {
+                "type": "integer"
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
-        "reference": {
+        "name": {
+            "description": "Name of the release",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "references": {
+        "project_id": {
+            "description": "ID of the project associated with the release",
             "type": [
                 "null",
-                "object"
+                "integer"
             ]
         },
-        "start_date": {
+        "released_at": {
+            "description": "Date and time when the release was published",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "start_date_fixed": {
-            "format": "date",
+        "tag_name": {
+            "description": "Name of the tag associated with the release",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "start_date_from_inherited_source": {
-            "type": [
-                "null",
-                "string",
-                "boolean"
-            ]
-        },
-        "start_date_from_milestones": {
-            "format": "date",
+        "tag_path": {
+            "description": "Path to the tag associated with the release",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "start_date_is_fixed": {
+        "upcoming_release": {
+            "description": "Indicator if the release is an upcoming release",
             "type": [
                 "null",
                 "boolean"
             ]
-        },
-        "state": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "text_color": {
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
-        "upvotes": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "web_edit_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "web_url": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/schemas/group_issue_boards.json` & `airbyte_source_gitlab-4.0.2/source_gitlab/schemas/project_members.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.850877192982456%*

 * *Differences: {"'properties'": "{'project_id': OrderedDict([('type', ['null', 'integer'])]), 'username': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'state': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'membership_state': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'avatar_url': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'web_url': OrderedDict([('type', ['null', 'string'])]), 'access_level': "*

 * *                 "OrderedDict([('type', ['nu […]*

```diff
@@ -1,138 +1,118 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "group": {
-            "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "web_url": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "access_level": {
             "type": [
                 "null",
-                "object"
+                "integer"
             ]
         },
-        "group_id": {
+        "avatar_url": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "hide_backlog_list": {
+        "created_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "hide_closed_list": {
+        "created_by": {
+            "avatar_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "id": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "name": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "state": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "username": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "web_url": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            }
+        },
+        "expires_at": {
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "id": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "lists": {
-            "items": {
-                "properties": {
-                    "id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "label": {
-                        "properties": {
-                            "color": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "description": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "description_html": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "id": {
-                                "type": [
-                                    "null",
-                                    "integer"
-                                ]
-                            },
-                            "name": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "text_color": {
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
-                    "position": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "locked": {
             "type": [
                 "null",
-                "array"
+                "boolean"
+            ]
+        },
+        "membership_state": {
+            "type": [
+                "null",
+                "string"
             ]
         },
         "name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "project": {
+        "project_id": {
             "type": [
                 "null",
                 "integer"
             ]
+        },
+        "state": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "username": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "web_url": {
+            "type": [
+                "null",
+                "string"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/schemas/tags.json` & `airbyte_source_gitlab-4.0.2/source_gitlab/schemas/users.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8422619047619048%*

 * *Differences: {"'properties'": "{'name': {'description': 'Full name of the user'}, 'id': "*

 * *                 "OrderedDict([('description', 'Unique identification number for the user'), "*

 * *                 "('type', ['null', 'integer'])]), 'username': OrderedDict([('description', "*

 * *                 "'Unique username chosen by the user'), ('type', ['null', 'string'])]), 'state': "*

 * *                 'OrderedDict([(\'description\', "Current state of the user\'s account (e.g., '*

 * *                 'active, blocked)"), (\'type\', [ […]*

```diff
@@ -1,68 +1,54 @@
 {
     "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
-        "commit": {
-            "additionalProperties": true,
+        "avatar_url": {
+            "description": "URL of the user's avatar image",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "commit_id": {
+        "id": {
+            "description": "Unique identification number for the user",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "message": {
+        "locked": {
+            "description": "Boolean flag indicating if the user's account is locked",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
         "name": {
+            "description": "Full name of the user",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "project_id": {
+        "state": {
+            "description": "Current state of the user's account (e.g., active, blocked)",
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "protected": {
-            "type": [
-                "null",
-                "boolean"
+                "string"
             ]
         },
-        "release": {
-            "properties": {
-                "description": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "tag_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "username": {
+            "description": "Unique username chosen by the user",
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "target": {
+        "web_url": {
+            "description": "URL of the user's profile page on the Gitlab platform",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": "object"
```

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/source.py` & `airbyte_source_gitlab-4.0.2/source_gitlab/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/source_gitlab/spec.json` & `airbyte_source_gitlab-4.0.2/source_gitlab/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_gitlab-4.0.1/PKG-INFO` & `airbyte_source_gitlab-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-gitlab
-Version: 4.0.1
+Version: 4.0.2
 Summary: Source implementation for GitLab.
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
 Requires-Dist: vcrpy (==4.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/gitlab
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Gitlab source connector
```

