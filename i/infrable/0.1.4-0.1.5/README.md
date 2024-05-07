# Comparing `tmp/infrable-0.1.4.tar.gz` & `tmp/infrable-0.1.5.tar.gz`

## Comparing `infrable-0.1.4.tar` & `infrable-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.4/.envrc
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 infrable-0.1.4/.null-ls_533285_README.md
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/errors.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/files.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/host.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/infra.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/paths.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/readfile.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/service.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/template.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/cli/files.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/cli/main.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.4/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.4/LICENSE
--rw-r--r--   0        0        0    17830 2020-02-02 00:00:00.000000 infrable-0.1.4/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    31656 2020-02-02 00:00:00.000000 infrable-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.5/.envrc
+-rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 infrable-0.1.5/.null-ls_186313_README.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/errors.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/files.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/host.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/infra.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/paths.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/readfile.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/service.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/template.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/files.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/main.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.5/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.5/LICENSE
+-rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 infrable-0.1.5/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    31637 2020-02-02 00:00:00.000000 infrable-0.1.5/PKG-INFO
```

### Comparing `infrable-0.1.4/.null-ls_533285_README.md` & `infrable-0.1.5/.null-ls_186313_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,21 @@
 
 dev_nginx = Service(host=dev_host, port=80)
 beta_nginx = Service(host=beta_host, port=80)
 prod_nginx = Service(host=prod_host, port=80)
 # /Services --------------------------------------------------------------------
 ```
 
+List the hosts and services:
+
+```bash
+infrable hosts
+infrable services
+```
+
 ## Chapter 3 - Templates
 
 Gradually piecing together her fragmented memories, Hanny realized configuration files
 for the host deployments ought to be maintained as **templates, drawing values as
 needed from "infra.py"**. Back on Earth, the challenge had been a lack of a coherent
 system to document the destination of these files, a problem of organization that posed a
 significant hurdle. Then, in a moment of genius, Hanny conceived a groundbreaking
@@ -288,15 +295,15 @@
 def deploy_dev_nginx():
     """[WORKFLOW] Deploy dev_nginx files: infrable deploy dev-nginx"""
 
     files.deploy(paths.templates / "nginx")
     hosts = files.affected_hosts()
     cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
     tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
-    for host, result in parallel(tasks):
+    for host, result in concurrent(tasks):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
 Running workflows:
 
 ```bash
@@ -388,16 +395,14 @@
 
 # Check all switch values
 infrable switches
 ```
 
 ## Chapter 7 - Meta and Secrets
 
-Chapter 7 - The Secret Keeper
-
 A veil of mystery cloaked Hanny's latest quest. She coveted the ability to access **secret
 values, untouched by the eyes of version control systems, and juxtapose these to hosts
 and services**. It was a daunting challenge — to embed securely these secret keys within
 the Python labyrinth without heightening complexity. She mused, her gaze focused on the
 stars scattered across the cosmos. If simplicity was the mother of invention, Hanny would
 be its devoted disciple. She engaged in the great **Pythonic tradition of simplicity**,
 armed with wisdom acquired from prior challenges, plunging into the task at hand. She
@@ -488,29 +493,27 @@
     # Provision the host
     host = cloud.provision_ubuntu_host(fqdn)
     if setup:
         host.setup(as_root=True)
 
     name = fqdn.split(".")[0]
     print("Add the host to the infra.py file.")
-    print(f"{name} = {repr(host)}")
+    print(f"{name} = {repr(host}")
 ```
 
 Plugging the module in infra.py:
 
 **infra.py**
 
 ```python
 from lib.modules import mycloud
 
 # Clouds/ ----------------------------------------------------------------------
 cloud = mycloud.MyCloud(secret_api_key=readfile("secrets/mycloud/secret_api_key"))
-
-cloud.typer = typer.Typer(help="MyCloud specific workflows.")
-cloud.typer.add_typer(mycloud.workflows, name="mycloud")
+cloud.typer = mycloud.workflows
 # /Clouds ----------------------------------------------------------------------
 ```
 
 Running the module workflows:
 
 ```bash
 infra cloud --help
```

### Comparing `infrable-0.1.4/infrable/errors.py` & `infrable-0.1.5/infrable/errors.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/files.py` & `infrable-0.1.5/infrable/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import random
 import shutil
 import subprocess as sp
 import time
-from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from difflib import unified_diff
 from pathlib import Path
 from shlex import quote as q
 from typing import IO, Any, Iterable
 
 import typer
 from click import Choice
 from jinja2 import Environment, FileSystemLoader
 from tqdm import tqdm
 
-from infrable import errors, infra, paths
+from infrable import errors, infra, paths, utils
 from infrable.host import Host
 from infrable.template import Metadata, render
 
 
 def affected_hosts(only: Iterable[str] | None = None) -> list[Host]:
     """List the affected hosts as per the files diff."""
 
@@ -79,44 +78,26 @@
             outpath.parent.mkdir(exist_ok=True, parents=True)
             rendered = render(src, dest_loc=dest.loc, **infra.items, **dest.ctx)
             outpath.write_text(rendered)
             print(outpath)
         print()
 
 
-def pull():
+def pull(workers: int | None = None):
     """For each generated file pull the current version from the server."""
 
     if not paths.files.exists():
         return
 
     for old in paths.files.glob("**/*.old"):
         old.unlink()
 
-    def _pull(new: Path):
-        dest = str(new).removesuffix(".new") + ".old"
-        remote, loc = (
-            str(new.relative_to(paths.files)).removesuffix(".new").split("/", 1)
-        )
-        src = f"/{loc}"
-        name = remote.split("@", 1)[-1]
-        host = infra.get_host(name)
-        if not host:
-            raise errors.InvalidDestinationError(dest=dest)
-        addr = f"{host.admin}@{host.ip}"
-        _sudo_pull_file(addr, src, dest)
-        return new, dest
-
-    futures = []
-    with ThreadPoolExecutor(max_workers=4) as pool:
-        for new in paths.files.glob("**/*.new"):
-            futures.append(pool.submit(_pull, new))
-        print()
-        for result in tqdm(as_completed(futures, timeout=2 * 60), total=len(futures)):
-            new, dest = result.result()
+    new_files = list(paths.files.glob("**/*.new"))
+    with utils.concurrentcontext(_pull, new_files, workers=workers) as results:
+        for new, dest in tqdm(results, total=len(new_files)):
             typer.secho(f"╭ {new}", bold=True)
             print(f"╰ {dest}")
             print()
 
 
 def backup():
     """Backup the files locally."""
@@ -231,14 +212,27 @@
 def recover(path: Path | None = None):
     """[WORKFLOW] revert and push files from backup."""
 
     revert(path)
     push()
 
 
+def _pull(new):
+    dest = str(new).removesuffix(".new") + ".old"
+    remote, loc = str(new.relative_to(paths.files)).removesuffix(".new").split("/", 1)
+    src = f"/{loc}"
+    name = remote.split("@", 1)[-1]
+    host = infra.get_host(name)
+    if not host:
+        raise errors.InvalidDestinationError(dest=dest)
+    addr = f"{host.admin}@{host.ip}"
+    _sudo_pull_file(addr, src, dest)
+    return new, dest
+
+
 def _old_path(new: Path) -> Path:
     return Path(str(new).removesuffix(".new") + ".old")
 
 
 def _diff(new: Path, old: Path) -> list[str]:
     new_lines = new.read_text().splitlines()
     old_lines = Path(old).read_text().splitlines()
```

### Comparing `infrable-0.1.4/infrable/host.py` & `infrable-0.1.5/infrable/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import asdict, dataclass, field
 
 from sh import Command, ssh
 from typer import Typer
 
 from infrable.meta import Meta
-from infrable.util import formatter
+from infrable.utils import format_item
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Host:
     """A generic host in the infrastructure."""
 
     ip: str  # The only required field
@@ -19,13 +19,13 @@
     typer: Typer | None = None
 
     def remote(self, login=None) -> Command:
         login = login or self.admin
         address = f"{login}@{self.ip}"
         return ssh.bake(address, "-o", "StrictHostKeyChecking=no")
 
-    def format(self, name: str, format) -> str:
-        return formatter(format).render(name=name, **asdict(self))
+    def format(self, name: str, format: str) -> str:
+        return format_item(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
         host = self.fqdn or self.ip
         return f"{self.admin}@{host}"
```

### Comparing `infrable-0.1.4/infrable/infra.py` & `infrable-0.1.5/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/init.py` & `infrable-0.1.5/infrable/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 INFRA_PY = '''
 import typer
-from infrable import Host, Meta, Service, Switch, files, parallel, paths, readfile
+from infrable import Host, Meta, Service, Switch, files, concurrent, paths, readfile
 from lib.modules import mycloud
 
 # To quickly find the configuration file template on GitHub
 template_prefix = "https://github.com/username/repository/blob/main"
 
 
 # Environments/ ----------------------------------------------------------------
@@ -64,18 +64,17 @@
 # Workflows/ -----------------------------------------------------------------------
 deploy = typer.Typer(help="Deployment workflows.")
 @deploy.command(name="nginx")
 def deploy_nginx():
     """[WORKFLOW] Deploy nginx files: infrable deploy nginx"""
 
     files.deploy(paths.templates / "nginx")
-    hosts = files.affected_hosts()
-    cmd = "sudo nginx -t && sudo systemctl reload nginx"
-    tasks = [lambda: (h, h.remote().sudo(cmd)) for h in hosts]
-    for host, result in parallel(tasks):
+    cmd = "sudo nginx -t && sudo systemctl reload nginx && echo success || echo failed"
+    fn = lambda host: (host, host.remote().sudo(cmd))
+    for host, result in concurrent(fn, files.affected_hosts()):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 '''.strip()
 
 NGINX_PROXY_PARAMS_TEMPLATE = """
 # vim: syn=nginx
```

### Comparing `infrable-0.1.4/infrable/readfile.py` & `infrable-0.1.5/infrable/readfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import Callable
 
 
 def readfile(
     path: Path | str,
+    *,
     init: Callable[[], str] = str,
     fmt: Callable[[str], str] | None = lambda s: s.strip(),
 ) -> str:
     """Get the contents of a file, creating it if it doesn't exist."""
 
     if isinstance(path, str):
         path = Path(path)
```

### Comparing `infrable-0.1.4/infrable/service.py` & `infrable-0.1.5/infrable/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import asdict, dataclass, field
 
 from typer import Typer
 
 from infrable.host import Host
 from infrable.meta import Meta
-from infrable.util import formatter
+from infrable.utils import format_item
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Service:
     """A generic service, maybe running on a host."""
 
     host: Host | None = None
     port: int | None = None
     meta: Meta = field(default_factory=Meta)
     typer: Typer | None = None
 
-    def format(self, name: str, format) -> str:
-        return formatter(format).render(name=name, **asdict(self))
+    def format(self, name: str, format: str) -> str:
+        return format_item(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
         return f'{self.host or ""}:{self.port or ""}'
```

### Comparing `infrable-0.1.4/infrable/switch.py` & `infrable-0.1.5/infrable/switch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import asdict, dataclass, field
 from typing import Any
 
 from typer import Typer
 
 from infrable import errors, paths
 from infrable.meta import Meta
-from infrable.util import formatter
+from infrable.utils import format_item
 
 
 @dataclass(unsafe_hash=True, order=True, eq=True)
 class Switch:
     """A switch for the infrastructure."""
 
     options: set[str]
@@ -53,12 +53,12 @@
             self.path.parent.mkdir(parents=True, exist_ok=True)
             self.path.write_text(value)
             return
 
         self.path.unlink(missing_ok=True)
         raise errors.SwitchValueError(self.path, value=value, options=self.options)
 
-    def format(self, name: str, format) -> str:
-        return formatter(format).render(name=name, **asdict(self))
+    def format(self, name: str, format: str) -> str:
+        return format_item(format).render(name=name, **asdict(self))
 
     def __str__(self) -> str:
-        return self()
+        return self.strict()
```

### Comparing `infrable-0.1.4/infrable/template.py` & `infrable-0.1.5/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/util.py` & `infrable-0.1.5/infrable/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
-from typing import Any, Callable, Iterable
+from typing import Any, Callable, Generator, Iterable, Iterator, TypeVar
 
 from jinja2 import Template
-from tqdm import tqdm
 
+T = TypeVar("T")
 
-def formatter(template: str) -> Template:
+
+def format_item(template: str) -> Template:
     return Template(
         template,
         variable_start_string="{",
         variable_end_string="}",
         autoescape=False,
         keep_trailing_newline=True,
         finalize=lambda x: x or "",
     )
 
 
 @contextmanager
-def parallelcontext(
-    generator: Iterable[Callable[[], Any]] | list[Callable[[], Any]],
+def concurrentcontext(
+    function: Callable[[T], Any],
+    generator: Iterable[T],
+    *,
     workers: int | None = None,
-    total: int | None = None,
-    progress: bool = True,
-):
-    """Context manager, run a list of functions in parallel."""
-
-    if progress:
-        generator = tqdm(generator, total=total)
+) -> Generator[Iterator[Any], Any, None]:
+    """With context, run a function on a batch of arguments concurrently."""
 
     with ThreadPoolExecutor(max_workers=workers) as executor:
-        yield executor.map(lambda x: x(), generator)
+        yield executor.map(function, generator)
 
 
-def parallel(
-    generator: Iterable[Callable[[], Any]] | list[Callable[[], Any]],
+def concurrent(
+    function: Callable[[T], Any],
+    generator: Iterable[T],
+    *,
     workers: int | None = None,
-    total: int | None = None,
-    progress: bool = True,
 ) -> list:
-    """Run a list of functions in parallel."""
+    """Run a functions on a batch of arguments in concurrently."""
 
-    with parallelcontext(
-        generator, workers=workers, total=total, progress=progress
-    ) as results:
+    with concurrentcontext(function, generator, workers=workers) as results:
         return list(results)
```

### Comparing `infrable-0.1.4/infrable/cli/files.py` & `infrable-0.1.5/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/cli/main.py` & `infrable-0.1.5/infrable/cli/main.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/cli/remote.py` & `infrable-0.1.5/infrable/cli/remote.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Iterable
 
 import typer
 from tqdm import tqdm
 
-from infrable import Host, files, infra
+from infrable import Host, files, infra, utils
 
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command(name="-")
-def from_stdin(command: str):
+def from_stdin(command: str, workers: int | None = None):
     """Execute a script on the list of hosts passed via stdin."""
 
     hosts = []
     for line in typer.get_text_stream("stdin").readlines():
         host = line.split(maxsplit=1)[0].split("@", 1)[-1].strip()
         if not host:
             continue
         for host in infra.filtered_hosts(only=[host]):
             hosts.append(host)
 
-    _execute(hosts, command=command)
+    _execute_batch(hosts, command=command, workers=workers)
 
 
 @app.command()
-def infra_hosts(command: str, only: list[str] = typer.Option(None)):
+def infra_hosts(
+    command: str, only: list[str] = typer.Option(None), workers: int | None = None
+):
     """Execute a script on the hosts listed in the infra."""
 
     hosts = infra.hosts.values()
     if only:
         hosts = infra.filtered_hosts(only=only)
 
-    _execute(hosts, command=command)
+    _execute_batch(hosts, command=command, workers=workers)
 
 
 @app.command()
-def affected_hosts(command: str, only: list[str] = typer.Option(None)):
+def affected_hosts(
+    command: str, only: list[str] = typer.Option(None), workers: int | None = None
+):
     """Execute a script on the affected hosts in the last deployment."""
 
     hosts = files.affected_hosts()
 
     if only:
         only_hosts = set(h.fqdn for h in infra.filtered_hosts(only=only))
         hosts = (h for h in hosts if h.fqdn in only_hosts)
 
-    _execute(hosts, command=command)
+    _execute_batch(hosts, command=command, workers=workers)
 
 
 for name, group in infra.host_groups.items():
 
-    def groupmain(command: str, only: list[str] = typer.Option(None)):
+    def groupmain(
+        command: str, only: list[str] = typer.Option(None), workers: int | None = None
+    ):
         hosts = group
         if only:
             only_hosts = set(h.fqdn for h in infra.filtered_hosts(only=only))
             hosts = (h for h in hosts if h.fqdn in only_hosts)
 
-        _execute(hosts, command=command)
+        _execute_batch(hosts, command=command, workers=workers)
 
     help = f"Execute a script on {name} hosts."
     app.command(name=name, help=help)(groupmain)
 
 
 for name, host in infra.hosts.items():
 
     def hostmaain(command: str):
         host.remote()(command, _fg=True)
 
     help = f"Execute a script on {name}."
     app.command(name=name, help=help)(hostmaain)
 
 
-def _execute(hosts: Iterable[Host], command: str):
+def _execute_batch(hosts: Iterable[Host], command: str, workers: int | None):
     hosts = {h.ip: h for h in hosts}.values()
-    futures = []
-    with ThreadPoolExecutor(max_workers=4) as pool:
-        for h in hosts:
-            fut = pool.submit(lambda: (h, h.remote()(command, _err_to_out=True)))
-            futures.append(fut)
-        print()
-        for result in tqdm(as_completed(futures), total=len(futures)):
-            host, result = result.result()
+    fn = lambda host: (host, host.remote()(command, _err_to_out=True))
+    with utils.concurrentcontext(fn, hosts, workers=workers) as results:
+        for host, result in tqdm(results, total=len(hosts)):
             typer.secho(f"╭ {host}", bold=True)
             print(result)
             print()
```

### Comparing `infrable-0.1.4/infrable/distro/linux.py` & `infrable-0.1.5/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/infrable/distro/ubuntu.py` & `infrable-0.1.5/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/.gitignore` & `infrable-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/LICENSE` & `infrable-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/README.md` & `infrable-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -282,28 +282,27 @@
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
-    for host, result in parallel(tasks):
+    fn = lambda host: (host, host.remote().sudo(cmd))
+    for host, result in concurrent(fn, files.affected_hosts()):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
 Running workflows:
 
 ```bash
```

### Comparing `infrable-0.1.4/pyproject.toml` & `infrable-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.4/PKG-INFO` & `infrable-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.4
+Version: 0.1.5
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -510,28 +510,27 @@
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
-    for host, result in parallel(tasks):
+    fn = lambda host: (host, host.remote().sudo(cmd))
+    for host, result in concurrent(fn, files.affected_hosts()):
         print(f"{host}: {result}")
 # /Workflows -----------------------------------------------------------------------
 ```
 
 Running workflows:
 
 ```bash
```

