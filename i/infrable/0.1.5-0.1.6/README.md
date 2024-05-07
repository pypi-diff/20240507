# Comparing `tmp/infrable-0.1.5.tar.gz` & `tmp/infrable-0.1.6.tar.gz`

## Comparing `infrable-0.1.5.tar` & `infrable-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.5/.envrc
--rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 infrable-0.1.5/.null-ls_186313_README.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/errors.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/files.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/host.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/infra.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/paths.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/readfile.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/service.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/template.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/files.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/main.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.5/LICENSE
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 infrable-0.1.5/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    31637 2020-02-02 00:00:00.000000 infrable-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.6/.envrc
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.6/.null-ls_767818_README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/errors.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/files.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/host.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/infra.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/paths.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/readfile.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/service.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/template.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/files.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/main.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.6/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.6/LICENSE
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 infrable-0.1.6/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    31622 2020-02-02 00:00:00.000000 infrable-0.1.6/PKG-INFO
```

### Comparing `infrable-0.1.5/.null-ls_186313_README.md` & `infrable-0.1.6/.null-ls_767818_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 [![PyPI version](https://img.shields.io/pypi/v/infrable.svg)](https://pypi.org/project/infrable)
 
 ```bash
 # Install
 pip install -U infrable  # requires python >= 3.10
 
 # Bootstrap a new project
-touch infra.py
 infrable init
 ```
 
 # Table of contents
 
 1. [Prologue](#prologue)
 2. [Chapter 1 - Chaos](#chapter-1---chaos)
@@ -282,28 +281,27 @@
 As she toiled to realize this vision, a brilliant idea swept over her - to
 orchestrate these tasks into coherent sequences, she christened them
 **"workflows"**, heralding the dawn of a new era in infrastructure management.
 
 **infra.py**
 
 ```python
-from infrable import parallel, paths
+from infrable import concurrent, paths
 
 # Workflows/ -----------------------------------------------------------------------
 deploy = typer.Typer(help="Deployment workflows.")
 
 @deploy.command(name="dev-nginx")
 def deploy_dev_nginx():
     """[WORKFLOW] Deploy dev_nginx files: infrable deploy dev-nginx"""
 
     files.deploy(paths.templates / "nginx")
-    hosts = files.affected_hosts()
     cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
-    tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
-    for host, result in concurrent(tasks):
+    fn = lambda host: (host, host.remote().sudo(cmd))
+    for host, result in concurrent(fn, files.affected_hosts()):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
 Running workflows:
 
 ```bash
```

### Comparing `infrable-0.1.5/infrable/errors.py` & `infrable-0.1.6/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/files.py` & `infrable-0.1.6/infrable/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/host.py` & `infrable-0.1.6/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/infra.py` & `infrable-0.1.6/infrable/infra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import sys
 from typing import Any, Iterable, Type
 
 from typer import Typer
 
-from infrable import errors
+from infrable import INFRA_MODULE_NAME, errors
 from infrable.host import Host
 from infrable.meta import Meta
 from infrable.service import Service
 from infrable.switch import Switch
 
-INFRA_MODULE_NAME = "infra"
-
 items: dict[str, Any] = {}
 item_types: dict[Type[Any], dict[str, Any]] = {}
 
 hosts: dict[str, Host] = {}
 services: dict[str, Service] = {}
 host_groups: dict[str, list[Host]] = {}
 switches: dict[str, Switch] = {}
@@ -34,18 +32,14 @@
     infra_module = __import__(INFRA_MODULE_NAME)
 
     for name in dir(infra_module):
         if name.startswith("_"):
             # Skip private members
             continue
         item = getattr(infra_module, name)
-        if type(item) == type:
-            # Skip classes
-            continue
-
         items[name] = item
         itemtype = type(item)
         if itemtype not in item_types:
             item_types[itemtype] = {}
         item_types[itemtype][name] = item
 
         if isinstance(item, Host):
```

### Comparing `infrable-0.1.5/infrable/init.py` & `infrable-0.1.6/infrable/init.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/readfile.py` & `infrable-0.1.6/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/service.py` & `infrable-0.1.6/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/switch.py` & `infrable-0.1.6/infrable/switch.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/template.py` & `infrable-0.1.6/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/utils.py` & `infrable-0.1.6/infrable/utils.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/cli/files.py` & `infrable-0.1.6/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/cli/main.py` & `infrable-0.1.6/infrable/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 import sys
 
 import typer
 
-from infrable import __version__, errors, infra, init
-from infrable.cli import files, remote, switch
-
 app = typer.Typer(no_args_is_help=True)
 
+from infrable import IS_PROJECT_DIR, __version__, init
+
 
 @app.command()
 def version():
     """Print the version."""
     print(f"infrable {__version__}")
 
 
-@app.command()
-def hosts(format: str | None = None, repr: bool = False):
-    """List all hosts in the infrastructure."""
-
-    for name, host in infra.hosts.items():
-        if format:
-            print(host.format(name, format=format))
-        elif repr:
-            print(f"{name} = {host.__repr__()}")
-        else:
-            print(f"{name} = {host}")
-
-
-@app.command()
-def services(format: str | None = None, repr: bool = False):
-    """List all services in the infrastructure."""
-
-    for name, service in infra.services.items():
-        if format:
-            print(service.format(name, format=format))
-        elif repr:
-            print(f"{name} = {service.__repr__()}")
-        else:
-            print(f"{name} = {service}")
-
-
-@app.command()
-def switches(format: str | None = None, repr: bool = False):
-    """List all switches in the infrastructure."""
-
-    for name, switch in infra.switches.items():
-        if format:
-            print(switch.format(name, format=format))
-        elif repr:
-            print(f"{name} = {switch.__repr__()}")
-        else:
-            print(f"{name} = {switch}")
-
-
 @app.command(name="init")
 def init_():
     """Bootstrap a dummy project."""
     init.init()
 
 
-app.add_typer(files.app, name="files", help="Manage files.")
-app.add_typer(switch.app, name="switch", help="Manage switches.")
-app.add_typer(remote.app, name="remote", help="Execute remote commands.")
-
-for name, ext in infra.typers.items():
-    app.add_typer(ext, name=name.replace("_", "-"))
-
-
-if __name__ == "__main__":
-    try:
-        app()
-    except errors.Error as e:
-        print(e, file=sys.stderr)
-        raise typer.Exit(1) from e
+if IS_PROJECT_DIR:
+    from infrable import __version__, errors, infra
+    from infrable.cli import files, remote, switch
+
+    @app.command()
+    def hosts(format: str | None = None, repr: bool = False):
+        """List all hosts in the infrastructure."""
+
+        for name, host in infra.hosts.items():
+            if format:
+                print(host.format(name, format=format))
+            elif repr:
+                print(f"{name} = {host.__repr__()}")
+            else:
+                print(f"{name} = {host}")
+
+    @app.command()
+    def services(format: str | None = None, repr: bool = False):
+        """List all services in the infrastructure."""
+
+        for name, service in infra.services.items():
+            if format:
+                print(service.format(name, format=format))
+            elif repr:
+                print(f"{name} = {service.__repr__()}")
+            else:
+                print(f"{name} = {service}")
+
+    @app.command()
+    def switches(format: str | None = None, repr: bool = False):
+        """List all switches in the infrastructure."""
+
+        for name, switch in infra.switches.items():
+            if format:
+                print(switch.format(name, format=format))
+            elif repr:
+                print(f"{name} = {switch.__repr__()}")
+            else:
+                print(f"{name} = {switch}")
+
+    app.add_typer(files.app, name="files", help="Manage files.")
+    app.add_typer(switch.app, name="switch", help="Manage switches.")
+    app.add_typer(remote.app, name="remote", help="Execute remote commands.")
+
+    for name, ext in infra.typers.items():
+        app.add_typer(ext, name=name.replace("_", "-"))
+
+    if __name__ == "__main__":
+        try:
+            app()
+        except errors.Error as e:
+            print(e, file=sys.stderr)
+            raise typer.Exit(1) from e
```

### Comparing `infrable-0.1.5/infrable/cli/remote.py` & `infrable-0.1.6/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/distro/linux.py` & `infrable-0.1.6/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/infrable/distro/ubuntu.py` & `infrable-0.1.6/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/.gitignore` & `infrable-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/LICENSE` & `infrable-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/README.md` & `infrable-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 [![PyPI version](https://img.shields.io/pypi/v/infrable.svg)](https://pypi.org/project/infrable)
 
 ```bash
 # Install
 pip install -U infrable  # requires python >= 3.10
 
 # Bootstrap a new project
-touch infra.py
 infrable init
 ```
 
 # Table of contents
 
 1. [Prologue](#prologue)
 2. [Chapter 1 - Chaos](#chapter-1---chaos)
```

### Comparing `infrable-0.1.5/pyproject.toml` & `infrable-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.5/PKG-INFO` & `infrable-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.5
+Version: 0.1.6
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -233,15 +233,14 @@
 [![PyPI version](https://img.shields.io/pypi/v/infrable.svg)](https://pypi.org/project/infrable)
 
 ```bash
 # Install
 pip install -U infrable  # requires python >= 3.10
 
 # Bootstrap a new project
-touch infra.py
 infrable init
 ```
 
 # Table of contents
 
 1. [Prologue](#prologue)
 2. [Chapter 1 - Chaos](#chapter-1---chaos)
```

