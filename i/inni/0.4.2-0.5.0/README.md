# Comparing `tmp/inni-0.4.2.tar.gz` & `tmp/inni-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inni-0.4.2.tar", max compression
+gzip compressed data, was "inni-0.5.0.tar", max compression
```

## Comparing `inni-0.4.2.tar` & `inni-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.4.2/LICENSE
--rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.4.2/inni/__init__.py
--rw-r--r--   0        0        0     4189 2024-04-26 09:01:57.398706 inni-0.4.2/inni/cli.py
--rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.4.2/inni/config.py
--rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.4.2/inni/loader.py
--rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.4.2/inni/modules/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.4.2/inni/modules/base.py
--rw-r--r--   0        0        0     3299 2024-04-23 10:24:40.930217 inni-0.4.2/inni/modules/bitrix.py
--rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.4.2/inni/modules/dummy.py
--rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.4.2/inni/modules/email.py
--rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.4.2/inni/modules/jira.py
--rw-r--r--   0        0        0     3204 2024-04-24 06:28:15.343430 inni-0.4.2/inni/modules/runner.py
--rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.4.2/inni/modules/skype.py
--rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.4.2/inni/template.py
--rw-r--r--   0        0        0      742 2024-04-26 09:03:29.416926 inni-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 inni-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.5.0/LICENSE
+-rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.5.0/inni/__init__.py
+-rw-r--r--   0        0        0     4900 2024-05-07 09:05:03.056356 inni-0.5.0/inni/cli.py
+-rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.5.0/inni/config.py
+-rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.5.0/inni/loader.py
+-rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.5.0/inni/modules/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.5.0/inni/modules/base.py
+-rw-r--r--   0        0        0     3299 2024-04-23 10:24:40.930217 inni-0.5.0/inni/modules/bitrix.py
+-rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.5.0/inni/modules/dummy.py
+-rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.5.0/inni/modules/email.py
+-rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.5.0/inni/modules/jira.py
+-rw-r--r--   0        0        0     3204 2024-04-24 06:28:15.343430 inni-0.5.0/inni/modules/runner.py
+-rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.5.0/inni/modules/skype.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.5.0/inni/template.py
+-rw-r--r--   0        0        0      742 2024-05-07 09:29:02.762823 inni-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 inni-0.5.0/PKG-INFO
```

### Comparing `inni-0.4.2/LICENSE` & `inni-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/cli.py` & `inni-0.5.0/inni/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,20 +36,34 @@
     if vars_module.exists():
         module_dir = vars_module.parent
         sys.path.append(str(module_dir))
         ctx.obj["vars"] = import_module(vars_module.name.removesuffix(".py"))
         sys.path.remove(str(module_dir))
 
 
-def _login_out(ctx: click.Context, login: bool, override_modules: Optional[str]):
+def _login_out(
+    ctx: click.Context,
+    login: bool,
+    override_modules: Optional[str],
+    skip_modules: Optional[str] = None,
+):
     config = ctx.obj["config"]
     module_names = config["inni"]["login" if login else "logout"]
     if override_modules:
         console.print("[yellow] CLI modules override the modules defined in config")
         module_names = [i.strip() for i in override_modules.split(",")]
+
+    if skip_modules:
+        modules_to_skip = [i.strip() for i in skip_modules.split(",")]
+        for module in modules_to_skip:
+            if module in module_names:
+                console.print(f"[yellow] Skipping module: [bold]{module}")
+                module_names.remove(module)
+            else:
+                console.print(f"[yellow] Module [bold]{module}[/bold] is not present.")
     prompts = config["inni"]["prompts"]
     modules = {}
 
     with console.status("") as status:
         for module_name in module_names:
             status.update(f"[green]Initializing {module_name}")
             try:
@@ -91,34 +105,44 @@
         except Exception:
             error_console.print(f"[red bold]Fatal error occured running module {name}")
             error_console.print_exception()
 
 
 @inni.command()
 @click.option("-m", "--modules", help="Modules to run (overrides config modules)")
+@click.option("-s", "--skip-modules", help="Modules to skip")
 @click.pass_context
-def login(ctx: click.Context, modules: Optional[str] = None):
+def login(
+    ctx: click.Context,
+    modules: Optional[str] = None,
+    skip_modules: Optional[str] = None,
+):
     """
     Login today
 
     Runs all the login modules along with prompting for user input
     """
-    return _login_out(ctx, True, modules)
+    return _login_out(ctx, True, modules, skip_modules)
 
 
 @inni.command()
 @click.option("-m", "--modules", help="Modules to run (overrides config modules)")
+@click.option("-s", "--skip-modules", help="Modules to skip")
 @click.pass_context
-def logout(ctx: click.Context, modules: Optional[str] = None):
+def logout(
+    ctx: click.Context,
+    modules: Optional[str] = None,
+    skip_modules: Optional[str] = None,
+):
     """
     Logout today
 
     Runs all the login modules along with prompting for user input
     """
-    return _login_out(ctx, False, modules)
+    return _login_out(ctx, False, modules, skip_modules)
 
 
 @inni.command()
 def download_browser():
     """
     Download Firefox for bitrix module
```

### Comparing `inni-0.4.2/inni/config.py` & `inni-0.5.0/inni/config.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/base.py` & `inni-0.5.0/inni/modules/base.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/bitrix.py` & `inni-0.5.0/inni/modules/bitrix.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/email.py` & `inni-0.5.0/inni/modules/email.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/jira.py` & `inni-0.5.0/inni/modules/jira.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/runner.py` & `inni-0.5.0/inni/modules/runner.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/inni/modules/skype.py` & `inni-0.5.0/inni/modules/skype.py`

 * *Files identical despite different names*

### Comparing `inni-0.4.2/pyproject.toml` & `inni-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inni"
-version = "0.4.2"
+version = "0.5.0"
 description = "Modular system to perform tasks surrounding log-in and log-out."
 authors = ["Ceda EI <ceda_ei@webionite.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://gitlab.com/ceda_ei/inni"
 repository = "https://gitlab.com/ceda_ei/inni"
```

### Comparing `inni-0.4.2/PKG-INFO` & `inni-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inni
-Version: 0.4.2
+Version: 0.5.0
 Summary: Modular system to perform tasks surrounding log-in and log-out.
 Home-page: https://gitlab.com/ceda_ei/inni
 License: GPL-3.0
 Author: Ceda EI
 Author-email: ceda_ei@webionite.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

