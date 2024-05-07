# Comparing `tmp/tenb2jira-2.0.0.dev0.tar.gz` & `tmp/tenb2jira-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenb2jira-2.0.0.dev0.tar", last modified: Fri Apr 26 15:10:39 2024, max compression
+gzip compressed data, was "tenb2jira-2.0.1.tar", last modified: Tue May  7 17:08:24 2024, max compression
```

## Comparing `tenb2jira-2.0.0.dev0.tar` & `tenb2jira-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.182614 tenb2jira-2.0.0.dev0/
--rw-r--r--   0 steve      (501) staff       (20)    11228 2024-04-26 15:10:39.182387 tenb2jira-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     9934 2024-04-25 19:49:39.000000 tenb2jira-2.0.0.dev0/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1685 2024-04-26 15:08:52.000000 tenb2jira-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-26 15:10:39.182657 tenb2jira-2.0.0.dev0/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.177330 tenb2jira-2.0.0.dev0/tenb2jira/
--rw-r--r--   0 steve      (501) staff       (20)       81 2024-04-25 20:00:29.000000 tenb2jira-2.0.0.dev0/tenb2jira/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     5065 2024-04-25 19:43:44.000000 tenb2jira-2.0.0.dev0/tenb2jira/cli.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.178984 tenb2jira-2.0.0.dev0/tenb2jira/jira/
--rw-r--r--   0 steve      (501) staff       (20)        0 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.180801 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/
--rw-r--r--   0 steve      (501) staff       (20)        0 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      872 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/fields.py
--rw-r--r--   0 steve      (501) staff       (20)     2176 2024-04-05 19:01:51.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/issues.py
--rw-r--r--   0 steve      (501) staff       (20)      624 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/issuetypes.py
--rw-r--r--   0 steve      (501) staff       (20)     1224 2024-04-05 23:05:10.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/iterator.py
--rw-r--r--   0 steve      (501) staff       (20)     1296 2024-04-05 23:35:20.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/projects.py
--rw-r--r--   0 steve      (501) staff       (20)     2312 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/screens.py
--rw-r--r--   0 steve      (501) staff       (20)      727 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/api/session.py
--rw-r--r--   0 steve      (501) staff       (20)     6990 2024-04-16 18:15:49.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/field.py
--rw-r--r--   0 steve      (501) staff       (20)     6938 2024-04-18 16:48:09.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/jira.py
--rw-r--r--   0 steve      (501) staff       (20)     5391 2024-04-15 22:23:00.000000 tenb2jira-2.0.0.dev0/tenb2jira/jira/task.py
--rw-r--r--   0 steve      (501) staff       (20)     1694 2024-04-16 21:19:54.000000 tenb2jira-2.0.0.dev0/tenb2jira/models.py
--rw-r--r--   0 steve      (501) staff       (20)    19287 2024-04-25 19:48:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/processor.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.181350 tenb2jira-2.0.0.dev0/tenb2jira/tenable/
--rw-r--r--   0 steve      (501) staff       (20)        0 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/tenable/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     5613 2024-04-16 19:30:10.000000 tenb2jira-2.0.0.dev0/tenb2jira/tenable/generators.py
--rw-r--r--   0 steve      (501) staff       (20)     4734 2024-04-25 20:05:10.000000 tenb2jira-2.0.0.dev0/tenb2jira/tenable/tenable.py
--rw-r--r--   0 steve      (501) staff       (20)     2606 2024-03-21 18:21:16.000000 tenb2jira-2.0.0.dev0/tenb2jira/validator.py
--rw-r--r--   0 steve      (501) staff       (20)       85 2024-04-26 15:10:34.000000 tenb2jira-2.0.0.dev0/tenb2jira/version.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.182157 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    11228 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      827 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       48 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      123 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       10 2024-04-26 15:10:39.000000 tenb2jira-2.0.0.dev0/tenb2jira.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 15:10:39.181871 tenb2jira-2.0.0.dev0/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1205 2024-04-25 20:01:35.000000 tenb2jira-2.0.0.dev0/tests/test_models.py
--rw-r--r--   0 steve      (501) staff       (20)     3927 2024-04-25 20:06:15.000000 tenb2jira-2.0.0.dev0/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.984754 tenb2jira-2.0.1/tenb2jira/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.984754 tenb2jira-2.0.1/tenb2jira/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira/jira/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/issuetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/jira/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira/tenable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/tenable/tenable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tenb2jira/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tenb2jira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:08:24.000000 tenb2jira-2.0.1/tenb2jira.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:08:24.988754 tenb2jira-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 17:08:20.000000 tenb2jira-2.0.1/tests/test_processor.py
```

### Comparing `tenb2jira-2.0.0.dev0/PKG-INFO` & `tenb2jira-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.0.dev0
+Version: 2.0.1
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.0.dev0/README.md` & `tenb2jira-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/pyproject.toml` & `tenb2jira-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/cli.py` & `tenb2jira-2.0.1/tenb2jira/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Validates the configuration file
     """
     with open(configfile, 'r', encoding='utf-8') as f:
         config = tomlkit.load(f)
     errors = validator.validate(config)
     if errors:
         for error in errors:
-            location = '.'.join(error.get('loc', []))
+            location = '.'.join([str(e) for e in error.get('loc', [])])
             data = tomlkit.dumps(error.get('input'))
             console.print(f'{location}: {error.get("msg")}')
             console.print(data)
         raise typer.Exit(code=1)
     console.print('Configuration loaded: OK')
```

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/fields.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/fields.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/issues.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/issues.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/issuetypes.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/issuetypes.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/iterator.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/iterator.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/projects.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/projects.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/screens.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/screens.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/api/session.py` & `tenb2jira-2.0.1/tenb2jira/jira/api/session.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/field.py` & `tenb2jira-2.0.1/tenb2jira/jira/field.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/jira.py` & `tenb2jira-2.0.1/tenb2jira/jira/jira.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/jira/task.py` & `tenb2jira-2.0.1/tenb2jira/jira/task.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/models.py` & `tenb2jira-2.0.1/tenb2jira/models.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/processor.py` & `tenb2jira-2.0.1/tenb2jira/processor.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/tenable/generators.py` & `tenb2jira-2.0.1/tenb2jira/tenable/generators.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/tenable/tenable.py` & `tenb2jira-2.0.1/tenb2jira/tenable/tenable.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira/validator.py` & `tenb2jira-2.0.1/tenb2jira/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import List, Dict, Optional
 from enum import Enum
 from pydantic import BaseModel, Field, ValidationError
 
 
-class Platform(Enum):
-    tvm = 'tvm'
-    tsc = 'tsc'
+class Platform(str, Enum):
+    tvm: str = 'tvm'
+    tsc: str = 'tsc'
 
 
-class Severity(Enum):
+class Severity(str, Enum):
     critical = 'critical'
     high = 'high'
     medium = 'medium'
     low = 'low'
 
 
-class TaskType(Enum):
-    task = 'task'
-    subtask = 'subtask'
+class TaskType(str, Enum):
+    task: str = 'task'
+    subtask: str = 'subtask'
 
 
-class State(Enum):
+class State(str, Enum):
     open = 'open'
     reopened = 'reopened'
     fixed = 'fixed'
 
 
 class JiraParagraph(BaseModel):
     name: str
     attr: str
 
 
-class JiraDescription(BaseModel):
+class JiraDescription(BaseModel, use_enum_values=True):
     tvm: List[JiraParagraph]
     tsc: List[JiraParagraph]
 
 
 class SeverityMap(BaseModel):
     critical: int
     high: int
     medium: int
     low: int
 
 
-class JiraField(BaseModel):
+class JiraField(BaseModel, use_enum_values=True):
     id: Optional[str] = None
     name: str
     screen_tab: str
     type: str
     searcher: str
     attr: Optional[Dict[Platform, str]] = None
     description: Optional[str] = None
     task_types: List[TaskType]
     map_to_priority: Optional[bool] = None
     platform_id: Optional[bool] = None
     static_value: Optional[str] = None
 
 
-class JiraTask(BaseModel):
+class JiraTask(BaseModel, use_enum_values=True):
     id: Optional[int] = None
     name: str
     type: str
     search: Dict[Platform, List[str]]
     summary: Dict[Platform, str]
     description: JiraDescription
 
@@ -73,27 +73,27 @@
     description: str
     url: str
     assignee: str
     type_key: str
     template_key: str
 
 
-class Jira(BaseModel):
+class Jira(BaseModel, use_enum_values=True):
     api_token: str
     api_username: str
     url: str
     closed: str
     closed_map: List[str]
     state_map: Dict[State, bool]
     severity_map: Dict[Severity, int]
     project: JiraProject
     fields: List[JiraField]
 
 
-class Tenable(BaseModel):
+class Tenable(BaseModel, use_enum_values=True):
     platform: Platform
     access_key: str
     secret_key: str
     url: str
     port: Optional[int] = 443
     severities: List[Severity]
     vuln_age: Optional[int] = 30
@@ -102,15 +102,15 @@
     platforms: Dict[Platform, str]
 
 
 class MappingDatabase(BaseModel):
     path: str
 
 
-class Configuration(BaseModel):
+class Configuration(BaseModel, use_enum_values=True):
     tenable: Tenable
     jira: Jira
     mapping_database: MappingDatabase
 
 
 def validate(config: dict) -> dict:
     """
```

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira.egg-info/PKG-INFO` & `tenb2jira-2.0.1/tenb2jira.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.0.dev0
+Version: 2.0.1
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.0.dev0/tenb2jira.egg-info/SOURCES.txt` & `tenb2jira-2.0.1/tenb2jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tests/test_models.py` & `tenb2jira-2.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.0.dev0/tests/test_processor.py` & `tenb2jira-2.0.1/tests/test_processor.py`

 * *Files identical despite different names*

