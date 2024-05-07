# Comparing `tmp/axem_dem-0.5.0.tar.gz` & `tmp/axem_dem-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axem_dem-0.5.0.tar", max compression
+gzip compressed data, was "axem_dem-0.6.0.tar", max compression
```

## Comparing `axem_dem-0.5.0.tar` & `axem_dem-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
--rw-r--r--   0        0        0    13291 2024-04-04 10:00:14.896884 axem_dem-0.5.0/LICENSE
--rw-r--r--   0        0        0     6008 2024-04-04 10:00:14.900884 axem_dem-0.5.0/README.md
--rw-r--r--   0        0        0       97 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/__init__.py
--rw-r--r--   0        0        0     2330 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/__main__.py
--rw-r--r--   0        0        0      745 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_cat_cmd.py
--rw-r--r--   0        0        0      826 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_host_cmd.py
--rw-r--r--   0        0        0      649 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_reg_cmd.py
--rw-r--r--   0        0        0     1134 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/assign_cmd.py
--rw-r--r--   0        0        0     2219 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/clone_cmd.py
--rw-r--r--   0        0        0     1508 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/cp_cmd.py
--rw-r--r--   0        0        0     4709 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/create_cmd.py
--rw-r--r--   0        0        0      755 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_cat_cmd.py
--rw-r--r--   0        0        0      647 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_host_cmd.py
--rw-r--r--   0        0        0      706 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_reg_cmd.py
--rw-r--r--   0        0        0     1158 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/delete_cmd.py
--rw-r--r--   0        0        0      909 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/export_cmd.py
--rw-r--r--   0        0        0     1911 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/import_cmd.py
--rw-r--r--   0        0        0     6440 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/info_cmd.py
--rw-r--r--   0        0        0     2048 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/init_cmd.py
--rw-r--r--   0        0        0     1173 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/install_cmd.py
--rw-r--r--   0        0        0      935 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/list_cat_cmd.py
--rw-r--r--   0        0        0     4110 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/list_cmd.py
--rw-r--r--   0        0        0      972 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/list_host_cmd.py
--rw-r--r--   0        0        0      636 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/list_reg_cmd.py
--rw-r--r--   0        0        0     5040 2024-04-16 08:55:39.456506 axem_dem-0.5.0/dem/cli/command/list_tools_cmd.py
--rw-r--r--   0        0        0     7181 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/modify_cmd.py
--rw-r--r--   0        0        0      545 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/cli/command/rename_cmd.py
--rw-r--r--   0        0        0     2372 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/run_cmd.py
--rw-r--r--   0        0        0     1119 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/uninstall_cmd.py
--rw-r--r--   0        0        0      167 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/console.py
--rw-r--r--   0        0        0    17635 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/cli/main.py
--rw-r--r--   0        0        0      964 2024-04-12 07:23:41.038261 axem_dem-0.5.0/dem/cli/tui/printable_tool_image.py
--rw-r--r--   0        0        0    10200 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/renderable/menu.py
--rw-r--r--   0        0        0     4411 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/tui_user_output.py
--rw-r--r--   0        0        0     5453 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/window/dev_env_settings_window.py
--rw-r--r--   0        0        0     5263 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/container_engine.py
--rw-r--r--   0        0        0      770 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/core.py
--rw-r--r--   0        0        0     4232 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/data_management.py
--rwxr-xr-x   0        0        0     4468 2024-04-16 08:55:39.456506 axem_dem-0.5.0/dem/core/dev_env.py
--rw-r--r--   0        0        0     4443 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/dev_env_catalog.py
--rw-r--r--   0        0        0     1461 2024-04-12 07:23:41.038261 axem_dem-0.5.0/dem/core/exceptions.py
--rw-r--r--   0        0        0     2122 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/hosts.py
--rw-r--r--   0        0        0    10273 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/core/platform.py
--rw-r--r--   0        0        0      129 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/properties.py
--rw-r--r--   0        0        0     9626 2024-04-12 07:23:41.042261 axem_dem-0.5.0/dem/core/registry.py
--rw-r--r--   0        0        0     3795 2024-04-12 07:23:41.042261 axem_dem-0.5.0/dem/core/tool_images.py
--rw-r--r--   0        0        0     2235 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/user_output.py
--rw-r--r--   0        0        0     1819 2024-04-24 10:29:35.511775 axem_dem-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7411 1970-01-01 00:00:00.000000 axem_dem-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    13291 2024-04-04 10:00:14.896884 axem_dem-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6008 2024-04-04 10:00:14.900884 axem_dem-0.6.0/README.md
+-rw-r--r--   0        0        0       97 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/__main__.py
+-rw-r--r--   0        0        0      745 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/add_cat_cmd.py
+-rw-r--r--   0        0        0      826 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/add_host_cmd.py
+-rw-r--r--   0        0        0      649 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/add_reg_cmd.py
+-rw-r--r--   0        0        0      890 2024-05-06 17:41:23.057515 axem_dem-0.6.0/dem/cli/command/add_task_cmd.py
+-rw-r--r--   0        0        0     1132 2024-04-30 08:50:12.666342 axem_dem-0.6.0/dem/cli/command/assign_cmd.py
+-rw-r--r--   0        0        0     2276 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/clone_cmd.py
+-rw-r--r--   0        0        0     1515 2024-04-30 08:50:12.666342 axem_dem-0.6.0/dem/cli/command/cp_cmd.py
+-rw-r--r--   0        0        0     4772 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/create_cmd.py
+-rw-r--r--   0        0        0      755 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/del_cat_cmd.py
+-rw-r--r--   0        0        0      647 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/del_host_cmd.py
+-rw-r--r--   0        0        0      706 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/del_reg_cmd.py
+-rw-r--r--   0        0        0      812 2024-04-30 15:33:09.071351 axem_dem-0.6.0/dem/cli/command/del_task_cmd.py
+-rw-r--r--   0        0        0     1232 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/delete_cmd.py
+-rw-r--r--   0        0        0      909 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/export_cmd.py
+-rw-r--r--   0        0        0     1918 2024-04-30 08:50:12.666342 axem_dem-0.6.0/dem/cli/command/import_cmd.py
+-rw-r--r--   0        0        0     7670 2024-05-01 08:26:00.308503 axem_dem-0.6.0/dem/cli/command/info_cmd.py
+-rw-r--r--   0        0        0     2113 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/init_cmd.py
+-rw-r--r--   0        0        0     1173 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/install_cmd.py
+-rw-r--r--   0        0        0      935 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/list_cat_cmd.py
+-rw-r--r--   0        0        0     4510 2024-05-07 15:12:04.623502 axem_dem-0.6.0/dem/cli/command/list_cmd.py
+-rw-r--r--   0        0        0      972 2024-04-04 10:00:14.900884 axem_dem-0.6.0/dem/cli/command/list_host_cmd.py
+-rw-r--r--   0        0        0      636 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/cli/command/list_reg_cmd.py
+-rw-r--r--   0        0        0     5040 2024-04-16 08:55:39.456506 axem_dem-0.6.0/dem/cli/command/list_tools_cmd.py
+-rw-r--r--   0        0        0     7240 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/modify_cmd.py
+-rw-r--r--   0        0        0      552 2024-04-30 08:50:12.666342 axem_dem-0.6.0/dem/cli/command/rename_cmd.py
+-rw-r--r--   0        0        0     3332 2024-05-06 17:41:23.057515 axem_dem-0.6.0/dem/cli/command/run_cmd.py
+-rw-r--r--   0        0        0     1044 2024-04-30 08:50:12.666342 axem_dem-0.6.0/dem/cli/command/set_default_cmd.py
+-rw-r--r--   0        0        0     1171 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/cli/command/uninstall_cmd.py
+-rw-r--r--   0        0        0      167 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/cli/console.py
+-rw-r--r--   0        0        0    21275 2024-05-06 17:41:23.057515 axem_dem-0.6.0/dem/cli/main.py
+-rw-r--r--   0        0        0      964 2024-04-12 07:23:41.038261 axem_dem-0.6.0/dem/cli/tui/printable_tool_image.py
+-rw-r--r--   0        0        0    10200 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/cli/tui/renderable/menu.py
+-rw-r--r--   0        0        0     4411 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/cli/tui/tui_user_output.py
+-rw-r--r--   0        0        0     5453 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/cli/tui/window/dev_env_settings_window.py
+-rw-r--r--   0        0        0     5165 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/core/container_engine.py
+-rw-r--r--   0        0        0      770 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/core/core.py
+-rw-r--r--   0        0        0     4232 2024-04-04 10:00:14.904884 axem_dem-0.6.0/dem/core/data_management.py
+-rwxr-xr-x   0        0        0     5306 2024-05-07 13:04:25.788514 axem_dem-0.6.0/dem/core/dev_env.py
+-rw-r--r--   0        0        0     4443 2024-04-04 10:00:14.908884 axem_dem-0.6.0/dem/core/dev_env_catalog.py
+-rw-r--r--   0        0        0     1461 2024-04-12 07:23:41.038261 axem_dem-0.6.0/dem/core/exceptions.py
+-rw-r--r--   0        0        0     2122 2024-04-04 10:00:14.908884 axem_dem-0.6.0/dem/core/hosts.py
+-rw-r--r--   0        0        0    11038 2024-05-07 15:09:04.285895 axem_dem-0.6.0/dem/core/platform.py
+-rw-r--r--   0        0        0      129 2024-04-04 10:00:14.908884 axem_dem-0.6.0/dem/core/properties.py
+-rw-r--r--   0        0        0     9626 2024-04-12 07:23:41.042261 axem_dem-0.6.0/dem/core/registry.py
+-rw-r--r--   0        0        0     3935 2024-05-06 17:41:23.057515 axem_dem-0.6.0/dem/core/tool_images.py
+-rw-r--r--   0        0        0     2235 2024-04-04 10:00:14.908884 axem_dem-0.6.0/dem/core/user_output.py
+-rw-r--r--   0        0        0     1819 2024-05-07 15:35:36.088433 axem_dem-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7411 1970-01-01 00:00:00.000000 axem_dem-0.6.0/PKG-INFO
```

### Comparing `axem_dem-0.5.0/LICENSE` & `axem_dem-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/README.md` & `axem_dem-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/__main__.py` & `axem_dem-0.6.0/dem/__main__.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/add_cat_cmd.py` & `axem_dem-0.6.0/dem/cli/command/add_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/add_host_cmd.py` & `axem_dem-0.6.0/dem/cli/command/add_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/add_reg_cmd.py` & `axem_dem-0.6.0/dem/cli/command/add_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/assign_cmd.py` & `axem_dem-0.6.0/dem/cli/command/assign_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     """Assign the given Development Environment to the given project.
 
         Args:
             platform -- the platform
             dev_env_name -- the name of the Development Environment to assign
             project_path -- the path to the project to assign the Development Environment to
     """
-
-
     if not os.path.isdir(project_path):
         stderr.print(f"[red]Error: The {project_path} path does not exist.[/]")
         return
 
     dev_env_to_assign: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env_to_assign is None:
```

### Comparing `axem_dem-0.5.0/dem/cli/command/clone_cmd.py` & `axem_dem-0.6.0/dem/cli/command/clone_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     stdout.print("[yellow]The Dev Env already exists.[/]")
     typer.confirm("Continue with overwrite?", abort=True)
     
     if local_dev_env.is_installed:
         typer.confirm("The Dev Env to overwrite is installed. Do you want to uninstall it?", 
                       abort=True)
         try:
-            platform.uninstall_dev_env(local_dev_env)
+            for status in platform.uninstall_dev_env(local_dev_env):
+                stdout.print(status)
         except PlatformError as e:
             stderr.print(f"[red]{str(e)}[/]")
             raise typer.Abort()
 
     platform.local_dev_envs.remove(local_dev_env)
 
 def execute(platform: Platform, dev_env_name: str) -> None:
@@ -33,16 +34,14 @@
 
         If the Dev Env already exists locally, the user will be asked to confirm the overwrite.
 
         Args:
             platform -- the platform
             dev_env_name -- name of the Dev Env to clone
     """
-
-
     catalog_dev_env: DevEnv | None = None
 
     if not platform.dev_env_catalogs.catalogs:
         stderr.print("[red]Error: No Development Environment Catalogs are available to clone from![/]")
         return
 
     for catalog in platform.dev_env_catalogs.catalogs:
@@ -55,10 +54,10 @@
         return
 
     local_dev_env: DevEnv | None = platform.get_dev_env_by_name(dev_env_name)
     if local_dev_env:
         handle_existing_local_dev_env(platform, local_dev_env)
 
     platform.local_dev_envs.append(catalog_dev_env)
-    platform.flush_descriptors()
+    platform.flush_dev_env_properties()
 
     stdout.print("[green]The Dev Env successfully cloned.[/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/cp_cmd.py` & `axem_dem-0.6.0/dem/cli/command/cp_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def cp_given_dev_env(platform: Platform, dev_env_to_cp: DevEnv,
                         new_dev_env_name: str):
     new_dev_env = copy.deepcopy(dev_env_to_cp)
     new_dev_env.name = new_dev_env_name
     new_dev_env.is_installed = False
     platform.local_dev_envs.append(new_dev_env)
-    platform.flush_descriptors()
+    platform.flush_dev_env_properties()
 
 def execute(platform: Platform, dev_env_to_cp_name: str, new_dev_env_name: str) -> None:
 
 
     dev_env_to_cp = get_dev_env_to_cp(platform, dev_env_to_cp_name)
 
     if (dev_env_to_cp is not None and
```

### Comparing `axem_dem-0.5.0/dem/cli/command/create_cmd.py` & `axem_dem-0.6.0/dem/cli/command/create_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,16 @@
         typer.confirm("The input name is already used by a Development Environment. Overwrite it?", 
                       abort=True)
 
         if dev_env_original.is_installed:
             typer.confirm("The Development Environment is installed, so it can't be overwritten. " + \
                           "Uninstall it first?", abort=True)
             try:
-                platform.uninstall_dev_env(dev_env_original)
+                for status in platform.uninstall_dev_env(dev_env_original):
+                    stdout.print(status)
             except PlatformError as e:
                 stderr.print(f"[red]{str(e)}[/]")
                 raise typer.Abort()
 
     selected_tool_images = open_dev_env_settings_panel(platform.tool_images.all_tool_images)
     new_dev_env_descriptor = create_new_dev_env_descriptor(dev_env_name, selected_tool_images)
     
@@ -114,10 +115,10 @@
 
         Exceptions:
             Abort -- if the name of the Development Environment contains whitespace characters
     """
     platform.assign_tool_image_instances_to_all_dev_envs()
 
     create_dev_env(platform, dev_env_name)
-    platform.flush_descriptors()
+    platform.flush_dev_env_properties()
     stdout.print(f"The [green]{dev_env_name}[/] Development Environment has been created!")
     stdout.print("Run [italic]dem install[/] to install it.")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/del_cat_cmd.py` & `axem_dem-0.6.0/dem/cli/command/del_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/del_host_cmd.py` & `axem_dem-0.6.0/dem/cli/command/del_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/del_reg_cmd.py` & `axem_dem-0.6.0/dem/cli/command/del_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/delete_cmd.py` & `axem_dem-0.6.0/dem/cli/command/delete_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,17 @@
         stderr.print(f"[red]Error: The [bold]{dev_env_name}[/bold] Development Environment doesn't exist.")
     else:
         if dev_env_to_delete.is_installed:
             typer.confirm("The Development Environment is installed. Do you want to uninstall it?", 
                           abort=True)
 
             try:
-                platform.uninstall_dev_env(dev_env_to_delete)
+                for status in platform.uninstall_dev_env(dev_env_to_delete):
+                    stdout.print(status)
             except PlatformError as e:
                 stderr.print(f"[red]{str(e)}[/]")
                 return
 
-        stdout.print("Deleting the Development Environment...")
+        stdout.print("Deleting the Development Environment descriptor...")
         platform.local_dev_envs.remove(dev_env_to_delete)
-        platform.flush_descriptors()
+        platform.flush_dev_env_properties()
         stdout.print(f"[green]Successfully deleted the {dev_env_name}![/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/export_cmd.py` & `axem_dem-0.6.0/dem/cli/command/export_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/import_cmd.py` & `axem_dem-0.6.0/dem/cli/command/import_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,10 +44,10 @@
             
         Raises:
             typer.Abort: If the Development Environment already exists, or the JSON format is 
             invalid.
     """
     if os.path.exists(path_to_dev_env):
         import_dev_env_from_json(platform,path_to_dev_env)        
-        platform.flush_descriptors()
+        platform.flush_dev_env_properties()
     else:
         stderr.print("[red]Error: The input file does not exist.[/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/info_cmd.py` & `axem_dem-0.6.0/dem/cli/command/info_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,35 +11,76 @@
 image_status_messages = {
     ToolImage.NOT_AVAILABLE: "[red]Error: not available![/]",
     ToolImage.LOCAL_ONLY: "Local",
     ToolImage.REGISTRY_ONLY: "Registry",
     ToolImage.LOCAL_AND_REGISTRY: "Local and Registry",
 }
 
-def print_local_dev_env_info(dev_env: DevEnv) -> None:
-    """ Print information about the given local Development Environment.
+def print_status(platform: Platform, dev_env: DevEnv) -> None:
+    """ Print the status of the Development Environment.
+    
+        Args:
+            platform -- the platform
+            dev_env -- the Development Environment to print the status of
+    """
+    if dev_env.is_installed:
+        status = "[green]Installed[/]"
+        if dev_env.name == platform.default_dev_env_name:
+            status = status.replace("[/]", " | Default[/]")
+    else:
+        status = "Not installed"
+
+    stdout.print(f"Status: {status}\n")
+
+def print_tools_info_table(dev_env: DevEnv, is_local: bool, platform: Platform = None) -> None:
+    """ Print information about the tools in the Development Environment.
     
         Args:
             dev_env -- the Development Environment to print information about
+            is_local -- flag to indicate if the Development Environment is local
+            platform -- the platform (only needed if is_local is True)
     """
-    tool_info_table = Table()
+    tool_info_table = Table(title="Tools")
     tool_info_table.add_column("Image")
     tool_info_table.add_column("Availability")
 
     for tool_image in sorted(dev_env.tool_images, key=lambda x: x.name):
         tool_info_table.add_row(tool_image.name,
                                 image_status_messages[tool_image.availability])
-    if dev_env.is_installed:
-        installation_status = "[green]Installed[/]"
-    else:
-        installation_status = "Not installed"
-    stdout.print(f"\n[bold]Development Environment: {dev_env.name}[/]\n")
-    stdout.print(f"Installation state: {installation_status}\n")
+    if is_local:
+        print_status(platform, dev_env)
     stdout.print(tool_info_table)
 
+def print_tasks_info_table(dev_env: DevEnv) -> None:
+    """ Print information about the tasks in the Development Environment.
+    
+        Args:
+            dev_env -- the Development Environment to print information about
+    """
+    task_table = Table(title="Tasks")
+    task_table.add_column("Task")
+    task_table.add_column("Command")
+
+    for task_name, command in dev_env.tasks.items():
+        task_table.add_row(task_name, command)
+
+    stdout.print(task_table)
+
+def print_local_dev_env_info(platform: Platform, dev_env: DevEnv) -> None:
+    """ Print information about the given local Development Environment.
+    
+        Args:
+            platform -- the platform
+            dev_env -- the Development Environment to print information about
+    """
+    stdout.print(f"\n[bold]Development Environment: {dev_env.name}[/]\n")
+    print_tools_info_table(dev_env, True, platform)
+    if dev_env.tasks:
+        print_tasks_info_table(dev_env)
+
     if dev_env.is_installed and dev_env.get_tool_image_status() == DevEnv.Status.REINSTALL_NEEDED:
         stderr.print("\n[red]Error: Incomplete local install! The Dev Env must be reinstalled![/]")
 
     if dev_env.get_tool_image_status() == DevEnv.Status.UNAVAILABLE_IMAGE:
         stderr.print("\n[red]Error: Required image could not be found either locally or in the registry![/]")
 
 def local_info(platform: Platform, dev_env_name: str) -> None:
@@ -56,33 +97,28 @@
 
     dev_env = platform.get_dev_env_by_name(dev_env_name)
 
     if dev_env is None:
         stderr.print(f"[red]Error: Unknown Development Environment: {dev_env_name}[/]\n")
         raise typer.Abort()
 
-    print_local_dev_env_info(dev_env)
+    print_local_dev_env_info(platform, dev_env)
 
 def print_cat_dev_env_info(dev_env: DevEnv, cat_name: str) -> None:
     """ Print information about the given catalog Development Environment.
     
         Args:
             dev_env -- the Development Environment to print information about
             cat_name -- the name of the catalog the Development Environment belongs to
     """
-    tool_info_table = Table()
-    tool_info_table.add_column("Image")
-    tool_info_table.add_column("Availability")
-
-    for tool_image in sorted(dev_env.tool_images, key=lambda x: x.name):
-        tool_info_table.add_row(tool_image.name,
-                                image_status_messages[tool_image.availability])
     stdout.print(f"\n[bold]Development Environment: {dev_env.name}[/]\n")
     stdout.print(f"Catalog: {cat_name}\n")
-    stdout.print(tool_info_table)
+    print_tools_info_table(dev_env, False)
+    if dev_env.tasks:
+        print_tasks_info_table(dev_env)
 
     if dev_env.get_tool_image_status() == DevEnv.Status.UNAVAILABLE_IMAGE:
         stderr.print("\n[red]Error: Required image could not be found in the registry![/]")
     
 def cat_dev_env_info(platform: Platform, dev_env_name: str, selected_cats: list[str]) -> None:
     """ Gather and print information about the given catalog Development Environment.
```

### Comparing `axem_dem-0.5.0/dem/cli/command/init_cmd.py` & `axem_dem-0.6.0/dem/cli/command/init_cmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 def execute(platform: Platform, project_path: str) -> None:
     """ Initialize a project at the given path.
 
         Args:
             platform -- the platform
             project_path -- the path to the project to initialize
     """
-
-
     if not os.path.isdir(project_path):
         stderr.print(f"[red]Error: The {project_path} path does not exist.[/]")
         return
 
     try:
         dev_env = DevEnv(descriptor_path=f"{project_path}/.axem/dev_env_descriptor.json")
     except FileNotFoundError as e:
@@ -32,19 +30,20 @@
             typer.confirm("Would you like to re-init the Dev Env? All local changes will be lost!", abort=True)
 
             if local_dev_env.is_installed:
                 typer.confirm("The Development Environment is installed, so it can't be deleted. Do you want to uninstall it first?", 
                               abort=True)
                 
                 try:
-                    platform.uninstall_dev_env(local_dev_env)
+                    for status in platform.uninstall_dev_env(local_dev_env):
+                        stdout.print(status)
                 except PlatformError as e:
                     stderr.print(f"[red]{str(e)}[/]")
                     return
             
             platform.local_dev_envs.remove(local_dev_env)
             break
 
     platform.local_dev_envs.append(dev_env)
-    platform.flush_descriptors()
+    platform.flush_dev_env_properties()
     stdout.print(f"[green]Successfully initialized the {dev_env.name} Dev Env for the project at {project_path}![/]")
     stdout.print(f"\nNow you can install the Dev Env with the `dem install {dev_env.name}` command.")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/install_cmd.py` & `axem_dem-0.6.0/dem/cli/command/install_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/list_cat_cmd.py` & `axem_dem-0.6.0/dem/cli/command/list_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/list_cmd.py` & `axem_dem-0.6.0/dem/cli/command/list_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,43 +12,48 @@
     """ Add Development Environment information to the table.
     
         Args:
             platform -- the Platform
             table -- the Table
             dev_env -- the Development Environment
     """
+    installed_column = ""
+    default_column = ""
     if dev_env.is_installed:
         dev_env.assign_tool_image_instances(platform.tool_images)
-        installed_column = "[green]Yes[/]"
+        installed_column = "[green]✓[/]"
         tool_image_status = dev_env.get_tool_image_status()
         if tool_image_status == DevEnv.Status.UNAVAILABLE_IMAGE:
             status_column = "[red]Error: Required image is not available![/]"
         elif tool_image_status == DevEnv.Status.REINSTALL_NEEDED:
             status_column = "[red]Error: Incomplete local install![/]"
         else:
-            status_column = "Ok"
+            status_column = "[green]Ok[/]"
+
+        if dev_env.name == platform.default_dev_env_name:
+            default_column = "[green]✓[/]"
     else:
-        installed_column = "No"
-        status_column = "Ok"
-    table.add_row(dev_env.name, installed_column, status_column)
+        status_column = "[green]Ok[/]"
+    table.add_row(dev_env.name, installed_column, default_column, status_column)
 
 def list_local_dev_envs(platform: Platform) -> None:
     """ List the local Development Environments.
     
         Args:
             platform -- the Platform
     """
     if not platform.local_dev_envs:
         stdout.print("[yellow]No Development Environment descriptors are available.[/]")
         return
     else:
         table = Table()
         table.add_column("Name")
-        table.add_column("Installed")
-        table.add_column("Status")
+        table.add_column("Installed", justify="center")
+        table.add_column("Default", justify="center")
+        table.add_column("Status", justify="center")
 
         for dev_env in sorted(platform.local_dev_envs, key=lambda dev_env: dev_env.name.lower()):
             add_dev_env_info_to_table(platform, table, dev_env)
 
         stdout.print(f"\n [italic]Local Development Environments[/]")
         stdout.print(table)
 
@@ -105,8 +110,11 @@
         selected_cats -- list the Development Environments from the specified catalogs
     """
     if cat and not selected_cats:
         list_all_cat_dev_envs(platform)
     elif selected_cats:
         list_selected_cat_dev_envs(platform, selected_cats)
     else:
-        list_local_dev_envs(platform)
+        list_local_dev_envs(platform)
+
+        if platform.default_dev_env_name:
+            stdout.print(f"\n[bold]The default Development Environment: {platform.default_dev_env_name}[/]")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `axem_dem-0.5.0/dem/cli/command/list_host_cmd.py` & `axem_dem-0.6.0/dem/cli/command/list_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/list_reg_cmd.py` & `axem_dem-0.6.0/dem/cli/command/list_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/list_tools_cmd.py` & `axem_dem-0.6.0/dem/cli/command/list_tools_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/command/modify_cmd.py` & `axem_dem-0.6.0/dem/cli/command/modify_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         if check_for_new_dev_env is None:
             platform.local_dev_envs.append(new_dev_env)
         else:
             stderr.print("[red]The Development Environment already exist.")
             raise typer.Abort()
 
-    platform.flush_descriptors()
+    platform.flush_dev_env_properties()
 
 def get_already_selected_tool_images(dev_env: DevEnv) -> set[str]:
     """ Get the already selected Tool Images.
     
         Args:
             dev_env -- the Development Environment
             
@@ -173,14 +173,15 @@
     if dev_env is None:
         stderr.print("[red]The Development Environment doesn't exist.")
         return
     elif dev_env.is_installed is True:
         stdout.print("[yellow]The Development Environment is installed, so it can't be modified.[/]")
         typer.confirm("Do you want to uninstall it first?", abort=True)
         try:
-            platform.uninstall_dev_env(dev_env)
+            for status in platform.uninstall_dev_env(dev_env):
+                stdout.print(status)
         except PlatformError as e:
             stderr.print(f"[red]{str(e)}[/]")
             return
 
     modify_with_tui(platform, dev_env)
     stdout.print("[green]The Development Environment has been modified successfully![/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/rename_cmd.py` & `axem_dem-0.6.0/dem/cli/command/rename_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 def execute(platform: Platform, dev_env_name_to_rename: str, new_dev_env_name: str) -> None:
 
 
     dev_env_to_rename = platform.get_dev_env_by_name(dev_env_name_to_rename)
 
     if dev_env_to_rename is not None:
         dev_env_to_rename.name = new_dev_env_name
-        platform.flush_descriptors()
+        platform.flush_dev_env_properties()
     else:
         stderr.print("[red]Error: The input Development Environment does not exist.[/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/command/uninstall_cmd.py` & `axem_dem-0.6.0/dem/cli/command/uninstall_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 
     if dev_env_to_uninstall is None:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment does not exist.[/]")
     elif not dev_env_to_uninstall.is_installed:
         stderr.print(f"[red]Error: The {dev_env_name} Development Environment is not installed.[/]")
     else:
         try:
-            platform.uninstall_dev_env(dev_env_to_uninstall)
+            for status in platform.uninstall_dev_env(dev_env_to_uninstall):
+                stdout.print(status)
         except PlatformError as e:
             stderr.print(f"[red]{str(e)}[/]")
         else:
             stdout.print(f"[green]Successfully uninstalled the {dev_env_name}![/]")
```

### Comparing `axem_dem-0.5.0/dem/cli/main.py` & `axem_dem-0.6.0/dem/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # dem/cli/main.py
 
 import typer, importlib.metadata
 from typing import Generator
 from typing_extensions import Annotated
 import os
 from dem import __command__, __app_name__
-from dem.cli.command import cp_cmd, import_cmd, info_cmd, list_cmd, create_cmd, modify_cmd, delete_cmd, \
-                            rename_cmd, run_cmd, export_cmd, clone_cmd, add_reg_cmd, \
+from dem.cli.command import cp_cmd, import_cmd, info_cmd, list_cmd, create_cmd, modify_cmd, \
+                            delete_cmd, rename_cmd, run_cmd, export_cmd, clone_cmd, add_reg_cmd, \
                             list_reg_cmd, del_reg_cmd, add_cat_cmd, list_cat_cmd, del_cat_cmd, \
-                            add_host_cmd, uninstall_cmd, install_cmd, assign_cmd, init_cmd, \
-                            list_host_cmd, del_host_cmd, list_tools_cmd
+                            add_host_cmd, set_default_cmd, uninstall_cmd, install_cmd, assign_cmd, \
+                            init_cmd, list_host_cmd, del_host_cmd, list_tools_cmd, add_task_cmd, \
+                            del_task_cmd
 from dem.cli.console import stdout
 from dem.core.platform import Platform
 from dem.core.exceptions import InternalError
 
 typer_cli: typer.Typer = typer.Typer(rich_markup_mode="rich")
 platform: Platform | None = None
 
@@ -29,14 +30,28 @@
         incomplete -- the parameter the user supplied so far when the tab was pressed
     """
     if platform is not None:
         for dev_env in platform.local_dev_envs:
             if dev_env.name.startswith(incomplete) or (incomplete == ""):
                 yield dev_env.name
 
+def autocomplete_installed_dev_env_name(incomplete: str) -> Generator:
+    """ 
+    Autocomplete the input Dev Env name with the available matching installed Dev Envs.
+
+    Return with the matching Dev Env names by a Generator.
+    
+    Args:
+        incomplete -- the parameter the user supplied so far when the tab was pressed
+    """
+    if platform is not None:
+        for dev_env in platform.local_dev_envs:
+            if dev_env.is_installed and (dev_env.name.startswith(incomplete) or (incomplete == "")):
+                yield dev_env.name
+
 def autocomplete_cat_name(incomplete: str) -> Generator:
     """ 
     Autocomplete the input Catalog name with the available matching catalogs.
 
     Return with the matching Catalog name by a Generator.
     
     Args:
@@ -71,15 +86,76 @@
         incomplete -- the parameter the user supplied so far when the tab was pressed
     """
     if platform is not None:
         for host_config in platform.hosts.list_host_configs():
             if host_config["name"].startswith(incomplete) or (incomplete == ""):
                 yield host_config["name"]
 
+def autocomplete_task_name(ctx: typer.Context, incomplete: str) -> Generator:
+    """ 
+    Autocomplete the input Task name with the available matching Task names.
+
+    Return with the matching Task name by a Generator.
+    
+    Args:
+        incomplete -- the parameter the user supplied so far when the tab was pressed
+    """
+    dev_env_name = ctx.params.get("dev_env_name", None)
+    if platform is not None and dev_env_name is not None:
+        for dev_env in platform.local_dev_envs:
+            if dev_env.name == dev_env_name:
+                for task_name in dev_env.tasks:
+                    if task_name.startswith(incomplete) or (incomplete == ""):
+                        yield task_name
+
 # DEM commands
+@typer_cli.command()
+def add_task(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to add the task to.",
+                                                         autocompletion=autocomplete_dev_env_name)],
+             task_name: Annotated[str, typer.Argument(help="Name of the task.")], 
+             command: Annotated[str, typer.Argument(help="The command the task should execute.")]) -> None:
+    """
+    Add a new task to the Development Environment.
+
+    The command will be executed when the `dem run dev_env_name task_name` command is called. The 
+    command must be surrounded by quotes.
+    """
+    if platform:
+        add_task_cmd.execute(platform, dev_env_name, task_name, command)
+    else:
+        raise InternalError("Error: The platform hasn't been initialized properly!")
+
+@typer_cli.command()
+def del_task(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to delete the task from.",
+                                                         autocompletion=autocomplete_dev_env_name)],
+             task_name: Annotated[str, typer.Argument(help="Name of the task to delete.",
+                                                      autocompletion=autocomplete_task_name)]) -> None:
+    """
+    Delete a task from the Development Environment.
+    """
+    if platform:
+        del_task_cmd.execute(platform, dev_env_name, task_name)
+    else:
+        raise InternalError("Error: The platform hasn't been initialized properly!")
+
+@typer_cli.command()
+def set_default(dev_env_name: Annotated[str, 
+                                     typer.Argument(help="The name of the Development Environment to set as default.",
+                                                    autocompletion=autocomplete_installed_dev_env_name)]) -> None:
+    """
+    Set the Development Environment as the default one.
+
+    The default Development Environment will be used by the run command when no Development 
+    Environment is specified.
+    """
+    if platform:
+        set_default_cmd.execute(platform, dev_env_name)
+    else:
+        raise InternalError("Error: The platform hasn't been initialized properly!")
+
 @typer_cli.command("list", context_settings={"allow_extra_args": True}) # "list" is a Python keyword
 def list_(cat: Annotated[bool, typer.Option(help="List the Dev Envs available from the catalogs.",
                                             show_default=False)] = False,
           ctx: Annotated[typer.Context, typer.Option()] = None) -> None:
     """
     List the Dev Envs.
 
@@ -268,29 +344,31 @@
     If the project path is not specified, the current working directory will be used.
     """
     if platform:
         init_cmd.execute(platform, project_path)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
-@typer_cli.command(context_settings={"allow_extra_args": True, "ignore_unknown_options": True})
-def run(dev_env_name: Annotated[str, typer.Argument(help="Run the container in this Development Environment context",
-                                                    autocompletion=autocomplete_dev_env_name)],
-        ctx: Annotated[typer.Context, typer.Option()]) -> None:
-    """
-    Run the `docker run` command in the Development Environment's context with the given parameters.  
-
-    This command can be used as the docker CLI one, except as first argument the name of the 
-    Development Environment must be set. 
-    Example: dem run dev_env --name test test_image_name:latest ls -la
-
-    See the documentation for the list of currently supported docker run parameters.
-    """
-    if platform:
-        run_cmd.execute(platform, dev_env_name, ctx.args)
+@typer_cli.command()
+def run(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to run the task in. If not set, the default Dev Env will be used.",
+                                                    autocompletion=autocomplete_installed_dev_env_name)] = "",
+        task_name: Annotated[str, typer.Argument(help="The name of the task to run.",
+                                                 autocompletion=autocomplete_task_name)] = "") -> None:
+    """
+    Run the task of the Development Environment. The Dev Env must be installed.
+
+    If the Dev Env is not specified, the default Dev Env will be used. If the default Dev Env is not
+    set, an error message will be printed.
+    """
+    if platform:
+        # If only a single parameter is supplied, we assume it's the task name
+        if not task_name and dev_env_name:
+            task_name = dev_env_name
+            dev_env_name = ""
+        run_cmd.execute(platform, dev_env_name, task_name)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
 @typer_cli.command()
 def add_reg(name: Annotated[str, typer.Argument(help="Name of the registry to add")], 
             url: Annotated[str, typer.Argument(help="API URL of the registry")]) -> None:
     """
```

### Comparing `axem_dem-0.5.0/dem/cli/tui/printable_tool_image.py` & `axem_dem-0.6.0/dem/cli/tui/printable_tool_image.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/tui/renderable/menu.py` & `axem_dem-0.6.0/dem/cli/tui/renderable/menu.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/tui/tui_user_output.py` & `axem_dem-0.6.0/dem/cli/tui/tui_user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/cli/tui/window/dev_env_settings_window.py` & `axem_dem-0.6.0/dem/cli/tui/window/dev_env_settings_window.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/container_engine.py` & `axem_dem-0.6.0/dem/core/container_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,27 +100,26 @@
         if stream_logs:
             for line in run_result.logs(stream=True):
                 self.user_output.msg(line.decode().strip())
 
     def remove(self, image: str) -> None:
         """ Remove a tool image.
 
-            If the removal was successful return with True, otherwise return with False.
-        
             Args: 
                 image -- the tool image to remove
+
+            Raises:
+                ContainerEngineError -- if the image is used by a container
         """
         try:
             self._docker_client.images.remove(image)
         except docker.errors.ImageNotFound:
             self.user_output.msg(f"[yellow]The {image} doesn't exist. Unable to remove it.[/]\n")
         except docker.errors.APIError:
             raise ContainerEngineError(f"The {image} is used by a container. Unable to remove it.\n")
-        else:
-            self.user_output.msg(f"[green]Successfully removed the {image}![/]\n")
 
     def search(self, registry: str) -> list[str]:
         """ Search repository in the axemsolutions registry.
         
             Args:
                 registry -- registry to search
         """
```

### Comparing `axem_dem-0.5.0/dem/core/core.py` & `axem_dem-0.6.0/dem/core/core.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/data_management.py` & `axem_dem-0.6.0/dem/core/data_management.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/dev_env.py` & `axem_dem-0.6.0/dem/core/dev_env.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,16 +41,16 @@
                 raise FileNotFoundError("dev_env_descriptor.json doesn't exist.")
             with open(descriptor_path, "r") as file:
                 descriptor = json.load(file)
 
         self.name: str = descriptor["name"]
         self.tool_image_descriptors: list[dict[str, str]] = descriptor["tools"]
         self.tool_images: list[ToolImage] = []
-        descriptor_installed = descriptor.get("installed", "False")
-        if "True" == descriptor_installed:
+        self.tasks: dict[str, str] = descriptor.get("tasks", {})
+        if "True" == descriptor.get("installed", "False"):
             self.is_installed = True
         else:
             self.is_installed = False
 
     def assign_tool_image_instances(self, tool_images: ToolImages) -> None:
         """ Assign the Tool Images to the Development Environment.
         
@@ -59,19 +59,45 @@
             
             Args:
                 tool_images -- the Tool Images to assign
                 
                 Exceptions:
                     ToolImageError -- if the Tool Image name is invalid
         """
+        self.tool_images = []
         for tool_descriptor in self.tool_image_descriptors:
             tool_image_name = tool_descriptor["image_name"] + ':' + tool_descriptor["image_version"]
             tool_image = tool_images.all_tool_images.get(tool_image_name, ToolImage(tool_image_name))
             self.tool_images.append(tool_image)
 
+    def add_task(self, task_name: str, command: str) -> None:
+        """ Add a task to the Development Environment.
+
+            If the task already exists, it will be overwritten.
+        
+            Args:
+                task_name -- the task name
+                command -- the command
+        """
+        self.tasks[task_name] = command
+
+    def del_task(self, task_name: str) -> None:
+        """ Delete a task from the Development Environment.
+
+            Args:
+                task_name -- the task name
+
+            Exceptions:
+                KeyError -- if the task doesn't exist
+        """
+        if task_name in self.tasks:
+            del self.tasks[task_name]
+        else:
+            raise KeyError(f"Task [bold]{task_name}[/] not found.")
+
     def get_tool_image_status(self) -> Status:
         """ Get the status of the Tool Images.
 
             This method checks the availability of the assigned Tool Images. 
             If at least one of the Tool Images is unkonwn: NOT_AVAILABLE. 
             If at least one of the Tool Images is only available in the registry: REINSTALL_NEEDED. 
             If all the Tool Images are available: OK.
@@ -89,15 +115,16 @@
     def get_deserialized(self, omit_is_installed: bool = False) -> dict[str, str]:
         """ Create the deserialized json. 
         
             Return the Dev Env as a dict.
         """
         dev_env_json_deserialized: dict = {
             "name": self.name,
-            "tools": self.tool_image_descriptors
+            "tools": self.tool_image_descriptors,
+            "tasks": self.tasks
         }
         
         if omit_is_installed is False:
             if self.is_installed:
                 dev_env_json_deserialized["installed"] = "True"
             else:
                 dev_env_json_deserialized["installed"] = "False"
```

### Comparing `axem_dem-0.5.0/dem/core/dev_env_catalog.py` & `axem_dem-0.6.0/dem/core/dev_env_catalog.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/exceptions.py` & `axem_dem-0.6.0/dem/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/hosts.py` & `axem_dem-0.6.0/dem/core/hosts.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/platform.py` & `axem_dem-0.6.0/dem/core/platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Repesents the Development Platform. The platform resources can be accessed through this interface.  
 """
 
 import os
-from typing import Any
+from typing import Any, Generator
 from dem.core.core import Core
 from dem.core.properties import __supported_dev_env_major_version__
 from dem.core.exceptions import DataStorageError, PlatformError, ContainerEngineError
 from dem.core.dev_env_catalog import DevEnvCatalogs
 from dem.core.data_management import LocalDevEnvJSON
 from dem.core.container_engine import ContainerEngine
 from dem.core.registry import Registries
@@ -34,14 +34,17 @@
     def __init__(self) -> None:
         """ Init the class."""
         self._dev_env_catalogs: DevEnvCatalogs | None = None
         self._tool_images = None
         self._container_engine = None
         self._registries = None
         self._hosts = None
+        self.default_dev_env_name: str = ""
+        self.local_dev_envs: list[DevEnv] = []
+        self.are_tool_images_assigned: bool = False
 
         # Set this to true in the platform instance to work with the local tool images only
         self.local_only = False
         # Set this to true in the platform instance so when first accessing the `tool_images` 
         # instance variable, do not automatically update the tool images from the registries
         self.disable_tool_update = False
 
@@ -50,22 +53,23 @@
         
             The Dev Envs will only contain the descriptors and not the ToolImage instances.
         """
         self.dev_env_json = LocalDevEnvJSON()
         self.dev_env_json.update()
         self.version = self.dev_env_json.deserialized["version"]
         self._dev_env_json_version_check(int(self.version.split('.', 1)[0]))
-        self.local_dev_envs: list[DevEnv] = []
+        self.default_dev_env_name = self.dev_env_json.deserialized.get("default_dev_env", "")
         for dev_env_descriptor in self.dev_env_json.deserialized["development_environments"]:
             self.local_dev_envs.append(DevEnv(descriptor=dev_env_descriptor))
 
     def assign_tool_image_instances_to_all_dev_envs(self) -> None:
         """ Assign the ToolImage instances to all Development Environments."""
         for dev_env in self.local_dev_envs:
             dev_env.assign_tool_image_instances(self.tool_images)
+        self.are_tool_images_assigned = True
 
     @property
     def tool_images(self) -> ToolImages:
         """ The tool images.
 
             The ToolImages() gets instantiated only at the first access.
         """
@@ -122,14 +126,15 @@
     def get_deserialized(self) -> dict:
             """ Create the deserialized json. 
             
                 Return the dev_env.json as a dict.
             """
             dev_env_json_deserialized: dict[str, Any] = {
                 "version": self.version,
+                "default_dev_env": self.default_dev_env_name,
                 "development_environments": [
                     dev_env.get_deserialized()
                     for dev_env in self.local_dev_envs
                 ]
             }
             return dev_env_json_deserialized
 
@@ -163,47 +168,60 @@
                 self.user_output.msg(f"\nPulling image {tool_image.name}", is_title=True)
                 try:                
                     self.container_engine.pull(tool_image.name)
                 except ContainerEngineError as e:
                     raise PlatformError(f"Dev Env install failed. --> {str(e)}")
 
         dev_env_to_install.is_installed = True
-        self.flush_descriptors()
+        self.flush_dev_env_properties()
 
-    def uninstall_dev_env(self, dev_env_to_uninstall: DevEnv) -> None:
+    def uninstall_dev_env(self, dev_env_to_uninstall: DevEnv) -> Generator:
         """ Uninstall the Dev Env by removing the images not required anymore.
 
             Args:
                 dev_env_to_uninstall -- the Development Environment to uninstall
 
-            Exceptions:
+            Returns:
+                Generator -- the status messages
+
+            Raises:
                 PlatformError -- if the uninstall fails
         """
+        if not self.are_tool_images_assigned:
+            self.assign_tool_image_instances_to_all_dev_envs()
+
         all_required_tool_images = set()
         for dev_env in self.local_dev_envs:
             if (dev_env is not dev_env_to_uninstall) and dev_env.is_installed:
-                for tool_image_descriptor in dev_env.tool_image_descriptors:
-                    all_required_tool_images.add(tool_image_descriptor["image_name"] + ":" + tool_image_descriptor["image_version"])
+                for tool_image in dev_env.tool_images:
+                    all_required_tool_images.add(tool_image.name)
 
         tool_images_to_remove = set()
-        for tool_image_descriptor in dev_env_to_uninstall.tool_image_descriptors:
-            tool_image_name = tool_image_descriptor["image_name"] + ":" + tool_image_descriptor["image_version"]
-            if tool_image_name not in all_required_tool_images:
-                tool_images_to_remove.add(tool_image_name)
+        for tool_image in dev_env_to_uninstall.tool_images:
+            if tool_image.availability == ToolImage.NOT_AVAILABLE or tool_image.availability == ToolImage.REGISTRY_ONLY:
+                yield f"[yellow]Warning: The {tool_image.name} image could not be removed, because it is not available locally.[/]"
+                continue
+
+            if tool_image.name not in all_required_tool_images:
+                tool_images_to_remove.add(tool_image.name)
 
         for tool_image_name in tool_images_to_remove:
             try:
                 self.container_engine.remove(tool_image_name)
             except ContainerEngineError as e:
                 raise PlatformError(f"Dev Env uninstall failed. --> {str(e)}")
+            else:
+                yield f"The {tool_image_name} image has been removed."
             
         dev_env_to_uninstall.is_installed = False
-        self.flush_descriptors()
+        if self.default_dev_env_name == dev_env_to_uninstall.name:
+            self.default_dev_env_name = ""
+        self.flush_dev_env_properties()
 
-    def flush_descriptors(self) -> None:
+    def flush_dev_env_properties(self) -> None:
         """ Writes the deserialized json to the dev_env.json file."""
         # Get the up-to-date deserialized data.
         self.dev_env_json.deserialized = self.get_deserialized()
         self.dev_env_json.flush()
 
     def assign_dev_env(self, dev_env_to_assign: DevEnv, project_path: str) -> None:
         """ Assign the Development Environment to the project, by exporting the Dev Env's desriptor
```

### Comparing `axem_dem-0.5.0/dem/core/registry.py` & `axem_dem-0.6.0/dem/core/registry.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/dem/core/tool_images.py` & `axem_dem-0.6.0/dem/core/tool_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """
         self.container_engine = container_engine
         self.registries = registries
         self.all_tool_images = {}
 
     def update(self, local_only: bool = False, registry_only: bool = False, 
                reg_selection: list[str] = []) -> None:
-        """ Update the list of available tools.
+        """ Update the list of available tools. If the tool image already exists, it will be updated.
         
             Args:
                 local_only -- update the local tools only
                 registry_only -- update the registry tools only
         """
         registry_tool_image_names = []
         local_tool_image_names = []
@@ -60,24 +60,24 @@
         if not registry_only:
             local_tool_image_names = self.container_engine.get_local_tool_images()
 
         if not local_only:
             registry_tool_image_names = self.registries.list_repos(reg_selection)
 
         for tool_image_name in local_tool_image_names:
-            tool_image = ToolImage(tool_image_name)
+            tool_image = self.all_tool_images.get(tool_image_name, ToolImage(tool_image_name))
             if tool_image_name in registry_tool_image_names:
                 tool_image.availability = ToolImage.LOCAL_AND_REGISTRY
             else:
                 tool_image.availability = ToolImage.LOCAL_ONLY
             self.all_tool_images[tool_image_name] = tool_image
 
         for tool_image_name in registry_tool_image_names:
             if tool_image_name not in local_tool_image_names:
-                tool_image = ToolImage(tool_image_name)
+                tool_image = self.all_tool_images.get(tool_image_name, ToolImage(tool_image_name))
                 tool_image.availability = ToolImage.REGISTRY_ONLY
                 self.all_tool_images[tool_image_name] = tool_image
 
     def get_local_ones(self) -> dict[str, ToolImage]:
         """ Get the local tool images.
         
             Return with the local tool images.
```

### Comparing `axem_dem-0.5.0/dem/core/user_output.py` & `axem_dem-0.6.0/dem/core/user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.5.0/pyproject.toml` & `axem_dem-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "axem-dem"
-version = "0.5.0"
+version = "0.6.0"
 description = "Manager for Containerized Development Environments"
 authors = ["Janos Murai <janos.murai@axemsolutions.io>"]
 license = "Eclipse Public License - v2.0"
 readme = "README.md"
 homepage = "https://axemsolutions.io/"
 documentation = "https://axemsolutions.io/dem_doc/"
 repository = "https://github.com/axem-solutions/dem"
```

### Comparing `axem_dem-0.5.0/PKG-INFO` & `axem_dem-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axem-dem
-Version: 0.5.0
+Version: 0.6.0
 Summary: Manager for Containerized Development Environments
 Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0
 Keywords: iot,embedded,edge,development environment,tools,containers
 Author: Janos Murai
 Author-email: janos.murai@axemsolutions.io
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: axem-dem Version: 0.5.0 Summary: Manager for
+Metadata-Version: 2.1 Name: axem-dem Version: 0.6.0 Summary: Manager for
 Containerized Development Environments Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0 Keywords: iot,embedded,edge,development
 environment,tools,containers Author: Janos Murai Author-email:
 janos.murai@axemsolutions.io Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Programming
```

