# Comparing `tmp/zpodcli-0.6.0.tar.gz` & `tmp/zpodcli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpodcli-0.6.0.tar", max compression
+gzip compressed data, was "zpodcli-0.6.1.tar", max compression
```

## Comparing `zpodcli-0.6.0.tar` & `zpodcli-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      519 2024-03-13 14:21:21.635846 zpodcli-0.6.0/README.md
--rw-r--r--   0        0        0      613 2024-04-30 17:04:56.153887 zpodcli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-30 17:04:45.121879 zpodcli-0.6.0/src/zpodcli/__init__.py
--rw-r--r--   0        0        0     4595 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/component_cli.py
--rw-r--r--   0        0        0    13037 2024-04-30 16:57:22.313577 zpodcli-0.6.0/src/zpodcli/cmd/endpoint_cli.py
--rw-r--r--   0        0        0     5184 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/endpoint_permission_cli.py
--rw-r--r--   0        0        0     2548 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/enet_cli.py
--rw-r--r--   0        0        0     5367 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/factory_cli.py
--rw-r--r--   0        0        0     5160 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/library_cli.py
--rw-r--r--   0        0        0     3272 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/permission_group_cli.py
--rw-r--r--   0        0        0     1960 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/permission_group_user_cli.py
--rw-r--r--   0        0        0     7518 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/profile_cli.py
--rw-r--r--   0        0        0     2128 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/setting_cli.py
--rw-r--r--   0        0        0     5447 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/user_cli.py
--rw-r--r--   0        0        0     5243 2024-03-20 17:51:37.453853 zpodcli-0.6.0/src/zpodcli/cmd/zpod_cli.py
--rw-r--r--   0        0        0     5419 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/zpod_component_cli.py
--rw-r--r--   0        0        0     5611 2024-03-20 17:51:37.453853 zpodcli-0.6.0/src/zpodcli/cmd/zpod_permission_cli.py
--rw-r--r--   0        0        0     2409 2024-03-19 13:51:03.280476 zpodcli-0.6.0/src/zpodcli/lib/factory_config.py
--rw-r--r--   0        0        0      624 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/file.py
--rw-r--r--   0        0        0       40 2024-03-12 19:29:59.732397 zpodcli-0.6.0/src/zpodcli/lib/global_flags.py
--rw-r--r--   0        0        0     1006 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/prompt.py
--rw-r--r--   0        0        0      422 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/utils.py
--rw-r--r--   0        0        0     2696 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/zpod_client.py
--rw-r--r--   0        0        0     1750 2024-03-20 17:51:37.545861 zpodcli-0.6.0/src/zpodcli/main_cli.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 zpodcli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      519 2024-03-13 08:43:24.396297 zpodcli-0.6.1/README.md
+-rw-r--r--   0        0        0      613 2024-05-07 14:59:38.873962 zpodcli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 14:59:28.101945 zpodcli-0.6.1/src/zpodcli/__init__.py
+-rw-r--r--   0        0        0     4593 2024-05-05 19:39:36.243422 zpodcli-0.6.1/src/zpodcli/cmd/component_cli.py
+-rw-r--r--   0        0        0    13065 2024-05-05 19:43:52.323578 zpodcli-0.6.1/src/zpodcli/cmd/endpoint_cli.py
+-rw-r--r--   0        0        0     5148 2024-05-05 19:43:54.683579 zpodcli-0.6.1/src/zpodcli/cmd/endpoint_permission_cli.py
+-rw-r--r--   0        0        0     2529 2024-05-05 19:45:17.779630 zpodcli-0.6.1/src/zpodcli/cmd/enet_cli.py
+-rw-r--r--   0        0        0     5642 2024-05-05 19:46:16.203665 zpodcli-0.6.1/src/zpodcli/cmd/factory_cli.py
+-rw-r--r--   0        0        0     5098 2024-05-05 19:49:02.323766 zpodcli-0.6.1/src/zpodcli/cmd/library_cli.py
+-rw-r--r--   0        0        0     3353 2024-05-05 19:52:20.355886 zpodcli-0.6.1/src/zpodcli/cmd/permission_group_cli.py
+-rw-r--r--   0        0        0     1960 2024-05-05 18:46:07.341508 zpodcli-0.6.1/src/zpodcli/cmd/permission_group_user_cli.py
+-rw-r--r--   0        0        0     7552 2024-05-05 19:54:59.111981 zpodcli-0.6.1/src/zpodcli/cmd/profile_cli.py
+-rw-r--r--   0        0        0     2139 2024-05-05 19:55:56.864016 zpodcli-0.6.1/src/zpodcli/cmd/setting_cli.py
+-rw-r--r--   0        0        0     5496 2024-05-05 19:57:56.304088 zpodcli-0.6.1/src/zpodcli/cmd/user_cli.py
+-rw-r--r--   0        0        0     5294 2024-05-05 19:59:43.624153 zpodcli-0.6.1/src/zpodcli/cmd/zpod_cli.py
+-rw-r--r--   0        0        0     5407 2024-05-05 20:01:30.476217 zpodcli-0.6.1/src/zpodcli/cmd/zpod_component_cli.py
+-rw-r--r--   0        0        0     5588 2024-05-05 20:04:15.956317 zpodcli-0.6.1/src/zpodcli/cmd/zpod_permission_cli.py
+-rw-r--r--   0        0        0     2416 2024-05-05 20:04:49.816337 zpodcli-0.6.1/src/zpodcli/lib/factory_config.py
+-rw-r--r--   0        0        0      624 2024-04-15 14:55:56.813893 zpodcli-0.6.1/src/zpodcli/lib/file.py
+-rw-r--r--   0        0        0       58 2024-05-05 12:45:32.862134 zpodcli-0.6.1/src/zpodcli/lib/global_flags.py
+-rw-r--r--   0        0        0     1006 2024-04-19 12:09:34.477070 zpodcli-0.6.1/src/zpodcli/lib/prompt.py
+-rw-r--r--   0        0        0      844 2024-05-05 19:39:17.015410 zpodcli-0.6.1/src/zpodcli/lib/utils.py
+-rw-r--r--   0        0        0     2696 2024-04-15 14:55:56.813893 zpodcli-0.6.1/src/zpodcli/lib/zpod_client.py
+-rw-r--r--   0        0        0     1969 2024-05-05 20:07:37.896438 zpodcli-0.6.1/src/zpodcli/main_cli.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 zpodcli-0.6.1/PKG-INFO
```

### Comparing `zpodcli-0.6.0/README.md` & `zpodcli-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zpodcli-0.6.0/pyproject.toml` & `zpodcli-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "zpodcli"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Timo Sugliani <timo.sugliani@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "zpodcli", from = "src"}]
 
 [tool.poetry.scripts]
 zcli = "zpodcli.main_cli:launch"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.6.3"
 typer = {extras = ["all"], version = "0.10.0"}
 #zpodsdk = {path = "../zpodsdk", develop = true}
-zpodsdk = "0.6.0"
+zpodsdk = "0.6.1"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3"
 ipython = "^8.9.0"
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/component_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/component_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import typer
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 
 app = typer.Typer(help="Manage Components")
 
-console = Console()
-
 
 def get_status_markdown(status: str):
     match status:
         case "NOT_STARTED" | "INACTIVE":
             return f"[grey63]{status}[/grey63]"
         case "SCHEDULED":
             return "[royal_blue1]SCHEDULED[/royal_blue1]"
@@ -39,27 +37,28 @@
     )
 
     table.add_column("UID")
     table.add_column("Name")
     table.add_column("Version")
     table.add_column("Library")
     table.add_column("Description")
-    table.add_column("Status")
     table.add_column("Download Status")
+    table.add_column("Status")
+
     for component in components:
         table.add_row(
             f"[yellow3]{component.component_uid}[/yellow3]",
             f"[medium_purple1]{component.component_name}[/medium_purple1]",
             f"[cornflower_blue]{component.component_version}[/cornflower_blue]",
             f"[green]{component.library_name}[/green]",
             component.component_description,
-            get_status_markdown(component.status),
             get_status_markdown(component.download_status),
+            get_status_markdown(component.status),
         )
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def component_list(
     all_: Annotated[
         bool,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/endpoint_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/endpoint_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rich.json import JSON
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.cmd import endpoint_permission_cli
 from zpodcli.lib.file import load_json_or_yaml_file
 from zpodcli.lib.prompt import ask
-from zpodcli.lib.utils import exit_with_error
+from zpodcli.lib.utils import console_print, exit_with_error
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.endpoint_compute_create import EndpointComputeCreate
 from zpodsdk.models.endpoint_compute_update import EndpointComputeUpdate
 from zpodsdk.models.endpoint_compute_view import EndpointComputeView
 from zpodsdk.models.endpoint_create import EndpointCreate
 from zpodsdk.models.endpoint_network_create import EndpointNetworkCreate
 from zpodsdk.models.endpoint_network_drivers import EndpointNetworkDrivers
@@ -96,26 +96,26 @@
         ep = endpoint.endpoints
         table.add_row(
             f"[dark_khaki]{endpoint.name}[/dark_khaki]",
             endpoint.description,
             endpoint_output(ep.compute, compute_endpoint_keys),
             endpoint_output(ep.network, network_endpoint_keys),
         )
-    print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def endpoint_list():
     """
     List Endpoints
     """
     z = ZpodClient()
     endpoints = z.endpoints_get_all.sync()
-    generate_table(endpoints, "List Endpoints")
+    generate_table(endpoints, "Endpoint List")
 
 
 @app.command(name="info", no_args_is_help=True)
 @unexpected_status_handler
 def endpoint_info(
     endpoint_name: Annotated[
         str,
@@ -199,15 +199,15 @@
             except json.JSONDecodeError:
                 exit_with_error("The provided JSON was invalid")
 
         if "compute" not in endpoints_dict:
             exit_with_error("The compute section was not found in the json")
 
         if "network" not in endpoints_dict:
-            exit_with_error(" The network section was not found in the json")
+            exit_with_error("The network section was not found in the json")
 
         errors = []
         endpoint_compute_dict = endpoints_dict["compute"]
         if err_c := validate_keywords(
             "compute",
             actual_keys=set(endpoint_compute_dict.keys()),
             expected_keys=set(fields_dict(EndpointComputeCreate)),
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/endpoint_permission_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/endpoint_permission_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from enum import Enum
 from typing import List, Optional
 
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
-from zpodcli.lib.utils import exit_with_error
+from zpodcli.lib.utils import console_print, exit_with_error
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.endpoint_permission_group_add_remove import (
     EndpointPermissionGroupAddRemove,
 )
 from zpodsdk.models.endpoint_permission_user_add_remove import (
     EndpointPermissionUserAddRemove,
 )
@@ -24,45 +23,43 @@
 
 
 app = typer.Typer(
     help="Endpoint Permissions",
     no_args_is_help=True,
 )
 
-console = Console()
-
 
 def generate_table(
     z: ZpodClient,
     endpoint: EndpointView,
 ):
     endpoint_permissions: List[EndpointPermissionView] = (
         z.endpoints_permissions_get_all.sync(endpoint.id)
     )
 
-    title = f"{endpoint.name} Permissions"
+    title = "Endpoint Permission List"
 
     table = Table(
         title=title,
-        min_width=25,
+        min_width=60,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     table.add_column("Users")
     table.add_column("Groups")
 
     for ip in endpoint_permissions:
         users = "\n".join(sorted(x.username for x in ip.users))
         groups = "\n".join(sorted(x.name for x in ip.permission_groups))
         table.add_row(
             f"[light_coral]{users}[/light_coral]",
             f"[cornflower_blue]{groups}[/cornflower_blue]",
         )
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list", no_args_is_help=True)
 @unexpected_status_handler
 def endpoint_permission_list(
     endpoint_name: Annotated[
         str,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/enet_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/enet_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.endpoint_enet_create import EndpointENetCreate
 from zpodsdk.models.endpoint_view_full import EndpointViewFull
 
 app = typer.Typer(help="Manage ENets")
 
 
-console = Console()
-
-
-def generate_table(enets: list, action: str = None):
+def generate_table(enets: list):
+    title = "ENet List"
     table = Table(
         "ENet Name",
         "Project Id",
-        title=f"{action} ENets",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     for enet in enets:
         table.add_row(enet.name, enet.project_id)
-    console.print(table)
+
+    console_print(title, table)
 
 
 @app.command(name="list", no_args_is_help=True)
 @unexpected_status_handler
 def enet_list(
     endpoint_name: Annotated[
         str,
@@ -42,15 +41,15 @@
     """
     List ENets
     """
     z = ZpodClient()
 
     ep: EndpointViewFull = z.endpoints_get.sync(id=f"name={endpoint_name}")
     enets = z.endpoints_enet_get_all.sync(id=ep.id)
-    generate_table(enets, "List")
+    generate_table(enets)
 
 
 @app.command(name="create", no_args_is_help=True)
 @unexpected_status_handler
 def enet_create(
     endpoint_name: Annotated[
         str,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/factory_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/factory_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 
 import typer
 from rich import print
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.lib.factory_config import FactoryConfig
-from zpodcli.lib.utils import exit_with_error
+from zpodcli.lib.utils import console_print, exit_with_error
 
 app = typer.Typer(help="Manage Factories")
 
 
+def get_status_markdown(status: bool):
+    if status:
+        return f"[dark_sea_green4]{status}[/dark_sea_green4]"
+    return f"[indian_red]{status}[/indian_red]"
+
+
 def validate_name(value):
     if re.match(r"^[A-Za-z0-9-]*$", value):
         return value.lower()
     raise typer.BadParameter("Invalid character in name")
 
 
 def validate_server(value):
@@ -27,36 +33,38 @@
 
 
 @app.command(name="list")
 def factory_list():
     """
     List Factories
     """
+
+    title = "Factory List"
     table = Table(
         "Name",
         "Server",
         "Token",
         "Active Context",
-        title="Factory List",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
 
     fc = FactoryConfig()
     for section in sorted(fc.config.sections()):
         factory = fc.config[section]
         token = factory["zpod_api_token"]
         table.add_row(
-            section,
-            factory["zpod_api_url"],
+            f"[tan]{section}[/tan]",
+            f"[sky_blue2]{factory['zpod_api_url']}[/sky_blue2]",
             f"{token[:5]}...{token[-5:]}",
-            str(factory.getboolean("active", False)),
+            get_status_markdown(factory.getboolean("active", False)),
         )
-    print(table)
+    console_print(title, table)
 
 
 @app.command(name="add", no_args_is_help=True)
 def factory_add(
     *,
     factory_name: Annotated[
         str,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/library_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/library_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from typing import Optional
 
 import typer
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
-from zpodcli.lib.utils import get_boolean_markdown
+from zpodcli.lib.utils import console_print, get_boolean_markdown
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.library_create import LibraryCreate
 from zpodsdk.models.library_update import LibraryUpdate
 
 app = typer.Typer(help="Manage Libraries")
 
-console = Console()
-
 
 def generate_table(libraries: list, action: str = None):
-    title = f"{action} Library"
+    title = f"Library {action}"
 
     table = Table(
         title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
@@ -35,15 +32,15 @@
             f"[green]{library.name}[/green]",
             library.description,
             f"[sky_blue2]{library.git_url}[/sky_blue2]",
             f"[tan]{library.creation_date.strftime('%Y-%m-%d %H:%M:%S')}[/tan]",
             f"[magenta]{library.last_modified_date.strftime('%Y-%m-%d %H:%M:%S')}[/magenta]",  # noqa e501
             get_boolean_markdown(library.enabled),
         )
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def library_list():
     """
     List Libraries
@@ -105,17 +102,16 @@
     ],
 ):
     """
     Delete Library
     """
     z: ZpodClient = ZpodClient()
     z.libraries_delete.sync(id=f"name={library_name}")
-    console.print(
-        f"Library [magenta]{library_name}[/magenta] has been deleted successfully",
-        style="green",
+    print(
+        f"Library [magenta]{library_name}[/magenta] has been deleted successfully.",
     )
 
 
 @app.command(name="update", no_args_is_help=True)
 @unexpected_status_handler
 def library_update(
     *,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/permission_group_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/permission_group_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import typer
 from rich import print
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.cmd import permission_group_user_cli
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.permission_group_create import PermissionGroupCreate
 from zpodsdk.models.permission_group_update import PermissionGroupUpdate
 from zpodsdk.models.permission_group_view import PermissionGroupView
 
 app = typer.Typer(help="Manage Permission Groups")
 app.add_typer(permission_group_user_cli.app, name="user", no_args_is_help=True)
 
 
 def generate_table(
     permission_groups: list[PermissionGroupView],
 ):
+    title = "Permission Group List"
     table = Table(
         "Permission Group",
         "Usernames",
-        title="Permission Groups",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     for permission_group in permission_groups:
         usernames = "\n".join(sorted(x.username for x in permission_group.users))
         table.add_row(
             f"[tan]{permission_group.name}[/tan]",
             f"[light_coral]{usernames}[/light_coral]",
         )
-    print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def permission_group_list():
     """
     List Permission Groups
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/permission_group_user_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/permission_group_user_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/profile_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/profile_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 import typer
 from rich import print
 from rich.json import JSON
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.lib.file import load_json_or_yaml_file
-from zpodcli.lib.utils import exit_with_error
+from zpodcli.lib.utils import console_print, exit_with_error
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.profile_create import ProfileCreate
 from zpodsdk.models.profile_item_create import ProfileItemCreate
 from zpodsdk.models.profile_item_update import ProfileItemUpdate
 from zpodsdk.models.profile_update import ProfileUpdate
 
 app = typer.Typer(help="Manage Profiles")
 
 
 def generate_table(profiles: list, action: str = None):
+    title = f"Profile {action}"
     table = Table(
         "Name",
         "Components",
-        title=f"Profile {action}",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     for profile in sorted(profiles, key=lambda p: p.name):
         table.add_row(
             f"[tan]{profile.name}[/tan]",
             profile_item_output(profile),
         )
-    return table
+    console_print(title, table)
 
 
 def profile_item_output(profile):
     profile_item_lines = []
     for profile_item in walk_profile(profile.profile):
         data_values = []
         if host_id := profile_item.host_id:
@@ -62,15 +63,15 @@
 @unexpected_status_handler
 def profile_list():
     """
     Profile List
     """
     z: ZpodClient = ZpodClient()
     profiles = z.profiles_get_all.sync()
-    print(generate_table(profiles, "List"))
+    generate_table(profiles, "List")
 
 
 @app.command(name="info", no_args_is_help=True)
 @unexpected_status_handler
 def profile_info(
     profile_name: Annotated[
         str,
@@ -94,15 +95,15 @@
     """
     z: ZpodClient = ZpodClient()
     profile = z.profiles_get.sync(id=f"name={profile_name}")
     if json_:
         profile_dict = profile.to_dict()["profile"]
         print(JSON.from_data(profile_dict, sort_keys=True))
     else:
-        print(generate_table([profile], "Info"))
+        generate_table([profile], "Info")
 
 
 @app.command(name="create", no_args_is_help=True)
 @unexpected_status_handler
 def profile_create(
     profile_name: Annotated[
         str,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/setting_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/setting_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from typing import Optional
 
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.setting_update import SettingUpdate
 
 app = typer.Typer(help="Manage Settings")
 
-console = Console()
-
 
 def generate_table(settings: list):
+    title = "Setting List"
     table = Table(
-        title="Settings",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     table.add_column("Name")
     table.add_column("Description")
     table.add_column("Value")
     for setting in settings:
         table.add_row(
             f"[tan]{setting.name}[/tan]",
             f"{setting.description}",
             f"[dark_khaki]{setting.value}[/dark_khaki]",
         )
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def setting_list():
     """
     List Settings
@@ -80,11 +79,11 @@
     setting = None
     if description is None:
         setting = SettingUpdate(value=value)
     else:
         setting = SettingUpdate(description=description, value=value)
 
     z.settings_update.sync(body=setting, id=f"name={name}")
-    console.print(
+    print(
         f"Setting [magenta]{name}[/magenta] has been modified to "
         f"[yellow]{value}[/yellow]."
     )
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/user_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/user_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import typer
 from rich import print
 from rich.table import Table
 from typing_extensions import Annotated
 
-from zpodcli.lib.utils import get_boolean_markdown
+from zpodcli.lib.utils import console_print, get_boolean_markdown
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.user_create import UserCreate
 from zpodsdk.models.user_update_admin import UserUpdateAdmin
 
 app = typer.Typer(help="Manage Users")
 
 
 def generate_table(users, all=False):
+    title = "User List"
     table = Table(
         "Username",
         "Email",
         "Description",
         "Creation Date",
         "Last Connection",
         "Superadmin",
-        title="User List",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     if all:
         table.add_column("Status")
 
@@ -42,15 +43,16 @@
             get_boolean_markdown(user.superadmin),
         ]
         if all:
             row.append(user.status)
         table.add_row(
             *row,
         )
-    print(table)
+
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def user_list(
     all: Annotated[
         bool,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/zpod_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/zpod_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from typing import List
 
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.cmd import zpod_component_cli, zpod_permission_cli
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.endpoint_view_full import EndpointViewFull
 from zpodsdk.models.zpod_create import ZpodCreate
 from zpodsdk.models.zpod_permission import ZpodPermission
 from zpodsdk.models.zpod_view import ZpodView
 
 app = typer.Typer(help="Manage zPods")
 app.add_typer(zpod_component_cli.app, name="component")
 app.add_typer(zpod_permission_cli.app, name="permission")
 
-console = Console()
-
 
 def get_status_markdown(status: str):
     match status:
         case "ACTIVE":
             return f"[dark_sea_green4]{status}[/dark_sea_green4]"
         case "PENDING" | "BUILDING":
             return f"[grey63]{status}...[/grey63]"
@@ -33,16 +31,17 @@
         case "DEPLOY_FAILED" | "DESTROY_FAILED":
             return f"[indian_red]{status}[/indian_red]"
         case _:
             return "[royal_blue1]UNKNOWN[/royal_blue1]"
 
 
 def generate_table(zpods: list[ZpodView]):
+    title = "zPod List"
     table = Table(
-        title="zPods",
+        title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     table.add_column("Name")
     table.add_column("Domain")
     table.add_column("Profile")
@@ -71,25 +70,25 @@
         owners = ""
         for zpod_perm in zpod.permissions:
             if zpod_perm.permission == ZpodPermission.OWNER:
                 owners = "\n".join(sorted(x.username for x in zpod_perm.users))
 
         table.add_row(
             f"[bold]{zpod.name}[/bold]",
-            f"[plum4]{zpod.domain}[/plum4]",
+            f"[sky_blue2]{zpod.domain}[/sky_blue2]",
             f"[tan]{zpod.profile}[/tan]",
             components,
             f"[dark_khaki]{zpod.endpoint.name}[/dark_khaki]",
             networks,
-            owners,
+            f"[light_pink1]{owners}[/light_pink1]",
             zpod.password,
             get_status_markdown(zpod.status),
         )
 
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list")
 @unexpected_status_handler
 def zpod_list():
     """
     List zPods
@@ -115,15 +114,15 @@
     """
     Destroy a zPod
     """
     z: ZpodClient = ZpodClient()
 
     for zpod_name in zpod_names:
         z.zpods_delete.sync(id=f"name={zpod_name}")
-        console.print(
+        print(
             f"zPod [magenta]{zpod_name}[/magenta] has been scheduled for destruction."
         )
 
 
 @app.command(name="create", no_args_is_help=True)
 @unexpected_status_handler
 def zpod_create(
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/zpod_component_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/zpod_component_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import List
 
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
 from zpodcli.lib.prompt import confirm
+from zpodcli.lib.utils import console_print
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.zpod_component_create import ZpodComponentCreate
 from zpodsdk.models.zpod_component_view import ZpodComponentView
 from zpodsdk.models.zpod_view import ZpodView
 
 app = typer.Typer(help="Manage zPod Components", no_args_is_help=True)
 
-console = Console()
-
 
 def get_status_markdown(status: str):
     match status:
         case "ACTIVE":
             return f"[dark_sea_green4]{status}[/dark_sea_green4]"
         case "BUILDING":
             return f"[grey63]{status}...[/grey63]"
@@ -29,42 +27,42 @@
             return "[royal_blue1]UNKNOWN[/royal_blue1]"
 
 
 def generate_table(
     zpod: ZpodView,
     zpod_components: list[ZpodComponentView],
 ):
-    title = f"{zpod.name} Component List"
+    title = "zPod Component List"
 
     table = Table(
         title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
     table.add_column("Hostname")
     table.add_column("FQDN")
-    table.add_column("Status")
     table.add_column("Component UID")
     table.add_column("Name")
     table.add_column("Version")
     table.add_column("Description")
+    table.add_column("Status")
 
     for zc in zpod_components:
         table.add_row(
             f"[sky_blue2]{zc.hostname}[/sky_blue2]",
             f"[sky_blue2]https://{zc.fqdn}[/sky_blue2]",
-            get_status_markdown(zc.status),
             f"[yellow3]{zc.component.component_uid}[/yellow3]",
             f"[light_coral]{zc.component.component_name}[/light_coral]",
             f"[cornflower_blue]{zc.component.component_version}[/cornflower_blue]",
             zc.component.component_description,
+            get_status_markdown(zc.status),
         )
 
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list", no_args_is_help=True)
 @unexpected_status_handler
 def zpod_component_list(
     zpod_name: Annotated[
         str,
@@ -74,15 +72,14 @@
         ),
     ],
 ):
     """
     List zPod Components
     """
     print(f"Listing {zpod_name} components")
-
     z: ZpodClient = ZpodClient()
     zpod = z.zpods_get.sync(id=f"name={zpod_name}")
 
     if zpod.name == zpod_name:
         zpod_components: List[ZpodComponentView] = z.zpods_components_get_all.sync(
             zpod.id
         )
```

### Comparing `zpodcli-0.6.0/src/zpodcli/cmd/zpod_permission_cli.py` & `zpodcli-0.6.1/src/zpodcli/cmd/zpod_permission_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from enum import Enum
 from typing import List, Optional
 
 import typer
 from rich import print
-from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
-from zpodcli.lib.utils import exit_with_error
+from zpodcli.lib.utils import console_print, exit_with_error
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.zpod_permission_group_add_remove import (
     ZpodPermissionGroupAddRemove,
 )
 from zpodsdk.models.zpod_permission_user_add_remove import (
     ZpodPermissionUserAddRemove,
 )
@@ -26,24 +25,22 @@
 
 
 app = typer.Typer(
     help="Manage zPod Permissions",
     no_args_is_help=True,
 )
 
-console = Console()
-
 
 def generate_table(
     z: ZpodClient,
     zp: ZpodView,
 ):
     zpod_permissions: List[ZpodPermissionView] = z.zpods_permissions_get_all.sync(zp.id)
 
-    title = f"{zp.name} Permissions"
+    title = f"zPod Permission list {zp.name}"
 
     table = Table(
         title=title,
         title_style="bold",
         show_header=True,
         header_style="bold cyan",
     )
@@ -59,15 +56,15 @@
         users = "\n".join(sorted(x.username for x in zp.users))
         groups = "\n".join(sorted(x.name for x in zp.permission_groups))
         table.add_row(
             f"[yellow3]{zp.permission}[/yellow3]",
             f"[light_coral]{users}[/light_coral]",
             f"[cornflower_blue]{groups}[/cornflower_blue]",
         )
-    console.print(table)
+    console_print(title, table)
 
 
 @app.command(name="list", no_args_is_help=True)
 @unexpected_status_handler
 def zpod_permission_list(
     zpod_name: Annotated[
         str,
```

### Comparing `zpodcli-0.6.0/src/zpodcli/lib/factory_config.py` & `zpodcli-0.6.1/src/zpodcli/lib/factory_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         factory_names = self.config.sections()
         for factory_name in factory_names:
             factory = self.config[factory_name]
             if factory.getboolean("active"):
                 return self.config[factory_name]
 
         exit_with_error(
-            "Please connect to a zPod Server first using the following command:\n\n"
+            "Please connect to a zPodFactory Server first using the following command:\n\n"
             "    zcli factory add --name <xxx> --server <xxx> --token <xxx>\n"
         )
 
     def setactive(self, name):
         for factory_name in self.config.sections():
             factory = self.config[factory_name]
             factory["active"] = str(factory_name == name)
```

### Comparing `zpodcli-0.6.0/src/zpodcli/lib/file.py` & `zpodcli-0.6.1/src/zpodcli/lib/file.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.6.0/src/zpodcli/lib/prompt.py` & `zpodcli-0.6.1/src/zpodcli/lib/prompt.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.6.0/src/zpodcli/lib/zpod_client.py` & `zpodcli-0.6.1/src/zpodcli/lib/zpod_client.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.6.0/src/zpodcli/main_cli.py` & `zpodcli-0.6.1/src/zpodcli/main_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from functools import partial
 from typing import Optional
 
 import typer
-from rich import print
 from typing_extensions import Annotated
 
 from zpodcli import __version__
 from zpodcli.cmd import (
     component_cli,
     endpoint_cli,
     enet_cli,
@@ -36,25 +35,34 @@
         typer.Option(
             "--factory",
             "-f",
             help="Use specified factory for current commmand.",
             show_default=False,
         ),
     ] = None,
+    svg: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--output-svg",
+            help="Output an SVG file for any list command.",
+            show_default=False,
+        ),
+    ] = None,
     version: Annotated[
         Optional[bool],
         typer.Option(
             "--version",
             "-V",
             help="Display version information.",
             callback=version_callback,
         ),
     ] = None,
 ):
     GLOBAL_FLAGS["factory"] = factory
+    GLOBAL_FLAGS["svg"] = svg
 
 
 def launch():
     child_typer = partial(app.add_typer, no_args_is_help=True)
 
     # commands
     child_typer(component_cli.app, name="component")
```

### Comparing `zpodcli-0.6.0/PKG-INFO` & `zpodcli-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: zpodcli
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 License: MIT
 Author: Timo Sugliani
 Author-email: timo.sugliani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (==2.6.3)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer[all] (==0.10.0)
-Requires-Dist: zpodsdk (==0.6.0)
+Requires-Dist: zpodsdk (==0.6.1)
 Description-Content-Type: text/markdown
 
 # zPodFactory CLI
 
 `zcli` is a command line interface for zPodFactory. It is used to create, manage and deploy zPods.
 
 The documentation for `zcli` is available on the main zPodFactory website: https://zpodfactory.github.io
```

