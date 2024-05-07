# Comparing `tmp/climb_onyx_client-4.4.0.tar.gz` & `tmp/climb_onyx_client-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climb_onyx_client-4.4.0.tar", last modified: Mon Apr 29 14:42:58 2024, max compression
+gzip compressed data, was "climb_onyx_client-4.5.0.tar", last modified: Tue May  7 15:00:40 2024, max compression
```

## Comparing `climb_onyx_client-4.4.0.tar` & `climb_onyx_client-4.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 14:42:58.000000 climb_onyx_client-4.4.0/climb_onyx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/onyx/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77753 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/onyx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:42:58.700443 climb_onyx_client-4.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    52657 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-29 14:42:54.000000 climb_onyx_client-4.4.0/tests/test_url_formation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 15:00:40.000000 climb_onyx_client-4.5.0/climb_onyx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/onyx/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79990 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36299 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/onyx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:00:40.575963 climb_onyx_client-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    56205 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-07 15:00:34.000000 climb_onyx_client-4.5.0/tests/test_url_formation.py
```

### Comparing `climb_onyx_client-4.4.0/LICENSE` & `climb_onyx_client-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/PKG-INFO` & `climb_onyx_client-4.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.4.0
+Version: 4.5.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -70,14 +70,15 @@
 │ fields      View the field specification for a project.                                   │
 │ choices     View options for a choice field in a project.                                 │
 │ get         Get a record from a project.                                                  │
 │ filter      Filter multiple records from a project.                                       │
 │ history     View the history of a record in a project.                                    │
 │ identify    Get the anonymised identifier for a value on a field.                         │
 │ profile     View profile information.                                                     │
+│ activity    View latest profile activity.                                                 │
 │ siteusers   View users from the same site.                                                │
 │ auth        Authentication commands.                                                      │
 │ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.4.0/README.md` & `climb_onyx_client-4.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 │ fields      View the field specification for a project.                                   │
 │ choices     View options for a choice field in a project.                                 │
 │ get         Get a record from a project.                                                  │
 │ filter      Filter multiple records from a project.                                       │
 │ history     View the history of a record in a project.                                    │
 │ identify    Get the anonymised identifier for a value on a field.                         │
 │ profile     View profile information.                                                     │
+│ activity    View latest profile activity.                                                 │
 │ siteusers   View users from the same site.                                                │
 │ auth        Authentication commands.                                                      │
 │ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.4.0/climb_onyx_client.egg-info/PKG-INFO` & `climb_onyx_client-4.5.0/climb_onyx_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.4.0
+Version: 4.5.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -70,14 +70,15 @@
 │ fields      View the field specification for a project.                                   │
 │ choices     View options for a choice field in a project.                                 │
 │ get         Get a record from a project.                                                  │
 │ filter      Filter multiple records from a project.                                       │
 │ history     View the history of a record in a project.                                    │
 │ identify    Get the anonymised identifier for a value on a field.                         │
 │ profile     View profile information.                                                     │
+│ activity    View latest profile activity.                                                 │
 │ siteusers   View users from the same site.                                                │
 │ auth        Authentication commands.                                                      │
 │ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.4.0/onyx/api.py` & `climb_onyx_client-4.5.0/onyx/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,21 @@
         "profile": lambda domain: OnyxClient._handle_endpoint(
             lambda: posixpath.join(
                 str(domain),
                 "accounts/profile/",
             ),
             domain=domain,
         ),
+        "activity": lambda domain: OnyxClient._handle_endpoint(
+            lambda: posixpath.join(
+                str(domain),
+                "accounts/activity/",
+            ),
+            domain=domain,
+        ),
         "waiting": lambda domain: OnyxClient._handle_endpoint(
             lambda: posixpath.join(
                 str(domain),
                 "accounts/waiting/",
             ),
             domain=domain,
         ),
@@ -477,25 +484,31 @@
         exclude: Union[List[str], str, None] = None,
         summarise: Union[List[str], str, None] = None,
         **kwargs: Any,
     ) -> Generator[requests.Response, Any, None]:
         if fields is None:
             fields = {}
 
+        for field, value in kwargs.items():
+            if type(value) in {list, tuple, set}:
+                value = ",".join(map(lambda x: str(x) if x is not None else "", value))
+            fields[field] = value
+
+        for field, value in fields.items():
+            if type(value) in {list, tuple, set}:
+                fields[field] = [v if v is not None else "" for v in value]
+            if value is None:
+                fields[field] = ""
+
         fields = fields | {
             "include": include,
             "exclude": exclude,
             "summarise": summarise,
         }
 
-        for field, value in kwargs.items():
-            if type(value) in {list, tuple, set}:
-                value = ",".join(map(lambda x: str(x) if x is not None else "", value))
-            fields[field] = value
-
         _next = OnyxClient.ENDPOINTS["filter"](self.config.domain, project)
 
         while _next is not None:
             response = self._request(
                 method="get",
                 url=_next,
                 params=fields,
@@ -780,14 +793,21 @@
     def profile(self) -> requests.Response:
         response = self._request(
             method="get",
             url=OnyxClient.ENDPOINTS["profile"](self.config.domain),
         )
         return response
 
+    def activity(self) -> requests.Response:
+        response = self._request(
+            method="get",
+            url=OnyxClient.ENDPOINTS["activity"](self.config.domain),
+        )
+        return response
+
     def approve(self, username: str) -> requests.Response:
         response = self._request(
             method="patch",
             url=OnyxClient.ENDPOINTS["approve"](self.config.domain, username),
         )
         return response
 
@@ -2348,14 +2368,64 @@
         """
 
         response = super().profile()
         response.raise_for_status()
         return response.json()["data"]
 
     @onyx_errors
+    def activity(self) -> List[Dict[str, Any]]:
+        """
+        View the user's latest activity.
+
+        Returns:
+            List of the user's latest activity.
+
+        Examples:
+            ```python
+            import os
+            from onyx import OnyxConfig, OnyxEnv, OnyxClient
+
+            config = OnyxConfig(
+                domain=os.environ[OnyxEnv.DOMAIN],
+                token=os.environ[OnyxEnv.TOKEN],
+            )
+
+            with OnyxClient(config) as client:
+                activity = client.activity()
+            ```
+            ```python
+            >>> activity
+            [
+                {
+                    "date": "2023-01-01T00:00:00.000000Z",
+                    "address": "127.0.0.1",
+                    "endpoint": "/projects/project/",
+                    "method": "POST",
+                    "status": 400,
+                    "exec_time": 29,
+                    "error_messages" : "b'{\"status\":\"fail\",\"code\":400,\"messages\":{\"site\":[\"Select a valid choice.\"]}}'",
+                },
+                {
+                    "timestamp": "2023-01-02T00:00:00.000000Z",
+                    "address": "127.0.0.1",
+                    "endpoint": "/accounts/activity/",
+                    "method": "GET",
+                    "status": 200,
+                    "exec_time": 22,
+                    "error_messages": "",
+                },
+            ]
+            ```
+        """
+
+        response = super().activity()
+        response.raise_for_status()
+        return response.json()["data"]
+
+    @onyx_errors
     def approve(self, username: str) -> Dict[str, Any]:
         """
         Approve another user.
 
         Args:
             username: Username of the user to be approved.
```

### Comparing `climb_onyx_client-4.4.0/onyx/cli.py` & `climb_onyx_client-4.5.0/onyx/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import csv
 import sys
+import ast
 import enum
 import json
 import dataclasses
 from typing import Optional, List, Dict, Any
+import http.client
 import click
 import typer
 from typer.core import TyperGroup
 from rich.console import Console
 from rich.table import Table
 from .version import __version__
 from .config import OnyxConfig, OnyxEnv
@@ -161,15 +163,15 @@
     """
 
     table = Table(
         show_lines=True,
     )
 
     for column in map.keys():
-        table.add_column(column)
+        table.add_column(column, overflow="fold")
 
     for row in data:
         table.add_row(*(str(row.get(key, "")) for key in map.values()))
 
     return table
 
 
@@ -254,25 +256,36 @@
     OPTIONAL = "[bold cyan]optional[/]"
 
 
 class Actions(enum.Enum):
     GET = "[bold cyan]get[/]"
     LIST = "[bold blue]list[/]"
     FILTER = "[bold magenta]filter[/]"
+    HISTORY = "[bold yellow]history[/]"
     IDENTIFY = "[bold white]identify[/]"
     ADD = "[bold green]add[/]"
     CHANGE = "[bold yellow]change[/]"
     DELETE = "[bold red]delete[/]"
 
 
 class ActiveStatus(enum.Enum):
     ACTIVE = "[bold green]active[/]"
     INACTIVE = "[bold red]inactive[/]"
 
 
+class Method(enum.Enum):
+    GET = "[bold cyan]GET[/]"
+    POST = "[bold green]POST[/]"
+    PUT = "[bold blue]PUT[/]"
+    PATCH = "[bold yellow]PATCH[/]"
+    DELETE = "[bold red]DELETE[/]"
+    OPTIONS = "[bold magenta]OPTIONS[/]"
+    HEAD = "[bold white]HEAD[/]"
+
+
 def format_action(action: str) -> str:
     """
     Format an action and apply its colour.
 
     Args:
         action: The action to format.
 
@@ -283,26 +296,90 @@
     match action:
         case "get":
             return Actions.GET.value
         case "list":
             return Actions.LIST.value
         case "filter":
             return Actions.FILTER.value
+        case "history":
+            return Actions.HISTORY.value
         case "identify":
             return Actions.IDENTIFY.value
         case "add":
             return Actions.ADD.value
         case "change":
             return Actions.CHANGE.value
         case "delete":
             return Actions.DELETE.value
         case _:
             return action
 
 
+def format_status_code(status: Optional[int]) -> str:
+    """
+    Format a status code, apply its colour and add a description of the status.
+
+    Args:
+        status: The status to format.
+
+    Returns:
+        The formatted status.
+    """
+
+    if status is None:
+        return ""
+
+    status_str = f"{status} ({http.client.responses[status]})"
+
+    if status_str.startswith("2"):
+        return f"[bold green]{status_str}[/]"
+
+    elif status_str.startswith("3"):
+        return f"[bold cyan]{status_str}[/]"
+
+    elif status_str.startswith("4"):
+        return f"[bold yellow]{status_str}[/]"
+
+    elif status_str.startswith("5"):
+        return f"[bold red]{status_str}[/]"
+
+    else:
+        return status_str
+
+
+def format_method(method: str) -> str:
+    """
+    Format a method and apply its colour.
+
+    Args:
+        method: The method to format.
+
+    Returns:
+        The formatted method.
+    """
+
+    match method:
+        case "GET":
+            return Method.GET.value
+        case "POST":
+            return Method.POST.value
+        case "PUT":
+            return Method.PUT.value
+        case "PATCH":
+            return Method.PATCH.value
+        case "DELETE":
+            return Method.DELETE.value
+        case "OPTIONS":
+            return Method.OPTIONS.value
+        case "HEAD":
+            return Method.HEAD.value
+        case _:
+            return method
+
+
 @app.command()
 def projects(
     context: typer.Context,
     format: Optional[InfoFormats] = typer.Option(
         InfoFormats.TABLE.value,
         "-F",
         "--format",
@@ -320,15 +397,15 @@
         if format == InfoFormats.TABLE:
             columns = ["Project", "Scope", "Actions"]
             table = Table(
                 show_lines=True,
             )
 
             for column in columns:
-                table.add_column(column)
+                table.add_column(column, overflow="fold")
 
             for project in projects:
                 table.add_row(
                     project.get("project", ""),
                     project.get("scope", ""),
                     " | ".join(
                         [format_action(action) for action in project.get("actions", [])]
@@ -363,15 +440,15 @@
         if format == InfoFormats.TABLE:
             columns = ["Type", "Description", "Lookups"]
             table = Table(
                 show_lines=True,
             )
 
             for column in columns:
-                table.add_column(column)
+                table.add_column(column, overflow="fold")
 
             for t in types:
                 table.add_row(
                     t.get("type", ""),
                     t.get("description", ""),
                     " | ".join(t.get("lookups", [])),
                 )
@@ -404,15 +481,15 @@
         if format == InfoFormats.TABLE:
             columns = ["Lookup", "Description", "Types"]
             table = Table(
                 show_lines=True,
             )
 
             for column in columns:
-                table.add_column(column)
+                table.add_column(column, overflow="fold")
 
             for lookup in lookups:
                 table.add_row(
                     lookup.get("lookup", ""),
                     lookup.get("description", ""),
                     " | ".join(lookup.get("types", [])),
                 )
@@ -628,17 +705,17 @@
         field = parse_extra_option([field])[0]
         choices = api.client.choices(project, field)
 
         if format == InfoFormats.TABLE:
             table = Table(
                 show_lines=True,
             )
-            table.add_column("Choice")
-            table.add_column("Description")
-            table.add_column("Status")
+            table.add_column("Choice", overflow="fold")
+            table.add_column("Description", overflow="fold")
+            table.add_column("Status", overflow="fold")
             for choice, choice_info in choices.items():
                 active_status = choice_info.get("is_active")
                 if active_status == True:
                     active_status = ActiveStatus.ACTIVE.value
                 elif active_status == False:
                     active_status = ActiveStatus.INACTIVE.value
                 else:
@@ -853,15 +930,15 @@
         history = api.client.history(project, climb_id)
 
         if format == InfoFormats.TABLE:
             columns = ["Username", "Timestamp", "Action", "Changes"]
 
             table = Table(show_lines=True)
             for column in columns:
-                table.add_column(column)
+                table.add_column(column, overflow="fold")
 
             actions = {
                 "add": "added",
                 "change": "changed",
                 "delete": "deleted",
             }
 
@@ -976,14 +1053,69 @@
         else:
             typer.echo(json_dump_pretty(user))
     except Exception as e:
         handle_error(e)
 
 
 @app.command()
+def activity(
+    context: typer.Context,
+    format: Optional[InfoFormats] = typer.Option(
+        InfoFormats.TABLE.value,
+        "-F",
+        "--format",
+        help=HelpText.FORMAT.value,
+    ),
+):
+    """
+    View latest profile activity.
+    """
+
+    try:
+        api = setup_onyx_api(context.obj)
+        activity = api.client.activity()
+
+        if format == InfoFormats.TABLE:
+            columns = [
+                "Address",
+                "Timestamp",
+                "Method",
+                "Endpoint",
+                "Status Code",
+                "Execution Time (ms)",
+                "Errors",
+            ]
+
+            table = Table(show_lines=True)
+            for column in columns:
+                table.add_column(column, overflow="fold")
+
+            for a in activity:
+                errors = a.get("error_messages", "")
+                if errors:
+                    errors = json_dump_pretty(json.loads(ast.literal_eval(errors)))
+
+                table.add_row(
+                    a.get("address", ""),
+                    a.get("date", ""),
+                    format_method(a.get("method", "")),
+                    a.get("endpoint", ""),
+                    format_status_code(a.get("status")),
+                    str(a.get("exec_time", "")),
+                    errors,
+                )
+
+            console.print(table)
+        else:
+            typer.echo(json_dump_pretty(activity))
+    except Exception as e:
+        handle_error(e)
+
+
+@app.command()
 def siteusers(
     context: typer.Context,
     format: Optional[InfoFormats] = typer.Option(
         InfoFormats.TABLE.value,
         "-F",
         "--format",
         help=HelpText.FORMAT.value,
```

### Comparing `climb_onyx_client-4.4.0/onyx/config.py` & `climb_onyx_client-4.5.0/onyx/config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/onyx/exceptions.py` & `climb_onyx_client-4.5.0/onyx/exceptions.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/onyx/field.py` & `climb_onyx_client-4.5.0/onyx/field.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/setup.py` & `climb_onyx_client-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/tests/test_api.py` & `climb_onyx_client-4.5.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,43 @@
             "climb_id": CLIMB_ID,
             "published_date": "2023-09-18",
             "sample_id": "sample-abc",
         },
     ],
 }
 UNKNOWN_FIELD = "haha"
+NONE_FIELD = "field-that-has-none-values"
+FILTER_NONE_DATA = {
+    "status": "success",
+    "code": 200,
+    "next": None,
+    "previous": None,
+    "data": [
+        {
+            "climb_id": CLIMB_ID,
+            NONE_FIELD: None,
+        }
+    ],
+}
+FILTER_NONE_IN_DATA = {
+    "status": "success",
+    "code": 200,
+    "next": None,
+    "previous": None,
+    "data": [
+        {
+            "climb_id": CLIMB_ID,
+            NONE_FIELD: None,
+        },
+        {
+            "climb_id": CLIMB_ID,
+            NONE_FIELD: "not-none",
+        },
+    ],
+}
 FILTER_UNKNOWN_FIELD_DATA = {
     "status": "fail",
     "code": 400,
     "messages": {UNKNOWN_FIELD: ["This field is unknown."]},
 }
 FILTER_ERROR_CAUSING_PROJECT_DATA = {
     "status": "fail",
@@ -502,14 +531,38 @@
     "code": 200,
     "data": {
         "username": USERNAME,
         "email": EMAIL,
         "site": SITE,
     },
 }
+ACTIVITY_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": [
+        {
+            "date": "2023-01-01T00:00:00.000000Z",
+            "address": "127.0.0.1",
+            "endpoint": "/projects/project/",
+            "method": "POST",
+            "status": 400,
+            "exec_time": 29,
+            "error_messages": 'b\'{"status":"fail","code":400,"messages":{"site":["Select a valid choice."]}}\'',
+        },
+        {
+            "timestamp": "2023-01-02T00:00:00.000000Z",
+            "address": "127.0.0.1",
+            "endpoint": "/accounts/activity/",
+            "method": "GET",
+            "status": 200,
+            "exec_time": 22,
+            "error_messages": "",
+        },
+    ],
+}
 WAITING_DATA = {
     "status": "success",
     "code": 200,
     "data": [
         {
             "username": OTHER_USERNAME,
             "email": OTHER_EMAIL,
@@ -681,14 +734,18 @@
 
         elif url == OnyxClient.ENDPOINTS["get"](DOMAIN, PROJECT, CLIMB_ID):
             return MockResponse(GET_DATA)
 
         elif url == OnyxClient.ENDPOINTS["filter"](DOMAIN, PROJECT):
             if params.get(UNKNOWN_FIELD):
                 return MockResponse(FILTER_UNKNOWN_FIELD_DATA)
+            elif params.get(NONE_FIELD) == "":
+                return MockResponse(FILTER_NONE_DATA)
+            elif "" in params.get(f"{NONE_FIELD}__in", []):
+                return MockResponse(FILTER_NONE_IN_DATA)
             elif (
                 params.get("sample_id") == SAMPLE_ID
                 and params.get("run_name") == RUN_NAME
                 and params.get("published_date__range")
                 == ",".join(PUBLISHED_DATE_RANGE)
             ):
                 if params.get("include") == INCLUDE_FIELDS:
@@ -708,14 +765,17 @@
 
         elif url == OnyxClient.ENDPOINTS["history"](DOMAIN, PROJECT, CLIMB_ID):
             return MockResponse(HISTORY_DATA)
 
         elif url == OnyxClient.ENDPOINTS["profile"](DOMAIN):
             return MockResponse(PROFILE_DATA)
 
+        elif url == OnyxClient.ENDPOINTS["activity"](DOMAIN):
+            return MockResponse(ACTIVITY_DATA)
+
         elif url == OnyxClient.ENDPOINTS["waiting"](DOMAIN):
             return MockResponse(WAITING_DATA)
 
         elif url == OnyxClient.ENDPOINTS["siteusers"](DOMAIN):
             return MockResponse(SITE_USERS_DATA)
 
         elif url == OnyxClient.ENDPOINTS["allusers"](DOMAIN):
@@ -1054,14 +1114,61 @@
                         "published_date__range": ",".join(PUBLISHED_DATE_RANGE),
                     },
                     exclude=EXCLUDE_FIELDS,
                 )
             ],
             FILTER_SPECIFIC_EXCLUDE_DATA["data"],
         )
+        for empty in ["", None]:
+            self.assertEqual(
+                [
+                    x
+                    for x in self.client.filter(
+                        PROJECT,
+                        fields={
+                            NONE_FIELD: empty,
+                        },
+                    )
+                ],
+                FILTER_NONE_DATA["data"],
+            )
+            self.assertEqual(
+                [
+                    x
+                    for x in self.client.filter(
+                        **{"project": PROJECT, NONE_FIELD: empty},
+                    )
+                ],
+                FILTER_NONE_DATA["data"],
+            )
+            for type_ in [list, tuple, set]:
+                self.assertEqual(
+                    [
+                        x
+                        for x in self.client.filter(
+                            PROJECT,
+                            fields={
+                                f"{NONE_FIELD}__in": type_([empty, "not-empty"]),
+                            },
+                        )
+                    ],
+                    FILTER_NONE_IN_DATA["data"],
+                )
+                self.assertEqual(
+                    [
+                        x
+                        for x in self.client.filter(
+                            **{
+                                "project": PROJECT,
+                                f"{NONE_FIELD}__in": type_([empty, "not-empty"]),
+                            },
+                        )
+                    ],
+                    FILTER_NONE_IN_DATA["data"],
+                )
         self.assertEqual(self.config.token, TOKEN)
 
         for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 [x for x in self.client.filter(invalid)]
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
@@ -1644,14 +1751,23 @@
         Test that the OnyxClient can retrieve the user profile.
         """
 
         self.assertEqual(self.client.profile(), PROFILE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_activity(self, mock_request):
+        """
+        Test that the OnyxClient can retrieve the user's latest activity.
+        """
+
+        self.assertEqual(self.client.activity(), ACTIVITY_DATA["data"])
+        self.assertEqual(self.config.token, TOKEN)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_approve(self, mock_request):
         """
         Test that the OnyxClient can approve a user.
         """
 
         self.assertEqual(self.client.approve(OTHER_USERNAME), APPROVE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
```

### Comparing `climb_onyx_client-4.4.0/tests/test_config.py` & `climb_onyx_client-4.5.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/tests/test_field.py` & `climb_onyx_client-4.5.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.4.0/tests/test_url_formation.py` & `climb_onyx_client-4.5.0/tests/test_url_formation.py`

 * *Files identical despite different names*

