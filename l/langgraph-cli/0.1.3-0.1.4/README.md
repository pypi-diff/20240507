# Comparing `tmp/langgraph_cli-0.1.3.tar.gz` & `tmp/langgraph_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.3.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.4.tar", max compression
```

## Comparing `langgraph_cli-0.1.3.tar` & `langgraph_cli-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.3/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     6293 2024-05-02 22:28:25.526691 langgraph_cli-0.1.3/langgraph_cli/cli.py
--rw-r--r--   0        0        0     4314 2024-05-03 18:58:48.530871 langgraph_cli-0.1.3/langgraph_cli/config.py
--rw-r--r--   0        0        0     1609 2024-05-02 20:46:38.017185 langgraph_cli-0.1.3/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.3/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-03 18:59:25.450956 langgraph_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.4/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     6539 2024-05-07 01:05:15.454799 langgraph_cli-0.1.4/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4266 2024-05-07 00:53:49.974157 langgraph_cli-0.1.4/langgraph_cli/config.py
+-rw-r--r--   0        0        0     2055 2024-05-07 01:10:15.644569 langgraph_cli-0.1.4/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.4/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-07 01:14:42.520096 langgraph_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.4/PKG-INFO
```

### Comparing `langgraph_cli-0.1.3/langgraph_cli/cli.py` & `langgraph_cli-0.1.4/langgraph_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,22 @@
         resolve_path=True,
         path_type=pathlib.Path,
     ),
 )
 OPT_PORT = click.option(
     "--port", "-p", type=int, default=8123, show_default=True, help="Port to expose"
 )
+OPT_DEBUGGER_PORT = click.option(
+    "--debugger-port",
+    "-dp",
+    type=int,
+    default=8124,
+    show_default=True,
+    help="Port to expose debug UI on",
+)
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -121,38 +129,40 @@
     default=False,
     show_default=True,
     help="Clear previous data",
 )
 @click.option(
     "--pull/--no-pull", default=True, show_default=True, help="Pull latest images"
 )
+@OPT_DEBUGGER_PORT
 @OPT_PORT
 @OPT_O
 @OPT_C
 @cli.command(help="Start langgraph API server")
 def up(
     config: pathlib.Path,
     docker_compose: Optional[pathlib.Path],
     port: int,
     recreate: bool,
     pull: bool,
+    debugger_port: Optional[int],
 ):
     with asyncio.Runner() as runner:
         # check docker available
         try:
             runner.run(exec("docker", "--version"))
             runner.run(exec("docker", "compose", "version"))
         except click.exceptions.Exit:
             click.echo("Docker not installed or not running")
             return
         # pull latest images
         if pull:
             runner.run(exec("docker", "pull", "langchain/langserve"))
         # prepare args
-        stdin = langgraph_cli.docker.compose(port=port)
+        stdin = langgraph_cli.docker.compose(port=port, debugger_port=debugger_port)
         args = [
             "--project-directory",
             config.parent,
             "-f",
             "-",  # stdin
         ]
         # apply options
```

### Comparing `langgraph_cli-0.1.3/langgraph_cli/config.py` & `langgraph_cli-0.1.4/langgraph_cli/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,18 +79,15 @@
             # update the config
             config["graphs"][graph_id] = f"{module_str}:{attr_str}"
 
     faux_pkgs_str = "\n\n".join(
         f"ADD {relpath} /tmp/{fullpath.name}/{fullpath.name}\n                RUN touch /tmp/{fullpath.name}/pyproject.toml"
         for fullpath, relpath in faux_pkgs.items()
     )
-    local_pkgs_str = "\n".join(
-        f"ADD {relpath} /tmp/{fullpath.name}"
-        for fullpath, relpath in local_pkgs.items()
-    )
+    local_pkgs_str = f"ADD {' '.join(local_pkgs.values())} /tmp/" if local_pkgs else ""
     env_vars_str = (
         "\n".join(f"            {k}: {v}" for k, v in config["env"].items())
         if isinstance(config["env"], dict)
         else ""
     )
     env_file_str = (
         f"env_file: {config['env']}" if isinstance(config["env"], str) else ""
```

### Comparing `langgraph_cli-0.1.3/langgraph_cli/docker.py` & `langgraph_cli-0.1.4/langgraph_cli/docker.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,30 +22,45 @@
             POSTGRES_USER: postgres
             POSTGRES_PASSWORD: postgres
         volumes:
             - ./.langserve-data:/var/lib/postgresql/data
             - {ROOT}/initdb:/docker-entrypoint-initdb.d
 """
 
+DEBUGGER = """
+    debugger:
+        image: langchain/langserve-debugger
+        restart: on-failure:3
+        ports:
+            - "{debugger_port}:5173"
+        depends_on:
+            langserve:
+                condition: service_healthy
+        environment:
+            VITE_API_BASE_URL: http://localhost:{port}
+"""
+
 
 def compose(
     *,
     # postgres://user:password@host:port/database?option=value
     postgres_uri: Optional[str] = None,
     port: int,
+    debugger_port: Optional[int] = None,
 ) -> str:
     if postgres_uri is None:
         include_db = True
         postgres_uri = "postgres://postgres:postgres@postgres:5432/postgres?sslmode=disable&search_path=langserve"
     else:
         include_db = False
 
     return f"""
 services:
 {DB if include_db else ""}
+{DEBUGGER.format(port=port, debugger_port=debugger_port) if debugger_port else ""}
     migrate:
         image: langchain/langserve-migrate
         pull_policy: always
         {'''depends_on:
             postgres:
                 condition: service_healthy''' if include_db else ""}
         environment:
```

### Comparing `langgraph_cli-0.1.3/pyproject.toml` & `langgraph_cli-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

