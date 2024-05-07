# Comparing `tmp/gitlabci_checker-0.1.2.tar.gz` & `tmp/gitlabci_checker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabci_checker-0.1.2.tar", max compression
+gzip compressed data, was "gitlabci_checker-0.1.3.tar", max compression
```

## Comparing `gitlabci_checker-0.1.2.tar` & `gitlabci_checker-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1073 2022-12-29 12:14:47.219153 gitlabci_checker-0.1.2/LICENSE
--rw-r--r--   0        0        0     3362 2023-02-16 11:02:04.650732 gitlabci_checker-0.1.2/README.md
--rw-r--r--   0        0        0       95 2023-01-13 15:45:35.926486 gitlabci_checker-0.1.2/gitlabci_checker/__init__.py
--rw-r--r--   0        0        0     3443 2023-01-14 15:18:09.975051 gitlabci_checker-0.1.2/gitlabci_checker/cli.py
--rw-r--r--   0        0        0     1747 2023-01-14 15:38:13.583628 gitlabci_checker-0.1.2/gitlabci_checker/helpers.py
--rw-r--r--   0        0        0     1037 2023-02-16 11:02:21.515717 gitlabci_checker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 gitlabci_checker-0.1.2/setup.py
--rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 gitlabci_checker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-12-29 12:14:47.219153 gitlabci_checker-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3362 2023-02-16 11:02:04.650732 gitlabci_checker-0.1.3/README.md
+-rw-r--r--   0        0        0       95 2023-01-13 15:45:35.926486 gitlabci_checker-0.1.3/gitlabci_checker/__init__.py
+-rw-r--r--   0        0        0     3335 2024-05-07 09:33:18.043306 gitlabci_checker-0.1.3/gitlabci_checker/cli.py
+-rw-r--r--   0        0        0     1747 2023-01-14 15:38:13.583628 gitlabci_checker-0.1.3/gitlabci_checker/helpers.py
+-rw-r--r--   0        0        0     1052 2024-05-07 10:20:47.396144 gitlabci_checker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 gitlabci_checker-0.1.3/PKG-INFO
```

### Comparing `gitlabci_checker-0.1.2/LICENSE` & `gitlabci_checker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabci_checker-0.1.2/README.md` & `gitlabci_checker-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gitlabci_checker-0.1.2/gitlabci_checker/cli.py` & `gitlabci_checker-0.1.3/gitlabci_checker/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,28 +95,20 @@
             bold=True,
             nl=True,
         )
         out = json.dumps(error, indent=2)
         click.secho(message=out, fg="red", bold=False, nl=True)
         ctx.exit(1)
     else:
-        if (
-            lint_results["status"] == "valid"
-            and lint_results["warnings"]
-            and warnings_are_errors
-        ):
-            click.secho(
-                message="Check failed with warning(s).", fg="yellow", bold=True, nl=True
-            )
+        if lint_results["status"] == "valid" and lint_results["warnings"] and warnings_are_errors:
+            click.secho(message="Check failed with warning(s).", fg="yellow", bold=True, nl=True)
             out = json.dumps(lint_results, indent=2)
             click.secho(message=out, fg="yellow", bold=False, nl=True)
             ctx.exit(1)
         elif lint_results["status"] == "valid":
             click.secho(message="Everything's fine.", fg="green", bold=True, nl=True)
             ctx.exit(0)
         else:
-            click.secho(
-                message="Check failed with error(s).", fg="red", bold=True, nl=True
-            )
+            click.secho(message="Check failed with error(s).", fg="red", bold=True, nl=True)
             out = json.dumps(lint_results, indent=2)
             click.secho(message=out, fg="red", bold=False, nl=True)
             ctx.exit(1)
```

### Comparing `gitlabci_checker-0.1.2/gitlabci_checker/helpers.py` & `gitlabci_checker-0.1.3/gitlabci_checker/helpers.py`

 * *Files identical despite different names*

### Comparing `gitlabci_checker-0.1.2/pyproject.toml` & `gitlabci_checker-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 [tool.poetry]
 name = "gitlabci-checker"
-version = "0.1.2"
+version = "0.1.3"
 description = "Checks if your gitlab-ci pipeline compiles correctly."
 authors = ["Lorenzo Maffioli <lorenzo.maffioli@gmail.com>"]
 readme = "README.md"
 
 repository = "https://github.com/lorenzophys/gitlabci-checker"
 keywords = ["gitlab", "ci", "pipeline"]
 
 [tool.poetry.scripts]
 cicheck = "gitlabci_checker.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 click = "^8.1.3"
 requests = "^2.28.1"
+tox-poetry = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
+black = "^24.0.0"
 isort = "^5.10.1"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-flake8 = "^5.0.4"
-flake8-simplify = "^0.19.3"
-flake8-bugbear = "^22.10.27"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
+flake8 = "^7.0.0"
+flake8-simplify = "^0.21.0"
+flake8-bugbear = "^24.0.0"
 flake8-comprehensions = "^3.10.1"
-mypy = "^0.990"
+mypy = "^1.0.0"
 pydocstyle = "^6.1.1"
-pre-commit = "^2.20.0"
+pre-commit = "^3.0.0"
 tox = "^3.27.0"
 tox-pyenv = "^1.1.0"
 types-setuptools = "^65.6.0.2"
 toml = "^0.10.2"
 types-requests = "^2.28.11.7"
-pytest-httpserver = "^1.0.6"
+pytest-httpserver = "^1.0.10"
 
 [tool.black]
-max-line-length = 100
+line-length = 100
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gitlabci_checker-0.1.2/setup.py` & `gitlabci_checker-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['gitlabci_checker']
+Metadata-Version: 2.1
+Name: gitlabci-checker
+Version: 0.1.3
+Summary: Checks if your gitlab-ci pipeline compiles correctly.
+Home-page: https://github.com/lorenzophys/gitlabci-checker
+Keywords: gitlab,ci,pipeline
+Author: Lorenzo Maffioli
+Author-email: lorenzo.maffioli@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: tox-poetry (>=0.5.0,<0.6.0)
+Project-URL: Repository, https://github.com/lorenzophys/gitlabci-checker
+Description-Content-Type: text/markdown
+
+# Gitlabci checker
+
+![release](https://img.shields.io/github/v/release/lorenzophys/gitlabci-checker)
+[![codecov](https://codecov.io/gh/lorenzophys/gitlabci-checker/branch/main/graph/badge.svg?token=WEZ1UH621Y)](https://codecov.io/gh/lorenzophys/gitlabci-checker)
+[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/lorenzophys/gitlabci-checker/test-workflow.yml?branch=main&label=tests)](https://img.shields.io/github/actions/workflow/status/lorenzophys/gitlabci-checker/test-workflow.yml)
+![pver](https://img.shields.io/pypi/pyversions/gitlabci-checker)
+![MIT](https://img.shields.io/github/license/lorenzophys/gitlabci-checker)
+
+## Installation
+
+You can install `gitlabci-checker` via `pip`:
+
+```console
+user@laptop:~$ pip install gitlabci-checker
+```
+
+You can interact with the CLI via the `cicheck` comand:
+
+```console
+user@laptop:~$ cicheck
+Usage: cicheck [OPTIONS] FILENAME
+
+  Check if your gitlab-ci pipeline compiles correctly.
+
+Options:
+  -h, --help                 Show this message and exit.
+  -v, --version              Show the version and exit.
+  -t, --token TEXT           Your Gitlab access token: by default the content
+                             of the GITLAB_TOKEN variable is used.  [required]
+  -s, --gitlab-server TEXT   The Gitlab server hostname.  [required]
+  -k, --insecure             Use insecure connection (http).
+  -w, --warnings-are-errors  Force the failure if warnings are found.
+```
+
+## How it works?
+
+`cicheck` just calls the [Gitlab CI lint API](https://docs.gitlab.com/15.7/ee/api/lint.html) with the file you pass to it.
+
+By default it will send the request to `gitlab.com`. If you want to use your own Gitlab instance you must pass the server address:
+
+```console
+user@laptop:~$ cicheck .gitlab-ci.yaml --gitlab-server code.company.com
+Everything's fine.
+```
+
+You must pass a valid token to the CLI: either as the environment variable `GITLAB_TOKEN` or via the `--token` flag.
+
+## Usage example
+
+If your pipeline is valid it returns a "Everything's fine." message
+
+```console
+user@laptop:~$ cicheck .gitlab-ci.yaml
+Everything's fine.
+```
+
+If your configuration is invalid it returns an error message together with the response from Gitlab:
+
+```console
+user@laptop:~$ cicheck .gitlab-ci.yaml
+Check failed with error(s).
+{
+  "status": "invalid",
+  "errors": [
+    "variables config should be a hash of key value pairs"
+  ],
+  "warnings": []
+}
+```
 
-package_data = \
-{'': ['*']}
+You can also force a failure whenever the linter returns a warning by appending `--warnings-are-errors` or `-w`:
 
-install_requires = \
-['click>=8.1.3,<9.0.0', 'requests>=2.28.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['cicheck = gitlabci_checker.cli:cli']}
-
-setup_kwargs = {
-    'name': 'gitlabci-checker',
-    'version': '0.1.2',
-    'description': 'Checks if your gitlab-ci pipeline compiles correctly.',
-    'long_description': '# Gitlabci checker\n\n![release](https://img.shields.io/github/v/release/lorenzophys/gitlabci-checker)\n[![codecov](https://codecov.io/gh/lorenzophys/gitlabci-checker/branch/main/graph/badge.svg?token=WEZ1UH621Y)](https://codecov.io/gh/lorenzophys/gitlabci-checker)\n[![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/lorenzophys/gitlabci-checker/test-workflow.yml?branch=main&label=tests)](https://img.shields.io/github/actions/workflow/status/lorenzophys/gitlabci-checker/test-workflow.yml)\n![pver](https://img.shields.io/pypi/pyversions/gitlabci-checker)\n![MIT](https://img.shields.io/github/license/lorenzophys/gitlabci-checker)\n\n## Installation\n\nYou can install `gitlabci-checker` via `pip`:\n\n```console\nuser@laptop:~$ pip install gitlabci-checker\n```\n\nYou can interact with the CLI via the `cicheck` comand:\n\n```console\nuser@laptop:~$ cicheck\nUsage: cicheck [OPTIONS] FILENAME\n\n  Check if your gitlab-ci pipeline compiles correctly.\n\nOptions:\n  -h, --help                 Show this message and exit.\n  -v, --version              Show the version and exit.\n  -t, --token TEXT           Your Gitlab access token: by default the content\n                             of the GITLAB_TOKEN variable is used.  [required]\n  -s, --gitlab-server TEXT   The Gitlab server hostname.  [required]\n  -k, --insecure             Use insecure connection (http).\n  -w, --warnings-are-errors  Force the failure if warnings are found.\n```\n\n## How it works?\n\n`cicheck` just calls the [Gitlab CI lint API](https://docs.gitlab.com/15.7/ee/api/lint.html) with the file you pass to it.\n\nBy default it will send the request to `gitlab.com`. If you want to use your own Gitlab instance you must pass the server address:\n\n```console\nuser@laptop:~$ cicheck .gitlab-ci.yaml --gitlab-server code.company.com\nEverything\'s fine.\n```\n\nYou must pass a valid token to the CLI: either as the environment variable `GITLAB_TOKEN` or via the `--token` flag.\n\n## Usage example\n\nIf your pipeline is valid it returns a "Everything\'s fine." message\n\n```console\nuser@laptop:~$ cicheck .gitlab-ci.yaml\nEverything\'s fine.\n```\n\nIf your configuration is invalid it returns an error message together with the response from Gitlab:\n\n```console\nuser@laptop:~$ cicheck .gitlab-ci.yaml\nCheck failed with error(s).\n{\n  "status": "invalid",\n  "errors": [\n    "variables config should be a hash of key value pairs"\n  ],\n  "warnings": []\n}\n```\n\nYou can also force a failure whenever the linter returns a warning by appending `--warnings-are-errors` or `-w`:\n\n```console\nuser@laptop:~$ cicheck .gitlab-ci.yaml --warnings-are-errors\nCheck failed with warning(s).\n{\n  "status": "valid",\n  "errors": [],\n  "warnings": ["jobs:job may allow multiple pipelines to run for a single action due to\n  `rules:when` clause with no `workflow:rules` - read more:\n  https://docs.gitlab.com/ee/ci/troubleshooting.html#pipeline-warnings"]\n}\n```\n\n## `pre-commit` hook\n\n`gitlabci-checker` can be also used as a [pre-commit](https://pre-commit.com) hook. For example:\n\n```yaml\nrepos:\n  - repo: https://github.com/lorenzophys/gitlabci-checker\n    rev: v0.1.1\n    hooks:\n      - id: gitlabci-checker\n        args:\n          - --gitlab-server code.company.com\n          - --warnings-are-errors\n```\n\n## License\n\nThis project is licensed under the **MIT License** - see the *LICENSE* file for details.\n',
-    'author': 'Lorenzo Maffioli',
-    'author_email': 'lorenzo.maffioli@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/lorenzophys/gitlabci-checker',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+```console
+user@laptop:~$ cicheck .gitlab-ci.yaml --warnings-are-errors
+Check failed with warning(s).
+{
+  "status": "valid",
+  "errors": [],
+  "warnings": ["jobs:job may allow multiple pipelines to run for a single action due to
+  `rules:when` clause with no `workflow:rules` - read more:
+  https://docs.gitlab.com/ee/ci/troubleshooting.html#pipeline-warnings"]
 }
+```
+
+## `pre-commit` hook
+
+`gitlabci-checker` can be also used as a [pre-commit](https://pre-commit.com) hook. For example:
+
+```yaml
+repos:
+  - repo: https://github.com/lorenzophys/gitlabci-checker
+    rev: v0.1.1
+    hooks:
+      - id: gitlabci-checker
+        args:
+          - --gitlab-server code.company.com
+          - --warnings-are-errors
+```
+
+## License
 
+This project is licensed under the **MIT License** - see the *LICENSE* file for details.
 
-setup(**setup_kwargs)
```

