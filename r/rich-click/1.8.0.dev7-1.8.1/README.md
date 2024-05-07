# Comparing `tmp/rich_click-1.8.0.dev7.tar.gz` & `tmp/rich_click-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_click-1.8.0.dev7.tar", last modified: Wed Apr 24 02:31:58 2024, max compression
+gzip compressed data, was "rich_click-1.8.1.tar", last modified: Tue May  7 13:05:34 2024, max compression
```

## Comparing `rich_click-1.8.0.dev7.tar` & `rich_click-1.8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.519460 rich_click-1.8.0.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.523460 rich_click-1.8.0.dev7/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31100 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 13:05:30.000000 rich_click-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 13:05:34.737436 rich_click-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-07 13:05:30.000000 rich_click-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 13:05:30.000000 rich_click-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:05:34.737436 rich_click-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.733436 rich_click-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.733436 rich_click-1.8.1/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31289 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_rich_click_cli.py
```

### Comparing `rich_click-1.8.0.dev7/LICENSE` & `rich_click-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/PKG-INFO` & `rich_click-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev7
+Version: 1.8.1
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -60,14 +60,15 @@
 Requires-Dist: types-setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: markdown_include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
 Requires-Dist: mkdocs-material[imaging]~=9.5.18; extra == "docs"
 Requires-Dist: mkdocs-material-extensions; extra == "docs"
+Requires-Dist: mkdocs-rss-plugin; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: rich-codex; extra == "docs"
 
 <p align="center">
     <picture>
         <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo-darkmode.png">
         <img alt="rich-click logo" src="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo.png">
@@ -161,15 +162,15 @@
 
 ```python
 import rich_click as click
 ```
 
 That's it! ✨ Then continue to use Click as you would normally.
 
-> See [`examples/01_simple.py`](examples/01_simple.py) for an example.
+> See [`examples/01_simple.py`](https://github.com/ewels/rich-click/blob/main/examples/01_simple.py) for an example.
 
 ### Declarative
 
 If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
 ```python
@@ -177,15 +178,15 @@
 from rich_click import RichCommand
 
 @click.command(cls=RichCommand)
 def main():
     """My amazing tool does all the things."""
 ```
 
-> See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
+> See [`examples/02_declarative.py`](https://github.com/ewels/rich-click/blob/main/examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
 For example, to get richified Click help text from a package called `awesometool`, you could run:
```

### Comparing `rich_click-1.8.0.dev7/README.md` & `rich_click-1.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 ```python
 import rich_click as click
 ```
 
 That's it! ✨ Then continue to use Click as you would normally.
 
-> See [`examples/01_simple.py`](examples/01_simple.py) for an example.
+> See [`examples/01_simple.py`](https://github.com/ewels/rich-click/blob/main/examples/01_simple.py) for an example.
 
 ### Declarative
 
 If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
 ```python
@@ -108,15 +108,15 @@
 from rich_click import RichCommand
 
 @click.command(cls=RichCommand)
 def main():
     """My amazing tool does all the things."""
 ```
 
-> See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
+> See [`examples/02_declarative.py`](https://github.com/ewels/rich-click/blob/main/examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
 For example, to get richified Click help text from a package called `awesometool`, you could run:
```

### Comparing `rich_click-1.8.0.dev7/pyproject.toml` & `rich_click-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ]
 docs = [
     "markdown_include",
     "mkdocs",
     "mkdocs-glightbox",
     "mkdocs-material[imaging]~=9.5.18",
     "mkdocs-material-extensions",
+    "mkdocs-rss-plugin",
     "mkdocstrings[python]",
     "rich-codex",
 ]
 [project.urls]
 Documentation = "https://github.com/ewels/rich-click"
 Homepage = "https://github.com/ewels/rich-click"
 Issues = "https://github.com/ewels/rich-click/issues"
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/__init__.py` & `rich_click-1.8.1/src/rich_click/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev7"
+__version__ = "1.8.1"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/_compat_click.py` & `rich_click-1.8.1/src/rich_click/_compat_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 
 
 try:
     click_version = click.__version__
-except NameError:
+except Exception:
     # Click 9+ deprecated __version__, so all these checks must necessarily be False if __version__ doesn't exist.
     CLICK_IS_BEFORE_VERSION_8X = False
     CLICK_IS_BEFORE_VERSION_9X = False
     CLICK_IS_VERSION_80 = False
 else:
     _major = int(click_version.split(".")[0])
     _minor = int(click_version.split(".")[1])
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/cli.py` & `rich_click-1.8.1/src/rich_click/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # ruff: noqa: D103
 
 import os
 import sys
 from functools import wraps
 from gettext import gettext as _
 from importlib import import_module
-from typing import Any, List, Optional, Union
+from typing import Any, List, Optional, Tuple, Union
 
 from typing_extensions import Literal
 
 
 try:
     from importlib import metadata  # type: ignore[import,unused-ignore]
 except ImportError:
@@ -89,14 +89,62 @@
                 if ctx is not None and ctx.params.get("show_help", False):
                     click.echo(ctx.get_help(), color=ctx.color)
                     ctx.exit()
                 else:
                     raise e
 
 
+def _get_module_path_and_function_name(script: str, suppress_warnings: bool) -> Tuple[str, str]:
+    _selected: List[str] = []
+    module_path = ""
+    function_name = ""
+
+    for s in entry_points(group="console_scripts"):
+        if script == s.name:
+            if not _selected:
+                module_path, function_name = s.value.split(":", 1)
+            if suppress_warnings:
+                break
+            if s.value not in _selected:
+                _selected.append(s.value)
+
+    if len(_selected) > 1 and not suppress_warnings:
+        # This is an extremely rare edge case that comes up when the user sets the PYTHONPATH themselves.
+        if script in sys.argv:
+            _args = sys.argv.copy()
+            _args[_args.index(script)] = f"{module_path}:{function_name}"
+        else:
+            _args = ["rich-click", f"{module_path}:{function_name}"]
+
+        click.echo(
+            click.style(
+                f"WARNING: Multiple entry_points correspond with script '{script}': {_selected!r}."
+                "\nThis can happen when an 'egg-info' directory exists, you're using a virtualenv,"
+                " and you have set a custom PYTHONPATH."
+                f"\n\nThe selected script is '{module_path}:{function_name}', which is being executed now."
+                "\n\nIt is safer and recommended that you specify the MODULE:CLICK_COMMAND"
+                f" ('{module_path}:{function_name}') instead of the script ('{script}'), like this:"
+                f"\n\n>>> rich-click {' '.join(_args)}"
+                "\n\nAlternatively, you can pass --suppress-warnings to the rich-click CLI,"
+                " which will disable this message.",
+                fg="red",
+            ),
+            file=sys.stderr,
+        )
+
+    if ":" in script and not module_path:
+        # the path to a function was passed
+        module_path, function_name = script.split(":", 1)
+
+    if not module_path:
+        raise click.ClickException(f"No such script: {script}")
+
+    return module_path, function_name
+
+
 @_rich_command("rich-click", context_settings=dict(allow_interspersed_args=False, help_option_names=[]))
 @click.argument("script_and_args", nargs=-1, metavar="[SCRIPT | MODULE:CLICK_COMMAND] [-- SCRIPT_ARGS...]")
 @click.option(
     "--rich-config",
     "-c",
     type=_RichHelpConfigurationParamType(),
     help="Keyword arguments to pass into the [de]RichHelpConfiguration()[/] used"
@@ -169,73 +217,35 @@
         if rich_config is not None:
             rich_config.use_markdown = False
             rich_config.use_rich_markup = True
             ctx.help_config = rich_config
         click.echo(ctx.get_help(), color=ctx.color)
         ctx.exit()
 
-    script, *args = script_and_args
-
-    _selected: List[str] = []
-    module_path = ""
-    function_name = ""
-
-    for s in entry_points(group="console_scripts"):
-        if script == s.name:
-            if not _selected:
-                module_path, function_name = s.value.split(":", 1)
-            if suppress_warnings:
-                break
-            if s.value not in _selected:
-                _selected.append(s.value)
+    # patch click before importing the program function
+    _patch(rich_config=rich_config)
 
-    if len(_selected) > 1 and not suppress_warnings:
-        # This is an extremely rare edge case that comes up when the user sets the PYTHONPATH themselves.
-        if script in sys.argv:
-            _args = sys.argv.copy()
-            _args[_args.index(script)] = f"{module_path}:{function_name}"
-        else:
-            _args = ["rich-click", f"{module_path}:{function_name}"]
+    script, *args = script_and_args
 
-        click.echo(
-            click.style(
-                f"WARNING: Multiple entry_points correspond with script '{script}': {_selected!r}."
-                "\nThis can happen when an 'egg-info' directory exists, you're using a virtualenv,"
-                " and you have set a custom PYTHONPATH."
-                f"\n\nThe selected script is '{module_path}:{function_name}', which is being executed now."
-                "\n\nIt is safer and recommended that you specify the MODULE:CLICK_COMMAND"
-                f" ('{module_path}:{function_name}') instead of the script ('{script}'), like this:"
-                f"\n\n>>> rich-click {' '.join(_args)}"
-                "\n\nAlternatively, you can pass --suppress-warnings to the rich-click CLI,"
-                " which will disable this message.",
-                fg="red",
-            ),
-            file=sys.stderr,
-        )
+    # import the program function
+    try:
+        module_path, function_name = _get_module_path_and_function_name(script, suppress_warnings)
+        module = import_module(module_path)
+    except (ModuleNotFoundError, click.ClickException):
+        sys.path.append(os.path.abspath("."))
+        # PYTHONPATH can change output of entry_points(group="console_scripts") in rare cases,
+        # so we want to rerun the whole search
+        module_path, function_name = _get_module_path_and_function_name(script, suppress_warnings)
+        module = import_module(module_path)
 
-    if ":" in script and not module_path:
-        # the path to a function was passed
-        module_path, function_name = script.split(":", 1)
+    function = getattr(module, function_name)
 
-    if not module_path:
-        raise click.ClickException(f"No such script: {script_and_args[0]}")
+    if output is not None:
+        RichContext.export_console_as = output
 
     prog = module_path.split(".", 1)[0]
     sys.argv = [prog, *args]
 
-    # patch click before importing the program function
-    _patch(rich_config=rich_config)
-    # import the program function
-    module = import_module(module_path)
-    function = getattr(module, function_name)
-    # simply run it: it should be patched as well
-    if output is not None:
-        ctx.help_config = RichHelpConfiguration.load_from_globals()
-        RichContext.console = console = ctx.make_formatter().console
-        console.record = True
-        console.file = open(os.devnull, "w")
-        RichContext.export_console_as = output
-
     if ctx.resilient_parsing and isinstance(function, click.Command):
         function.main(resilient_parsing=True)
     else:
         function()
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/decorators.py` & `rich_click-1.8.1/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/src/rich_click/patch.py` & `rich_click-1.8.1/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_click.py` & `rich_click-1.8.1/src/rich_click/rich_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 # Behaviours
 SHOW_ARGUMENTS: bool = False  # Show positional arguments
 SHOW_METAVARS_COLUMN: bool = True  # Show a column with the option metavar (eg. INTEGER)
 APPEND_METAVARS_HELP: bool = False  # Append metavar (eg. [TEXT]) after the help text
 GROUP_ARGUMENTS_OPTIONS: bool = False  # Show arguments with options instead of in own panel
 OPTION_ENVVAR_FIRST: bool = False  # Show env vars before option help text instead of avert
-TEXT_MARKUP: Literal["rich", "markdown", None] = None
+TEXT_MARKUP: Literal["ansi", "rich", "markdown", None] = "ansi"
 USE_MARKDOWN: bool = False  # Parse help strings as markdown
 USE_MARKDOWN_EMOJI: bool = True  # Parse emoji codes in markdown :smile:
 USE_RICH_MARKUP: bool = False  # Parse help strings for rich markup (eg. [red]my text[/])
 # Define sorted groups of panels to display subcommands
 COMMAND_GROUPS: Dict[str, List[CommandGroupDict]] = {}
 # Define sorted groups of panels to display options and arguments
 OPTION_GROUPS: Dict[str, List[OptionGroupDict]] = {}
@@ -112,26 +112,28 @@
             DeprecationWarning,
             stacklevel=2,
         )
         from rich_click.rich_help_configuration import RichHelpConfiguration
 
         return RichHelpConfiguration.load_from_globals
     if name == "highlighter":
-        import warnings
+        # TODO: Fix deprecation warning. For now, exclude.
 
-        from rich_click.rich_help_configuration import OptionHighlighter
+        # import warnings
 
-        warnings.warn(
-            "`highlighter` config option is deprecated."
-            " Please do one of the following instead: either set HIGHLIGHTER_PATTERNS = [...] if you want"
-            " to use regex; or for more advanced use cases where you'd like to use a different type"
-            " of rich.highlighter.Highlighter, subclass the `RichHelpFormatter` and update its `highlighter`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
+        # warnings.warn(
+        #     "`highlighter` config option is deprecated."
+        #     " Please do one of the following instead: either set HIGHLIGHTER_PATTERNS = [...] if you want"
+        #     " to use regex; or for more advanced use cases where you'd like to use a different type"
+        #     " of rich.highlighter.Highlighter, subclass the `RichHelpFormatter` and update its `highlighter`.",
+        #     DeprecationWarning,
+        #     stacklevel=2,
+        # )
+
+        from rich_click.rich_help_configuration import OptionHighlighter
 
         globals()["highlighter"] = highlighter = OptionHighlighter()
         return highlighter
 
     elif name in {
         "_make_rich_rext",
         "_get_help_text",
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_command.py` & `rich_click-1.8.1/src/rich_click/rich_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import errno
 import os
 import sys
 import warnings
-from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, List, Mapping, Optional, Sequence, TextIO, Type, Union, cast, overload
 
 import click
 
 # Group, Command, and CommandCollection need to be imported directly,
 # or else rich_click.cli.patch() causes a recursion error.
-from click import Command, CommandCollection, Group
+from click import CommandCollection, Group
 from click.utils import PacifyFlushWrapper, make_str
 
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X, CLICK_IS_BEFORE_VERSION_9X
 from rich_click.rich_context import RichContext
 from rich_click.rich_help_configuration import RichHelpConfiguration
 from rich_click.rich_help_formatter import RichHelpFormatter
 
@@ -37,15 +36,14 @@
 
     This class can be used as a mixin for other click command objects.
     """
 
     context_class: Type[RichContext] = RichContext
     _formatter: Optional[RichHelpFormatter] = None
 
-    @wraps(Command.__init__)
     def __init__(self, *args: Any, **kwargs: Any):
         """Create Rich Command instance."""
         super().__init__(*args, **kwargs)
         self._register_rich_context_settings_from_callback()
 
     def _register_rich_context_settings_from_callback(self) -> None:
         if self.callback is not None:
@@ -218,18 +216,24 @@
             self.format_epilog(ctx, formatter)
 
     def format_help_text(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
         from rich_click.rich_help_rendering import get_rich_help_text
 
         get_rich_help_text(self, ctx, formatter)
 
-    def format_options(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
+    # TODO:
+    #  Switching from base click to rich click causes mypy problems.
+    #  Either we: (a) swap MRO (incompatible with click 9, without handling 8 and 9 differently)
+    #  or (b) we allow issues when users attempt multiple inheritance with a RichCommand
+    #  or (c) we use incorrect types here.
+    #  We are looking for a solution that fixes all 3. For now, we opt for (c).
+    def format_options(self, ctx: click.Context, formatter: click.HelpFormatter) -> None:
         from rich_click.rich_help_rendering import get_rich_options
 
-        get_rich_options(self, ctx, formatter)
+        get_rich_options(self, ctx, formatter)  # type: ignore[arg-type]
 
     def format_epilog(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
         from rich_click.rich_help_rendering import get_rich_epilog
 
         get_rich_epilog(self, ctx, formatter)
 
     def make_context(
@@ -262,61 +266,60 @@
         from click import MultiCommand
 
 else:
 
     MultiCommand = Group  # type: ignore[misc,assignment]
 
 
-class RichMultiCommand(MultiCommand, RichCommand):
+class RichMultiCommand(RichCommand, MultiCommand):
     """
     Richly formatted click MultiCommand.
 
     Inherits click.MultiCommand and overrides help and error methods
     to print richly formatted output.
     """
 
-    @wraps(MultiCommand.__init__)
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize RichMultiCommand class."""
         MultiCommand.__init__(self, *args, **kwargs)
         self._register_rich_context_settings_from_callback()
 
     def format_commands(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
         from rich_click.rich_help_rendering import get_rich_commands
 
         get_rich_commands(self, ctx, formatter)
 
-    def format_options(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
+    def format_options(self, ctx: click.Context, formatter: click.HelpFormatter) -> None:
         from rich_click.rich_help_rendering import get_rich_options
 
-        get_rich_options(self, ctx, formatter)
-        self.format_commands(ctx, formatter)
+        get_rich_options(self, ctx, formatter)  # type: ignore[arg-type]
+
+        self.format_commands(ctx, formatter)  # type: ignore[arg-type]
 
     def format_help(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
         if OVERRIDES_GUARD:
             prevent_incompatible_overrides(self, "RichMultiCommand", ctx, formatter)
         else:
             self.format_usage(ctx, formatter)
             self.format_help_text(ctx, formatter)
             self.format_options(ctx, formatter)
             self.format_epilog(ctx, formatter)
 
 
-class RichGroup(Group, RichMultiCommand):
+class RichGroup(RichMultiCommand, Group):
     """
     Richly formatted click Group.
 
     Inherits click.Group and overrides help and error methods
     to print richly formatted output.
     """
 
     command_class: Optional[Type[RichCommand]] = RichCommand
     group_class: Optional[Union[Type[Group], Type[type]]] = type
 
-    @wraps(Group.__init__)
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize RichGroup class."""
         Group.__init__(self, *args, **kwargs)
         self._register_rich_context_settings_from_callback()
 
     @overload
     def command(self, __func: Callable[..., Any]) -> RichCommand: ...
@@ -360,23 +363,22 @@
         """Alias for :meth:`main`."""
         # Include this here because I run into a false warning
         # in the PyCharm IDE otherwise; for some reason PyCharm doesn't
         # seem to think RichGroups are callable. (No issues with Mypy, though.)
         return super().__call__(*args, **kwargs)
 
 
-class RichCommandCollection(RichGroup, CommandCollection):
+class RichCommandCollection(CommandCollection, RichGroup):
     """
     Richly formatted click CommandCollection.
 
     Inherits click.CommandCollection and overrides help and error methods
     to print richly formatted output.
     """
 
-    @wraps(CommandCollection.__init__)
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize RichCommandCollection class."""
         CommandCollection.__init__(self, *args, **kwargs)
         self._register_rich_context_settings_from_callback()
 
     def format_help(self, ctx: RichContext, formatter: RichHelpFormatter) -> None:  # type: ignore[override]
         if OVERRIDES_GUARD:
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_context.py` & `rich_click-1.8.1/src/rich_click/rich_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Type, Union
 
 import click
 from typing_extensions import Literal, NoReturn
 
 from rich_click.rich_help_configuration import RichHelpConfiguration
 from rich_click.rich_help_formatter import RichHelpFormatter
@@ -66,15 +67,20 @@
     def make_formatter(self) -> RichHelpFormatter:
         """Create the Rich Help Formatter."""
         formatter = self.formatter_class(
             width=self.terminal_width,
             max_width=self.max_content_width,
             config=self.help_config,
             console=self.console,
+            file=open(os.devnull, "w") if self.export_console_as is not None else None,
         )
+        if self.export_console_as is not None:
+            if self.console is None:
+                self.console = formatter.console
+            self.console.record = True
         return formatter
 
     if TYPE_CHECKING:
 
         def __enter__(self) -> "RichContext":
             return super().__enter__()  # type: ignore[return-value]
 
@@ -83,13 +89,13 @@
             exc_type: Optional[Type[BaseException]],
             exc_value: Optional[BaseException],
             tb: Optional[TracebackType],
         ) -> None:
             return super().__exit__(exc_type, exc_value, tb)
 
     def exit(self, code: int = 0) -> NoReturn:
-        if self.console is not None and self.console.record:
+        if self.export_console_as is not None and self.console is not None and self.console.record:
             if self.export_console_as == "html":
                 print(self.console.export_html(inline_styles=True, code_format="{code}"))
             elif self.export_console_as == "svg":
                 print(self.console.export_svg())
         super().exit(code)
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_help_configuration.py` & `rich_click-1.8.1/src/rich_click/rich_help_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     """Show a column with the option metavar (eg. INTEGER)"""
     append_metavars_help: bool = field(default=False)
     """Append metavar (eg. [TEXT]) after the help text"""
     group_arguments_options: bool = field(default=False)
     """Show arguments with options instead of in own panel"""
     option_envvar_first: bool = field(default=False)
     """Show env vars before option help text instead of after"""
-    text_markup: Literal["rich", "markdown", None] = None
+    text_markup: Literal["ansi", "rich", "markdown", None] = "ansi"
     use_markdown: bool = field(default=False)
     """Silently deprecated; use `text_markup` field instead."""
     use_markdown_emoji: bool = field(default=True)
     """Parse emoji codes in markdown :smile:"""
     use_rich_markup: bool = field(default=False)
     """Silently deprecated; use `text_markup` field instead."""
     command_groups: Dict[str, List[CommandGroupDict]] = field(default_factory=lambda: {})
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_help_formatter.py` & `rich_click-1.8.1/src/rich_click/rich_help_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 
 if sys.version_info >= (3, 8):
     from functools import cached_property
 else:
     cached_property = property
 
 
-def create_console(
-    config: RichHelpConfiguration,
-    file: Optional[IO[str]] = None,
-) -> "Console":
+def create_console(config: RichHelpConfiguration, file: Optional[IO[str]] = None) -> "Console":
     """
     Create a Rich Console configured from Rich Help Configuration.
 
     Args:
     ----
         config: Rich Help Configuration instance
         file: Optional IO stream to write Rich Console output
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/rich_help_rendering.py` & `rich_click-1.8.1/src/rich_click/rich_help_rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,33 +59,41 @@
     Returns:
     -------
         MarkdownElement or Text: Styled text object
     """
     config = formatter.config
     # Remove indentations from input text
     text = inspect.cleandoc(text)
-    if config.text_markup == "markdown":
+
+    use_ansi = False
+    use_markdown = False
+    use_rich = False
+
+    if config.use_markdown:
+        use_markdown = True
+    elif config.use_rich_markup:
+        use_rich = True
+    elif config.text_markup == "markdown":
         use_markdown = True
-        use_rich = False
     elif config.text_markup == "rich":
-        use_markdown = False
         use_rich = True
-    else:
-        use_markdown = config.use_markdown
-        use_rich = config.use_rich_markup
+    elif config.text_markup == "ansi":
+        use_ansi = True
 
     # TODO:
     #  In a future major version release, decouple emojis and markdown.
     #  Decoupling isn't something that is sensible without breaking the API.
     if use_markdown:
         if config.use_markdown_emoji:
             text = Emoji.replace(text)
         return Markdown(text, style=style)
     elif use_rich:
         return formatter.highlighter(Text.from_markup(text, style=style))
+    elif use_ansi:
+        return formatter.highlighter(Text.from_ansi(text, style=style))
     else:
         return formatter.highlighter(Text(text, style=style))
 
 
 @group()
 def _get_help_text(obj: Union[Command, Group], formatter: RichHelpFormatter) -> Iterable[Union[Markdown, Text]]:
     """
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click/utils.py` & `rich_click-1.8.1/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/src/rich_click.egg-info/PKG-INFO` & `rich_click-1.8.1/src/rich_click.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev7
+Version: 1.8.1
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -60,14 +60,15 @@
 Requires-Dist: types-setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: markdown_include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
 Requires-Dist: mkdocs-material[imaging]~=9.5.18; extra == "docs"
 Requires-Dist: mkdocs-material-extensions; extra == "docs"
+Requires-Dist: mkdocs-rss-plugin; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: rich-codex; extra == "docs"
 
 <p align="center">
     <picture>
         <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo-darkmode.png">
         <img alt="rich-click logo" src="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo.png">
@@ -161,15 +162,15 @@
 
 ```python
 import rich_click as click
 ```
 
 That's it! ✨ Then continue to use Click as you would normally.
 
-> See [`examples/01_simple.py`](examples/01_simple.py) for an example.
+> See [`examples/01_simple.py`](https://github.com/ewels/rich-click/blob/main/examples/01_simple.py) for an example.
 
 ### Declarative
 
 If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
 ```python
@@ -177,15 +178,15 @@
 from rich_click import RichCommand
 
 @click.command(cls=RichCommand)
 def main():
     """My amazing tool does all the things."""
 ```
 
-> See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
+> See [`examples/02_declarative.py`](https://github.com/ewels/rich-click/blob/main/examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
 For example, to get richified Click help text from a package called `awesometool`, you could run:
```

### Comparing `rich_click-1.8.0.dev7/src/rich_click.egg-info/SOURCES.txt` & `rich_click-1.8.1/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/tests/test_config.py` & `rich_click-1.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/tests/test_exit_code.py` & `rich_click-1.8.1/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/tests/test_help.py` & `rich_click-1.8.1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev7/tests/test_rich_click_cli.py` & `rich_click-1.8.1/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

