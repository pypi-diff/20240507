# Comparing `tmp/todoist_api_python-2.1.3.tar.gz` & `tmp/todoist_api_python-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoist_api_python-2.1.3.tar", max compression
+gzip compressed data, was "todoist_api_python-2.1.4.tar", max compression
```

## Comparing `todoist_api_python-2.1.3.tar` & `todoist_api_python-2.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-08-15 15:11:00.047136 todoist_api_python-2.1.3/LICENSE
--rw-r--r--   0        0        0     2356 2023-08-15 15:11:00.047136 todoist_api_python-2.1.3/README.md
--rw-r--r--   0        0        0      984 2023-08-15 15:11:00.047136 todoist_api_python-2.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/__init__.py
--rw-r--r--   0        0        0     9394 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/api.py
--rw-r--r--   0        0        0     5595 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/api_async.py
--rw-r--r--   0        0        0     2002 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/authentication.py
--rw-r--r--   0        0        0     1103 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/endpoints.py
--rw-r--r--   0        0        0      645 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/headers.py
--rw-r--r--   0        0        0     1427 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/http_requests.py
--rw-r--r--   0        0        0    10870 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/models.py
--rw-r--r--   0        0        0        0 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/py.typed
--rw-r--r--   0        0        0      436 2023-08-15 15:11:00.051136 todoist_api_python-2.1.3/todoist_api_python/utils.py
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 todoist_api_python-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/LICENSE
+-rw-r--r--   0        0        0     2906 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/README.md
+-rw-r--r--   0        0        0     4880 2024-05-07 13:43:04.045588 todoist_api_python-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/__init__.py
+-rw-r--r--   0        0        0     9394 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/api.py
+-rw-r--r--   0        0        0     5595 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/api_async.py
+-rw-r--r--   0        0        0     2002 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/authentication.py
+-rw-r--r--   0        0        0     1103 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/endpoints.py
+-rw-r--r--   0        0        0      645 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/headers.py
+-rw-r--r--   0        0        0     1414 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/http_requests.py
+-rw-r--r--   0        0        0    11615 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/models.py
+-rw-r--r--   0        0        0        0 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/py.typed
+-rw-r--r--   0        0        0      436 2024-05-07 13:43:04.049588 todoist_api_python-2.1.4/todoist_api_python/utils.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 todoist_api_python-2.1.4/PKG-INFO
```

### Comparing `todoist_api_python-2.1.3/LICENSE` & `todoist_api_python-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/README.md` & `todoist_api_python-2.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,36 @@
     try:
         tasks = api.get_tasks()
         print(tasks)
     except Exception as error:
         print(error)
 ```
 
+Example of paginating through a completed project tasks:
+
+```python
+def get_all_completed_items(original_params: dict):
+    params = original_params.copy()
+    results = []
+
+    while True:
+        response = api.get_completed_items(**(params | {"limit": 100}))
+        results.append(response.items)
+
+        if not response.has_more:
+            break
+
+        params["cursor"] = response.next_cursor
+
+    # flatten the results
+    return [item for sublist in results for item in sublist]
+
+items = get_all_completed_items({"project_id": 123})
+```
+
 ### Documentation
 
 For more detailed reference documentation, have a look at the [API documentation with Python examples](https://developer.todoist.com/rest/v2/?python).
 
 ### Development
 
 To install Python dependencies:
```

### Comparing `todoist_api_python-2.1.3/todoist_api_python/api.py` & `todoist_api_python-2.1.4/todoist_api_python/api.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/todoist_api_python/api_async.py` & `todoist_api_python-2.1.4/todoist_api_python/api_async.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/todoist_api_python/authentication.py` & `todoist_api_python-2.1.4/todoist_api_python/authentication.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/todoist_api_python/endpoints.py` & `todoist_api_python-2.1.4/todoist_api_python/endpoints.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/todoist_api_python/headers.py` & `todoist_api_python-2.1.4/todoist_api_python/headers.py`

 * *Files identical despite different names*

### Comparing `todoist_api_python-2.1.3/todoist_api_python/http_requests.py` & `todoist_api_python-2.1.4/todoist_api_python/http_requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     url: str,
     token: str | None = None,
     data: Dict[str, Any] | None = None,
 ):
     request_id = data.pop("request_id", None) if data else None
 
     headers = create_headers(
-        token=token, with_content=True if data else False, request_id=request_id
+        token=token, with_content=bool(data), request_id=request_id
     )
 
     response = session.post(
         url,
         headers=headers,
         data=json.dumps(data) if data else None,
     )
```

### Comparing `todoist_api_python-2.1.3/todoist_api_python/models.py` & `todoist_api_python-2.1.4/todoist_api_python/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 from todoist_api_python.utils import get_url_for_task
 
 VIEW_STYLE = Literal["list", "board"]
 
 
 @dataclass
-class Project(object):
+class Project:
     color: str
     comment_count: int
     id: str
     is_favorite: bool
     is_inbox_project: bool
     is_shared: bool
     is_team_inbox: bool
+    can_assign_tasks: bool
     name: str
     order: int
     parent_id: str | None
     url: str
     view_style: VIEW_STYLE
 
     @classmethod
@@ -29,24 +30,25 @@
             color=obj["color"],
             comment_count=obj["comment_count"],
             id=obj["id"],
             is_favorite=obj["is_favorite"],
             is_inbox_project=obj.get("is_inbox_project"),
             is_shared=obj["is_shared"],
             is_team_inbox=obj.get("is_team_inbox"),
+            can_assign_tasks=obj["can_assign_tasks"],
             name=obj["name"],
             order=obj.get("order"),
             parent_id=obj.get("parent_id"),
             url=obj["url"],
             view_style=obj["view_style"],
         )
 
 
 @dataclass
-class Section(object):
+class Section:
     id: str
     name: str
     order: int
     project_id: str
 
     @classmethod
     def from_dict(cls, obj):
@@ -55,15 +57,15 @@
             name=obj["name"],
             order=obj["order"],
             project_id=obj["project_id"],
         )
 
 
 @dataclass
-class Due(object):
+class Due:
     date: str
     is_recurring: bool
     string: str
 
     datetime: str | None = None
     timezone: str | None = None
 
@@ -106,15 +108,15 @@
             string=due["string"],
             datetime=datetime,
             timezone=timezone,
         )
 
 
 @dataclass
-class Task(object):
+class Task:
     assignee_id: str | None
     assigner_id: str | None
     comment_count: int
     is_completed: bool
     content: str
     created_at: str
     creator_id: str
@@ -124,24 +126,29 @@
     labels: List[str]
     order: int
     parent_id: str | None
     priority: int
     project_id: str
     section_id: str | None
     url: str
+    duration: Duration | None
 
     sync_id: str | None = None
 
     @classmethod
     def from_dict(cls, obj):
         due: Due | None = None
+        duration: Duration | None = None
 
         if obj.get("due"):
             due = Due.from_dict(obj["due"])
 
+        if obj.get("duration"):
+            duration = Duration.from_dict(obj["duration"])
+
         return cls(
             assignee_id=obj.get("assignee_id"),
             assigner_id=obj.get("assigner_id"),
             comment_count=obj["comment_count"],
             is_completed=obj["is_completed"],
             content=obj["content"],
             created_at=obj["created_at"],
@@ -152,14 +159,15 @@
             labels=obj.get("labels"),
             order=obj.get("order"),
             parent_id=obj.get("parent_id"),
             priority=obj["priority"],
             project_id=obj["project_id"],
             section_id=obj["section_id"],
             url=obj["url"],
+            duration=duration
         )
 
     def to_dict(self):
         due: dict | None = None
 
         if self.due:
             due = self.due.to_dict()
@@ -179,33 +187,39 @@
             "order": self.order,
             "parent_id": self.parent_id,
             "priority": self.priority,
             "project_id": self.project_id,
             "section_id": self.section_id,
             "sync_id": self.sync_id,
             "url": self.url,
+            "duration": self.duration
         }
 
     @classmethod
     def from_quick_add_response(cls, obj):
         due: Due | None = None
+        duration: Duration | None = None
 
         if obj.get("due"):
             due = Due.from_quick_add_response(obj)
 
+        if obj.get("duration"):
+            duration = Duration.from_dict(obj["duration"])
+
         return cls(
             assignee_id=obj.get("responsible_uid"),
             assigner_id=obj.get("assigned_by_uid"),
             comment_count=0,
             is_completed=False,
             content=obj["content"],
             created_at=obj["added_at"],
             creator_id=obj["added_by_uid"],
             description=obj["description"],
             due=due,
+            duration=duration,
             id=obj["id"],
             labels=obj["labels"],
             order=obj["child_order"],
             parent_id=obj["parent_id"] or None,
             priority=obj["priority"],
             project_id=obj["project_id"],
             section_id=obj["section_id"] or None,
@@ -248,30 +262,30 @@
             resolved_assignee_name=resolved_assignee_name,
             resolved_label_names=list(obj["meta"]["labels"].values()),
             resolved_section_name=resolved_section_name,
         )
 
 
 @dataclass
-class Collaborator(object):
+class Collaborator:
     id: str
     email: str
     name: str
 
     @classmethod
     def from_dict(cls, obj):
         return cls(
             id=obj["id"],
             email=obj["email"],
             name=obj["name"],
         )
 
 
 @dataclass
-class Attachment(object):
+class Attachment:
     resource_type: str | None = None
 
     file_name: str | None = None
     file_size: int | None = None
     file_type: str | None = None
     file_url: str | None = None
     file_duration: int | None = None
@@ -298,15 +312,15 @@
             image_height=obj.get("image_height"),
             url=obj.get("url"),
             title=obj.get("title"),
         )
 
 
 @dataclass
-class Comment(object):
+class Comment:
     attachment: Attachment | None
     content: str
     id: str
     posted_at: str
     project_id: str | None
     task_id: str | None
 
@@ -417,7 +431,26 @@
             total=obj["total"],
             completed_info=[
                 ItemCompletedInfo.from_dict(v) for v in obj["completed_info"]
             ],
             has_more=obj["has_more"],
             next_cursor=obj.get("next_cursor"),
         )
+
+
+@dataclass
+class Duration(object):
+    amount: int
+    unit: str
+
+    @classmethod
+    def from_dict(cls, obj):
+        return cls(
+            amount=obj["amount"],
+            unit=obj["unit"],
+        )
+
+    def to_dict(self):
+        return {
+            "amount": self.amount,
+            "unit": self.unit,
+        }
```

### Comparing `todoist_api_python-2.1.3/PKG-INFO` & `todoist_api_python-2.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: todoist-api-python
-Version: 2.1.3
+Name: todoist_api_python
+Version: 2.1.4
 Summary: Official Python SDK for the Todoist REST API.
 Home-page: https://github.com/Doist/todoist-api-python
 License: MIT
 Keywords: todoist,rest,api,python
 Author: Doist Developers
 Author-email: dev@doist.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Documentation, https://developer.todoist.com/rest/
 Project-URL: Repository, https://github.com/Doist/todoist-api-python
 Description-Content-Type: text/markdown
 
 # Todoist API Python Client
@@ -61,14 +62,36 @@
     try:
         tasks = api.get_tasks()
         print(tasks)
     except Exception as error:
         print(error)
 ```
 
+Example of paginating through a completed project tasks:
+
+```python
+def get_all_completed_items(original_params: dict):
+    params = original_params.copy()
+    results = []
+
+    while True:
+        response = api.get_completed_items(**(params | {"limit": 100}))
+        results.append(response.items)
+
+        if not response.has_more:
+            break
+
+        params["cursor"] = response.next_cursor
+
+    # flatten the results
+    return [item for sublist in results for item in sublist]
+
+items = get_all_completed_items({"project_id": 123})
+```
+
 ### Documentation
 
 For more detailed reference documentation, have a look at the [API documentation with Python examples](https://developer.todoist.com/rest/v2/?python).
 
 ### Development
 
 To install Python dependencies:
```

