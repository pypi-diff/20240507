# Comparing `tmp/jupyter_vscode_proxy-0.5.tar.gz` & `tmp/jupyter_vscode_proxy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_vscode_proxy-0.5.tar", last modified: Fri Aug 18 09:24:30 2023, max compression
+gzip compressed data, was "jupyter_vscode_proxy-0.6.tar", last modified: Tue May  7 07:12:15 2024, max compression
```

## Comparing `jupyter_vscode_proxy-0.5.tar` & `jupyter_vscode_proxy-0.6.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.954649 jupyter_vscode_proxy-0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.958649 jupyter_vscode_proxy-0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.958649 jupyter_vscode_proxy-0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/examples/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/icons/vscode.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-18 09:24:30.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-18 09:24:30.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-18 09:24:30.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-18 09:24:30.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-18 09:24:30.000000 jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-18 09:24:18.000000 jupyter_vscode_proxy-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-18 09:24:30.962649 jupyter_vscode_proxy-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.387012 jupyter_vscode_proxy-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.383012 jupyter_vscode_proxy-0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.383012 jupyter_vscode_proxy-0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.383012 jupyter_vscode_proxy-0.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-07 07:12:15.387012 jupyter_vscode_proxy-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.383012 jupyter_vscode_proxy-0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/examples/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.383012 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.387012 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/icons/code-server.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/icons/vscode.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:12:15.387012 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-07 07:12:15.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-07 07:12:15.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:12:15.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 07:12:15.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 07:12:15.000000 jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-07 07:12:09.000000 jupyter_vscode_proxy-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:12:15.387012 jupyter_vscode_proxy-0.6/setup.cfg
```

### Comparing `jupyter_vscode_proxy-0.5/.github/workflows/ci.yaml` & `jupyter_vscode_proxy-0.6/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 jobs:
   build_artifacts:
     name: Build artifacts
     runs-on: ubuntu-latest
     strategy:
       fail-fast: true
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Fetch full git history
         run: git fetch --prune --unshallow
       - name: Set up Conda env
-        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
+        uses: mamba-org/setup-micromamba@422500192359a097648154e8db4e39bdb6c6eed7
         with:
           environment-file: environment.yml
           cache-environment: true
       - shell: bash -el {0}
         run:
           python -m build
-      - uses: pypa/gh-action-pypi-publish@v1.5.1
+      - uses: pypa/gh-action-pypi-publish@v1.8.14
         if: github.event_name == 'release'
         with:
           user: __token__
           password: ${{ secrets.PYPI_RELEASE_TOKEN }}
```

### Comparing `jupyter_vscode_proxy-0.5/.pre-commit-config.yaml` & `jupyter_vscode_proxy-0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_vscode_proxy-0.5/LICENSE` & `jupyter_vscode_proxy-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_vscode_proxy-0.5/PKG-INFO` & `jupyter_vscode_proxy-0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_vscode_proxy
-Version: 0.5
+Version: 0.6
 Summary: VS Code extension for Jupyter
 Author-email: Tim Head <noreply@example.com>
 License: BSD-3-clause
 Project-URL: repository, https://github.com/betatim/vscode-binder
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/__init__.py` & `jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,18 +57,19 @@
         return cmd
 
     return _get_cmd
 
 
 def setup_vscode() -> Dict[str, Any]:
     executable = os.environ.get("CODE_EXECUTABLE", "code-server")
+    icon = "code-server.svg" if executable == "code-server" else "vscode.svg"
     return {
         "command": _get_cmd_factory(executable),
         "timeout": 300,
         "new_browser_tab": True,
         "launcher_entry": {
             "title": "VS Code",
             "icon_path": os.path.join(
-                os.path.dirname(os.path.abspath(__file__)), "icons", "vscode.svg"
+                os.path.dirname(os.path.abspath(__file__)), "icons", icon
             ),
         },
     }
```

### Comparing `jupyter_vscode_proxy-0.5/jupyter_vscode_proxy/icons/vscode.svg` & `jupyter_vscode_proxy-0.6/jupyter_vscode_proxy/icons/vscode.svg`

 * *Files identical despite different names*

### Comparing `jupyter_vscode_proxy-0.5/jupyter_vscode_proxy.egg-info/PKG-INFO` & `jupyter_vscode_proxy-0.6/jupyter_vscode_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter-vscode-proxy
-Version: 0.5
+Name: jupyter_vscode_proxy
+Version: 0.6
 Summary: VS Code extension for Jupyter
 Author-email: Tim Head <noreply@example.com>
 License: BSD-3-clause
 Project-URL: repository, https://github.com/betatim/vscode-binder
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `jupyter_vscode_proxy-0.5/pyproject.toml` & `jupyter_vscode_proxy-0.6/pyproject.toml`

 * *Files identical despite different names*

