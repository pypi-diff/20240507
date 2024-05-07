# Comparing `tmp/litestar_asyncpg-0.1.3.tar.gz` & `tmp/litestar_asyncpg-0.2.0.tar.gz`

## Comparing `litestar_asyncpg-0.1.3.tar` & `litestar_asyncpg-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/Makefile
--rw-r--r--   0        0        0   181614 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/pdm.lock
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/docs-preview.yaml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/pr-title.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/Makefile
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/conf.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/contribution-guide.rst
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/fix_missing_references.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/reference/config.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/reference/plugin.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/usage/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/docs/usage/placeholder.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/examples/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/examples/basic.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/litestar_asyncpg/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/litestar_asyncpg/__metadata__.py
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/litestar_asyncpg/config.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/litestar_asyncpg/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/litestar_asyncpg/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/tests/docker-compose.yml
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/LICENSE
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/README.md
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 litestar_asyncpg-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.sourcery.yaml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/Makefile
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/codecov.yml
+-rw-r--r--   0        0        0   145837 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/pdm.lock
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/sonar-project.properties
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/docs-preview.yaml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/pr-title.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/contribution-guide.rst
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/fix_missing_references.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/reference/config.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/reference/plugin.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/usage/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/docs/usage/placeholder.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/examples/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/examples/basic.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/__metadata__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/_utils.py
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/config.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/litestar_asyncpg/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/README.md
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 litestar_asyncpg-0.2.0/PKG-INFO
```

### Comparing `litestar_asyncpg-0.1.3/.pre-commit-config.yaml` & `litestar_asyncpg-0.2.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 default_language_version:
-  python: "3.11"
+  python: python3
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.4.0
+    rev: v3.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.291"
+    rev: "v0.4.3"
     hooks:
       - id: ruff
         args: ["--fix"]
         exclude: "docs"
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.6
     hooks:
       - id: codespell
-  - repo: https://github.com/psf/black
-    rev: 23.9.1
-    hooks:
-      - id: black
-        args: [--config=./pyproject.toml]
+        exclude: "pdm.lock|examples/us_state_lookup.json"
+        additional_dependencies:
+          - tomli
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.5.1"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         exclude: "docs"
         additional_dependencies:
           [
             asyncpg,
+            "anyio",
             asyncpg_stubs,
             pytest,
-            pytest-asyncio,
-            pytest-lazy-fixture,
             time-machine,
-            httpx,
             pytest-mock,
             pytest-timeout,
-            msgspec,
-            "litestar[cli]",
+            "litestar",
+            "types-click",
           ]
   - repo: https://github.com/sphinx-contrib/sphinx-lint
-    rev: "v0.6.8"
+    rev: "v0.9.1"
     hooks:
       - id: sphinx-lint
```

### Comparing `litestar_asyncpg-0.1.3/CONTRIBUTING.rst` & `litestar_asyncpg-0.2.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Code contributions
 ------------------
 
 Workflow
 ++++++++
 
-1. `Fork <https://github.com/cofin/litestar-asyncpg/fork>`_ the `Advanced Alchemy repository <https://github.com/cofin/litestar-asyncpg>`_
+1. `Fork <https://github.com/litestar-org/litestar-asyncpg/fork>`_ the `Litestar Asyncpg repository <https://github.com/litestar-org/litestar-asyncpg>`_
 2. Clone your fork locally with git
 3. `Set up the environment <#setting-up-the-environment>`_
 4. Make your changes
 5. (Optional) Run ``pre-commit run --all-files`` to run linters and formatters. This step is optional and will be executed
    automatically by git before you make a commit, but you may want to run it manually in order to apply fixes
 6. Commit your changes to git
 7. Push the changes to your fork
@@ -62,17 +62,17 @@
 ``pdm install -G:docs``
 
 Then you can serve the documentation with ``make docs-serve``, or build them with ``make docs``.
 
 Creating a new release
 ----------------------
 
-1. Increment the version in `pyproject.toml <https://github.com/cofin/litestar-asyncpg/blob/main/pyproject.toml>`_.
+1. Increment the version in `pyproject.toml <https://github.com/litestar-org/litestar-asyncpg/blob/main/pyproject.toml>`_.
     .. note:: The version should follow `semantic versioning <https://semver.org/>`_ and `PEP 440 <https://www.python.org/dev/peps/pep-0440/>`_.
-2. `Draft a new release <https://github.com/cofin/litestar-asyncpg/releases/new>`_ on GitHub
+2. `Draft a new release <https://github.com/litestar-org/litestar-asyncpg/releases/new>`_ on GitHub
 
    * Use ``vMAJOR.MINOR.PATCH`` (e.g. ``v1.2.3``) as both the tag and release title
    * Fill in the release description. You can use the "Generate release notes" function to get a draft for this
 3. Commit your changes and push to ``main``
 4. Publish the release
-5. Go to `Actions <https://github.com/cofin/litestar-asyncpg/actions>`_ and approve the release workflow
+5. Go to `Actions <https://github.com/litestar-org/litestar-asyncpg/actions>`_ and approve the release workflow
 6. Check that the workflow runs successfully
```

### Comparing `litestar_asyncpg-0.1.3/Makefile` & `litestar_asyncpg-0.2.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 	@if [ "$(USING_PDM)" ]; then $(PDM) config venv.in_project true && python3 -m venv --copies .venv && . $(ENV_PREFIX)/activate && $(ENV_PREFIX)/pip install --quiet -U wheel setuptools cython pip; fi
 	@if [ "$(USING_PDM)" ]; then $(PDM) install -G:all; fi
 	@echo "=> Install complete! Note: If you want to re-install re-run 'make install'"
 
 
 clean: 												## Cleanup temporary build artifacts
 	@echo "=> Cleaning working directory"
+	@if [ "$(USING_PDM)" ]; then $(PDM) run pre-commit clean; fi
 	@rm -rf .pytest_cache .ruff_cache .hypothesis build/ -rf dist/ .eggs/
 	@find . -name '*.egg-info' -exec rm -rf {} +
 	@find . -name '*.egg' -exec rm -f {} +
 	@find . -name '*.pyc' -exec rm -f {} +
 	@find . -name '*.pyo' -exec rm -f {} +
 	@find . -name '*~' -exec rm -f {} +
 	@find . -name '__pycache__' -exec rm -rf {} +
```

### Comparing `litestar_asyncpg-0.1.3/pdm.lock` & `litestar_asyncpg-0.2.0/pdm.lock`

 * *Files 13% similar despite different names*

```diff
@@ -1,1477 +1,1452 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
-groups = ["default", "dev", "docs", "linting", "test"]
-cross_platform = true
-static_urls = false
-lock_version = "4.3"
-content_hash = "sha256:7c09e2e1408e2025e7a721eb27fbf9602fa47a4e1611fb5f25260157e27cd3b9"
+groups = ["default", "docs", "linting", "test"]
+strategy = ["cross_platform", "inherit_metadata"]
+lock_version = "4.4.1"
+content_hash = "sha256:caa388d5faaf1efadba8e6c5dcc9eee106fb0e941614956bf743f214bcb58d47"
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 requires_python = ">=3.6"
 summary = "A configurable sidebar-enabled Sphinx theme"
+groups = ["docs"]
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
-name = "alembic"
-version = "1.12.0"
-requires_python = ">=3.7"
-summary = "A database migration tool for SQLAlchemy."
-dependencies = [
-    "Mako",
-    "SQLAlchemy>=1.3.0",
-    "importlib-metadata; python_version < \"3.9\"",
-    "importlib-resources; python_version < \"3.9\"",
-    "typing-extensions>=4",
-]
-files = [
-    {file = "alembic-1.12.0-py3-none-any.whl", hash = "sha256:03226222f1cf943deee6c85d9464261a6c710cd19b4fe867a3ad1f25afda610f"},
-    {file = "alembic-1.12.0.tar.gz", hash = "sha256:8e7645c32e4f200675e69f0745415335eb59a3663f5feb487abfa0b30c45888b"},
-]
-
-[[package]]
 name = "anyio"
-version = "4.0.0"
+version = "4.3.0"
 requires_python = ">=3.8"
 summary = "High level compatibility layer for multiple asynchronous event loop implementations"
+groups = ["default", "test"]
 dependencies = [
     "exceptiongroup>=1.0.2; python_version < \"3.11\"",
     "idna>=2.8",
     "sniffio>=1.1",
+    "typing-extensions>=4.1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "anyio-4.0.0-py3-none-any.whl", hash = "sha256:cfdb2b588b9fc25ede96d8db56ed50848b0b649dca3dd1df0b11f683bb9e0b5f"},
-    {file = "anyio-4.0.0.tar.gz", hash = "sha256:f7ed51751b2c2add651e5747c891b47e26d2a21be5d32d9311dfe9692f3e5d7a"},
+    {file = "anyio-4.3.0-py3-none-any.whl", hash = "sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8"},
+    {file = "anyio-4.3.0.tar.gz", hash = "sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6"},
 ]
 
 [[package]]
 name = "apeye"
 version = "1.4.1"
 requires_python = ">=3.6.1"
 summary = "Handy tools for working with URLs and APIs."
+groups = ["docs"]
 dependencies = [
     "apeye-core>=1.0.0b2",
     "domdf-python-tools>=2.6.0",
     "platformdirs>=2.3.0",
     "requests>=2.24.0",
 ]
 files = [
     {file = "apeye-1.4.1-py3-none-any.whl", hash = "sha256:44e58a9104ec189bf42e76b3a7fe91e2b2879d96d48e9a77e5e32ff699c9204e"},
     {file = "apeye-1.4.1.tar.gz", hash = "sha256:14ea542fad689e3bfdbda2189a354a4908e90aee4bf84c15ab75d68453d76a36"},
 ]
 
 [[package]]
 name = "apeye-core"
-version = "1.1.4"
+version = "1.1.5"
 requires_python = ">=3.6.1"
 summary = "Core (offline) functionality for the apeye library."
+groups = ["docs"]
 dependencies = [
     "domdf-python-tools>=2.6.0",
     "idna>=2.5",
 ]
 files = [
-    {file = "apeye_core-1.1.4-py3-none-any.whl", hash = "sha256:084bc696448d3ac428fece41c1f2eb08fa9d9ce1d1b2f4d43187e3def4528a60"},
-    {file = "apeye_core-1.1.4.tar.gz", hash = "sha256:72bb89fed3baa647cb81aa28e1d851787edcbf9573853b5d2b5f87c02f50eaf5"},
+    {file = "apeye_core-1.1.5-py3-none-any.whl", hash = "sha256:dc27a93f8c9e246b3b238c5ea51edf6115ab2618ef029b9f2d9a190ec8228fbf"},
+    {file = "apeye_core-1.1.5.tar.gz", hash = "sha256:5de72ed3d00cc9b20fea55e54b7ab8f5ef8500eb33a5368bc162a5585e238a55"},
+]
+
+[[package]]
+name = "async-timeout"
+version = "4.0.3"
+requires_python = ">=3.7"
+summary = "Timeout context manager for asyncio programs"
+groups = ["default", "linting"]
+marker = "python_version < \"3.12.0\""
+files = [
+    {file = "async-timeout-4.0.3.tar.gz", hash = "sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f"},
+    {file = "async_timeout-4.0.3-py3-none-any.whl", hash = "sha256:7405140ff1230c310e51dc27b3145b9092d659ce68ff733fb0cefe3ee42be028"},
 ]
 
 [[package]]
 name = "asyncpg"
-version = "0.28.0"
-requires_python = ">=3.7.0"
+version = "0.29.0"
+requires_python = ">=3.8.0"
 summary = "An asyncio PostgreSQL driver"
+groups = ["default", "linting"]
+dependencies = [
+    "async-timeout>=4.0.3; python_version < \"3.12.0\"",
+]
 files = [
-    {file = "asyncpg-0.28.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0a6d1b954d2b296292ddff4e0060f494bb4270d87fb3655dd23c5c6096d16d83"},
-    {file = "asyncpg-0.28.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0740f836985fd2bd73dca42c50c6074d1d61376e134d7ad3ad7566c4f79f8184"},
-    {file = "asyncpg-0.28.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e907cf620a819fab1737f2dd90c0f185e2a796f139ac7de6aa3212a8af96c050"},
-    {file = "asyncpg-0.28.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:86b339984d55e8202e0c4b252e9573e26e5afa05617ed02252544f7b3e6de3e9"},
-    {file = "asyncpg-0.28.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:0c402745185414e4c204a02daca3d22d732b37359db4d2e705172324e2d94e85"},
-    {file = "asyncpg-0.28.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c88eef5e096296626e9688f00ab627231f709d0e7e3fb84bb4413dff81d996d7"},
-    {file = "asyncpg-0.28.0-cp310-cp310-win32.whl", hash = "sha256:90a7bae882a9e65a9e448fdad3e090c2609bb4637d2a9c90bfdcebbfc334bf89"},
-    {file = "asyncpg-0.28.0-cp310-cp310-win_amd64.whl", hash = "sha256:76aacdcd5e2e9999e83c8fbcb748208b60925cc714a578925adcb446d709016c"},
-    {file = "asyncpg-0.28.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:a0e08fe2c9b3618459caaef35979d45f4e4f8d4f79490c9fa3367251366af207"},
-    {file = "asyncpg-0.28.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b24e521f6060ff5d35f761a623b0042c84b9c9b9fb82786aadca95a9cb4a893b"},
-    {file = "asyncpg-0.28.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:99417210461a41891c4ff301490a8713d1ca99b694fef05dabd7139f9d64bd6c"},
-    {file = "asyncpg-0.28.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f029c5adf08c47b10bcdc857001bbef551ae51c57b3110964844a9d79ca0f267"},
-    {file = "asyncpg-0.28.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ad1d6abf6c2f5152f46fff06b0e74f25800ce8ec6c80967f0bc789974de3c652"},
-    {file = "asyncpg-0.28.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d7fa81ada2807bc50fea1dc741b26a4e99258825ba55913b0ddbf199a10d69d8"},
-    {file = "asyncpg-0.28.0-cp311-cp311-win32.whl", hash = "sha256:f33c5685e97821533df3ada9384e7784bd1e7865d2b22f153f2e4bd4a083e102"},
-    {file = "asyncpg-0.28.0-cp311-cp311-win_amd64.whl", hash = "sha256:5e7337c98fb493079d686a4a6965e8bcb059b8e1b8ec42106322fc6c1c889bb0"},
-    {file = "asyncpg-0.28.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b337ededaabc91c26bf577bfcd19b5508d879c0ad009722be5bb0a9dd30b85a0"},
-    {file = "asyncpg-0.28.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4d32b680a9b16d2957a0a3cc6b7fa39068baba8e6b728f2e0a148a67644578f4"},
-    {file = "asyncpg-0.28.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f4f62f04cdf38441a70f279505ef3b4eadf64479b17e707c950515846a2df197"},
-    {file = "asyncpg-0.28.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4f20cac332c2576c79c2e8e6464791c1f1628416d1115935a34ddd7121bfc6a4"},
-    {file = "asyncpg-0.28.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:59f9712ce01e146ff71d95d561fb68bd2d588a35a187116ef05028675462d5ed"},
-    {file = "asyncpg-0.28.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fc9e9f9ff1aa0eddcc3247a180ac9e9b51a62311e988809ac6152e8fb8097756"},
-    {file = "asyncpg-0.28.0-cp38-cp38-win32.whl", hash = "sha256:9e721dccd3838fcff66da98709ed884df1e30a95f6ba19f595a3706b4bc757e3"},
-    {file = "asyncpg-0.28.0-cp38-cp38-win_amd64.whl", hash = "sha256:8ba7d06a0bea539e0487234511d4adf81dc8762249858ed2a580534e1720db00"},
-    {file = "asyncpg-0.28.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d009b08602b8b18edef3a731f2ce6d3f57d8dac2a0a4140367e194eabd3de457"},
-    {file = "asyncpg-0.28.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:ec46a58d81446d580fb21b376ec6baecab7288ce5a578943e2fc7ab73bf7eb39"},
-    {file = "asyncpg-0.28.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7b48ceed606cce9e64fd5480a9b0b9a95cea2b798bb95129687abd8599c8b019"},
-    {file = "asyncpg-0.28.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8858f713810f4fe67876728680f42e93b7e7d5c7b61cf2118ef9153ec16b9423"},
-    {file = "asyncpg-0.28.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:5e18438a0730d1c0c1715016eacda6e9a505fc5aa931b37c97d928d44941b4bf"},
-    {file = "asyncpg-0.28.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e9c433f6fcdd61c21a715ee9128a3ca48be8ac16fa07be69262f016bb0f4dbd2"},
-    {file = "asyncpg-0.28.0-cp39-cp39-win32.whl", hash = "sha256:41e97248d9076bc8e4849da9e33e051be7ba37cd507cbd51dfe4b2d99c70e3dc"},
-    {file = "asyncpg-0.28.0-cp39-cp39-win_amd64.whl", hash = "sha256:3ed77f00c6aacfe9d79e9eff9e21729ce92a4b38e80ea99a58ed382f42ebd55b"},
-    {file = "asyncpg-0.28.0.tar.gz", hash = "sha256:7252cdc3acb2f52feaa3664280d3bcd78a46bd6c10bfd681acfffefa1120e278"},
+    {file = "asyncpg-0.29.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:72fd0ef9f00aeed37179c62282a3d14262dbbafb74ec0ba16e1b1864d8a12169"},
+    {file = "asyncpg-0.29.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:52e8f8f9ff6e21f9b39ca9f8e3e33a5fcdceaf5667a8c5c32bee158e313be385"},
+    {file = "asyncpg-0.29.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a9e6823a7012be8b68301342ba33b4740e5a166f6bbda0aee32bc01638491a22"},
+    {file = "asyncpg-0.29.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:746e80d83ad5d5464cfbf94315eb6744222ab00aa4e522b704322fb182b83610"},
+    {file = "asyncpg-0.29.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ff8e8109cd6a46ff852a5e6bab8b0a047d7ea42fcb7ca5ae6eaae97d8eacf397"},
+    {file = "asyncpg-0.29.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:97eb024685b1d7e72b1972863de527c11ff87960837919dac6e34754768098eb"},
+    {file = "asyncpg-0.29.0-cp310-cp310-win32.whl", hash = "sha256:5bbb7f2cafd8d1fa3e65431833de2642f4b2124be61a449fa064e1a08d27e449"},
+    {file = "asyncpg-0.29.0-cp310-cp310-win_amd64.whl", hash = "sha256:76c3ac6530904838a4b650b2880f8e7af938ee049e769ec2fba7cd66469d7772"},
+    {file = "asyncpg-0.29.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d4900ee08e85af01adb207519bb4e14b1cae8fd21e0ccf80fac6aa60b6da37b4"},
+    {file = "asyncpg-0.29.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:a65c1dcd820d5aea7c7d82a3fdcb70e096f8f70d1a8bf93eb458e49bfad036ac"},
+    {file = "asyncpg-0.29.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5b52e46f165585fd6af4863f268566668407c76b2c72d366bb8b522fa66f1870"},
+    {file = "asyncpg-0.29.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dc600ee8ef3dd38b8d67421359779f8ccec30b463e7aec7ed481c8346decf99f"},
+    {file = "asyncpg-0.29.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:039a261af4f38f949095e1e780bae84a25ffe3e370175193174eb08d3cecab23"},
+    {file = "asyncpg-0.29.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6feaf2d8f9138d190e5ec4390c1715c3e87b37715cd69b2c3dfca616134efd2b"},
+    {file = "asyncpg-0.29.0-cp311-cp311-win32.whl", hash = "sha256:1e186427c88225ef730555f5fdda6c1812daa884064bfe6bc462fd3a71c4b675"},
+    {file = "asyncpg-0.29.0-cp311-cp311-win_amd64.whl", hash = "sha256:cfe73ffae35f518cfd6e4e5f5abb2618ceb5ef02a2365ce64f132601000587d3"},
+    {file = "asyncpg-0.29.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:6011b0dc29886ab424dc042bf9eeb507670a3b40aece3439944006aafe023178"},
+    {file = "asyncpg-0.29.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b544ffc66b039d5ec5a7454667f855f7fec08e0dfaf5a5490dfafbb7abbd2cfb"},
+    {file = "asyncpg-0.29.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d84156d5fb530b06c493f9e7635aa18f518fa1d1395ef240d211cb563c4e2364"},
+    {file = "asyncpg-0.29.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:54858bc25b49d1114178d65a88e48ad50cb2b6f3e475caa0f0c092d5f527c106"},
+    {file = "asyncpg-0.29.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:bde17a1861cf10d5afce80a36fca736a86769ab3579532c03e45f83ba8a09c59"},
+    {file = "asyncpg-0.29.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:37a2ec1b9ff88d8773d3eb6d3784dc7e3fee7756a5317b67f923172a4748a175"},
+    {file = "asyncpg-0.29.0-cp312-cp312-win32.whl", hash = "sha256:bb1292d9fad43112a85e98ecdc2e051602bce97c199920586be83254d9dafc02"},
+    {file = "asyncpg-0.29.0-cp312-cp312-win_amd64.whl", hash = "sha256:2245be8ec5047a605e0b454c894e54bf2ec787ac04b1cb7e0d3c67aa1e32f0fe"},
+    {file = "asyncpg-0.29.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0009a300cae37b8c525e5b449233d59cd9868fd35431abc470a3e364d2b85cb9"},
+    {file = "asyncpg-0.29.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5cad1324dbb33f3ca0cd2074d5114354ed3be2b94d48ddfd88af75ebda7c43cc"},
+    {file = "asyncpg-0.29.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:012d01df61e009015944ac7543d6ee30c2dc1eb2f6b10b62a3f598beb6531548"},
+    {file = "asyncpg-0.29.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:000c996c53c04770798053e1730d34e30cb645ad95a63265aec82da9093d88e7"},
+    {file = "asyncpg-0.29.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:e0bfe9c4d3429706cf70d3249089de14d6a01192d617e9093a8e941fea8ee775"},
+    {file = "asyncpg-0.29.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:642a36eb41b6313ffa328e8a5c5c2b5bea6ee138546c9c3cf1bffaad8ee36dd9"},
+    {file = "asyncpg-0.29.0-cp38-cp38-win32.whl", hash = "sha256:a921372bbd0aa3a5822dd0409da61b4cd50df89ae85150149f8c119f23e8c408"},
+    {file = "asyncpg-0.29.0-cp38-cp38-win_amd64.whl", hash = "sha256:103aad2b92d1506700cbf51cd8bb5441e7e72e87a7b3a2ca4e32c840f051a6a3"},
+    {file = "asyncpg-0.29.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5340dd515d7e52f4c11ada32171d87c05570479dc01dc66d03ee3e150fb695da"},
+    {file = "asyncpg-0.29.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e17b52c6cf83e170d3d865571ba574577ab8e533e7361a2b8ce6157d02c665d3"},
+    {file = "asyncpg-0.29.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f100d23f273555f4b19b74a96840aa27b85e99ba4b1f18d4ebff0734e78dc090"},
+    {file = "asyncpg-0.29.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:48e7c58b516057126b363cec8ca02b804644fd012ef8e6c7e23386b7d5e6ce83"},
+    {file = "asyncpg-0.29.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:f9ea3f24eb4c49a615573724d88a48bd1b7821c890c2effe04f05382ed9e8810"},
+    {file = "asyncpg-0.29.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8d36c7f14a22ec9e928f15f92a48207546ffe68bc412f3be718eedccdf10dc5c"},
+    {file = "asyncpg-0.29.0-cp39-cp39-win32.whl", hash = "sha256:797ab8123ebaed304a1fad4d7576d5376c3a006a4100380fb9d517f0b59c1ab2"},
+    {file = "asyncpg-0.29.0-cp39-cp39-win_amd64.whl", hash = "sha256:cce08a178858b426ae1aa8409b5cc171def45d4293626e7aa6510696d46decd8"},
+    {file = "asyncpg-0.29.0.tar.gz", hash = "sha256:d1c49e1f44fffafd9a55e1a9b101590859d881d639ea2922516f5d9c512d354e"},
 ]
 
 [[package]]
 name = "asyncpg-stubs"
-version = "0.28.0"
-requires_python = ">=3.7,<4.0"
+version = "0.29.1"
+requires_python = ">=3.8,<4.0"
 summary = "asyncpg stubs"
+groups = ["linting"]
 dependencies = [
-    "asyncpg<0.29,>=0.28",
-    "typing-extensions<5.0.0,>=4.2.0",
+    "asyncpg<0.30,>=0.29",
+    "typing-extensions<5.0.0,>=4.7.0",
 ]
 files = [
-    {file = "asyncpg_stubs-0.28.0-py3-none-any.whl", hash = "sha256:db89ae4ec715e8ba5ba6f103b1e322ff101f39940333a0f68dc22f57ecaeda82"},
-    {file = "asyncpg_stubs-0.28.0.tar.gz", hash = "sha256:dd3a93e153046a92fb85d704457fe6020a3db3865308a796419e74736d70d167"},
+    {file = "asyncpg_stubs-0.29.1-py3-none-any.whl", hash = "sha256:cce994d5a19394249e74ae8d252bde3c77cee0ddfc776cc708b724fdb4adebb6"},
+    {file = "asyncpg_stubs-0.29.1.tar.gz", hash = "sha256:686afcc0af3a2f3c8e393cd850e0de430e5a139ce82b2f28ef8f693ecdf918bf"},
+]
+
+[[package]]
+name = "auto-pytabs"
+version = "0.4.0"
+requires_python = ">=3.8,<4.0"
+summary = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
+groups = ["docs"]
+dependencies = [
+    "ruff>=0.0.260",
+]
+files = [
+    {file = "auto_pytabs-0.4.0-py3-none-any.whl", hash = "sha256:941ca4f21b218249ee4d026ebaf4a8a7788a066fdb223571f1f7b93d44ac6a74"},
+    {file = "auto_pytabs-0.4.0.tar.gz", hash = "sha256:4c596aa02ea20c6c85809e5f60a22aa60499dcaa637e52d6313d07c58c5bb61e"},
+]
+
+[[package]]
+name = "auto-pytabs"
+version = "0.4.0"
+extras = ["sphinx"]
+requires_python = ">=3.8,<4.0"
+summary = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
+groups = ["docs"]
+dependencies = [
+    "auto-pytabs==0.4.0",
+    "sphinx>=4",
+]
+files = [
+    {file = "auto_pytabs-0.4.0-py3-none-any.whl", hash = "sha256:941ca4f21b218249ee4d026ebaf4a8a7788a066fdb223571f1f7b93d44ac6a74"},
+    {file = "auto_pytabs-0.4.0.tar.gz", hash = "sha256:4c596aa02ea20c6c85809e5f60a22aa60499dcaa637e52d6313d07c58c5bb61e"},
 ]
 
 [[package]]
 name = "autodocsumm"
-version = "0.2.11"
+version = "0.2.12"
 requires_python = ">=3.7"
 summary = "Extended sphinx autodoc including automatic autosummaries"
+groups = ["docs"]
 dependencies = [
     "Sphinx<8.0,>=2.2",
 ]
 files = [
-    {file = "autodocsumm-0.2.11-py3-none-any.whl", hash = "sha256:f1d0a623bf1ad64d979a9e23fd360d1fb1b8f869beaf3197f711552cddc174e2"},
-    {file = "autodocsumm-0.2.11.tar.gz", hash = "sha256:183212bd9e9f3b58a96bb21b7958ee4e06224107aa45b2fd894b61b83581b9a9"},
+    {file = "autodocsumm-0.2.12-py3-none-any.whl", hash = "sha256:b842b53c686c07a4f174721ca4e729b027367703dbf42e2508863a3c6d6c049c"},
+    {file = "autodocsumm-0.2.12.tar.gz", hash = "sha256:848fe8c38df433c6635489499b969cb47cc389ed3d7b6e75c8ccbc94d4b3bf9e"},
 ]
 
 [[package]]
 name = "babel"
-version = "2.12.1"
-requires_python = ">=3.7"
+version = "2.15.0"
+requires_python = ">=3.8"
 summary = "Internationalization utilities"
+groups = ["docs"]
 dependencies = [
     "pytz>=2015.7; python_version < \"3.9\"",
 ]
 files = [
-    {file = "Babel-2.12.1-py3-none-any.whl", hash = "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610"},
-    {file = "Babel-2.12.1.tar.gz", hash = "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"},
+    {file = "Babel-2.15.0-py3-none-any.whl", hash = "sha256:08706bdad8d0a3413266ab61bd6c34d0c28d6e1e7badf40a2cebe67644e2e1fb"},
+    {file = "babel-2.15.0.tar.gz", hash = "sha256:8daf0e265d05768bc6c7a314cf1321e9a123afc328cc635c18622a2f30a04413"},
 ]
 
 [[package]]
 name = "beautifulsoup4"
-version = "4.12.2"
+version = "4.12.3"
 requires_python = ">=3.6.0"
 summary = "Screen-scraping library"
+groups = ["docs"]
 dependencies = [
     "soupsieve>1.2",
 ]
 files = [
-    {file = "beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
-    {file = "beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
+    {file = "beautifulsoup4-4.12.3-py3-none-any.whl", hash = "sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed"},
+    {file = "beautifulsoup4-4.12.3.tar.gz", hash = "sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051"},
 ]
 
 [[package]]
 name = "black"
-version = "23.9.1"
+version = "24.4.2"
 requires_python = ">=3.8"
 summary = "The uncompromising code formatter."
+groups = ["docs"]
 dependencies = [
     "click>=8.0.0",
     "mypy-extensions>=0.4.3",
     "packaging>=22.0",
     "pathspec>=0.9.0",
     "platformdirs>=2",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typing-extensions>=4.0.1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "black-23.9.1-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:d6bc09188020c9ac2555a498949401ab35bb6bf76d4e0f8ee251694664df6301"},
-    {file = "black-23.9.1-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:13ef033794029b85dfea8032c9d3b92b42b526f1ff4bf13b2182ce4e917f5100"},
-    {file = "black-23.9.1-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:75a2dc41b183d4872d3a500d2b9c9016e67ed95738a3624f4751a0cb4818fe71"},
-    {file = "black-23.9.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13a2e4a93bb8ca74a749b6974925c27219bb3df4d42fc45e948a5d9feb5122b7"},
-    {file = "black-23.9.1-cp310-cp310-win_amd64.whl", hash = "sha256:adc3e4442eef57f99b5590b245a328aad19c99552e0bdc7f0b04db6656debd80"},
-    {file = "black-23.9.1-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:8431445bf62d2a914b541da7ab3e2b4f3bc052d2ccbf157ebad18ea126efb91f"},
-    {file = "black-23.9.1-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:8fc1ddcf83f996247505db6b715294eba56ea9372e107fd54963c7553f2b6dfe"},
-    {file = "black-23.9.1-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:7d30ec46de88091e4316b17ae58bbbfc12b2de05e069030f6b747dfc649ad186"},
-    {file = "black-23.9.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:031e8c69f3d3b09e1aa471a926a1eeb0b9071f80b17689a655f7885ac9325a6f"},
-    {file = "black-23.9.1-cp311-cp311-win_amd64.whl", hash = "sha256:538efb451cd50f43aba394e9ec7ad55a37598faae3348d723b59ea8e91616300"},
-    {file = "black-23.9.1-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:638619a559280de0c2aa4d76f504891c9860bb8fa214267358f0a20f27c12948"},
-    {file = "black-23.9.1-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:a732b82747235e0542c03bf352c126052c0fbc458d8a239a94701175b17d4855"},
-    {file = "black-23.9.1-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:cf3a4d00e4cdb6734b64bf23cd4341421e8953615cba6b3670453737a72ec204"},
-    {file = "black-23.9.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cf99f3de8b3273a8317681d8194ea222f10e0133a24a7548c73ce44ea1679377"},
-    {file = "black-23.9.1-cp38-cp38-win_amd64.whl", hash = "sha256:14f04c990259576acd093871e7e9b14918eb28f1866f91968ff5524293f9c573"},
-    {file = "black-23.9.1-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:c619f063c2d68f19b2d7270f4cf3192cb81c9ec5bc5ba02df91471d0b88c4c5c"},
-    {file = "black-23.9.1-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:6a3b50e4b93f43b34a9d3ef00d9b6728b4a722c997c99ab09102fd5efdb88325"},
-    {file = "black-23.9.1-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:c46767e8df1b7beefb0899c4a95fb43058fa8500b6db144f4ff3ca38eb2f6393"},
-    {file = "black-23.9.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50254ebfa56aa46a9fdd5d651f9637485068a1adf42270148cd101cdf56e0ad9"},
-    {file = "black-23.9.1-cp39-cp39-win_amd64.whl", hash = "sha256:403397c033adbc45c2bd41747da1f7fc7eaa44efbee256b53842470d4ac5a70f"},
-    {file = "black-23.9.1-py3-none-any.whl", hash = "sha256:6ccd59584cc834b6d127628713e4b6b968e5f79572da66284532525a042549f9"},
-    {file = "black-23.9.1.tar.gz", hash = "sha256:24b6b3ff5c6d9ea08a8888f6977eae858e1f340d7260cf56d70a49823236b62d"},
+    {file = "black-24.4.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:dd1b5a14e417189db4c7b64a6540f31730713d173f0b63e55fabd52d61d8fdce"},
+    {file = "black-24.4.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8e537d281831ad0e71007dcdcbe50a71470b978c453fa41ce77186bbe0ed6021"},
+    {file = "black-24.4.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eaea3008c281f1038edb473c1aa8ed8143a5535ff18f978a318f10302b254063"},
+    {file = "black-24.4.2-cp310-cp310-win_amd64.whl", hash = "sha256:7768a0dbf16a39aa5e9a3ded568bb545c8c2727396d063bbaf847df05b08cd96"},
+    {file = "black-24.4.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:257d724c2c9b1660f353b36c802ccece186a30accc7742c176d29c146df6e474"},
+    {file = "black-24.4.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:bdde6f877a18f24844e381d45e9947a49e97933573ac9d4345399be37621e26c"},
+    {file = "black-24.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e151054aa00bad1f4e1f04919542885f89f5f7d086b8a59e5000e6c616896ffb"},
+    {file = "black-24.4.2-cp311-cp311-win_amd64.whl", hash = "sha256:7e122b1c4fb252fd85df3ca93578732b4749d9be076593076ef4d07a0233c3e1"},
+    {file = "black-24.4.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:accf49e151c8ed2c0cdc528691838afd217c50412534e876a19270fea1e28e2d"},
+    {file = "black-24.4.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:88c57dc656038f1ab9f92b3eb5335ee9b021412feaa46330d5eba4e51fe49b04"},
+    {file = "black-24.4.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be8bef99eb46d5021bf053114442914baeb3649a89dc5f3a555c88737e5e98fc"},
+    {file = "black-24.4.2-cp312-cp312-win_amd64.whl", hash = "sha256:415e686e87dbbe6f4cd5ef0fbf764af7b89f9057b97c908742b6008cc554b9c0"},
+    {file = "black-24.4.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bf10f7310db693bb62692609b397e8d67257c55f949abde4c67f9cc574492cc7"},
+    {file = "black-24.4.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:98e123f1d5cfd42f886624d84464f7756f60ff6eab89ae845210631714f6db94"},
+    {file = "black-24.4.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:48a85f2cb5e6799a9ef05347b476cce6c182d6c71ee36925a6c194d074336ef8"},
+    {file = "black-24.4.2-cp38-cp38-win_amd64.whl", hash = "sha256:b1530ae42e9d6d5b670a34db49a94115a64596bc77710b1d05e9801e62ca0a7c"},
+    {file = "black-24.4.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:37aae07b029fa0174d39daf02748b379399b909652a806e5708199bd93899da1"},
+    {file = "black-24.4.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:da33a1a5e49c4122ccdfd56cd021ff1ebc4a1ec4e2d01594fef9b6f267a9e741"},
+    {file = "black-24.4.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef703f83fc32e131e9bcc0a5094cfe85599e7109f896fe8bc96cc402f3eb4b6e"},
+    {file = "black-24.4.2-cp39-cp39-win_amd64.whl", hash = "sha256:b9176b9832e84308818a99a561e90aa479e73c523b3f77afd07913380ae2eab7"},
+    {file = "black-24.4.2-py3-none-any.whl", hash = "sha256:d36ed1124bb81b32f8614555b34cc4259c3fbc7eec17870e8ff8ded335b58d8c"},
+    {file = "black-24.4.2.tar.gz", hash = "sha256:c872b53057f000085da66a19c55d68f6f8ddcac2642392ad3a355878406fbd4d"},
 ]
 
 [[package]]
 name = "blacken-docs"
 version = "1.16.0"
 requires_python = ">=3.8"
 summary = "Run Black on Python code blocks in documentation files."
+groups = ["docs"]
 dependencies = [
     "black>=22.1.0",
 ]
 files = [
     {file = "blacken_docs-1.16.0-py3-none-any.whl", hash = "sha256:b0dcb84b28ebfb352a2539202d396f50e15a54211e204a8005798f1d1edb7df8"},
     {file = "blacken_docs-1.16.0.tar.gz", hash = "sha256:b4bdc3f3d73898dfbf0166f292c6ccfe343e65fc22ddef5319c95d1a8dcc6c1c"},
 ]
 
 [[package]]
 name = "cachecontrol"
-version = "0.13.1"
+version = "0.14.0"
 requires_python = ">=3.7"
 summary = "httplib2 caching for requests"
+groups = ["docs"]
 dependencies = [
-    "msgpack>=0.5.2",
+    "msgpack<2.0.0,>=0.5.2",
     "requests>=2.16.0",
 ]
 files = [
-    {file = "cachecontrol-0.13.1-py3-none-any.whl", hash = "sha256:95dedbec849f46dda3137866dc28b9d133fc9af55f5b805ab1291833e4457aa4"},
-    {file = "cachecontrol-0.13.1.tar.gz", hash = "sha256:f012366b79d2243a6118309ce73151bf52a38d4a5dac8ea57f09bd29087e506b"},
+    {file = "cachecontrol-0.14.0-py3-none-any.whl", hash = "sha256:f5bf3f0620c38db2e5122c0726bdebb0d16869de966ea6a2befe92470b740ea0"},
+    {file = "cachecontrol-0.14.0.tar.gz", hash = "sha256:7db1195b41c81f8274a7bbd97c956f44e8348265a1bc7641c37dfebc39f0c938"},
 ]
 
 [[package]]
 name = "cachecontrol"
-version = "0.13.1"
+version = "0.14.0"
 extras = ["filecache"]
 requires_python = ">=3.7"
 summary = "httplib2 caching for requests"
+groups = ["docs"]
 dependencies = [
-    "cachecontrol==0.13.1",
+    "cachecontrol==0.14.0",
     "filelock>=3.8.0",
 ]
 files = [
-    {file = "cachecontrol-0.13.1-py3-none-any.whl", hash = "sha256:95dedbec849f46dda3137866dc28b9d133fc9af55f5b805ab1291833e4457aa4"},
-    {file = "cachecontrol-0.13.1.tar.gz", hash = "sha256:f012366b79d2243a6118309ce73151bf52a38d4a5dac8ea57f09bd29087e506b"},
+    {file = "cachecontrol-0.14.0-py3-none-any.whl", hash = "sha256:f5bf3f0620c38db2e5122c0726bdebb0d16869de966ea6a2befe92470b740ea0"},
+    {file = "cachecontrol-0.14.0.tar.gz", hash = "sha256:7db1195b41c81f8274a7bbd97c956f44e8348265a1bc7641c37dfebc39f0c938"},
 ]
 
 [[package]]
 name = "certifi"
-version = "2023.7.22"
+version = "2024.2.2"
 requires_python = ">=3.6"
 summary = "Python package for providing Mozilla's CA Bundle."
+groups = ["default", "docs"]
 files = [
-    {file = "certifi-2023.7.22-py3-none-any.whl", hash = "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"},
-    {file = "certifi-2023.7.22.tar.gz", hash = "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082"},
+    {file = "certifi-2024.2.2-py3-none-any.whl", hash = "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"},
+    {file = "certifi-2024.2.2.tar.gz", hash = "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f"},
 ]
 
 [[package]]
 name = "cfgv"
 version = "3.4.0"
 requires_python = ">=3.8"
 summary = "Validate configuration and produce human readable error messages."
+groups = ["linting"]
 files = [
     {file = "cfgv-3.4.0-py2.py3-none-any.whl", hash = "sha256:b7265b1f29fd3316bfcd2b330d63d024f2bfd8bcb8b0272f8e19a504856c48f9"},
     {file = "cfgv-3.4.0.tar.gz", hash = "sha256:e52591d4c5f5dead8e0f673fb16db7949d2cfb3f7da4582893288f0ded8fe560"},
 ]
 
 [[package]]
 name = "charset-normalizer"
-version = "3.3.0"
+version = "3.3.2"
 requires_python = ">=3.7.0"
 summary = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
+groups = ["docs"]
 files = [
-    {file = "charset-normalizer-3.3.0.tar.gz", hash = "sha256:63563193aec44bce707e0c5ca64ff69fa72ed7cf34ce6e11d5127555756fd2f6"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:effe5406c9bd748a871dbcaf3ac69167c38d72db8c9baf3ff954c344f31c4cbe"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4162918ef3098851fcd8a628bf9b6a98d10c380725df9e04caf5ca6dd48c847a"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0570d21da019941634a531444364f2482e8db0b3425fcd5ac0c36565a64142c8"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5707a746c6083a3a74b46b3a631d78d129edab06195a92a8ece755aac25a3f3d"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:278c296c6f96fa686d74eb449ea1697f3c03dc28b75f873b65b5201806346a69"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a4b71f4d1765639372a3b32d2638197f5cd5221b19531f9245fcc9ee62d38f56"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f5969baeaea61c97efa706b9b107dcba02784b1601c74ac84f2a532ea079403e"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a3f93dab657839dfa61025056606600a11d0b696d79386f974e459a3fbc568ec"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:db756e48f9c5c607b5e33dd36b1d5872d0422e960145b08ab0ec7fd420e9d649"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:232ac332403e37e4a03d209a3f92ed9071f7d3dbda70e2a5e9cff1c4ba9f0678"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:e5c1502d4ace69a179305abb3f0bb6141cbe4714bc9b31d427329a95acfc8bdd"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:2502dd2a736c879c0f0d3e2161e74d9907231e25d35794584b1ca5284e43f596"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:23e8565ab7ff33218530bc817922fae827420f143479b753104ab801145b1d5b"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-win32.whl", hash = "sha256:1872d01ac8c618a8da634e232f24793883d6e456a66593135aeafe3784b0848d"},
-    {file = "charset_normalizer-3.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:557b21a44ceac6c6b9773bc65aa1b4cc3e248a5ad2f5b914b91579a32e22204d"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:d7eff0f27edc5afa9e405f7165f85a6d782d308f3b6b9d96016c010597958e63"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6a685067d05e46641d5d1623d7c7fdf15a357546cbb2f71b0ebde91b175ffc3e"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:0d3d5b7db9ed8a2b11a774db2bbea7ba1884430a205dbd54a32d61d7c2a190fa"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2935ffc78db9645cb2086c2f8f4cfd23d9b73cc0dc80334bc30aac6f03f68f8c"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9fe359b2e3a7729010060fbca442ca225280c16e923b37db0e955ac2a2b72a05"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:380c4bde80bce25c6e4f77b19386f5ec9db230df9f2f2ac1e5ad7af2caa70459"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0d1e3732768fecb052d90d62b220af62ead5748ac51ef61e7b32c266cac9293"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1b2919306936ac6efb3aed1fbf81039f7087ddadb3160882a57ee2ff74fd2382"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f8888e31e3a85943743f8fc15e71536bda1c81d5aa36d014a3c0c44481d7db6e"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:82eb849f085624f6a607538ee7b83a6d8126df6d2f7d3b319cb837b289123078"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:7b8b8bf1189b3ba9b8de5c8db4d541b406611a71a955bbbd7385bbc45fcb786c"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:5adf257bd58c1b8632046bbe43ee38c04e1038e9d37de9c57a94d6bd6ce5da34"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:c350354efb159b8767a6244c166f66e67506e06c8924ed74669b2c70bc8735b1"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-win32.whl", hash = "sha256:02af06682e3590ab952599fbadac535ede5d60d78848e555aa58d0c0abbde786"},
-    {file = "charset_normalizer-3.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:86d1f65ac145e2c9ed71d8ffb1905e9bba3a91ae29ba55b4c46ae6fc31d7c0d4"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:3b447982ad46348c02cb90d230b75ac34e9886273df3a93eec0539308a6296d7"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:abf0d9f45ea5fb95051c8bfe43cb40cda383772f7e5023a83cc481ca2604d74e"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b09719a17a2301178fac4470d54b1680b18a5048b481cb8890e1ef820cb80455"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b3d9b48ee6e3967b7901c052b670c7dda6deb812c309439adaffdec55c6d7b78"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:edfe077ab09442d4ef3c52cb1f9dab89bff02f4524afc0acf2d46be17dc479f5"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3debd1150027933210c2fc321527c2299118aa929c2f5a0a80ab6953e3bd1908"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:86f63face3a527284f7bb8a9d4f78988e3c06823f7bea2bd6f0e0e9298ca0403"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:24817cb02cbef7cd499f7c9a2735286b4782bd47a5b3516a0e84c50eab44b98e"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:c71f16da1ed8949774ef79f4a0260d28b83b3a50c6576f8f4f0288d109777989"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:9cf3126b85822c4e53aa28c7ec9869b924d6fcfb76e77a45c44b83d91afd74f9"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:b3b2316b25644b23b54a6f6401074cebcecd1244c0b8e80111c9a3f1c8e83d65"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:03680bb39035fbcffe828eae9c3f8afc0428c91d38e7d61aa992ef7a59fb120e"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cc152c5dd831641e995764f9f0b6589519f6f5123258ccaca8c6d34572fefa8"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-win32.whl", hash = "sha256:b8f3307af845803fb0b060ab76cf6dd3a13adc15b6b451f54281d25911eb92df"},
-    {file = "charset_normalizer-3.3.0-cp312-cp312-win_amd64.whl", hash = "sha256:8eaf82f0eccd1505cf39a45a6bd0a8cf1c70dcfc30dba338207a969d91b965c0"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:67b8cc9574bb518ec76dc8e705d4c39ae78bb96237cb533edac149352c1f39fe"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ac71b2977fb90c35d41c9453116e283fac47bb9096ad917b8819ca8b943abecd"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:3ae38d325b512f63f8da31f826e6cb6c367336f95e418137286ba362925c877e"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:542da1178c1c6af8873e143910e2269add130a299c9106eef2594e15dae5e482"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:30a85aed0b864ac88309b7d94be09f6046c834ef60762a8833b660139cfbad13"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:aae32c93e0f64469f74ccc730a7cb21c7610af3a775157e50bbd38f816536b38"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:15b26ddf78d57f1d143bdf32e820fd8935d36abe8a25eb9ec0b5a71c82eb3895"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7f5d10bae5d78e4551b7be7a9b29643a95aded9d0f602aa2ba584f0388e7a557"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:249c6470a2b60935bafd1d1d13cd613f8cd8388d53461c67397ee6a0f5dce741"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:c5a74c359b2d47d26cdbbc7845e9662d6b08a1e915eb015d044729e92e7050b7"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:b5bcf60a228acae568e9911f410f9d9e0d43197d030ae5799e20dca8df588287"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:187d18082694a29005ba2944c882344b6748d5be69e3a89bf3cc9d878e548d5a"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:81bf654678e575403736b85ba3a7867e31c2c30a69bc57fe88e3ace52fb17b89"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-win32.whl", hash = "sha256:85a32721ddde63c9df9ebb0d2045b9691d9750cb139c161c80e500d210f5e26e"},
-    {file = "charset_normalizer-3.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:468d2a840567b13a590e67dd276c570f8de00ed767ecc611994c301d0f8c014f"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:e0fc42822278451bc13a2e8626cf2218ba570f27856b536e00cfa53099724828"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:09c77f964f351a7369cc343911e0df63e762e42bac24cd7d18525961c81754f4"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:12ebea541c44fdc88ccb794a13fe861cc5e35d64ed689513a5c03d05b53b7c82"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:805dfea4ca10411a5296bcc75638017215a93ffb584c9e344731eef0dcfb026a"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:96c2b49eb6a72c0e4991d62406e365d87067ca14c1a729a870d22354e6f68115"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:aaf7b34c5bc56b38c931a54f7952f1ff0ae77a2e82496583b247f7c969eb1479"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:619d1c96099be5823db34fe89e2582b336b5b074a7f47f819d6b3a57ff7bdb86"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a0ac5e7015a5920cfce654c06618ec40c33e12801711da6b4258af59a8eff00a"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:93aa7eef6ee71c629b51ef873991d6911b906d7312c6e8e99790c0f33c576f89"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7966951325782121e67c81299a031f4c115615e68046f79b85856b86ebffc4cd"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:02673e456dc5ab13659f85196c534dc596d4ef260e4d86e856c3b2773ce09843"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:c2af80fb58f0f24b3f3adcb9148e6203fa67dd3f61c4af146ecad033024dde43"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:153e7b6e724761741e0974fc4dcd406d35ba70b92bfe3fedcb497226c93b9da7"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-win32.whl", hash = "sha256:d47ecf253780c90ee181d4d871cd655a789da937454045b17b5798da9393901a"},
-    {file = "charset_normalizer-3.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:d97d85fa63f315a8bdaba2af9a6a686e0eceab77b3089af45133252618e70884"},
-    {file = "charset_normalizer-3.3.0-py3-none-any.whl", hash = "sha256:e46cd37076971c1040fc8c41273a8b3e2c624ce4f2be3f5dfcb7a430c1d3acc2"},
+    {file = "charset-normalizer-3.3.2.tar.gz", hash = "sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-win32.whl", hash = "sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73"},
+    {file = "charset_normalizer-3.3.2-cp310-cp310-win_amd64.whl", hash = "sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-win32.whl", hash = "sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab"},
+    {file = "charset_normalizer-3.3.2-cp311-cp311-win_amd64.whl", hash = "sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-win32.whl", hash = "sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7"},
+    {file = "charset_normalizer-3.3.2-cp312-cp312-win_amd64.whl", hash = "sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-win32.whl", hash = "sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25"},
+    {file = "charset_normalizer-3.3.2-cp38-cp38-win_amd64.whl", hash = "sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-win32.whl", hash = "sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f"},
+    {file = "charset_normalizer-3.3.2-cp39-cp39-win_amd64.whl", hash = "sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d"},
+    {file = "charset_normalizer-3.3.2-py3-none-any.whl", hash = "sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc"},
 ]
 
 [[package]]
 name = "click"
 version = "8.1.7"
 requires_python = ">=3.7"
 summary = "Composable command line interface toolkit"
+groups = ["default", "docs"]
 dependencies = [
     "colorama; platform_system == \"Windows\"",
 ]
 files = [
     {file = "click-8.1.7-py3-none-any.whl", hash = "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28"},
     {file = "click-8.1.7.tar.gz", hash = "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"},
 ]
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 summary = "Cross-platform colored terminal text."
+groups = ["default", "docs", "test"]
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.3.1"
+version = "7.5.1"
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
+groups = ["test"]
 files = [
-    {file = "coverage-7.3.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:cd0f7429ecfd1ff597389907045ff209c8fdb5b013d38cfa7c60728cb484b6e3"},
-    {file = "coverage-7.3.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:966f10df9b2b2115da87f50f6a248e313c72a668248be1b9060ce935c871f276"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0575c37e207bb9b98b6cf72fdaaa18ac909fb3d153083400c2d48e2e6d28bd8e"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:245c5a99254e83875c7fed8b8b2536f040997a9b76ac4c1da5bff398c06e860f"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c96dd7798d83b960afc6c1feb9e5af537fc4908852ef025600374ff1a017392"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:de30c1aa80f30af0f6b2058a91505ea6e36d6535d437520067f525f7df123887"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:50dd1e2dd13dbbd856ffef69196781edff26c800a74f070d3b3e3389cab2600d"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b9c0c19f70d30219113b18fe07e372b244fb2a773d4afde29d5a2f7930765136"},
-    {file = "coverage-7.3.1-cp310-cp310-win32.whl", hash = "sha256:770f143980cc16eb601ccfd571846e89a5fe4c03b4193f2e485268f224ab602f"},
-    {file = "coverage-7.3.1-cp310-cp310-win_amd64.whl", hash = "sha256:cdd088c00c39a27cfa5329349cc763a48761fdc785879220d54eb785c8a38520"},
-    {file = "coverage-7.3.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:74bb470399dc1989b535cb41f5ca7ab2af561e40def22d7e188e0a445e7639e3"},
-    {file = "coverage-7.3.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:025ded371f1ca280c035d91b43252adbb04d2aea4c7105252d3cbc227f03b375"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a6191b3a6ad3e09b6cfd75b45c6aeeffe7e3b0ad46b268345d159b8df8d835f9"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7eb0b188f30e41ddd659a529e385470aa6782f3b412f860ce22b2491c89b8593"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75c8f0df9dfd8ff745bccff75867d63ef336e57cc22b2908ee725cc552689ec8"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:7eb3cd48d54b9bd0e73026dedce44773214064be93611deab0b6a43158c3d5a0"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:ac3c5b7e75acac31e490b7851595212ed951889918d398b7afa12736c85e13ce"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5b4ee7080878077af0afa7238df1b967f00dc10763f6e1b66f5cced4abebb0a3"},
-    {file = "coverage-7.3.1-cp311-cp311-win32.whl", hash = "sha256:229c0dd2ccf956bf5aeede7e3131ca48b65beacde2029f0361b54bf93d36f45a"},
-    {file = "coverage-7.3.1-cp311-cp311-win_amd64.whl", hash = "sha256:c6f55d38818ca9596dc9019eae19a47410d5322408140d9a0076001a3dcb938c"},
-    {file = "coverage-7.3.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:5289490dd1c3bb86de4730a92261ae66ea8d44b79ed3cc26464f4c2cde581fbc"},
-    {file = "coverage-7.3.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ca833941ec701fda15414be400c3259479bfde7ae6d806b69e63b3dc423b1832"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cd694e19c031733e446c8024dedd12a00cda87e1c10bd7b8539a87963685e969"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:aab8e9464c00da5cb9c536150b7fbcd8850d376d1151741dd0d16dfe1ba4fd26"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:87d38444efffd5b056fcc026c1e8d862191881143c3aa80bb11fcf9dca9ae204"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:8a07b692129b8a14ad7a37941a3029c291254feb7a4237f245cfae2de78de037"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:2829c65c8faaf55b868ed7af3c7477b76b1c6ebeee99a28f59a2cb5907a45760"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:1f111a7d85658ea52ffad7084088277135ec5f368457275fc57f11cebb15607f"},
-    {file = "coverage-7.3.1-cp312-cp312-win32.whl", hash = "sha256:c397c70cd20f6df7d2a52283857af622d5f23300c4ca8e5bd8c7a543825baa5a"},
-    {file = "coverage-7.3.1-cp312-cp312-win_amd64.whl", hash = "sha256:5ae4c6da8b3d123500f9525b50bf0168023313963e0e2e814badf9000dd6ef92"},
-    {file = "coverage-7.3.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ca70466ca3a17460e8fc9cea7123c8cbef5ada4be3140a1ef8f7b63f2f37108f"},
-    {file = "coverage-7.3.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f2781fd3cabc28278dc982a352f50c81c09a1a500cc2086dc4249853ea96b981"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6407424621f40205bbe6325686417e5e552f6b2dba3535dd1f90afc88a61d465"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:04312b036580ec505f2b77cbbdfb15137d5efdfade09156961f5277149f5e344"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ac9ad38204887349853d7c313f53a7b1c210ce138c73859e925bc4e5d8fc18e7"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:53669b79f3d599da95a0afbef039ac0fadbb236532feb042c534fbb81b1a4e40"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:614f1f98b84eb256e4f35e726bfe5ca82349f8dfa576faabf8a49ca09e630086"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f1a317fdf5c122ad642db8a97964733ab7c3cf6009e1a8ae8821089993f175ff"},
-    {file = "coverage-7.3.1-cp38-cp38-win32.whl", hash = "sha256:defbbb51121189722420a208957e26e49809feafca6afeef325df66c39c4fdb3"},
-    {file = "coverage-7.3.1-cp38-cp38-win_amd64.whl", hash = "sha256:f4f456590eefb6e1b3c9ea6328c1e9fa0f1006e7481179d749b3376fc793478e"},
-    {file = "coverage-7.3.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:f12d8b11a54f32688b165fd1a788c408f927b0960984b899be7e4c190ae758f1"},
-    {file = "coverage-7.3.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f09195dda68d94a53123883de75bb97b0e35f5f6f9f3aa5bf6e496da718f0cb6"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c6601a60318f9c3945be6ea0f2a80571f4299b6801716f8a6e4846892737ebe4"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:07d156269718670d00a3b06db2288b48527fc5f36859425ff7cec07c6b367745"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:636a8ac0b044cfeccae76a36f3b18264edcc810a76a49884b96dd744613ec0b7"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:5d991e13ad2ed3aced177f524e4d670f304c8233edad3210e02c465351f785a0"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:586649ada7cf139445da386ab6f8ef00e6172f11a939fc3b2b7e7c9082052fa0"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:4aba512a15a3e1e4fdbfed2f5392ec221434a614cc68100ca99dcad7af29f3f8"},
-    {file = "coverage-7.3.1-cp39-cp39-win32.whl", hash = "sha256:6bc6f3f4692d806831c136c5acad5ccedd0262aa44c087c46b7101c77e139140"},
-    {file = "coverage-7.3.1-cp39-cp39-win_amd64.whl", hash = "sha256:553d7094cb27db58ea91332e8b5681bac107e7242c23f7629ab1316ee73c4981"},
-    {file = "coverage-7.3.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:220eb51f5fb38dfdb7e5d54284ca4d0cd70ddac047d750111a68ab1798945194"},
-    {file = "coverage-7.3.1.tar.gz", hash = "sha256:6cb7fe1581deb67b782c153136541e20901aa312ceedaf1467dcb35255787952"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d"},
+    {file = "coverage-7.5.1-cp38-cp38-win32.whl", hash = "sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41"},
+    {file = "coverage-7.5.1-cp38-cp38-win_amd64.whl", hash = "sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668"},
+    {file = "coverage-7.5.1-cp39-cp39-win32.whl", hash = "sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981"},
+    {file = "coverage-7.5.1-cp39-cp39-win_amd64.whl", hash = "sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.3.1"
+version = "7.5.1"
 extras = ["toml"]
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
+groups = ["test"]
 dependencies = [
-    "coverage==7.3.1",
+    "coverage==7.5.1",
     "tomli; python_full_version <= \"3.11.0a6\"",
 ]
 files = [
-    {file = "coverage-7.3.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:cd0f7429ecfd1ff597389907045ff209c8fdb5b013d38cfa7c60728cb484b6e3"},
-    {file = "coverage-7.3.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:966f10df9b2b2115da87f50f6a248e313c72a668248be1b9060ce935c871f276"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0575c37e207bb9b98b6cf72fdaaa18ac909fb3d153083400c2d48e2e6d28bd8e"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:245c5a99254e83875c7fed8b8b2536f040997a9b76ac4c1da5bff398c06e860f"},
-    {file = "coverage-7.3.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4c96dd7798d83b960afc6c1feb9e5af537fc4908852ef025600374ff1a017392"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:de30c1aa80f30af0f6b2058a91505ea6e36d6535d437520067f525f7df123887"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:50dd1e2dd13dbbd856ffef69196781edff26c800a74f070d3b3e3389cab2600d"},
-    {file = "coverage-7.3.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b9c0c19f70d30219113b18fe07e372b244fb2a773d4afde29d5a2f7930765136"},
-    {file = "coverage-7.3.1-cp310-cp310-win32.whl", hash = "sha256:770f143980cc16eb601ccfd571846e89a5fe4c03b4193f2e485268f224ab602f"},
-    {file = "coverage-7.3.1-cp310-cp310-win_amd64.whl", hash = "sha256:cdd088c00c39a27cfa5329349cc763a48761fdc785879220d54eb785c8a38520"},
-    {file = "coverage-7.3.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:74bb470399dc1989b535cb41f5ca7ab2af561e40def22d7e188e0a445e7639e3"},
-    {file = "coverage-7.3.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:025ded371f1ca280c035d91b43252adbb04d2aea4c7105252d3cbc227f03b375"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a6191b3a6ad3e09b6cfd75b45c6aeeffe7e3b0ad46b268345d159b8df8d835f9"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7eb0b188f30e41ddd659a529e385470aa6782f3b412f860ce22b2491c89b8593"},
-    {file = "coverage-7.3.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75c8f0df9dfd8ff745bccff75867d63ef336e57cc22b2908ee725cc552689ec8"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:7eb3cd48d54b9bd0e73026dedce44773214064be93611deab0b6a43158c3d5a0"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:ac3c5b7e75acac31e490b7851595212ed951889918d398b7afa12736c85e13ce"},
-    {file = "coverage-7.3.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5b4ee7080878077af0afa7238df1b967f00dc10763f6e1b66f5cced4abebb0a3"},
-    {file = "coverage-7.3.1-cp311-cp311-win32.whl", hash = "sha256:229c0dd2ccf956bf5aeede7e3131ca48b65beacde2029f0361b54bf93d36f45a"},
-    {file = "coverage-7.3.1-cp311-cp311-win_amd64.whl", hash = "sha256:c6f55d38818ca9596dc9019eae19a47410d5322408140d9a0076001a3dcb938c"},
-    {file = "coverage-7.3.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:5289490dd1c3bb86de4730a92261ae66ea8d44b79ed3cc26464f4c2cde581fbc"},
-    {file = "coverage-7.3.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ca833941ec701fda15414be400c3259479bfde7ae6d806b69e63b3dc423b1832"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cd694e19c031733e446c8024dedd12a00cda87e1c10bd7b8539a87963685e969"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:aab8e9464c00da5cb9c536150b7fbcd8850d376d1151741dd0d16dfe1ba4fd26"},
-    {file = "coverage-7.3.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:87d38444efffd5b056fcc026c1e8d862191881143c3aa80bb11fcf9dca9ae204"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:8a07b692129b8a14ad7a37941a3029c291254feb7a4237f245cfae2de78de037"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:2829c65c8faaf55b868ed7af3c7477b76b1c6ebeee99a28f59a2cb5907a45760"},
-    {file = "coverage-7.3.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:1f111a7d85658ea52ffad7084088277135ec5f368457275fc57f11cebb15607f"},
-    {file = "coverage-7.3.1-cp312-cp312-win32.whl", hash = "sha256:c397c70cd20f6df7d2a52283857af622d5f23300c4ca8e5bd8c7a543825baa5a"},
-    {file = "coverage-7.3.1-cp312-cp312-win_amd64.whl", hash = "sha256:5ae4c6da8b3d123500f9525b50bf0168023313963e0e2e814badf9000dd6ef92"},
-    {file = "coverage-7.3.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ca70466ca3a17460e8fc9cea7123c8cbef5ada4be3140a1ef8f7b63f2f37108f"},
-    {file = "coverage-7.3.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f2781fd3cabc28278dc982a352f50c81c09a1a500cc2086dc4249853ea96b981"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6407424621f40205bbe6325686417e5e552f6b2dba3535dd1f90afc88a61d465"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:04312b036580ec505f2b77cbbdfb15137d5efdfade09156961f5277149f5e344"},
-    {file = "coverage-7.3.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ac9ad38204887349853d7c313f53a7b1c210ce138c73859e925bc4e5d8fc18e7"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:53669b79f3d599da95a0afbef039ac0fadbb236532feb042c534fbb81b1a4e40"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:614f1f98b84eb256e4f35e726bfe5ca82349f8dfa576faabf8a49ca09e630086"},
-    {file = "coverage-7.3.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f1a317fdf5c122ad642db8a97964733ab7c3cf6009e1a8ae8821089993f175ff"},
-    {file = "coverage-7.3.1-cp38-cp38-win32.whl", hash = "sha256:defbbb51121189722420a208957e26e49809feafca6afeef325df66c39c4fdb3"},
-    {file = "coverage-7.3.1-cp38-cp38-win_amd64.whl", hash = "sha256:f4f456590eefb6e1b3c9ea6328c1e9fa0f1006e7481179d749b3376fc793478e"},
-    {file = "coverage-7.3.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:f12d8b11a54f32688b165fd1a788c408f927b0960984b899be7e4c190ae758f1"},
-    {file = "coverage-7.3.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f09195dda68d94a53123883de75bb97b0e35f5f6f9f3aa5bf6e496da718f0cb6"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c6601a60318f9c3945be6ea0f2a80571f4299b6801716f8a6e4846892737ebe4"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:07d156269718670d00a3b06db2288b48527fc5f36859425ff7cec07c6b367745"},
-    {file = "coverage-7.3.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:636a8ac0b044cfeccae76a36f3b18264edcc810a76a49884b96dd744613ec0b7"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:5d991e13ad2ed3aced177f524e4d670f304c8233edad3210e02c465351f785a0"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:586649ada7cf139445da386ab6f8ef00e6172f11a939fc3b2b7e7c9082052fa0"},
-    {file = "coverage-7.3.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:4aba512a15a3e1e4fdbfed2f5392ec221434a614cc68100ca99dcad7af29f3f8"},
-    {file = "coverage-7.3.1-cp39-cp39-win32.whl", hash = "sha256:6bc6f3f4692d806831c136c5acad5ccedd0262aa44c087c46b7101c77e139140"},
-    {file = "coverage-7.3.1-cp39-cp39-win_amd64.whl", hash = "sha256:553d7094cb27db58ea91332e8b5681bac107e7242c23f7629ab1316ee73c4981"},
-    {file = "coverage-7.3.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:220eb51f5fb38dfdb7e5d54284ca4d0cd70ddac047d750111a68ab1798945194"},
-    {file = "coverage-7.3.1.tar.gz", hash = "sha256:6cb7fe1581deb67b782c153136541e20901aa312ceedaf1467dcb35255787952"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d"},
+    {file = "coverage-7.5.1-cp38-cp38-win32.whl", hash = "sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41"},
+    {file = "coverage-7.5.1-cp38-cp38-win_amd64.whl", hash = "sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668"},
+    {file = "coverage-7.5.1-cp39-cp39-win32.whl", hash = "sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981"},
+    {file = "coverage-7.5.1-cp39-cp39-win_amd64.whl", hash = "sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "cssutils"
-version = "2.7.1"
-requires_python = ">=3.7"
+version = "2.10.2"
+requires_python = ">=3.8"
 summary = "A CSS Cascading Style Sheets library for Python"
+groups = ["docs"]
 files = [
-    {file = "cssutils-2.7.1-py3-none-any.whl", hash = "sha256:1e92e0d9dab2ec8af9f38d715393964ba533dc3beacab9b072511dfc241db775"},
-    {file = "cssutils-2.7.1.tar.gz", hash = "sha256:340ecfd9835d21df8f98500f0dfcea0aee41cb4e19ecbc2cf94f0a6d36d7cb6c"},
+    {file = "cssutils-2.10.2-py3-none-any.whl", hash = "sha256:4ad7d2f29270b22cf199f65a6b5e795f2c3130f3b9fb50c3d45e5054ef86e41a"},
+    {file = "cssutils-2.10.2.tar.gz", hash = "sha256:93cf92a350b1c123b17feff042e212f94d960975a3ed145743d84ebe8ccec7ab"},
 ]
 
 [[package]]
 name = "dict2css"
-version = "0.3.0"
+version = "0.3.0.post1"
 requires_python = ">=3.6"
 summary = "A μ-library for constructing cascading style sheets from Python dictionaries."
+groups = ["docs"]
 dependencies = [
     "cssutils>=2.2.0",
     "domdf-python-tools>=2.2.0",
 ]
 files = [
-    {file = "dict2css-0.3.0-py3-none-any.whl", hash = "sha256:ef934ce73a225fdd5f811b484fe9e2dd768f7ef14a89fc8f4eb5672597131d00"},
-    {file = "dict2css-0.3.0.tar.gz", hash = "sha256:1e8b1bf580dca2083198f88a60ec88c878a8829d760dfe45483ef80fe2905117"},
+    {file = "dict2css-0.3.0.post1-py3-none-any.whl", hash = "sha256:f006a6b774c3e31869015122ae82c491fd25e7de4a75607a62aa3e798f837e0d"},
+    {file = "dict2css-0.3.0.post1.tar.gz", hash = "sha256:89c544c21c4ca7472c3fffb9d37d3d926f606329afdb751dc1de67a411b70719"},
 ]
 
 [[package]]
 name = "distlib"
-version = "0.3.7"
+version = "0.3.8"
 summary = "Distribution utilities"
+groups = ["linting"]
 files = [
-    {file = "distlib-0.3.7-py2.py3-none-any.whl", hash = "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057"},
-    {file = "distlib-0.3.7.tar.gz", hash = "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"},
+    {file = "distlib-0.3.8-py2.py3-none-any.whl", hash = "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784"},
+    {file = "distlib-0.3.8.tar.gz", hash = "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"},
 ]
 
 [[package]]
 name = "docutils"
-version = "0.18.1"
-requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
+version = "0.20.1"
+requires_python = ">=3.7"
 summary = "Docutils -- Python Documentation Utilities"
+groups = ["docs"]
 files = [
-    {file = "docutils-0.18.1-py2.py3-none-any.whl", hash = "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c"},
-    {file = "docutils-0.18.1.tar.gz", hash = "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"},
+    {file = "docutils-0.20.1-py3-none-any.whl", hash = "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6"},
+    {file = "docutils-0.20.1.tar.gz", hash = "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"},
 ]
 
 [[package]]
 name = "domdf-python-tools"
-version = "3.6.1"
+version = "3.8.0.post2"
 requires_python = ">=3.6"
 summary = "Helpful functions for Python 🐍 🛠️"
+groups = ["docs"]
 dependencies = [
     "importlib-metadata>=3.6.0; python_version < \"3.9\"",
     "natsort>=7.0.1",
     "typing-extensions>=3.7.4.1",
 ]
 files = [
-    {file = "domdf_python_tools-3.6.1-py3-none-any.whl", hash = "sha256:e18158460850957f18e740eb94ede56f580ddb0cb162ab9d9834ed8bbb1b6431"},
-    {file = "domdf_python_tools-3.6.1.tar.gz", hash = "sha256:acc04563d23bce4d437dd08af6b9bea788328c412772a044d8ca428a7ad861be"},
-]
-
-[[package]]
-name = "editorconfig"
-version = "0.12.3"
-summary = "EditorConfig File Locator and Interpreter for Python"
-files = [
-    {file = "EditorConfig-0.12.3-py3-none-any.whl", hash = "sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1"},
-    {file = "EditorConfig-0.12.3.tar.gz", hash = "sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e"},
+    {file = "domdf_python_tools-3.8.0.post2-py3-none-any.whl", hash = "sha256:ad2c763c8d00850a7fa92ad95e9891a1918281ea25322c4dbb1734fd32f905dd"},
+    {file = "domdf_python_tools-3.8.0.post2.tar.gz", hash = "sha256:a1fd255ea29f767b08de462d2da39d360262304389227d980bc307ee8aa3366a"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.1.3"
+version = "1.2.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
+groups = ["default", "test"]
+marker = "python_version < \"3.11\""
 files = [
-    {file = "exceptiongroup-1.1.3-py3-none-any.whl", hash = "sha256:343280667a4585d195ca1cf9cef84a4e178c4b6cf2274caef9859782b567d5e3"},
-    {file = "exceptiongroup-1.1.3.tar.gz", hash = "sha256:097acd85d473d75af5bb98e41b61ff7fe35efe6675e4f9370ec6ec5126d160e9"},
-]
-
-[[package]]
-name = "execnet"
-version = "2.0.2"
-requires_python = ">=3.7"
-summary = "execnet: rapid multi-Python deployment"
-files = [
-    {file = "execnet-2.0.2-py3-none-any.whl", hash = "sha256:88256416ae766bc9e8895c76a87928c0012183da3cc4fc18016e6f050e025f41"},
-    {file = "execnet-2.0.2.tar.gz", hash = "sha256:cc59bc4423742fd71ad227122eb0dd44db51efb3dc4095b45ac9a08c770096af"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [[package]]
 name = "faker"
-version = "19.6.2"
+version = "25.0.1"
 requires_python = ">=3.8"
 summary = "Faker is a Python package that generates fake data for you."
+groups = ["default"]
 dependencies = [
     "python-dateutil>=2.4",
-    "typing-extensions>=3.10.0.1; python_version <= \"3.8\"",
 ]
 files = [
-    {file = "Faker-19.6.2-py3-none-any.whl", hash = "sha256:8fba91068dc26e3159c1ac9f22444a2338704b0991d86605322e454bda420092"},
-    {file = "Faker-19.6.2.tar.gz", hash = "sha256:d5d5953556b0fb428a46019e03fc2d40eab2980135ddef5a9eb3d054947fdf83"},
-]
-
-[[package]]
-name = "fast-query-parsers"
-version = "1.0.3"
-requires_python = ">=3.8"
-summary = "Ultra-fast query string and url-encoded form-data parsers"
-files = [
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-macosx_10_7_x86_64.whl", hash = "sha256:afbf71c1b4398dacfb9d84755eb026f8e759f68a066f1f3cc19e471fc342e74f"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:42f26875311d1b151c3406adfa39ec2db98df111a369d75f6fa243ec8462f147"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:66630ad423b5b1f5709f82a4d8482cd6aa2f3fa73d2c779ff1877f25dee08d55"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:a6e3d816c572a6fad1ae9b93713b2db0d3db6e8f594e035ad52361d668dd94a8"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:0bdcc0ddb4cc69d823c2c0dedd8f5affc71042db39908ad2ca06261bf388cac6"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6720505f2d2a764c76bcc4f3730a9dff69d9871740e46264f6605d73f9ce3794"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e947e7251769593da93832a10861f59565a46149fa117ebdf25377e7b2853936"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:55a30b7cee0a53cddf9016b86fdad87221980d5a02a6126c491bd309755e6de9"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:9bc2b457caa38371df1a30cfdfc57bd9bfdf348367abdaf6f36533416a0b0e93"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-musllinux_1_2_aarch64.whl", hash = "sha256:5736d3c32d6ba23995fa569fe572feabcfcfc30ac9e4709e94cff6f2c456a3d1"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-musllinux_1_2_armv7l.whl", hash = "sha256:3a6377eb0c5b172fbc77c3f96deaf1e51708b4b96d27ce173658bf11c1c00b20"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-musllinux_1_2_i686.whl", hash = "sha256:7ca6be04f443a1b055e910ccad01b1d72212f269a530415df99a87c5f1e9c927"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-musllinux_1_2_x86_64.whl", hash = "sha256:a70d4d8852606f2dd5b798ab628b9d8dc6970ddfdd9e96f4543eb0cc89a74fb5"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-win32.whl", hash = "sha256:14b3fab7e9a6ac1c1efaf66c3fd2a3fd1e25ede03ed14118035e530433830a11"},
-    {file = "fast_query_parsers-1.0.3-cp38-abi3-win_amd64.whl", hash = "sha256:21ae5f3a209aee7d3b84bdcdb33dd79f39fc8cb608b3ae8cfcb78123758c1a16"},
-    {file = "fast_query_parsers-1.0.3.tar.gz", hash = "sha256:5200a9e02997ad51d4d76a60ea1b256a68a184b04359540eb6310a15013df68f"},
+    {file = "Faker-25.0.1-py3-none-any.whl", hash = "sha256:6737cc6d591cd83421fdc5e494f6e2c1a6e32266214f158b745aa9fa15687c98"},
+    {file = "Faker-25.0.1.tar.gz", hash = "sha256:c153505618801f1704807b258a6010ea8cabf91f66f4788939bfdba83b887e76"},
 ]
 
 [[package]]
 name = "filelock"
-version = "3.12.4"
+version = "3.14.0"
 requires_python = ">=3.8"
 summary = "A platform independent file lock."
+groups = ["docs", "linting"]
 files = [
-    {file = "filelock-3.12.4-py3-none-any.whl", hash = "sha256:08c21d87ded6e2b9da6728c3dff51baf1dcecf973b768ef35bcbc3447edb9ad4"},
-    {file = "filelock-3.12.4.tar.gz", hash = "sha256:2e6f249f1f3654291606e046b09f1fd5eac39b360664c27f5aad072012f8bcbd"},
+    {file = "filelock-3.14.0-py3-none-any.whl", hash = "sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f"},
+    {file = "filelock-3.14.0.tar.gz", hash = "sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a"},
 ]
 
 [[package]]
-name = "greenlet"
-version = "2.0.2"
-requires_python = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*"
-summary = "Lightweight in-process concurrent programming"
-files = [
-    {file = "greenlet-2.0.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d967650d3f56af314b72df7089d96cda1083a7fc2da05b375d2bc48c82ab3f3c"},
-    {file = "greenlet-2.0.2-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:30bcf80dda7f15ac77ba5af2b961bdd9dbc77fd4ac6105cee85b0d0a5fcf74df"},
-    {file = "greenlet-2.0.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:26fbfce90728d82bc9e6c38ea4d038cba20b7faf8a0ca53a9c07b67318d46088"},
-    {file = "greenlet-2.0.2-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9190f09060ea4debddd24665d6804b995a9c122ef5917ab26e1566dcc712ceeb"},
-    {file = "greenlet-2.0.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d75209eed723105f9596807495d58d10b3470fa6732dd6756595e89925ce2470"},
-    {file = "greenlet-2.0.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:3a51c9751078733d88e013587b108f1b7a1fb106d402fb390740f002b6f6551a"},
-    {file = "greenlet-2.0.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:76ae285c8104046b3a7f06b42f29c7b73f77683df18c49ab5af7983994c2dd91"},
-    {file = "greenlet-2.0.2-cp310-cp310-win_amd64.whl", hash = "sha256:2d4686f195e32d36b4d7cf2d166857dbd0ee9f3d20ae349b6bf8afc8485b3645"},
-    {file = "greenlet-2.0.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:c4302695ad8027363e96311df24ee28978162cdcdd2006476c43970b384a244c"},
-    {file = "greenlet-2.0.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d4606a527e30548153be1a9f155f4e283d109ffba663a15856089fb55f933e47"},
-    {file = "greenlet-2.0.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c48f54ef8e05f04d6eff74b8233f6063cb1ed960243eacc474ee73a2ea8573ca"},
-    {file = "greenlet-2.0.2-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a1846f1b999e78e13837c93c778dcfc3365902cfb8d1bdb7dd73ead37059f0d0"},
-    {file = "greenlet-2.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a06ad5312349fec0ab944664b01d26f8d1f05009566339ac6f63f56589bc1a2"},
-    {file = "greenlet-2.0.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:eff4eb9b7eb3e4d0cae3d28c283dc16d9bed6b193c2e1ace3ed86ce48ea8df19"},
-    {file = "greenlet-2.0.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5454276c07d27a740c5892f4907c86327b632127dd9abec42ee62e12427ff7e3"},
-    {file = "greenlet-2.0.2-cp311-cp311-win_amd64.whl", hash = "sha256:7cafd1208fdbe93b67c7086876f061f660cfddc44f404279c1585bbf3cdc64c5"},
-    {file = "greenlet-2.0.2-cp38-cp38-macosx_10_15_x86_64.whl", hash = "sha256:b864ba53912b6c3ab6bcb2beb19f19edd01a6bfcbdfe1f37ddd1778abfe75a30"},
-    {file = "greenlet-2.0.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:1087300cf9700bbf455b1b97e24db18f2f77b55302a68272c56209d5587c12d1"},
-    {file = "greenlet-2.0.2-cp38-cp38-manylinux2010_x86_64.whl", hash = "sha256:ba2956617f1c42598a308a84c6cf021a90ff3862eddafd20c3333d50f0edb45b"},
-    {file = "greenlet-2.0.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fc3a569657468b6f3fb60587e48356fe512c1754ca05a564f11366ac9e306526"},
-    {file = "greenlet-2.0.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:8eab883b3b2a38cc1e050819ef06a7e6344d4a990d24d45bc6f2cf959045a45b"},
-    {file = "greenlet-2.0.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:acd2162a36d3de67ee896c43effcd5ee3de247eb00354db411feb025aa319857"},
-    {file = "greenlet-2.0.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:0bf60faf0bc2468089bdc5edd10555bab6e85152191df713e2ab1fcc86382b5a"},
-    {file = "greenlet-2.0.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b0ef99cdbe2b682b9ccbb964743a6aca37905fda5e0452e5ee239b1654d37f2a"},
-    {file = "greenlet-2.0.2-cp38-cp38-win32.whl", hash = "sha256:b80f600eddddce72320dbbc8e3784d16bd3fb7b517e82476d8da921f27d4b249"},
-    {file = "greenlet-2.0.2-cp38-cp38-win_amd64.whl", hash = "sha256:4d2e11331fc0c02b6e84b0d28ece3a36e0548ee1a1ce9ddde03752d9b79bba40"},
-    {file = "greenlet-2.0.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:8512a0c38cfd4e66a858ddd1b17705587900dd760c6003998e9472b77b56d417"},
-    {file = "greenlet-2.0.2-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:88d9ab96491d38a5ab7c56dd7a3cc37d83336ecc564e4e8816dbed12e5aaefc8"},
-    {file = "greenlet-2.0.2-cp39-cp39-manylinux2010_x86_64.whl", hash = "sha256:561091a7be172ab497a3527602d467e2b3fbe75f9e783d8b8ce403fa414f71a6"},
-    {file = "greenlet-2.0.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:971ce5e14dc5e73715755d0ca2975ac88cfdaefcaab078a284fea6cfabf866df"},
-    {file = "greenlet-2.0.2-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:be4ed120b52ae4d974aa40215fcdfde9194d63541c7ded40ee12eb4dda57b76b"},
-    {file = "greenlet-2.0.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:94c817e84245513926588caf1152e3b559ff794d505555211ca041f032abbb6b"},
-    {file = "greenlet-2.0.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:1a819eef4b0e0b96bb0d98d797bef17dc1b4a10e8d7446be32d1da33e095dbb8"},
-    {file = "greenlet-2.0.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:7efde645ca1cc441d6dc4b48c0f7101e8d86b54c8530141b09fd31cef5149ec9"},
-    {file = "greenlet-2.0.2-cp39-cp39-win32.whl", hash = "sha256:ea9872c80c132f4663822dd2a08d404073a5a9b5ba6155bea72fb2a79d1093b5"},
-    {file = "greenlet-2.0.2-cp39-cp39-win_amd64.whl", hash = "sha256:db1a39669102a1d8d12b57de2bb7e2ec9066a6f2b3da35ae511ff93b01b5d564"},
-    {file = "greenlet-2.0.2.tar.gz", hash = "sha256:e7c8dc13af7db097bed64a051d2dd49e9f0af495c26995c00a9ee842690d34c0"},
+name = "git-cliff"
+version = "2.2.1"
+requires_python = ">=3.7"
+summary = "A highly customizable changelog generator ⛰️"
+groups = ["docs"]
+files = [
+    {file = "git_cliff-2.2.1-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:f7c6550733a60e135f821ac999ee6804f185089ae6b7bb4f91dad32a8d95a2d5"},
+    {file = "git_cliff-2.2.1-py3-none-macosx_11_0_arm64.whl", hash = "sha256:e624814e9273f8a4000fb7425842a7c062631234a84092a9d551f24520c956db"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:548c994d902e74e2e104e4603ac29419020d3d54eaf5ce3b8e17e77493448faf"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:739447e3c22c7aa964f0900b4f63234a5ff8246988797a70f3245fc37cebf1b5"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_28_aarch64.whl", hash = "sha256:aea2aa2250b5fff738294e7eee1c458ba4dadc81fc823d31f29eb1c689ee09d0"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:0645822f4ff4aaf68e7fa61fd31a583ccef9793a71b0a34c50c9fac43d90a254"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:01a02869e3b186f173d1f14db11f7c7130394195fc6e352ac0e3cd505d65104f"},
+    {file = "git_cliff-2.2.1-py3-none-win32.whl", hash = "sha256:e98bf87ee7b22eacdba0e74016f93b6d6d1fea6cb2cf67742c3aaa1614fafef9"},
+    {file = "git_cliff-2.2.1-py3-none-win_amd64.whl", hash = "sha256:e57155dbb3a895c09ed358137d0d1d30d3f15971456f3c48ede9bfd37434ce75"},
+    {file = "git_cliff-2.2.1.tar.gz", hash = "sha256:6db64534dc5ec3d7656b9be6ddf7004cfd1ddf8f815f66d41bc9330f42b61d6d"},
 ]
 
 [[package]]
 name = "h11"
 version = "0.14.0"
 requires_python = ">=3.7"
 summary = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
+groups = ["default"]
 files = [
     {file = "h11-0.14.0-py3-none-any.whl", hash = "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"},
     {file = "h11-0.14.0.tar.gz", hash = "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d"},
 ]
 
 [[package]]
 name = "html5lib"
 version = "1.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "HTML parser based on the WHATWG HTML specification"
+groups = ["docs"]
 dependencies = [
     "six>=1.9",
     "webencodings",
 ]
 files = [
     {file = "html5lib-1.1-py2.py3-none-any.whl", hash = "sha256:0d78f8fde1c230e99fe37986a60526d7049ed4bf8a9fadbad5f00e22e58e041d"},
     {file = "html5lib-1.1.tar.gz", hash = "sha256:b2e5b40261e20f354d198eae92afc10d750afb487ed5e50f9c4eaf07c184146f"},
 ]
 
 [[package]]
 name = "httpcore"
-version = "0.18.0"
+version = "1.0.5"
 requires_python = ">=3.8"
 summary = "A minimal low-level HTTP client."
+groups = ["default"]
 dependencies = [
-    "anyio<5.0,>=3.0",
     "certifi",
     "h11<0.15,>=0.13",
-    "sniffio==1.*",
 ]
 files = [
-    {file = "httpcore-0.18.0-py3-none-any.whl", hash = "sha256:adc5398ee0a476567bf87467063ee63584a8bce86078bf748e48754f60202ced"},
-    {file = "httpcore-0.18.0.tar.gz", hash = "sha256:13b5e5cd1dca1a6636a6aaea212b19f4f85cd88c366a2b82304181b769aab3c9"},
-]
-
-[[package]]
-name = "httptools"
-version = "0.6.0"
-requires_python = ">=3.5.0"
-summary = "A collection of framework independent HTTP protocol utils."
-files = [
-    {file = "httptools-0.6.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:818325afee467d483bfab1647a72054246d29f9053fd17cc4b86cda09cc60339"},
-    {file = "httptools-0.6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:72205730bf1be875003692ca54a4a7c35fac77b4746008966061d9d41a61b0f5"},
-    {file = "httptools-0.6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:33eb1d4e609c835966e969a31b1dedf5ba16b38cab356c2ce4f3e33ffa94cad3"},
-    {file = "httptools-0.6.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6bdc6675ec6cb79d27e0575750ac6e2b47032742e24eed011b8db73f2da9ed40"},
-    {file = "httptools-0.6.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:463c3bc5ef64b9cf091be9ac0e0556199503f6e80456b790a917774a616aff6e"},
-    {file = "httptools-0.6.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:82f228b88b0e8c6099a9c4757ce9fdbb8b45548074f8d0b1f0fc071e35655d1c"},
-    {file = "httptools-0.6.0-cp310-cp310-win_amd64.whl", hash = "sha256:0781fedc610293a2716bc7fa142d4c85e6776bc59d617a807ff91246a95dea35"},
-    {file = "httptools-0.6.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:721e503245d591527cddd0f6fd771d156c509e831caa7a57929b55ac91ee2b51"},
-    {file = "httptools-0.6.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:274bf20eeb41b0956e34f6a81f84d26ed57c84dd9253f13dcb7174b27ccd8aaf"},
-    {file = "httptools-0.6.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:259920bbae18740a40236807915def554132ad70af5067e562f4660b62c59b90"},
-    {file = "httptools-0.6.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:03bfd2ae8a2d532952ac54445a2fb2504c804135ed28b53fefaf03d3a93eb1fd"},
-    {file = "httptools-0.6.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f959e4770b3fc8ee4dbc3578fd910fab9003e093f20ac8c621452c4d62e517cb"},
-    {file = "httptools-0.6.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6e22896b42b95b3237eccc42278cd72c0df6f23247d886b7ded3163452481e38"},
-    {file = "httptools-0.6.0-cp311-cp311-win_amd64.whl", hash = "sha256:38f3cafedd6aa20ae05f81f2e616ea6f92116c8a0f8dcb79dc798df3356836e2"},
-    {file = "httptools-0.6.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:cf8169e839a0d740f3d3c9c4fa630ac1a5aaf81641a34575ca6773ed7ce041a1"},
-    {file = "httptools-0.6.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:5dcc14c090ab57b35908d4a4585ec5c0715439df07be2913405991dbb37e049d"},
-    {file = "httptools-0.6.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d0b0571806a5168013b8c3d180d9f9d6997365a4212cb18ea20df18b938aa0b"},
-    {file = "httptools-0.6.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0fb4a608c631f7dcbdf986f40af7a030521a10ba6bc3d36b28c1dc9e9035a3c0"},
-    {file = "httptools-0.6.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:93f89975465133619aea8b1952bc6fa0e6bad22a447c6d982fc338fbb4c89649"},
-    {file = "httptools-0.6.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:73e9d66a5a28b2d5d9fbd9e197a31edd02be310186db423b28e6052472dc8201"},
-    {file = "httptools-0.6.0-cp38-cp38-win_amd64.whl", hash = "sha256:22c01fcd53648162730a71c42842f73b50f989daae36534c818b3f5050b54589"},
-    {file = "httptools-0.6.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:3f96d2a351b5625a9fd9133c95744e8ca06f7a4f8f0b8231e4bbaae2c485046a"},
-    {file = "httptools-0.6.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:72ec7c70bd9f95ef1083d14a755f321d181f046ca685b6358676737a5fecd26a"},
-    {file = "httptools-0.6.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b703d15dbe082cc23266bf5d9448e764c7cb3fcfe7cb358d79d3fd8248673ef9"},
-    {file = "httptools-0.6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:82c723ed5982f8ead00f8e7605c53e55ffe47c47465d878305ebe0082b6a1755"},
-    {file = "httptools-0.6.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b0a816bb425c116a160fbc6f34cece097fd22ece15059d68932af686520966bd"},
-    {file = "httptools-0.6.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:dea66d94e5a3f68c5e9d86e0894653b87d952e624845e0b0e3ad1c733c6cc75d"},
-    {file = "httptools-0.6.0-cp39-cp39-win_amd64.whl", hash = "sha256:23b09537086a5a611fad5696fc8963d67c7e7f98cb329d38ee114d588b0b74cd"},
-    {file = "httptools-0.6.0.tar.gz", hash = "sha256:9fc6e409ad38cbd68b177cd5158fc4042c796b82ca88d99ec78f07bed6c6b796"},
+    {file = "httpcore-1.0.5-py3-none-any.whl", hash = "sha256:421f18bac248b25d310f3cacd198d55b8e6125c107797b609ff9b7a6ba7991b5"},
+    {file = "httpcore-1.0.5.tar.gz", hash = "sha256:34a38e2f9291467ee3b44e89dd52615370e152954ba21721378a87b2960f7a61"},
 ]
 
 [[package]]
 name = "httpx"
-version = "0.25.0"
+version = "0.27.0"
 requires_python = ">=3.8"
 summary = "The next generation HTTP client."
+groups = ["default"]
 dependencies = [
+    "anyio",
     "certifi",
-    "httpcore<0.19.0,>=0.18.0",
+    "httpcore==1.*",
     "idna",
     "sniffio",
 ]
 files = [
-    {file = "httpx-0.25.0-py3-none-any.whl", hash = "sha256:181ea7f8ba3a82578be86ef4171554dd45fec26a02556a744db029a0a27b7100"},
-    {file = "httpx-0.25.0.tar.gz", hash = "sha256:47ecda285389cb32bb2691cc6e069e3ab0205956f681c5b2ad2325719751d875"},
+    {file = "httpx-0.27.0-py3-none-any.whl", hash = "sha256:71d5465162c13681bff01ad59b2cc68dd838ea1f10e51574bac27103f00c91a5"},
+    {file = "httpx-0.27.0.tar.gz", hash = "sha256:a0cb88a46f32dc874e04ee956e4c2764aba2aa228f650b06788ba6bda2962ab5"},
 ]
 
 [[package]]
 name = "identify"
-version = "2.5.30"
+version = "2.5.36"
 requires_python = ">=3.8"
 summary = "File identification library for Python"
+groups = ["linting"]
 files = [
-    {file = "identify-2.5.30-py2.py3-none-any.whl", hash = "sha256:afe67f26ae29bab007ec21b03d4114f41316ab9dd15aa8736a167481e108da54"},
-    {file = "identify-2.5.30.tar.gz", hash = "sha256:f302a4256a15c849b91cfcdcec052a8ce914634b2f77ae87dad29cd749f2d88d"},
+    {file = "identify-2.5.36-py2.py3-none-any.whl", hash = "sha256:37d93f380f4de590500d9dba7db359d0d3da95ffe7f9de1753faa159e71e7dfa"},
+    {file = "identify-2.5.36.tar.gz", hash = "sha256:e5e00f54165f9047fbebeb4a560f9acfb8af4c88232be60a488e9b68d122745d"},
 ]
 
 [[package]]
 name = "idna"
-version = "3.4"
+version = "3.7"
 requires_python = ">=3.5"
 summary = "Internationalized Domain Names in Applications (IDNA)"
+groups = ["default", "docs", "test"]
 files = [
-    {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
-    {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
+    {file = "idna-3.7-py3-none-any.whl", hash = "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"},
+    {file = "idna-3.7.tar.gz", hash = "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Getting image size from png/jpeg/jpeg2000/gif file"
+groups = ["docs"]
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.8.0"
+version = "7.1.0"
 requires_python = ">=3.8"
 summary = "Read metadata from Python packages"
+groups = ["default", "docs"]
+marker = "python_version < \"3.10\""
 dependencies = [
     "zipp>=0.5",
 ]
 files = [
-    {file = "importlib_metadata-6.8.0-py3-none-any.whl", hash = "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb"},
-    {file = "importlib_metadata-6.8.0.tar.gz", hash = "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"},
+    {file = "importlib_metadata-7.1.0-py3-none-any.whl", hash = "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570"},
+    {file = "importlib_metadata-7.1.0.tar.gz", hash = "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"},
 ]
 
 [[package]]
 name = "importlib-resources"
-version = "6.1.0"
+version = "6.4.0"
 requires_python = ">=3.8"
 summary = "Read resources from Python packages"
+groups = ["default"]
+marker = "python_version < \"3.9\""
 dependencies = [
     "zipp>=3.1.0; python_version < \"3.10\"",
 ]
 files = [
-    {file = "importlib_resources-6.1.0-py3-none-any.whl", hash = "sha256:aa50258bbfa56d4e33fbd8aa3ef48ded10d1735f11532b8df95388cc6bdb7e83"},
-    {file = "importlib_resources-6.1.0.tar.gz", hash = "sha256:9d48dcccc213325e810fd723e7fbb45ccb39f6cf5c31f00cf2b965f5f10f3cb9"},
+    {file = "importlib_resources-6.4.0-py3-none-any.whl", hash = "sha256:50d10f043df931902d4194ea07ec57960f66a80449ff867bfe782b4c486ba78c"},
+    {file = "importlib_resources-6.4.0.tar.gz", hash = "sha256:cdb2b453b8046ca4e3798eb1d84f3cce1446a0e8e7b5ef4efb600f19fc398145"},
 ]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
+groups = ["test"]
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "jinja2"
-version = "3.1.2"
+version = "3.1.4"
 requires_python = ">=3.7"
 summary = "A very fast and expressive template engine."
+groups = ["docs"]
 dependencies = [
     "MarkupSafe>=2.0",
 ]
 files = [
-    {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
-    {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
-]
-
-[[package]]
-name = "jsbeautifier"
-version = "1.14.9"
-summary = "JavaScript unobfuscator and beautifier."
-dependencies = [
-    "editorconfig>=0.12.2",
-    "six>=1.13.0",
-]
-files = [
-    {file = "jsbeautifier-1.14.9.tar.gz", hash = "sha256:c738ebc36b47bd94e4ca6dd17a9004c3cc74edad582ca1d60e0e5d5945a63cb9"},
+    {file = "jinja2-3.1.4-py3-none-any.whl", hash = "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"},
+    {file = "jinja2-3.1.4.tar.gz", hash = "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369"},
 ]
 
 [[package]]
 name = "litestar"
-version = "2.1.1"
-requires_python = ">=3.8,<4.0"
+version = "2.8.2"
+requires_python = "<4.0,>=3.8"
 summary = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
+groups = ["default"]
 dependencies = [
-    "alembic",
     "anyio>=3",
-    "fast-query-parsers>=1.0.2",
+    "click",
+    "exceptiongroup; python_version < \"3.11\"",
     "httpx>=0.22",
     "importlib-metadata; python_version < \"3.10\"",
     "importlib-resources>=5.12.0; python_version < \"3.9\"",
     "msgspec>=0.18.2",
     "multidict>=6.0.2",
     "polyfactory>=2.6.3",
     "pyyaml",
-    "sqlalchemy>=2.0.12",
+    "rich-click",
+    "rich>=13.0.0",
     "typing-extensions",
 ]
 files = [
-    {file = "litestar-2.1.1-py3-none-any.whl", hash = "sha256:b8575a868d0dbe021b665a6c66d9e1feb65fcb94c8a386dad2b2895ce8f30896"},
-    {file = "litestar-2.1.1.tar.gz", hash = "sha256:33a4134807e9ffb70b856fe1565066c050ebc00df0cb768fc59efa41e8f8b3de"},
+    {file = "litestar-2.8.2-py3-none-any.whl", hash = "sha256:c891baf8a17d66cfed5c40bef7b5bf4c02c2831babf5fca0af404f441610557a"},
+    {file = "litestar-2.8.2.tar.gz", hash = "sha256:18353cb7246ba2e7f8d4aac4fe2d8772b503c931cf5ee16efc759cbbc3a2344b"},
 ]
 
 [[package]]
-name = "litestar"
-version = "2.1.1"
-extras = ["cli"]
+name = "litestar-sphinx-theme"
+version = "0.3.1"
 requires_python = ">=3.8,<4.0"
-summary = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
-dependencies = [
-    "click",
-    "jsbeautifier",
-    "litestar==2.1.1",
-    "rich-click",
-    "rich>=13.0.0",
-    "uvicorn[standard]>=0.22.0",
-]
-files = [
-    {file = "litestar-2.1.1-py3-none-any.whl", hash = "sha256:b8575a868d0dbe021b665a6c66d9e1feb65fcb94c8a386dad2b2895ce8f30896"},
-    {file = "litestar-2.1.1.tar.gz", hash = "sha256:33a4134807e9ffb70b856fe1565066c050ebc00df0cb768fc59efa41e8f8b3de"},
+git = "https://github.com/litestar-org/litestar-sphinx-theme.git"
+ref = "v3"
+revision = "4799f935c3023afb222058cba8c849e8fa9ae3ba"
+summary = "A Sphinx theme for the Litestar organization"
+groups = ["docs"]
+dependencies = [
+    "blacken-docs>=1.16.0",
+    "shibuya>=2024.4.4",
+    "sphinx-autobuild>=2021.3.14",
+    "sphinx-copybutton>=0.5.2",
+    "sphinx-design<1.0.0,>=0.3.0",
+    "sphinx-togglebutton",
+    "sphinx-toolbox>=3.5.0",
 ]
 
 [[package]]
 name = "livereload"
 version = "2.6.3"
 summary = "Python LiveReload is an awesome tool for web developers"
+groups = ["docs"]
 dependencies = [
     "six",
     "tornado; python_version > \"2.7\"",
 ]
 files = [
     {file = "livereload-2.6.3-py2.py3-none-any.whl", hash = "sha256:ad4ac6f53b2d62bb6ce1a5e6e96f1f00976a32348afedcb4b6d68df2a1d346e4"},
     {file = "livereload-2.6.3.tar.gz", hash = "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869"},
 ]
 
 [[package]]
-name = "mako"
-version = "1.2.4"
-requires_python = ">=3.7"
-summary = "A super-fast templating language that borrows the best ideas from the existing templating languages."
-dependencies = [
-    "MarkupSafe>=0.9.2",
-]
-files = [
-    {file = "Mako-1.2.4-py3-none-any.whl", hash = "sha256:c97c79c018b9165ac9922ae4f32da095ffd3c4e6872b45eded42926deea46818"},
-    {file = "Mako-1.2.4.tar.gz", hash = "sha256:d60a3903dc3bb01a18ad6a89cdbe2e4eadc69c0bc8ef1e3773ba53d44c3f7a34"},
-]
-
-[[package]]
 name = "markdown-it-py"
 version = "3.0.0"
 requires_python = ">=3.8"
 summary = "Python port of markdown-it. Markdown parsing, done right!"
+groups = ["default"]
 dependencies = [
     "mdurl~=0.1",
 ]
 files = [
     {file = "markdown-it-py-3.0.0.tar.gz", hash = "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"},
     {file = "markdown_it_py-3.0.0-py3-none-any.whl", hash = "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1"},
 ]
 
 [[package]]
 name = "markupsafe"
-version = "2.1.3"
+version = "2.1.5"
 requires_python = ">=3.7"
 summary = "Safely add untrusted strings to HTML/XML markup."
+groups = ["docs"]
 files = [
-    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-win32.whl", hash = "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431"},
-    {file = "MarkupSafe-2.1.3-cp310-cp310-win_amd64.whl", hash = "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
-    {file = "MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-win32.whl", hash = "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007"},
-    {file = "MarkupSafe-2.1.3-cp312-cp312-win_amd64.whl", hash = "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
-    {file = "MarkupSafe-2.1.3-cp38-cp38-win_amd64.whl", hash = "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-win32.whl", hash = "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"},
-    {file = "MarkupSafe-2.1.3-cp39-cp39-win_amd64.whl", hash = "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba"},
-    {file = "MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-win32.whl", hash = "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4"},
+    {file = "MarkupSafe-2.1.5-cp310-cp310-win_amd64.whl", hash = "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-win32.whl", hash = "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906"},
+    {file = "MarkupSafe-2.1.5-cp311-cp311-win_amd64.whl", hash = "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-win32.whl", hash = "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad"},
+    {file = "MarkupSafe-2.1.5-cp312-cp312-win_amd64.whl", hash = "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-win32.whl", hash = "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff"},
+    {file = "MarkupSafe-2.1.5-cp38-cp38-win_amd64.whl", hash = "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-win32.whl", hash = "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf"},
+    {file = "MarkupSafe-2.1.5-cp39-cp39-win_amd64.whl", hash = "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5"},
+    {file = "MarkupSafe-2.1.5.tar.gz", hash = "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b"},
 ]
 
 [[package]]
 name = "mdurl"
 version = "0.1.2"
 requires_python = ">=3.7"
 summary = "Markdown URL utilities"
+groups = ["default"]
 files = [
     {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
     {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
 ]
 
 [[package]]
 name = "msgpack"
-version = "1.0.7"
+version = "1.0.8"
 requires_python = ">=3.8"
 summary = "MessagePack serializer"
+groups = ["docs"]
 files = [
-    {file = "msgpack-1.0.7-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:04ad6069c86e531682f9e1e71b71c1c3937d6014a7c3e9edd2aa81ad58842862"},
-    {file = "msgpack-1.0.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:cca1b62fe70d761a282496b96a5e51c44c213e410a964bdffe0928e611368329"},
-    {file = "msgpack-1.0.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e50ebce52f41370707f1e21a59514e3375e3edd6e1832f5e5235237db933c98b"},
-    {file = "msgpack-1.0.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b4f35de6a304b5533c238bee86b670b75b03d31b7797929caa7a624b5dda6"},
-    {file = "msgpack-1.0.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28efb066cde83c479dfe5a48141a53bc7e5f13f785b92ddde336c716663039ee"},
-    {file = "msgpack-1.0.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4cb14ce54d9b857be9591ac364cb08dc2d6a5c4318c1182cb1d02274029d590d"},
-    {file = "msgpack-1.0.7-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:b573a43ef7c368ba4ea06050a957c2a7550f729c31f11dd616d2ac4aba99888d"},
-    {file = "msgpack-1.0.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:ccf9a39706b604d884d2cb1e27fe973bc55f2890c52f38df742bc1d79ab9f5e1"},
-    {file = "msgpack-1.0.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:cb70766519500281815dfd7a87d3a178acf7ce95390544b8c90587d76b227681"},
-    {file = "msgpack-1.0.7-cp310-cp310-win32.whl", hash = "sha256:b610ff0f24e9f11c9ae653c67ff8cc03c075131401b3e5ef4b82570d1728f8a9"},
-    {file = "msgpack-1.0.7-cp310-cp310-win_amd64.whl", hash = "sha256:a40821a89dc373d6427e2b44b572efc36a2778d3f543299e2f24eb1a5de65415"},
-    {file = "msgpack-1.0.7-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:576eb384292b139821c41995523654ad82d1916da6a60cff129c715a6223ea84"},
-    {file = "msgpack-1.0.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:730076207cb816138cf1af7f7237b208340a2c5e749707457d70705715c93b93"},
-    {file = "msgpack-1.0.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:85765fdf4b27eb5086f05ac0491090fc76f4f2b28e09d9350c31aac25a5aaff8"},
-    {file = "msgpack-1.0.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3476fae43db72bd11f29a5147ae2f3cb22e2f1a91d575ef130d2bf49afd21c46"},
-    {file = "msgpack-1.0.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6d4c80667de2e36970ebf74f42d1088cc9ee7ef5f4e8c35eee1b40eafd33ca5b"},
-    {file = "msgpack-1.0.7-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5b0bf0effb196ed76b7ad883848143427a73c355ae8e569fa538365064188b8e"},
-    {file = "msgpack-1.0.7-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:f9a7c509542db4eceed3dcf21ee5267ab565a83555c9b88a8109dcecc4709002"},
-    {file = "msgpack-1.0.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:84b0daf226913133f899ea9b30618722d45feffa67e4fe867b0b5ae83a34060c"},
-    {file = "msgpack-1.0.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ec79ff6159dffcc30853b2ad612ed572af86c92b5168aa3fc01a67b0fa40665e"},
-    {file = "msgpack-1.0.7-cp311-cp311-win32.whl", hash = "sha256:3e7bf4442b310ff154b7bb9d81eb2c016b7d597e364f97d72b1acc3817a0fdc1"},
-    {file = "msgpack-1.0.7-cp311-cp311-win_amd64.whl", hash = "sha256:3f0c8c6dfa6605ab8ff0611995ee30d4f9fcff89966cf562733b4008a3d60d82"},
-    {file = "msgpack-1.0.7-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:f0936e08e0003f66bfd97e74ee530427707297b0d0361247e9b4f59ab78ddc8b"},
-    {file = "msgpack-1.0.7-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:98bbd754a422a0b123c66a4c341de0474cad4a5c10c164ceed6ea090f3563db4"},
-    {file = "msgpack-1.0.7-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b291f0ee7961a597cbbcc77709374087fa2a9afe7bdb6a40dbbd9b127e79afee"},
-    {file = "msgpack-1.0.7-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ebbbba226f0a108a7366bf4b59bf0f30a12fd5e75100c630267d94d7f0ad20e5"},
-    {file = "msgpack-1.0.7-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1e2d69948e4132813b8d1131f29f9101bc2c915f26089a6d632001a5c1349672"},
-    {file = "msgpack-1.0.7-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bdf38ba2d393c7911ae989c3bbba510ebbcdf4ecbdbfec36272abe350c454075"},
-    {file = "msgpack-1.0.7-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:993584fc821c58d5993521bfdcd31a4adf025c7d745bbd4d12ccfecf695af5ba"},
-    {file = "msgpack-1.0.7-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:52700dc63a4676669b341ba33520f4d6e43d3ca58d422e22ba66d1736b0a6e4c"},
-    {file = "msgpack-1.0.7-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:e45ae4927759289c30ccba8d9fdce62bb414977ba158286b5ddaf8df2cddb5c5"},
-    {file = "msgpack-1.0.7-cp312-cp312-win32.whl", hash = "sha256:27dcd6f46a21c18fa5e5deed92a43d4554e3df8d8ca5a47bf0615d6a5f39dbc9"},
-    {file = "msgpack-1.0.7-cp312-cp312-win_amd64.whl", hash = "sha256:7687e22a31e976a0e7fc99c2f4d11ca45eff652a81eb8c8085e9609298916dcf"},
-    {file = "msgpack-1.0.7-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:5b6ccc0c85916998d788b295765ea0e9cb9aac7e4a8ed71d12e7d8ac31c23c95"},
-    {file = "msgpack-1.0.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:235a31ec7db685f5c82233bddf9858748b89b8119bf4538d514536c485c15fe0"},
-    {file = "msgpack-1.0.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cab3db8bab4b7e635c1c97270d7a4b2a90c070b33cbc00c99ef3f9be03d3e1f7"},
-    {file = "msgpack-1.0.7-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0bfdd914e55e0d2c9e1526de210f6fe8ffe9705f2b1dfcc4aecc92a4cb4b533d"},
-    {file = "msgpack-1.0.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:36e17c4592231a7dbd2ed09027823ab295d2791b3b1efb2aee874b10548b7524"},
-    {file = "msgpack-1.0.7-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:38949d30b11ae5f95c3c91917ee7a6b239f5ec276f271f28638dec9156f82cfc"},
-    {file = "msgpack-1.0.7-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ff1d0899f104f3921d94579a5638847f783c9b04f2d5f229392ca77fba5b82fc"},
-    {file = "msgpack-1.0.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:dc43f1ec66eb8440567186ae2f8c447d91e0372d793dfe8c222aec857b81a8cf"},
-    {file = "msgpack-1.0.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:dd632777ff3beaaf629f1ab4396caf7ba0bdd075d948a69460d13d44357aca4c"},
-    {file = "msgpack-1.0.7-cp38-cp38-win32.whl", hash = "sha256:4e71bc4416de195d6e9b4ee93ad3f2f6b2ce11d042b4d7a7ee00bbe0358bd0c2"},
-    {file = "msgpack-1.0.7-cp38-cp38-win_amd64.whl", hash = "sha256:8f5b234f567cf76ee489502ceb7165c2a5cecec081db2b37e35332b537f8157c"},
-    {file = "msgpack-1.0.7-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:bfef2bb6ef068827bbd021017a107194956918ab43ce4d6dc945ffa13efbc25f"},
-    {file = "msgpack-1.0.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:484ae3240666ad34cfa31eea7b8c6cd2f1fdaae21d73ce2974211df099a95d81"},
-    {file = "msgpack-1.0.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3967e4ad1aa9da62fd53e346ed17d7b2e922cba5ab93bdd46febcac39be636fc"},
-    {file = "msgpack-1.0.7-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8dd178c4c80706546702c59529ffc005681bd6dc2ea234c450661b205445a34d"},
-    {file = "msgpack-1.0.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f6ffbc252eb0d229aeb2f9ad051200668fc3a9aaa8994e49f0cb2ffe2b7867e7"},
-    {file = "msgpack-1.0.7-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:822ea70dc4018c7e6223f13affd1c5c30c0f5c12ac1f96cd8e9949acddb48a61"},
-    {file = "msgpack-1.0.7-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:384d779f0d6f1b110eae74cb0659d9aa6ff35aaf547b3955abf2ab4c901c4819"},
-    {file = "msgpack-1.0.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:f64e376cd20d3f030190e8c32e1c64582eba56ac6dc7d5b0b49a9d44021b52fd"},
-    {file = "msgpack-1.0.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5ed82f5a7af3697b1c4786053736f24a0efd0a1b8a130d4c7bfee4b9ded0f08f"},
-    {file = "msgpack-1.0.7-cp39-cp39-win32.whl", hash = "sha256:f26a07a6e877c76a88e3cecac8531908d980d3d5067ff69213653649ec0f60ad"},
-    {file = "msgpack-1.0.7-cp39-cp39-win_amd64.whl", hash = "sha256:1dc93e8e4653bdb5910aed79f11e165c85732067614f180f70534f056da97db3"},
-    {file = "msgpack-1.0.7.tar.gz", hash = "sha256:572efc93db7a4d27e404501975ca6d2d9775705c2d922390d878fcf768d92c87"},
+    {file = "msgpack-1.0.8-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:505fe3d03856ac7d215dbe005414bc28505d26f0c128906037e66d98c4e95868"},
+    {file = "msgpack-1.0.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e6b7842518a63a9f17107eb176320960ec095a8ee3b4420b5f688e24bf50c53c"},
+    {file = "msgpack-1.0.8-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:376081f471a2ef24828b83a641a02c575d6103a3ad7fd7dade5486cad10ea659"},
+    {file = "msgpack-1.0.8-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e390971d082dba073c05dbd56322427d3280b7cc8b53484c9377adfbae67dc2"},
+    {file = "msgpack-1.0.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:00e073efcba9ea99db5acef3959efa45b52bc67b61b00823d2a1a6944bf45982"},
+    {file = "msgpack-1.0.8-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:82d92c773fbc6942a7a8b520d22c11cfc8fd83bba86116bfcf962c2f5c2ecdaa"},
+    {file = "msgpack-1.0.8-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:9ee32dcb8e531adae1f1ca568822e9b3a738369b3b686d1477cbc643c4a9c128"},
+    {file = "msgpack-1.0.8-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:e3aa7e51d738e0ec0afbed661261513b38b3014754c9459508399baf14ae0c9d"},
+    {file = "msgpack-1.0.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:69284049d07fce531c17404fcba2bb1df472bc2dcdac642ae71a2d079d950653"},
+    {file = "msgpack-1.0.8-cp310-cp310-win32.whl", hash = "sha256:13577ec9e247f8741c84d06b9ece5f654920d8365a4b636ce0e44f15e07ec693"},
+    {file = "msgpack-1.0.8-cp310-cp310-win_amd64.whl", hash = "sha256:e532dbd6ddfe13946de050d7474e3f5fb6ec774fbb1a188aaf469b08cf04189a"},
+    {file = "msgpack-1.0.8-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:9517004e21664f2b5a5fd6333b0731b9cf0817403a941b393d89a2f1dc2bd836"},
+    {file = "msgpack-1.0.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d16a786905034e7e34098634b184a7d81f91d4c3d246edc6bd7aefb2fd8ea6ad"},
+    {file = "msgpack-1.0.8-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e2872993e209f7ed04d963e4b4fbae72d034844ec66bc4ca403329db2074377b"},
+    {file = "msgpack-1.0.8-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c330eace3dd100bdb54b5653b966de7f51c26ec4a7d4e87132d9b4f738220ba"},
+    {file = "msgpack-1.0.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83b5c044f3eff2a6534768ccfd50425939e7a8b5cf9a7261c385de1e20dcfc85"},
+    {file = "msgpack-1.0.8-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1876b0b653a808fcd50123b953af170c535027bf1d053b59790eebb0aeb38950"},
+    {file = "msgpack-1.0.8-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:dfe1f0f0ed5785c187144c46a292b8c34c1295c01da12e10ccddfc16def4448a"},
+    {file = "msgpack-1.0.8-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:3528807cbbb7f315bb81959d5961855e7ba52aa60a3097151cb21956fbc7502b"},
+    {file = "msgpack-1.0.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e2f879ab92ce502a1e65fce390eab619774dda6a6ff719718069ac94084098ce"},
+    {file = "msgpack-1.0.8-cp311-cp311-win32.whl", hash = "sha256:26ee97a8261e6e35885c2ecd2fd4a6d38252246f94a2aec23665a4e66d066305"},
+    {file = "msgpack-1.0.8-cp311-cp311-win_amd64.whl", hash = "sha256:eadb9f826c138e6cf3c49d6f8de88225a3c0ab181a9b4ba792e006e5292d150e"},
+    {file = "msgpack-1.0.8-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:114be227f5213ef8b215c22dde19532f5da9652e56e8ce969bf0a26d7c419fee"},
+    {file = "msgpack-1.0.8-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d661dc4785affa9d0edfdd1e59ec056a58b3dbb9f196fa43587f3ddac654ac7b"},
+    {file = "msgpack-1.0.8-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:d56fd9f1f1cdc8227d7b7918f55091349741904d9520c65f0139a9755952c9e8"},
+    {file = "msgpack-1.0.8-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0726c282d188e204281ebd8de31724b7d749adebc086873a59efb8cf7ae27df3"},
+    {file = "msgpack-1.0.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8db8e423192303ed77cff4dce3a4b88dbfaf43979d280181558af5e2c3c71afc"},
+    {file = "msgpack-1.0.8-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:99881222f4a8c2f641f25703963a5cefb076adffd959e0558dc9f803a52d6a58"},
+    {file = "msgpack-1.0.8-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:b5505774ea2a73a86ea176e8a9a4a7c8bf5d521050f0f6f8426afe798689243f"},
+    {file = "msgpack-1.0.8-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:ef254a06bcea461e65ff0373d8a0dd1ed3aa004af48839f002a0c994a6f72d04"},
+    {file = "msgpack-1.0.8-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:e1dd7839443592d00e96db831eddb4111a2a81a46b028f0facd60a09ebbdd543"},
+    {file = "msgpack-1.0.8-cp312-cp312-win32.whl", hash = "sha256:64d0fcd436c5683fdd7c907eeae5e2cbb5eb872fafbc03a43609d7941840995c"},
+    {file = "msgpack-1.0.8-cp312-cp312-win_amd64.whl", hash = "sha256:74398a4cf19de42e1498368c36eed45d9528f5fd0155241e82c4082b7e16cffd"},
+    {file = "msgpack-1.0.8-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:0ceea77719d45c839fd73abcb190b8390412a890df2f83fb8cf49b2a4b5c2f40"},
+    {file = "msgpack-1.0.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1ab0bbcd4d1f7b6991ee7c753655b481c50084294218de69365f8f1970d4c151"},
+    {file = "msgpack-1.0.8-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:1cce488457370ffd1f953846f82323cb6b2ad2190987cd4d70b2713e17268d24"},
+    {file = "msgpack-1.0.8-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3923a1778f7e5ef31865893fdca12a8d7dc03a44b33e2a5f3295416314c09f5d"},
+    {file = "msgpack-1.0.8-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a22e47578b30a3e199ab067a4d43d790249b3c0587d9a771921f86250c8435db"},
+    {file = "msgpack-1.0.8-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bd739c9251d01e0279ce729e37b39d49a08c0420d3fee7f2a4968c0576678f77"},
+    {file = "msgpack-1.0.8-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:d3420522057ebab1728b21ad473aa950026d07cb09da41103f8e597dfbfaeb13"},
+    {file = "msgpack-1.0.8-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:5845fdf5e5d5b78a49b826fcdc0eb2e2aa7191980e3d2cfd2a30303a74f212e2"},
+    {file = "msgpack-1.0.8-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6a0e76621f6e1f908ae52860bdcb58e1ca85231a9b0545e64509c931dd34275a"},
+    {file = "msgpack-1.0.8-cp38-cp38-win32.whl", hash = "sha256:374a8e88ddab84b9ada695d255679fb99c53513c0a51778796fcf0944d6c789c"},
+    {file = "msgpack-1.0.8-cp38-cp38-win_amd64.whl", hash = "sha256:f3709997b228685fe53e8c433e2df9f0cdb5f4542bd5114ed17ac3c0129b0480"},
+    {file = "msgpack-1.0.8-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:f51bab98d52739c50c56658cc303f190785f9a2cd97b823357e7aeae54c8f68a"},
+    {file = "msgpack-1.0.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:73ee792784d48aa338bba28063e19a27e8d989344f34aad14ea6e1b9bd83f596"},
+    {file = "msgpack-1.0.8-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f9904e24646570539a8950400602d66d2b2c492b9010ea7e965025cb71d0c86d"},
+    {file = "msgpack-1.0.8-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e75753aeda0ddc4c28dce4c32ba2f6ec30b1b02f6c0b14e547841ba5b24f753f"},
+    {file = "msgpack-1.0.8-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5dbf059fb4b7c240c873c1245ee112505be27497e90f7c6591261c7d3c3a8228"},
+    {file = "msgpack-1.0.8-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4916727e31c28be8beaf11cf117d6f6f188dcc36daae4e851fee88646f5b6b18"},
+    {file = "msgpack-1.0.8-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:7938111ed1358f536daf311be244f34df7bf3cdedb3ed883787aca97778b28d8"},
+    {file = "msgpack-1.0.8-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:493c5c5e44b06d6c9268ce21b302c9ca055c1fd3484c25ba41d34476c76ee746"},
+    {file = "msgpack-1.0.8-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5fbb160554e319f7b22ecf530a80a3ff496d38e8e07ae763b9e82fadfe96f273"},
+    {file = "msgpack-1.0.8-cp39-cp39-win32.whl", hash = "sha256:f9af38a89b6a5c04b7d18c492c8ccf2aee7048aff1ce8437c4683bb5a1df893d"},
+    {file = "msgpack-1.0.8-cp39-cp39-win_amd64.whl", hash = "sha256:ed59dd52075f8fc91da6053b12e8c89e37aa043f8986efd89e61fae69dc1b011"},
+    {file = "msgpack-1.0.8.tar.gz", hash = "sha256:95c02b0e27e706e48d0e5426d1710ca78e0f0628d6e89d5b5a5b91a5f12274f3"},
 ]
 
 [[package]]
 name = "msgspec"
-version = "0.18.2"
+version = "0.18.6"
 requires_python = ">=3.8"
 summary = "A fast serialization and validation library, with builtin support for JSON, MessagePack, YAML, and TOML."
+groups = ["default"]
 files = [
-    {file = "msgspec-0.18.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1535855b0db1bee4e5c79384010861de2a23391b45095785e84ec9489abc56cd"},
-    {file = "msgspec-0.18.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:2ad4f4704045a0fb1b5226769d9cdc00a4a69adec2e6770064f3db73bb91bbf9"},
-    {file = "msgspec-0.18.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:abcb92ffbca77bcfbedd5b29b68629628948982aafb994658e7abfad6e15913c"},
-    {file = "msgspec-0.18.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:358c2b908f1ed63419ccc5f185150c0caa3fc49599f4582504637cbfd5ff6242"},
-    {file = "msgspec-0.18.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:78a593bc0db95416d633b28cff00af0465f04590d53ff1a80a33d7e2728820ad"},
-    {file = "msgspec-0.18.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7b065995f3a41e4c8274a86e1ee84ac432969918373c777de239ef14f9537d80"},
-    {file = "msgspec-0.18.2-cp310-cp310-win_amd64.whl", hash = "sha256:d127bf90f29f1211520f1baa897b10f2a9c05b8648ce7dc89dfc9ca45599be53"},
-    {file = "msgspec-0.18.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3bfc55d5ca60b3aa2c2287191aa9e943c54eb0aef16d4babb92fddcc047093b1"},
-    {file = "msgspec-0.18.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e03ff009f3a2e1fe883703f98098d12aea6b30934707b404fd994e9ea1c1bfa7"},
-    {file = "msgspec-0.18.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ade3959577bff46c7d9476962d2d7aa086b2820f3da03ee000e9be4958404829"},
-    {file = "msgspec-0.18.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:80e57102469ee0d2186c72d42fa9460981ccd4252bdb997bf04ef2af0818984f"},
-    {file = "msgspec-0.18.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:25f7e3adaf1ca5d80455057576785069475b1d941eb877dbd0ae738cc5d1fefa"},
-    {file = "msgspec-0.18.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:b56cc7b9956daefb309447bbbb2581c84e5d5e3b89d573b1d5a25647522d2e43"},
-    {file = "msgspec-0.18.2-cp311-cp311-win_amd64.whl", hash = "sha256:84cc7932f78aeec6ef014cca4bb4ecea8469bc05f13c9eacdfa27baa785e54b9"},
-    {file = "msgspec-0.18.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:35420ae8afaa90498733541c0d8b2a73c70548a8a4d86da11201ed6df557e98f"},
-    {file = "msgspec-0.18.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:3f71c33efda990ecddc878ea2bb37f22e941d4264ded83e1b2309f86d335cde7"},
-    {file = "msgspec-0.18.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ccaddb764b5abe457c0eded4a252f5fbeb8b04a946b46a06a7e6ca299c35dcb1"},
-    {file = "msgspec-0.18.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:23e65efaef864bf66a4ddfae9c2200c40ce1a50411f454de1757f3651e5762cd"},
-    {file = "msgspec-0.18.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:baaba2411003f2e7a4328b5a58eba9efeb4c5e6a27e8ffd2adaccdc8feb0a805"},
-    {file = "msgspec-0.18.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:eb80befd343f3b378c8abad0367154703c74bde02fc62cbcf1a0e6b5fa779459"},
-    {file = "msgspec-0.18.2-cp38-cp38-win_amd64.whl", hash = "sha256:b9b3ed82f71816cddf0a9cdaae30a1d1addf8fe56ec09e7368db93ce43b29a81"},
-    {file = "msgspec-0.18.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:84fcf74b6371494aa536bf438ef96b08ce8f6e40483a01ed305535a40113136b"},
-    {file = "msgspec-0.18.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:a75c4efa7565048f81e709a366e14b9dc10752b3fb5ea1f3c8de5abfca3db3c2"},
-    {file = "msgspec-0.18.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c1ee8b9667fde3b5d7e0e0b555a8b70e2fa7bf2e02e9e8673af262c82c7b691"},
-    {file = "msgspec-0.18.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c79ac853409b0000727f4c3e5fb32fe38122ad94b9e074f992fa9ea7f00eb498"},
-    {file = "msgspec-0.18.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:595f14f628825d9d79eeea6e08514144a3d516eb014f0c6191f91899c83a6836"},
-    {file = "msgspec-0.18.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b90a44550f19ee0b8c37dbca75f96473299275001af2a00273d736b7347ead6d"},
-    {file = "msgspec-0.18.2-cp39-cp39-win_amd64.whl", hash = "sha256:70fa7f008008e2c823ecc1a143258bb2820ac76010cf6003091fa3832b6334c9"},
-    {file = "msgspec-0.18.2.tar.gz", hash = "sha256:3996bf1fc252658a7e028a0c263d28ac4dc48476e35f6fd8ebaf461a39459825"},
+    {file = "msgspec-0.18.6-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:77f30b0234eceeff0f651119b9821ce80949b4d667ad38f3bfed0d0ebf9d6d8f"},
+    {file = "msgspec-0.18.6-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:1a76b60e501b3932782a9da039bd1cd552b7d8dec54ce38332b87136c64852dd"},
+    {file = "msgspec-0.18.6-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:06acbd6edf175bee0e36295d6b0302c6de3aaf61246b46f9549ca0041a9d7177"},
+    {file = "msgspec-0.18.6-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40a4df891676d9c28a67c2cc39947c33de516335680d1316a89e8f7218660410"},
+    {file = "msgspec-0.18.6-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:a6896f4cd5b4b7d688018805520769a8446df911eb93b421c6c68155cdf9dd5a"},
+    {file = "msgspec-0.18.6-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:3ac4dd63fd5309dd42a8c8c36c1563531069152be7819518be0a9d03be9788e4"},
+    {file = "msgspec-0.18.6-cp310-cp310-win_amd64.whl", hash = "sha256:fda4c357145cf0b760000c4ad597e19b53adf01382b711f281720a10a0fe72b7"},
+    {file = "msgspec-0.18.6-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:e77e56ffe2701e83a96e35770c6adb655ffc074d530018d1b584a8e635b4f36f"},
+    {file = "msgspec-0.18.6-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d5351afb216b743df4b6b147691523697ff3a2fc5f3d54f771e91219f5c23aaa"},
+    {file = "msgspec-0.18.6-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c3232fabacef86fe8323cecbe99abbc5c02f7698e3f5f2e248e3480b66a3596b"},
+    {file = "msgspec-0.18.6-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e3b524df6ea9998bbc99ea6ee4d0276a101bcc1aa8d14887bb823914d9f60d07"},
+    {file = "msgspec-0.18.6-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:37f67c1d81272131895bb20d388dd8d341390acd0e192a55ab02d4d6468b434c"},
+    {file = "msgspec-0.18.6-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:d0feb7a03d971c1c0353de1a8fe30bb6579c2dc5ccf29b5f7c7ab01172010492"},
+    {file = "msgspec-0.18.6-cp311-cp311-win_amd64.whl", hash = "sha256:41cf758d3f40428c235c0f27bc6f322d43063bc32da7b9643e3f805c21ed57b4"},
+    {file = "msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c"},
+    {file = "msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1"},
+    {file = "msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466"},
+    {file = "msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca"},
+    {file = "msgspec-0.18.6-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:db1d8626748fa5d29bbd15da58b2d73af25b10aa98abf85aab8028119188ed57"},
+    {file = "msgspec-0.18.6-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:d70cb3d00d9f4de14d0b31d38dfe60c88ae16f3182988246a9861259c6722af6"},
+    {file = "msgspec-0.18.6-cp312-cp312-win_amd64.whl", hash = "sha256:1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0"},
+    {file = "msgspec-0.18.6-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:f7d9faed6dfff654a9ca7d9b0068456517f63dbc3aa704a527f493b9200b210a"},
+    {file = "msgspec-0.18.6-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:9da21f804c1a1471f26d32b5d9bc0480450ea77fbb8d9db431463ab64aaac2cf"},
+    {file = "msgspec-0.18.6-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:46eb2f6b22b0e61c137e65795b97dc515860bf6ec761d8fb65fdb62aa094ba61"},
+    {file = "msgspec-0.18.6-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c8355b55c80ac3e04885d72db515817d9fbb0def3bab936bba104e99ad22cf46"},
+    {file = "msgspec-0.18.6-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:9080eb12b8f59e177bd1eb5c21e24dd2ba2fa88a1dbc9a98e05ad7779b54c681"},
+    {file = "msgspec-0.18.6-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:cc001cf39becf8d2dcd3f413a4797c55009b3a3cdbf78a8bf5a7ca8fdb76032c"},
+    {file = "msgspec-0.18.6-cp38-cp38-win_amd64.whl", hash = "sha256:fac5834e14ac4da1fca373753e0c4ec9c8069d1fe5f534fa5208453b6065d5be"},
+    {file = "msgspec-0.18.6-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:974d3520fcc6b824a6dedbdf2b411df31a73e6e7414301abac62e6b8d03791b4"},
+    {file = "msgspec-0.18.6-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fd62e5818731a66aaa8e9b0a1e5543dc979a46278da01e85c3c9a1a4f047ef7e"},
+    {file = "msgspec-0.18.6-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7481355a1adcf1f08dedd9311193c674ffb8bf7b79314b4314752b89a2cf7f1c"},
+    {file = "msgspec-0.18.6-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6aa85198f8f154cf35d6f979998f6dadd3dc46a8a8c714632f53f5d65b315c07"},
+    {file = "msgspec-0.18.6-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:0e24539b25c85c8f0597274f11061c102ad6b0c56af053373ba4629772b407be"},
+    {file = "msgspec-0.18.6-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:c61ee4d3be03ea9cd089f7c8e36158786cd06e51fbb62529276452bbf2d52ece"},
+    {file = "msgspec-0.18.6-cp39-cp39-win_amd64.whl", hash = "sha256:b5c390b0b0b7da879520d4ae26044d74aeee5144f83087eb7842ba59c02bc090"},
+    {file = "msgspec-0.18.6.tar.gz", hash = "sha256:a59fc3b4fcdb972d09138cb516dbde600c99d07c38fd9372a6ef500d2d031b4e"},
 ]
 
 [[package]]
 name = "multidict"
-version = "6.0.4"
+version = "6.0.5"
 requires_python = ">=3.7"
 summary = "multidict implementation"
+groups = ["default"]
 files = [
-    {file = "multidict-6.0.4-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8"},
-    {file = "multidict-6.0.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171"},
-    {file = "multidict-6.0.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d6d635d5209b82a3492508cf5b365f3446afb65ae7ebd755e70e18f287b0adf7"},
-    {file = "multidict-6.0.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c048099e4c9e9d615545e2001d3d8a4380bd403e1a0578734e0d31703d1b0c0b"},
-    {file = "multidict-6.0.4-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547"},
-    {file = "multidict-6.0.4-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:16d232d4e5396c2efbbf4f6d4df89bfa905eb0d4dc5b3549d872ab898451f569"},
-    {file = "multidict-6.0.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:36c63aaa167f6c6b04ef2c85704e93af16c11d20de1d133e39de6a0e84582a93"},
-    {file = "multidict-6.0.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:64bdf1086b6043bf519869678f5f2757f473dee970d7abf6da91ec00acb9cb98"},
-    {file = "multidict-6.0.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:43644e38f42e3af682690876cff722d301ac585c5b9e1eacc013b7a3f7b696a0"},
-    {file = "multidict-6.0.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7582a1d1030e15422262de9f58711774e02fa80df0d1578995c76214f6954988"},
-    {file = "multidict-6.0.4-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:ddff9c4e225a63a5afab9dd15590432c22e8057e1a9a13d28ed128ecf047bbdc"},
-    {file = "multidict-6.0.4-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:ee2a1ece51b9b9e7752e742cfb661d2a29e7bcdba2d27e66e28a99f1890e4fa0"},
-    {file = "multidict-6.0.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:a2e4369eb3d47d2034032a26c7a80fcb21a2cb22e1173d761a162f11e562caa5"},
-    {file = "multidict-6.0.4-cp310-cp310-win32.whl", hash = "sha256:574b7eae1ab267e5f8285f0fe881f17efe4b98c39a40858247720935b893bba8"},
-    {file = "multidict-6.0.4-cp310-cp310-win_amd64.whl", hash = "sha256:4dcbb0906e38440fa3e325df2359ac6cb043df8e58c965bb45f4e406ecb162cc"},
-    {file = "multidict-6.0.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03"},
-    {file = "multidict-6.0.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:64da238a09d6039e3bd39bb3aee9c21a5e34f28bfa5aa22518581f910ff94af3"},
-    {file = "multidict-6.0.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ff959bee35038c4624250473988b24f846cbeb2c6639de3602c073f10410ceba"},
-    {file = "multidict-6.0.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9"},
-    {file = "multidict-6.0.4-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c5cb09abb18c1ea940fb99360ea0396f34d46566f157122c92dfa069d3e0e982"},
-    {file = "multidict-6.0.4-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:666daae833559deb2d609afa4490b85830ab0dfca811a98b70a205621a6109fe"},
-    {file = "multidict-6.0.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710"},
-    {file = "multidict-6.0.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7d18748f2d30f94f498e852c67d61261c643b349b9d2a581131725595c45ec6c"},
-    {file = "multidict-6.0.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:458f37be2d9e4c95e2d8866a851663cbc76e865b78395090786f6cd9b3bbf4f4"},
-    {file = "multidict-6.0.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:b1a2eeedcead3a41694130495593a559a668f382eee0727352b9a41e1c45759a"},
-    {file = "multidict-6.0.4-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:7d6ae9d593ef8641544d6263c7fa6408cc90370c8cb2bbb65f8d43e5b0351d9c"},
-    {file = "multidict-6.0.4-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:5979b5632c3e3534e42ca6ff856bb24b2e3071b37861c2c727ce220d80eee9ed"},
-    {file = "multidict-6.0.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:dcfe792765fab89c365123c81046ad4103fcabbc4f56d1c1997e6715e8015461"},
-    {file = "multidict-6.0.4-cp311-cp311-win32.whl", hash = "sha256:3601a3cece3819534b11d4efc1eb76047488fddd0c85a3948099d5da4d504636"},
-    {file = "multidict-6.0.4-cp311-cp311-win_amd64.whl", hash = "sha256:81a4f0b34bd92df3da93315c6a59034df95866014ac08535fc819f043bfd51f0"},
-    {file = "multidict-6.0.4-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:5fc1b16f586f049820c5c5b17bb4ee7583092fa0d1c4e28b5239181ff9532e0c"},
-    {file = "multidict-6.0.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161"},
-    {file = "multidict-6.0.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:b692f419760c0e65d060959df05f2a531945af31fda0c8a3b3195d4efd06de11"},
-    {file = "multidict-6.0.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45e1ecb0379bfaab5eef059f50115b54571acfbe422a14f668fc8c27ba410e7e"},
-    {file = "multidict-6.0.4-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ddd3915998d93fbcd2566ddf9cf62cdb35c9e093075f862935573d265cf8f65d"},
-    {file = "multidict-6.0.4-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:59d43b61c59d82f2effb39a93c48b845efe23a3852d201ed2d24ba830d0b4cf2"},
-    {file = "multidict-6.0.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cc8e1d0c705233c5dd0c5e6460fbad7827d5d36f310a0fadfd45cc3029762258"},
-    {file = "multidict-6.0.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d6aa0418fcc838522256761b3415822626f866758ee0bc6632c9486b179d0b52"},
-    {file = "multidict-6.0.4-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:6748717bb10339c4760c1e63da040f5f29f5ed6e59d76daee30305894069a660"},
-    {file = "multidict-6.0.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4d1a3d7ef5e96b1c9e92f973e43aa5e5b96c659c9bc3124acbbd81b0b9c8a951"},
-    {file = "multidict-6.0.4-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:4372381634485bec7e46718edc71528024fcdc6f835baefe517b34a33c731d60"},
-    {file = "multidict-6.0.4-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:fc35cb4676846ef752816d5be2193a1e8367b4c1397b74a565a9d0389c433a1d"},
-    {file = "multidict-6.0.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:4b9d9e4e2b37daddb5c23ea33a3417901fa7c7b3dee2d855f63ee67a0b21e5b1"},
-    {file = "multidict-6.0.4-cp38-cp38-win32.whl", hash = "sha256:e41b7e2b59679edfa309e8db64fdf22399eec4b0b24694e1b2104fb789207779"},
-    {file = "multidict-6.0.4-cp38-cp38-win_amd64.whl", hash = "sha256:d6c254ba6e45d8e72739281ebc46ea5eb5f101234f3ce171f0e9f5cc86991480"},
-    {file = "multidict-6.0.4-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:16ab77bbeb596e14212e7bab8429f24c1579234a3a462105cda4a66904998664"},
-    {file = "multidict-6.0.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bc779e9e6f7fda81b3f9aa58e3a6091d49ad528b11ed19f6621408806204ad35"},
-    {file = "multidict-6.0.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ceef517eca3e03c1cceb22030a3e39cb399ac86bff4e426d4fc6ae49052cc60"},
-    {file = "multidict-6.0.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:281af09f488903fde97923c7744bb001a9b23b039a909460d0f14edc7bf59706"},
-    {file = "multidict-6.0.4-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:52f2dffc8acaba9a2f27174c41c9e57f60b907bb9f096b36b1a1f3be71c6284d"},
-    {file = "multidict-6.0.4-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b41156839806aecb3641f3208c0dafd3ac7775b9c4c422d82ee2a45c34ba81ca"},
-    {file = "multidict-6.0.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d5e3fc56f88cc98ef8139255cf8cd63eb2c586531e43310ff859d6bb3a6b51f1"},
-    {file = "multidict-6.0.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8316a77808c501004802f9beebde51c9f857054a0c871bd6da8280e718444449"},
-    {file = "multidict-6.0.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:f70b98cd94886b49d91170ef23ec5c0e8ebb6f242d734ed7ed677b24d50c82cf"},
-    {file = "multidict-6.0.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:bf6774e60d67a9efe02b3616fee22441d86fab4c6d335f9d2051d19d90a40063"},
-    {file = "multidict-6.0.4-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:e69924bfcdda39b722ef4d9aa762b2dd38e4632b3641b1d9a57ca9cd18f2f83a"},
-    {file = "multidict-6.0.4-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:6b181d8c23da913d4ff585afd1155a0e1194c0b50c54fcfe286f70cdaf2b7176"},
-    {file = "multidict-6.0.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:52509b5be062d9eafc8170e53026fbc54cf3b32759a23d07fd935fb04fc22d95"},
-    {file = "multidict-6.0.4-cp39-cp39-win32.whl", hash = "sha256:27c523fbfbdfd19c6867af7346332b62b586eed663887392cff78d614f9ec313"},
-    {file = "multidict-6.0.4-cp39-cp39-win_amd64.whl", hash = "sha256:33029f5734336aa0d4c0384525da0387ef89148dc7191aae00ca5fb23d7aafc2"},
-    {file = "multidict-6.0.4.tar.gz", hash = "sha256:3666906492efb76453c0e7b97f2cf459b0682e7402c0489a95484965dbc1da49"},
+    {file = "multidict-6.0.5-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:228b644ae063c10e7f324ab1ab6b548bdf6f8b47f3ec234fef1093bc2735e5f9"},
+    {file = "multidict-6.0.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:896ebdcf62683551312c30e20614305f53125750803b614e9e6ce74a96232604"},
+    {file = "multidict-6.0.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:411bf8515f3be9813d06004cac41ccf7d1cd46dfe233705933dd163b60e37600"},
+    {file = "multidict-6.0.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1d147090048129ce3c453f0292e7697d333db95e52616b3793922945804a433c"},
+    {file = "multidict-6.0.5-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:215ed703caf15f578dca76ee6f6b21b7603791ae090fbf1ef9d865571039ade5"},
+    {file = "multidict-6.0.5-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:7c6390cf87ff6234643428991b7359b5f59cc15155695deb4eda5c777d2b880f"},
+    {file = "multidict-6.0.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21fd81c4ebdb4f214161be351eb5bcf385426bf023041da2fd9e60681f3cebae"},
+    {file = "multidict-6.0.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3cc2ad10255f903656017363cd59436f2111443a76f996584d1077e43ee51182"},
+    {file = "multidict-6.0.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:6939c95381e003f54cd4c5516740faba40cf5ad3eeff460c3ad1d3e0ea2549bf"},
+    {file = "multidict-6.0.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:220dd781e3f7af2c2c1053da9fa96d9cf3072ca58f057f4c5adaaa1cab8fc442"},
+    {file = "multidict-6.0.5-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:766c8f7511df26d9f11cd3a8be623e59cca73d44643abab3f8c8c07620524e4a"},
+    {file = "multidict-6.0.5-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:fe5d7785250541f7f5019ab9cba2c71169dc7d74d0f45253f8313f436458a4ef"},
+    {file = "multidict-6.0.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c1c1496e73051918fcd4f58ff2e0f2f3066d1c76a0c6aeffd9b45d53243702cc"},
+    {file = "multidict-6.0.5-cp310-cp310-win32.whl", hash = "sha256:7afcdd1fc07befad18ec4523a782cde4e93e0a2bf71239894b8d61ee578c1319"},
+    {file = "multidict-6.0.5-cp310-cp310-win_amd64.whl", hash = "sha256:99f60d34c048c5c2fabc766108c103612344c46e35d4ed9ae0673d33c8fb26e8"},
+    {file = "multidict-6.0.5-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:f285e862d2f153a70586579c15c44656f888806ed0e5b56b64489afe4a2dbfba"},
+    {file = "multidict-6.0.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:53689bb4e102200a4fafa9de9c7c3c212ab40a7ab2c8e474491914d2305f187e"},
+    {file = "multidict-6.0.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:612d1156111ae11d14afaf3a0669ebf6c170dbb735e510a7438ffe2369a847fd"},
+    {file = "multidict-6.0.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7be7047bd08accdb7487737631d25735c9a04327911de89ff1b26b81745bd4e3"},
+    {file = "multidict-6.0.5-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:de170c7b4fe6859beb8926e84f7d7d6c693dfe8e27372ce3b76f01c46e489fcf"},
+    {file = "multidict-6.0.5-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:04bde7a7b3de05732a4eb39c94574db1ec99abb56162d6c520ad26f83267de29"},
+    {file = "multidict-6.0.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:85f67aed7bb647f93e7520633d8f51d3cbc6ab96957c71272b286b2f30dc70ed"},
+    {file = "multidict-6.0.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:425bf820055005bfc8aa9a0b99ccb52cc2f4070153e34b701acc98d201693733"},
+    {file = "multidict-6.0.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d3eb1ceec286eba8220c26f3b0096cf189aea7057b6e7b7a2e60ed36b373b77f"},
+    {file = "multidict-6.0.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:7901c05ead4b3fb75113fb1dd33eb1253c6d3ee37ce93305acd9d38e0b5f21a4"},
+    {file = "multidict-6.0.5-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:e0e79d91e71b9867c73323a3444724d496c037e578a0e1755ae159ba14f4f3d1"},
+    {file = "multidict-6.0.5-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:29bfeb0dff5cb5fdab2023a7a9947b3b4af63e9c47cae2a10ad58394b517fddc"},
+    {file = "multidict-6.0.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e030047e85cbcedbfc073f71836d62dd5dadfbe7531cae27789ff66bc551bd5e"},
+    {file = "multidict-6.0.5-cp311-cp311-win32.whl", hash = "sha256:2f4848aa3baa109e6ab81fe2006c77ed4d3cd1e0ac2c1fbddb7b1277c168788c"},
+    {file = "multidict-6.0.5-cp311-cp311-win_amd64.whl", hash = "sha256:2faa5ae9376faba05f630d7e5e6be05be22913782b927b19d12b8145968a85ea"},
+    {file = "multidict-6.0.5-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:51d035609b86722963404f711db441cf7134f1889107fb171a970c9701f92e1e"},
+    {file = "multidict-6.0.5-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:cbebcd5bcaf1eaf302617c114aa67569dd3f090dd0ce8ba9e35e9985b41ac35b"},
+    {file = "multidict-6.0.5-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ffc42c922dbfddb4a4c3b438eb056828719f07608af27d163191cb3e3aa6cc5"},
+    {file = "multidict-6.0.5-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ceb3b7e6a0135e092de86110c5a74e46bda4bd4fbfeeb3a3bcec79c0f861e450"},
+    {file = "multidict-6.0.5-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:79660376075cfd4b2c80f295528aa6beb2058fd289f4c9252f986751a4cd0496"},
+    {file = "multidict-6.0.5-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e4428b29611e989719874670fd152b6625500ad6c686d464e99f5aaeeaca175a"},
+    {file = "multidict-6.0.5-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d84a5c3a5f7ce6db1f999fb9438f686bc2e09d38143f2d93d8406ed2dd6b9226"},
+    {file = "multidict-6.0.5-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:76c0de87358b192de7ea9649beb392f107dcad9ad27276324c24c91774ca5271"},
+    {file = "multidict-6.0.5-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:79a6d2ba910adb2cbafc95dad936f8b9386e77c84c35bc0add315b856d7c3abb"},
+    {file = "multidict-6.0.5-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:92d16a3e275e38293623ebf639c471d3e03bb20b8ebb845237e0d3664914caef"},
+    {file = "multidict-6.0.5-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:fb616be3538599e797a2017cccca78e354c767165e8858ab5116813146041a24"},
+    {file = "multidict-6.0.5-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:14c2976aa9038c2629efa2c148022ed5eb4cb939e15ec7aace7ca932f48f9ba6"},
+    {file = "multidict-6.0.5-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:435a0984199d81ca178b9ae2c26ec3d49692d20ee29bc4c11a2a8d4514c67eda"},
+    {file = "multidict-6.0.5-cp312-cp312-win32.whl", hash = "sha256:9fe7b0653ba3d9d65cbe7698cca585bf0f8c83dbbcc710db9c90f478e175f2d5"},
+    {file = "multidict-6.0.5-cp312-cp312-win_amd64.whl", hash = "sha256:01265f5e40f5a17f8241d52656ed27192be03bfa8764d88e8220141d1e4b3556"},
+    {file = "multidict-6.0.5-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:76f067f5121dcecf0d63a67f29080b26c43c71a98b10c701b0677e4a065fbd54"},
+    {file = "multidict-6.0.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b82cc8ace10ab5bd93235dfaab2021c70637005e1ac787031f4d1da63d493c1d"},
+    {file = "multidict-6.0.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5cb241881eefd96b46f89b1a056187ea8e9ba14ab88ba632e68d7a2ecb7aadf7"},
+    {file = "multidict-6.0.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e8e94e6912639a02ce173341ff62cc1201232ab86b8a8fcc05572741a5dc7d93"},
+    {file = "multidict-6.0.5-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:09a892e4a9fb47331da06948690ae38eaa2426de97b4ccbfafbdcbe5c8f37ff8"},
+    {file = "multidict-6.0.5-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:55205d03e8a598cfc688c71ca8ea5f66447164efff8869517f175ea632c7cb7b"},
+    {file = "multidict-6.0.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:37b15024f864916b4951adb95d3a80c9431299080341ab9544ed148091b53f50"},
+    {file = "multidict-6.0.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f2a1dee728b52b33eebff5072817176c172050d44d67befd681609b4746e1c2e"},
+    {file = "multidict-6.0.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:edd08e6f2f1a390bf137080507e44ccc086353c8e98c657e666c017718561b89"},
+    {file = "multidict-6.0.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:60d698e8179a42ec85172d12f50b1668254628425a6bd611aba022257cac1386"},
+    {file = "multidict-6.0.5-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:3d25f19500588cbc47dc19081d78131c32637c25804df8414463ec908631e453"},
+    {file = "multidict-6.0.5-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:4cc0ef8b962ac7a5e62b9e826bd0cd5040e7d401bc45a6835910ed699037a461"},
+    {file = "multidict-6.0.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:eca2e9d0cc5a889850e9bbd68e98314ada174ff6ccd1129500103df7a94a7a44"},
+    {file = "multidict-6.0.5-cp38-cp38-win32.whl", hash = "sha256:4a6a4f196f08c58c59e0b8ef8ec441d12aee4125a7d4f4fef000ccb22f8d7241"},
+    {file = "multidict-6.0.5-cp38-cp38-win_amd64.whl", hash = "sha256:0275e35209c27a3f7951e1ce7aaf93ce0d163b28948444bec61dd7badc6d3f8c"},
+    {file = "multidict-6.0.5-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:e7be68734bd8c9a513f2b0cfd508802d6609da068f40dc57d4e3494cefc92929"},
+    {file = "multidict-6.0.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:1d9ea7a7e779d7a3561aade7d596649fbecfa5c08a7674b11b423783217933f9"},
+    {file = "multidict-6.0.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:ea1456df2a27c73ce51120fa2f519f1bea2f4a03a917f4a43c8707cf4cbbae1a"},
+    {file = "multidict-6.0.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf590b134eb70629e350691ecca88eac3e3b8b3c86992042fb82e3cb1830d5e1"},
+    {file = "multidict-6.0.5-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5c0631926c4f58e9a5ccce555ad7747d9a9f8b10619621f22f9635f069f6233e"},
+    {file = "multidict-6.0.5-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:dce1c6912ab9ff5f179eaf6efe7365c1f425ed690b03341911bf4939ef2f3046"},
+    {file = "multidict-6.0.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c0868d64af83169e4d4152ec612637a543f7a336e4a307b119e98042e852ad9c"},
+    {file = "multidict-6.0.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:141b43360bfd3bdd75f15ed811850763555a251e38b2405967f8e25fb43f7d40"},
+    {file = "multidict-6.0.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:7df704ca8cf4a073334e0427ae2345323613e4df18cc224f647f251e5e75a527"},
+    {file = "multidict-6.0.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:6214c5a5571802c33f80e6c84713b2c79e024995b9c5897f794b43e714daeec9"},
+    {file = "multidict-6.0.5-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:cd6c8fca38178e12c00418de737aef1261576bd1b6e8c6134d3e729a4e858b38"},
+    {file = "multidict-6.0.5-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:e02021f87a5b6932fa6ce916ca004c4d441509d33bbdbeca70d05dff5e9d2479"},
+    {file = "multidict-6.0.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ebd8d160f91a764652d3e51ce0d2956b38efe37c9231cd82cfc0bed2e40b581c"},
+    {file = "multidict-6.0.5-cp39-cp39-win32.whl", hash = "sha256:04da1bb8c8dbadf2a18a452639771951c662c5ad03aefe4884775454be322c9b"},
+    {file = "multidict-6.0.5-cp39-cp39-win_amd64.whl", hash = "sha256:d6f6d4f185481c9669b9447bf9d9cf3b95a0e9df9d169bbc17e363b7d5487755"},
+    {file = "multidict-6.0.5-py3-none-any.whl", hash = "sha256:0d63c74e3d7ab26de115c49bffc92cc77ed23395303d496eae515d4204a625e7"},
+    {file = "multidict-6.0.5.tar.gz", hash = "sha256:f7e301075edaf50500f0b341543c41194d8df3ae5caf4702f2095f3ca73dd8da"},
 ]
 
 [[package]]
 name = "mypy"
-version = "1.5.1"
+version = "1.10.0"
 requires_python = ">=3.8"
 summary = "Optional static typing for Python"
+groups = ["linting"]
 dependencies = [
     "mypy-extensions>=1.0.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typing-extensions>=4.1.0",
 ]
 files = [
-    {file = "mypy-1.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f33592ddf9655a4894aef22d134de7393e95fcbdc2d15c1ab65828eee5c66c70"},
-    {file = "mypy-1.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:258b22210a4a258ccd077426c7a181d789d1121aca6db73a83f79372f5569ae0"},
-    {file = "mypy-1.5.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9ec1f695f0c25986e6f7f8778e5ce61659063268836a38c951200c57479cc12"},
-    {file = "mypy-1.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:abed92d9c8f08643c7d831300b739562b0a6c9fcb028d211134fc9ab20ccad5d"},
-    {file = "mypy-1.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:a156e6390944c265eb56afa67c74c0636f10283429171018446b732f1a05af25"},
-    {file = "mypy-1.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6ac9c21bfe7bc9f7f1b6fae441746e6a106e48fc9de530dea29e8cd37a2c0cc4"},
-    {file = "mypy-1.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:51cb1323064b1099e177098cb939eab2da42fea5d818d40113957ec954fc85f4"},
-    {file = "mypy-1.5.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:596fae69f2bfcb7305808c75c00f81fe2829b6236eadda536f00610ac5ec2243"},
-    {file = "mypy-1.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:32cb59609b0534f0bd67faebb6e022fe534bdb0e2ecab4290d683d248be1b275"},
-    {file = "mypy-1.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:159aa9acb16086b79bbb0016145034a1a05360626046a929f84579ce1666b315"},
-    {file = "mypy-1.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f6b0e77db9ff4fda74de7df13f30016a0a663928d669c9f2c057048ba44f09bb"},
-    {file = "mypy-1.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:26f71b535dfc158a71264e6dc805a9f8d2e60b67215ca0bfa26e2e1aa4d4d373"},
-    {file = "mypy-1.5.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2fc3a600f749b1008cc75e02b6fb3d4db8dbcca2d733030fe7a3b3502902f161"},
-    {file = "mypy-1.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:26fb32e4d4afa205b24bf645eddfbb36a1e17e995c5c99d6d00edb24b693406a"},
-    {file = "mypy-1.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:82cb6193de9bbb3844bab4c7cf80e6227d5225cc7625b068a06d005d861ad5f1"},
-    {file = "mypy-1.5.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:4a465ea2ca12804d5b34bb056be3a29dc47aea5973b892d0417c6a10a40b2d65"},
-    {file = "mypy-1.5.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:9fece120dbb041771a63eb95e4896791386fe287fefb2837258925b8326d6160"},
-    {file = "mypy-1.5.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d28ddc3e3dfeab553e743e532fb95b4e6afad51d4706dd22f28e1e5e664828d2"},
-    {file = "mypy-1.5.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:57b10c56016adce71fba6bc6e9fd45d8083f74361f629390c556738565af8eeb"},
-    {file = "mypy-1.5.1-cp38-cp38-win_amd64.whl", hash = "sha256:ff0cedc84184115202475bbb46dd99f8dcb87fe24d5d0ddfc0fe6b8575c88d2f"},
-    {file = "mypy-1.5.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8f772942d372c8cbac575be99f9cc9d9fb3bd95c8bc2de6c01411e2c84ebca8a"},
-    {file = "mypy-1.5.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:5d627124700b92b6bbaa99f27cbe615c8ea7b3402960f6372ea7d65faf376c14"},
-    {file = "mypy-1.5.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:361da43c4f5a96173220eb53340ace68cda81845cd88218f8862dfb0adc8cddb"},
-    {file = "mypy-1.5.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:330857f9507c24de5c5724235e66858f8364a0693894342485e543f5b07c8693"},
-    {file = "mypy-1.5.1-cp39-cp39-win_amd64.whl", hash = "sha256:c543214ffdd422623e9fedd0869166c2f16affe4ba37463975043ef7d2ea8770"},
-    {file = "mypy-1.5.1-py3-none-any.whl", hash = "sha256:f757063a83970d67c444f6e01d9550a7402322af3557ce7630d3c957386fa8f5"},
-    {file = "mypy-1.5.1.tar.gz", hash = "sha256:b031b9601f1060bf1281feab89697324726ba0c0bae9d7cd7ab4b690940f0b92"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99"},
+    {file = "mypy-1.10.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2"},
+    {file = "mypy-1.10.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9"},
+    {file = "mypy-1.10.0-cp310-cp310-win_amd64.whl", hash = "sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee"},
+    {file = "mypy-1.10.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de"},
+    {file = "mypy-1.10.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7"},
+    {file = "mypy-1.10.0-cp311-cp311-win_amd64.whl", hash = "sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30"},
+    {file = "mypy-1.10.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e"},
+    {file = "mypy-1.10.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5"},
+    {file = "mypy-1.10.0-cp312-cp312-win_amd64.whl", hash = "sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727"},
+    {file = "mypy-1.10.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4"},
+    {file = "mypy-1.10.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061"},
+    {file = "mypy-1.10.0-cp38-cp38-win_amd64.whl", hash = "sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec"},
+    {file = "mypy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821"},
+    {file = "mypy-1.10.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746"},
+    {file = "mypy-1.10.0-cp39-cp39-win_amd64.whl", hash = "sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a"},
+    {file = "mypy-1.10.0-py3-none-any.whl", hash = "sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee"},
+    {file = "mypy-1.10.0.tar.gz", hash = "sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131"},
 ]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 requires_python = ">=3.5"
 summary = "Type system extensions for programs checked with the mypy type checker."
+groups = ["docs", "linting"]
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "natsort"
 version = "8.4.0"
 requires_python = ">=3.7"
 summary = "Simple yet flexible natural sorting in Python."
+groups = ["docs"]
 files = [
     {file = "natsort-8.4.0-py3-none-any.whl", hash = "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"},
     {file = "natsort-8.4.0.tar.gz", hash = "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581"},
 ]
 
 [[package]]
 name = "nodeenv"
 version = "1.8.0"
 requires_python = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*"
 summary = "Node.js virtual environment builder"
+groups = ["linting"]
 dependencies = [
     "setuptools",
 ]
 files = [
     {file = "nodeenv-1.8.0-py2.py3-none-any.whl", hash = "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"},
     {file = "nodeenv-1.8.0.tar.gz", hash = "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
+groups = ["docs", "test"]
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "pathspec"
-version = "0.11.2"
-requires_python = ">=3.7"
+version = "0.12.1"
+requires_python = ">=3.8"
 summary = "Utility library for gitignore style pattern matching of file paths."
+groups = ["docs"]
 files = [
-    {file = "pathspec-0.11.2-py3-none-any.whl", hash = "sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20"},
-    {file = "pathspec-0.11.2.tar.gz", hash = "sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3"},
+    {file = "pathspec-0.12.1-py3-none-any.whl", hash = "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08"},
+    {file = "pathspec-0.12.1.tar.gz", hash = "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.10.0"
-requires_python = ">=3.7"
-summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
+version = "4.2.1"
+requires_python = ">=3.8"
+summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
+groups = ["docs", "linting"]
 files = [
-    {file = "platformdirs-3.10.0-py3-none-any.whl", hash = "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"},
-    {file = "platformdirs-3.10.0.tar.gz", hash = "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d"},
+    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
+    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
 ]
 
 [[package]]
 name = "pluggy"
-version = "1.3.0"
+version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
+groups = ["test"]
 files = [
-    {file = "pluggy-1.3.0-py3-none-any.whl", hash = "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"},
-    {file = "pluggy-1.3.0.tar.gz", hash = "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [[package]]
 name = "polyfactory"
-version = "2.9.0"
-requires_python = ">=3.8,<4.0"
+version = "2.15.0"
+requires_python = "<4.0,>=3.8"
 summary = "Mock data generation factories"
+groups = ["default"]
 dependencies = [
     "faker",
-    "typing-extensions",
+    "typing-extensions>=4.6.0",
 ]
 files = [
-    {file = "polyfactory-2.9.0-py3-none-any.whl", hash = "sha256:7513347be6327739174dbd4ca6ddd96981fb697437283acb5362a604cf6d7f58"},
-    {file = "polyfactory-2.9.0.tar.gz", hash = "sha256:af61fc5b03d0c5bb343a2289bdce457f27bbf8aefba69c592dca0841f905e7a5"},
+    {file = "polyfactory-2.15.0-py3-none-any.whl", hash = "sha256:ff5b6a8742cbd6fbde9f81310b9732d5421fbec31916d6ede5a977753110fbe9"},
+    {file = "polyfactory-2.15.0.tar.gz", hash = "sha256:a3ff5263756ad74acf4001f04c1b6aab7d1197cbaa070352df79573a8dcd85ec"},
 ]
 
 [[package]]
 name = "pre-commit"
-version = "3.4.0"
+version = "3.5.0"
 requires_python = ">=3.8"
 summary = "A framework for managing and maintaining multi-language pre-commit hooks."
+groups = ["linting"]
 dependencies = [
     "cfgv>=2.0.0",
     "identify>=1.0.0",
     "nodeenv>=0.11.1",
     "pyyaml>=5.1",
     "virtualenv>=20.10.0",
 ]
 files = [
-    {file = "pre_commit-3.4.0-py2.py3-none-any.whl", hash = "sha256:96d529a951f8b677f730a7212442027e8ba53f9b04d217c4c67dc56c393ad945"},
-    {file = "pre_commit-3.4.0.tar.gz", hash = "sha256:6bbd5129a64cad4c0dfaeeb12cd8f7ea7e15b77028d985341478c8af3c759522"},
+    {file = "pre_commit-3.5.0-py2.py3-none-any.whl", hash = "sha256:841dc9aef25daba9a0238cd27984041fa0467b4199fc4852e27950664919f660"},
+    {file = "pre_commit-3.5.0.tar.gz", hash = "sha256:5804465c675b659b0862f07907f96295d490822a450c4c40e747d0b1c6ebcb32"},
 ]
 
 [[package]]
 name = "pygments"
-version = "2.16.1"
-requires_python = ">=3.7"
+version = "2.18.0"
+requires_python = ">=3.8"
 summary = "Pygments is a syntax highlighting package written in Python."
+groups = ["default", "docs"]
 files = [
-    {file = "Pygments-2.16.1-py3-none-any.whl", hash = "sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692"},
-    {file = "Pygments-2.16.1.tar.gz", hash = "sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29"},
+    {file = "pygments-2.18.0-py3-none-any.whl", hash = "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"},
+    {file = "pygments-2.18.0.tar.gz", hash = "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199"},
 ]
 
 [[package]]
 name = "pytest"
-version = "7.4.2"
-requires_python = ">=3.7"
+version = "8.2.0"
+requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
+groups = ["test"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=0.12",
-    "tomli>=1.0.0; python_version < \"3.11\"",
+    "pluggy<2.0,>=1.5",
+    "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-7.4.2-py3-none-any.whl", hash = "sha256:1d881c6124e08ff0a1bb75ba3ec0bfd8b5354a01c194ddd5a0a870a48d99b002"},
-    {file = "pytest-7.4.2.tar.gz", hash = "sha256:a766259cfab564a2ad52cb1aae1b881a75c3eb7e34ca3779697c23ed47c47069"},
-]
-
-[[package]]
-name = "pytest-asyncio"
-version = "0.21.1"
-requires_python = ">=3.7"
-summary = "Pytest support for asyncio"
-dependencies = [
-    "pytest>=7.0.0",
-]
-files = [
-    {file = "pytest-asyncio-0.21.1.tar.gz", hash = "sha256:40a7eae6dded22c7b604986855ea48400ab15b069ae38116e8c01238e9eeb64d"},
-    {file = "pytest_asyncio-0.21.1-py3-none-any.whl", hash = "sha256:8666c1c8ac02631d7c51ba282e0c69a8a452b211ffedf2599099845da5c5c37b"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [[package]]
 name = "pytest-cov"
-version = "4.1.0"
-requires_python = ">=3.7"
+version = "5.0.0"
+requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
+groups = ["test"]
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 files = [
-    {file = "pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
-    {file = "pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
+    {file = "pytest-cov-5.0.0.tar.gz", hash = "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"},
+    {file = "pytest_cov-5.0.0-py3-none-any.whl", hash = "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652"},
 ]
 
 [[package]]
-name = "pytest-lazy-fixture"
-version = "0.6.3"
-summary = "It helps to use fixtures in pytest.mark.parametrize"
+name = "pytest-databases"
+version = "0.5.0"
+requires_python = ">=3.8"
+summary = "Reusable database fixtures for any and all databases."
+groups = ["test"]
 dependencies = [
-    "pytest>=3.2.5",
+    "pytest",
 ]
 files = [
-    {file = "pytest-lazy-fixture-0.6.3.tar.gz", hash = "sha256:0e7d0c7f74ba33e6e80905e9bfd81f9d15ef9a790de97993e34213deb5ad10ac"},
-    {file = "pytest_lazy_fixture-0.6.3-py3-none-any.whl", hash = "sha256:e0b379f38299ff27a653f03eaa69b08a6fd4484e46fd1c9907d984b9f9daeda6"},
+    {file = "pytest_databases-0.5.0-py3-none-any.whl", hash = "sha256:27b6b9ef4114b28b595ad4c4d9a74428611555e5360ebcb7c4a074b4efd09cd9"},
+    {file = "pytest_databases-0.5.0.tar.gz", hash = "sha256:7b9e07133964a07dd7eed1216a8879f252468e8aaa0acee1235501ca6809cd3c"},
 ]
 
 [[package]]
 name = "pytest-mock"
-version = "3.11.1"
-requires_python = ">=3.7"
+version = "3.14.0"
+requires_python = ">=3.8"
 summary = "Thin-wrapper around the mock package for easier use with pytest"
+groups = ["test"]
 dependencies = [
-    "pytest>=5.0",
+    "pytest>=6.2.5",
 ]
 files = [
-    {file = "pytest-mock-3.11.1.tar.gz", hash = "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"},
-    {file = "pytest_mock-3.11.1-py3-none-any.whl", hash = "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39"},
+    {file = "pytest-mock-3.14.0.tar.gz", hash = "sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0"},
+    {file = "pytest_mock-3.14.0-py3-none-any.whl", hash = "sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f"},
 ]
 
 [[package]]
-name = "pytest-xdist"
-version = "3.3.1"
-requires_python = ">=3.7"
-summary = "pytest xdist plugin for distributed testing, most importantly across multiple CPUs"
+name = "pytest-sugar"
+version = "1.0.0"
+summary = "pytest-sugar is a plugin for pytest that changes the default look and feel of pytest (e.g. progressbar, show tests that fail instantly)."
+groups = ["test"]
 dependencies = [
-    "execnet>=1.1",
+    "packaging>=21.3",
     "pytest>=6.2.0",
+    "termcolor>=2.1.0",
 ]
 files = [
-    {file = "pytest-xdist-3.3.1.tar.gz", hash = "sha256:d5ee0520eb1b7bcca50a60a518ab7a7707992812c578198f8b44fdfac78e8c93"},
-    {file = "pytest_xdist-3.3.1-py3-none-any.whl", hash = "sha256:ff9daa7793569e6a68544850fd3927cd257cc03a7ef76c95e86915355e82b5f2"},
+    {file = "pytest-sugar-1.0.0.tar.gz", hash = "sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a"},
+    {file = "pytest_sugar-1.0.0-py3-none-any.whl", hash = "sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd"},
 ]
 
 [[package]]
 name = "python-dateutil"
-version = "2.8.2"
+version = "2.9.0.post0"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 summary = "Extensions to the standard Python datetime module"
+groups = ["default"]
 dependencies = [
     "six>=1.5",
 ]
 files = [
-    {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
-    {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
-]
-
-[[package]]
-name = "python-dotenv"
-version = "1.0.0"
-requires_python = ">=3.8"
-summary = "Read key-value pairs from a .env file and set them as environment variables"
-files = [
-    {file = "python-dotenv-1.0.0.tar.gz", hash = "sha256:a8df96034aae6d2d50a4ebe8216326c61c3eb64836776504fcca410e5937a3ba"},
-    {file = "python_dotenv-1.0.0-py3-none-any.whl", hash = "sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a"},
+    {file = "python-dateutil-2.9.0.post0.tar.gz", hash = "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3"},
+    {file = "python_dateutil-2.9.0.post0-py2.py3-none-any.whl", hash = "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"},
 ]
 
 [[package]]
 name = "pytz"
-version = "2023.3.post1"
+version = "2024.1"
 summary = "World timezone definitions, modern and historical"
+groups = ["docs"]
+marker = "python_version < \"3.9\""
 files = [
-    {file = "pytz-2023.3.post1-py2.py3-none-any.whl", hash = "sha256:ce42d816b81b68506614c11e8937d3aa9e41007ceb50bfdcb0749b921bf646c7"},
-    {file = "pytz-2023.3.post1.tar.gz", hash = "sha256:7b4fddbeb94a1eba4b557da24f19fdf9db575192544270a9101d8509f9f43d7b"},
+    {file = "pytz-2024.1-py2.py3-none-any.whl", hash = "sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319"},
+    {file = "pytz-2024.1.tar.gz", hash = "sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812"},
 ]
 
 [[package]]
 name = "pyyaml"
 version = "6.0.1"
 requires_python = ">=3.6"
 summary = "YAML parser and emitter for Python"
+groups = ["default", "linting"]
 files = [
     {file = "PyYAML-6.0.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a"},
     {file = "PyYAML-6.0.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"},
     {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938"},
     {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d"},
     {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515"},
     {file = "PyYAML-6.0.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290"},
@@ -1483,14 +1458,15 @@
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc"},
     {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673"},
     {file = "PyYAML-6.0.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b"},
     {file = "PyYAML-6.0.1-cp311-cp311-win32.whl", hash = "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741"},
     {file = "PyYAML-6.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28"},
     {file = "PyYAML-6.0.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9"},
+    {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef"},
     {file = "PyYAML-6.0.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0"},
     {file = "PyYAML-6.0.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4"},
     {file = "PyYAML-6.0.1-cp312-cp312-win32.whl", hash = "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54"},
     {file = "PyYAML-6.0.1-cp312-cp312-win_amd64.whl", hash = "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df"},
     {file = "PyYAML-6.0.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595"},
     {file = "PyYAML-6.0.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5"},
     {file = "PyYAML-6.0.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696"},
@@ -1510,192 +1486,223 @@
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 requires_python = ">=3.7"
 summary = "Python HTTP for Humans."
+groups = ["docs"]
 dependencies = [
     "certifi>=2017.4.17",
     "charset-normalizer<4,>=2",
     "idna<4,>=2.5",
     "urllib3<3,>=1.21.1",
 ]
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
     {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
 [[package]]
 name = "rich"
-version = "13.6.0"
+version = "13.7.1"
 requires_python = ">=3.7.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
+groups = ["default"]
 dependencies = [
     "markdown-it-py>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 files = [
-    {file = "rich-13.6.0-py3-none-any.whl", hash = "sha256:2b38e2fe9ca72c9a00170a1a2d20c63c790d0e10ef1fe35eba76e1e7b1d7d245"},
-    {file = "rich-13.6.0.tar.gz", hash = "sha256:5c14d22737e6d5084ef4771b62d5d4363165b403455a30a1c8ca39dc7b644bef"},
+    {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
+    {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "rich-click"
-version = "1.6.1"
+version = "1.8.0"
 requires_python = ">=3.7"
 summary = "Format click help output nicely with rich"
+groups = ["default"]
 dependencies = [
     "click>=7",
-    "rich>=10.7.0",
+    "rich>=10.7",
+    "typing-extensions",
 ]
 files = [
-    {file = "rich-click-1.6.1.tar.gz", hash = "sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e"},
-    {file = "rich_click-1.6.1-py3-none-any.whl", hash = "sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95"},
+    {file = "rich_click-1.8.0-py3-none-any.whl", hash = "sha256:846f504eb83a948d864888b2d73c71e52c310490c2babceac57e388aead086e2"},
+    {file = "rich_click-1.8.0.tar.gz", hash = "sha256:f8cad0d67d286d6cd6fc9f69f2d6f25c6c4c2d99fb9d6cb3b8987b593dbe6fa8"},
 ]
 
 [[package]]
 name = "ruamel-yaml"
-version = "0.17.33"
-requires_python = ">=3"
+version = "0.18.6"
+requires_python = ">=3.7"
 summary = "ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order"
+groups = ["docs"]
 dependencies = [
-    "ruamel-yaml-clib>=0.2.7; platform_python_implementation == \"CPython\" and python_version < \"3.12\"",
+    "ruamel-yaml-clib>=0.2.7; platform_python_implementation == \"CPython\" and python_version < \"3.13\"",
 ]
 files = [
-    {file = "ruamel.yaml-0.17.33-py3-none-any.whl", hash = "sha256:2080c7a02b8a30fb3c06727cdf3e254a64055eedf3aa2d17c2b669639c04971b"},
-    {file = "ruamel.yaml-0.17.33.tar.gz", hash = "sha256:5c56aa0bff2afceaa93bffbfc78b450b7dc1e01d5edb80b3a570695286ae62b1"},
+    {file = "ruamel.yaml-0.18.6-py3-none-any.whl", hash = "sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636"},
+    {file = "ruamel.yaml-0.18.6.tar.gz", hash = "sha256:8b27e6a217e786c6fbe5634d8f3f11bc63e0f80f6a5890f28863d9c45aac311b"},
 ]
 
 [[package]]
 name = "ruamel-yaml-clib"
-version = "0.2.7"
-requires_python = ">=3.5"
+version = "0.2.8"
+requires_python = ">=3.6"
 summary = "C version of reader, parser and emitter for ruamel.yaml derived from libyaml"
+groups = ["docs"]
+marker = "platform_python_implementation == \"CPython\" and python_version < \"3.13\""
 files = [
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71"},
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7"},
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-manylinux2014_aarch64.whl", hash = "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80"},
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab"},
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-win32.whl", hash = "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231"},
-    {file = "ruamel.yaml.clib-0.2.7-cp310-cp310-win_amd64.whl", hash = "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-macosx_13_0_arm64.whl", hash = "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-manylinux2014_aarch64.whl", hash = "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-win32.whl", hash = "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"},
-    {file = "ruamel.yaml.clib-0.2.7-cp311-cp311-win_amd64.whl", hash = "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-macosx_12_0_arm64.whl", hash = "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-manylinux2014_aarch64.whl", hash = "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-win32.whl", hash = "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac"},
-    {file = "ruamel.yaml.clib-0.2.7-cp38-cp38-win_amd64.whl", hash = "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5bc0667c1eb8f83a3752b71b9c4ba55ef7c7058ae57022dd9b29065186a113d9"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-macosx_12_0_arm64.whl", hash = "sha256:4a4d8d417868d68b979076a9be6a38c676eca060785abaa6709c7b31593c35d1"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-manylinux2014_aarch64.whl", hash = "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-win32.whl", hash = "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8"},
-    {file = "ruamel.yaml.clib-0.2.7-cp39-cp39-win_amd64.whl", hash = "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5"},
-    {file = "ruamel.yaml.clib-0.2.7.tar.gz", hash = "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:b42169467c42b692c19cf539c38d4602069d8c1505e97b86387fcf7afb766e1d"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-macosx_13_0_arm64.whl", hash = "sha256:07238db9cbdf8fc1e9de2489a4f68474e70dffcb32232db7c08fa61ca0c7c462"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-manylinux_2_24_aarch64.whl", hash = "sha256:aa2267c6a303eb483de8d02db2871afb5c5fc15618d894300b88958f729ad74f"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:840f0c7f194986a63d2c2465ca63af8ccbbc90ab1c6001b1978f05119b5e7334"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:024cfe1fc7c7f4e1aff4a81e718109e13409767e4f871443cbff3dba3578203d"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-win32.whl", hash = "sha256:c69212f63169ec1cfc9bb44723bf2917cbbd8f6191a00ef3410f5a7fe300722d"},
+    {file = "ruamel.yaml.clib-0.2.8-cp310-cp310-win_amd64.whl", hash = "sha256:cabddb8d8ead485e255fe80429f833172b4cadf99274db39abc080e068cbcc31"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:bef08cd86169d9eafb3ccb0a39edb11d8e25f3dae2b28f5c52fd997521133069"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-macosx_13_0_arm64.whl", hash = "sha256:b16420e621d26fdfa949a8b4b47ade8810c56002f5389970db4ddda51dbff248"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:25c515e350e5b739842fc3228d662413ef28f295791af5e5110b543cf0b57d9b"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-manylinux_2_24_aarch64.whl", hash = "sha256:1707814f0d9791df063f8c19bb51b0d1278b8e9a2353abbb676c2f685dee6afe"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:46d378daaac94f454b3a0e3d8d78cafd78a026b1d71443f4966c696b48a6d899"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:09b055c05697b38ecacb7ac50bdab2240bfca1a0c4872b0fd309bb07dc9aa3a9"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-win32.whl", hash = "sha256:53a300ed9cea38cf5a2a9b069058137c2ca1ce658a874b79baceb8f892f915a7"},
+    {file = "ruamel.yaml.clib-0.2.8-cp311-cp311-win_amd64.whl", hash = "sha256:c2a72e9109ea74e511e29032f3b670835f8a59bbdc9ce692c5b4ed91ccf1eedb"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-macosx_13_0_arm64.whl", hash = "sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_28_x86_64.whl", hash = "sha256:d176b57452ab5b7028ac47e7b3cf644bcfdc8cacfecf7e71759f7f51a59e5c92"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-manylinux_2_24_aarch64.whl", hash = "sha256:1dc67314e7e1086c9fdf2680b7b6c2be1c0d8e3a8279f2e993ca2a7545fecf62"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:3213ece08ea033eb159ac52ae052a4899b56ecc124bb80020d9bbceeb50258e9"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:aab7fd643f71d7946f2ee58cc88c9b7bfc97debd71dcc93e03e2d174628e7e2d"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-win32.whl", hash = "sha256:5c365d91c88390c8d0a8545df0b5857172824b1c604e867161e6b3d59a827eaa"},
+    {file = "ruamel.yaml.clib-0.2.8-cp312-cp312-win_amd64.whl", hash = "sha256:1758ce7d8e1a29d23de54a16ae867abd370f01b5a69e1a3ba75223eaa3ca1a1b"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1b617618914cb00bf5c34d4357c37aa15183fa229b24767259657746c9077615"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-macosx_12_0_arm64.whl", hash = "sha256:a6a9ffd280b71ad062eae53ac1659ad86a17f59a0fdc7699fd9be40525153337"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-manylinux_2_24_aarch64.whl", hash = "sha256:305889baa4043a09e5b76f8e2a51d4ffba44259f6b4c72dec8ca56207d9c6fe1"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:700e4ebb569e59e16a976857c8798aee258dceac7c7d6b50cab63e080058df91"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-win32.whl", hash = "sha256:955eae71ac26c1ab35924203fda6220f84dce57d6d7884f189743e2abe3a9fbe"},
+    {file = "ruamel.yaml.clib-0.2.8-cp38-cp38-win_amd64.whl", hash = "sha256:56f4252222c067b4ce51ae12cbac231bce32aee1d33fbfc9d17e5b8d6966c312"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:03d1162b6d1df1caa3a4bd27aa51ce17c9afc2046c31b0ad60a0a96ec22f8001"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-macosx_12_0_arm64.whl", hash = "sha256:bba64af9fa9cebe325a62fa398760f5c7206b215201b0ec825005f1b18b9bccf"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-manylinux_2_24_aarch64.whl", hash = "sha256:a1a45e0bb052edf6a1d3a93baef85319733a888363938e1fc9924cb00c8df24c"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:da09ad1c359a728e112d60116f626cc9f29730ff3e0e7db72b9a2dbc2e4beed5"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:184565012b60405d93838167f425713180b949e9d8dd0bbc7b49f074407c5a8b"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:a75879bacf2c987c003368cf14bed0ffe99e8e85acfa6c0bfffc21a090f16880"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win32.whl", hash = "sha256:84b554931e932c46f94ab306913ad7e11bba988104c5cff26d90d03f68258cd5"},
+    {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win_amd64.whl", hash = "sha256:25ac8c08322002b06fa1d49d1646181f0b2c72f5cbc15a85e80b4c30a544bb15"},
+    {file = "ruamel.yaml.clib-0.2.8.tar.gz", hash = "sha256:beb2e0404003de9a4cab9753a8805a8fe9320ee6673136ed7f04255fe60bb512"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.291"
+version = "0.4.3"
 requires_python = ">=3.7"
-summary = "An extremely fast Python linter, written in Rust."
+summary = "An extremely fast Python linter and code formatter, written in Rust."
+groups = ["docs", "linting"]
 files = [
-    {file = "ruff-0.0.291-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:b97d0d7c136a85badbc7fd8397fdbb336e9409b01c07027622f28dcd7db366f2"},
-    {file = "ruff-0.0.291-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:6ab44ea607967171e18aa5c80335237be12f3a1523375fa0cede83c5cf77feb4"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a04b384f2d36f00d5fb55313d52a7d66236531195ef08157a09c4728090f2ef0"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:b727c219b43f903875b7503a76c86237a00d1a39579bb3e21ce027eec9534051"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:87671e33175ae949702774071b35ed4937da06f11851af75cd087e1b5a488ac4"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:b75f5801547f79b7541d72a211949754c21dc0705c70eddf7f21c88a64de8b97"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b09b94efdcd162fe32b472b2dd5bf1c969fcc15b8ff52f478b048f41d4590e09"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:8d5b56bc3a2f83a7a1d7f4447c54d8d3db52021f726fdd55d549ca87bca5d747"},
-    {file = "ruff-0.0.291-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:13f0d88e5f367b2dc8c7d90a8afdcfff9dd7d174e324fd3ed8e0b5cb5dc9b7f6"},
-    {file = "ruff-0.0.291-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b3eeee1b1a45a247758ecdc3ab26c307336d157aafc61edb98b825cadb153df3"},
-    {file = "ruff-0.0.291-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:6c06006350c3bb689765d71f810128c9cdf4a1121fd01afc655c87bab4fb4f83"},
-    {file = "ruff-0.0.291-py3-none-musllinux_1_2_i686.whl", hash = "sha256:fd17220611047de247b635596e3174f3d7f2becf63bd56301fc758778df9b629"},
-    {file = "ruff-0.0.291-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:5383ba67ad360caf6060d09012f1fb2ab8bd605ab766d10ca4427a28ab106e0b"},
-    {file = "ruff-0.0.291-py3-none-win32.whl", hash = "sha256:1d5f0616ae4cdc7a938b493b6a1a71c8a47d0300c0d65f6e41c281c2f7490ad3"},
-    {file = "ruff-0.0.291-py3-none-win_amd64.whl", hash = "sha256:8a69bfbde72db8ca1c43ee3570f59daad155196c3fbe357047cd9b77de65f15b"},
-    {file = "ruff-0.0.291-py3-none-win_arm64.whl", hash = "sha256:d867384a4615b7f30b223a849b52104214442b5ba79b473d7edd18da3cde22d6"},
-    {file = "ruff-0.0.291.tar.gz", hash = "sha256:c61109661dde9db73469d14a82b42a88c7164f731e6a3b0042e71394c1c7ceed"},
+    {file = "ruff-0.4.3-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:b70800c290f14ae6fcbb41bbe201cf62dfca024d124a1f373e76371a007454ce"},
+    {file = "ruff-0.4.3-py3-none-macosx_11_0_arm64.whl", hash = "sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eba1f14df3c758dd7de5b55fbae7e1c8af238597961e5fb628f3de446c3c40c5"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:819fb06d535cc76dfddbfe8d3068ff602ddeb40e3eacbc90e0d1272bb8d97113"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:510a67d232d2ebe983fddea324dbf9d69b71c4d2dfeb8a862f4a127536dd4cfb"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9ff11cd9a092ee7680a56d21f302bdda14327772cd870d806610a3503d001f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:7363691198719c26459e08cc17c6a3dac6f592e9ea3d2fa772f4e561b5fe82a3"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_i686.whl", hash = "sha256:eeb039f8428fcb6725bb63cbae92ad67b0559e68b5d80f840f11914afd8ddf7f"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:927b11c1e4d0727ce1a729eace61cee88a334623ec424c0b1c8fe3e5f9d3c865"},
+    {file = "ruff-0.4.3-py3-none-win32.whl", hash = "sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30"},
+    {file = "ruff-0.4.3-py3-none-win_amd64.whl", hash = "sha256:7a1c3a450bc6539ef00da6c819fb1b76b6b065dec585f91456e7c0d6a0bbc725"},
+    {file = "ruff-0.4.3-py3-none-win_arm64.whl", hash = "sha256:71ca5f8ccf1121b95a59649482470c5601c60a416bf189d553955b0338e34614"},
+    {file = "ruff-0.4.3.tar.gz", hash = "sha256:ff0a3ef2e3c4b6d133fbedcf9586abfbe38d076041f2dc18ffb2c7e0485d5a07"},
 ]
 
 [[package]]
 name = "setuptools"
-version = "68.2.2"
+version = "69.5.1"
 requires_python = ">=3.8"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
+groups = ["docs", "linting"]
 files = [
-    {file = "setuptools-68.2.2-py3-none-any.whl", hash = "sha256:b454a35605876da60632df1a60f736524eb73cc47bbc9f3f1ef1b644de74fd2a"},
-    {file = "setuptools-68.2.2.tar.gz", hash = "sha256:4ac1475276d2f1c48684874089fefcd83bd7162ddaafb81fac866ba0db282a87"},
+    {file = "setuptools-69.5.1-py3-none-any.whl", hash = "sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32"},
+    {file = "setuptools-69.5.1.tar.gz", hash = "sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987"},
 ]
 
 [[package]]
 name = "shibuya"
-version = "2023.9.3"
+version = "2024.4.27"
 requires_python = ">=3.7"
 summary = "A clean, responsive, and customizable Sphinx documentation theme with light/dark mode."
+groups = ["docs"]
 dependencies = [
     "Sphinx",
 ]
 files = [
-    {file = "shibuya-2023.9.3-py3-none-any.whl", hash = "sha256:9e518389e1bf590bfceb588392450c09b80dac29f4f49f171a2bd7284f993429"},
-    {file = "shibuya-2023.9.3.tar.gz", hash = "sha256:9dc2edb13db07d37ad4a774be94aaee68a4a530ce46141daa5f40afcc228b90e"},
+    {file = "shibuya-2024.4.27-py3-none-any.whl", hash = "sha256:b0eaf3ae415eaefb898ca1ad07012c86f6ef12f43aaad73f0d8ef9a13d42bd5e"},
+    {file = "shibuya-2024.4.27.tar.gz", hash = "sha256:6c7c83d49ae3f1d56c0d4c4ccddd31f5dab4aed4e6caf8f397f4de5da5af1911"},
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
+groups = ["default", "docs"]
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
 name = "sniffio"
-version = "1.3.0"
+version = "1.3.1"
 requires_python = ">=3.7"
 summary = "Sniff out which async library your code is running under"
+groups = ["default", "test"]
 files = [
-    {file = "sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
-    {file = "sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
+    {file = "sniffio-1.3.1-py3-none-any.whl", hash = "sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2"},
+    {file = "sniffio-1.3.1.tar.gz", hash = "sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc"},
 ]
 
 [[package]]
 name = "snowballstemmer"
 version = "2.2.0"
 summary = "This package provides 29 stemmers for 28 languages generated from Snowball algorithms."
+groups = ["docs"]
 files = [
     {file = "snowballstemmer-2.2.0-py2.py3-none-any.whl", hash = "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"},
     {file = "snowballstemmer-2.2.0.tar.gz", hash = "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1"},
 ]
 
 [[package]]
 name = "soupsieve"
 version = "2.5"
 requires_python = ">=3.8"
 summary = "A modern CSS selector implementation for Beautiful Soup."
+groups = ["docs"]
 files = [
     {file = "soupsieve-2.5-py3-none-any.whl", hash = "sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7"},
     {file = "soupsieve-2.5.tar.gz", hash = "sha256:5663d5a7b3bfaeee0bc4372e7fc48f9cff4940b3eec54a6451cc5299f1097690"},
 ]
 
 [[package]]
 name = "sphinx"
 version = "7.1.2"
 requires_python = ">=3.8"
 summary = "Python documentation generator"
+groups = ["docs"]
 dependencies = [
     "Jinja2>=3.0",
     "Pygments>=2.13",
     "alabaster<0.8,>=0.7",
     "babel>=2.9",
     "colorama>=0.4.5; sys_platform == \"win32\"",
     "docutils<0.21,>=0.18.1",
@@ -1717,124 +1724,162 @@
 ]
 
 [[package]]
 name = "sphinx-autobuild"
 version = "2021.3.14"
 requires_python = ">=3.6"
 summary = "Rebuild Sphinx documentation on changes, with live-reload in the browser."
+groups = ["docs"]
 dependencies = [
     "colorama",
     "livereload",
     "sphinx",
 ]
 files = [
     {file = "sphinx-autobuild-2021.3.14.tar.gz", hash = "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"},
     {file = "sphinx_autobuild-2021.3.14-py3-none-any.whl", hash = "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac"},
 ]
 
 [[package]]
 name = "sphinx-autodoc-typehints"
-version = "1.24.0"
+version = "2.0.1"
 requires_python = ">=3.8"
 summary = "Type hints (PEP 484) support for the Sphinx autodoc extension"
+groups = ["docs"]
 dependencies = [
-    "sphinx>=7.0.1",
+    "sphinx>=7.1.2",
 ]
 files = [
-    {file = "sphinx_autodoc_typehints-1.24.0-py3-none-any.whl", hash = "sha256:6a73c0c61a9144ce2ed5ef2bed99d615254e5005c1cc32002017d72d69fb70e6"},
-    {file = "sphinx_autodoc_typehints-1.24.0.tar.gz", hash = "sha256:94e440066941bb237704bb880785e2d05e8ae5406c88674feefbb938ad0dc6af"},
+    {file = "sphinx_autodoc_typehints-2.0.1-py3-none-any.whl", hash = "sha256:f73ae89b43a799e587e39266672c1075b2ef783aeb382d3ebed77c38a3fc0149"},
+    {file = "sphinx_autodoc_typehints-2.0.1.tar.gz", hash = "sha256:60ed1e3b2c970acc0aa6e877be42d48029a9faec7378a17838716cacd8c10b12"},
 ]
 
 [[package]]
 name = "sphinx-click"
-version = "5.0.1"
+version = "5.1.0"
 requires_python = ">=3.8"
 summary = "Sphinx extension that automatically documents click applications"
+groups = ["docs"]
 dependencies = [
     "click>=7.0",
     "docutils",
     "sphinx>=2.0",
 ]
 files = [
-    {file = "sphinx-click-5.0.1.tar.gz", hash = "sha256:fcc7df15e56e3ff17ebf446cdd316c2eb79580b37c49579fba11e5468802ef25"},
-    {file = "sphinx_click-5.0.1-py3-none-any.whl", hash = "sha256:31836ca22f746d3c26cbfdfe0c58edf0bca5783731a0b2e25bb6d59800bb75a1"},
+    {file = "sphinx-click-5.1.0.tar.gz", hash = "sha256:6812c2db62d3fae71a4addbe5a8a0a16c97eb491f3cd63fe34b4ed7e07236f33"},
+    {file = "sphinx_click-5.1.0-py3-none-any.whl", hash = "sha256:ae97557a4e9ec646045089326c3b90e026c58a45e083b8f35f17d5d6558d08a0"},
 ]
 
 [[package]]
 name = "sphinx-copybutton"
 version = "0.5.2"
 requires_python = ">=3.7"
 summary = "Add a copy button to each of your code cells."
+groups = ["docs"]
 dependencies = [
     "sphinx>=1.8",
 ]
 files = [
     {file = "sphinx-copybutton-0.5.2.tar.gz", hash = "sha256:4cf17c82fb9646d1bc9ca92ac280813a3b605d8c421225fd9913154103ee1fbd"},
     {file = "sphinx_copybutton-0.5.2-py3-none-any.whl", hash = "sha256:fb543fd386d917746c9a2c50360c7905b605726b9355cd26e9974857afeae06e"},
 ]
 
 [[package]]
 name = "sphinx-design"
 version = "0.5.0"
 requires_python = ">=3.8"
 summary = "A sphinx extension for designing beautiful, view size responsive web components."
+groups = ["docs"]
 dependencies = [
     "sphinx<8,>=5",
 ]
 files = [
     {file = "sphinx_design-0.5.0-py3-none-any.whl", hash = "sha256:1af1267b4cea2eedd6724614f19dcc88fe2e15aff65d06b2f6252cee9c4f4c1e"},
     {file = "sphinx_design-0.5.0.tar.gz", hash = "sha256:e8e513acea6f92d15c6de3b34e954458f245b8e761b45b63950f65373352ab00"},
 ]
 
 [[package]]
 name = "sphinx-jinja2-compat"
-version = "0.2.0"
+version = "0.2.0.post1"
 requires_python = ">=3.6"
 summary = "Patches Jinja2 v3 to restore compatibility with earlier Sphinx versions."
+groups = ["docs"]
 dependencies = [
     "jinja2>=2.10",
     "markupsafe>=1",
 ]
 files = [
-    {file = "sphinx_jinja2_compat-0.2.0-py3-none-any.whl", hash = "sha256:a5f3112d6873991c2cf28e37287163a0485d9c0812863b8aa4df7182722501fb"},
-    {file = "sphinx_jinja2_compat-0.2.0.tar.gz", hash = "sha256:c41346d859653e202b623f4236da8936243ed734abf5984adc3bef59d6f9a946"},
+    {file = "sphinx_jinja2_compat-0.2.0.post1-py3-none-any.whl", hash = "sha256:f9d329174bdde8db19dc12c62528367196eb2f6b46c91754eca604acd0c0f6ad"},
+    {file = "sphinx_jinja2_compat-0.2.0.post1.tar.gz", hash = "sha256:974289a12a9f402108dead621e9c15f7004e945d5cfcaea8d6419e94d3fa95a3"},
+]
+
+[[package]]
+name = "sphinx-paramlinks"
+version = "0.6.0"
+summary = "Allows param links in Sphinx function/method descriptions to be linkable"
+groups = ["docs"]
+dependencies = [
+    "Sphinx>=4.0.0",
+    "docutils",
+]
+files = [
+    {file = "sphinx-paramlinks-0.6.0.tar.gz", hash = "sha256:746a0816860aa3fff5d8d746efcbec4deead421f152687411db1d613d29f915e"},
 ]
 
 [[package]]
 name = "sphinx-prompt"
 version = "1.5.0"
 summary = "Sphinx directive to add unselectable prompt"
+groups = ["docs"]
 dependencies = [
     "Sphinx",
     "pygments",
 ]
 files = [
     {file = "sphinx_prompt-1.5.0-py3-none-any.whl", hash = "sha256:fa4e90d8088b5a996c76087d701fc7e31175f8b9dc4aab03a507e45051067162"},
 ]
 
 [[package]]
 name = "sphinx-tabs"
-version = "3.4.1"
+version = "3.4.5"
 requires_python = "~=3.7"
 summary = "Tabbed views for Sphinx"
+groups = ["docs"]
 dependencies = [
-    "docutils~=0.18.0",
+    "docutils",
     "pygments",
     "sphinx",
 ]
 files = [
-    {file = "sphinx-tabs-3.4.1.tar.gz", hash = "sha256:d2a09f9e8316e400d57503f6df1c78005fdde220e5af589cc79d493159e1b832"},
-    {file = "sphinx_tabs-3.4.1-py3-none-any.whl", hash = "sha256:7cea8942aeccc5d01a995789c01804b787334b55927f29b36ba16ed1e7cb27c6"},
+    {file = "sphinx-tabs-3.4.5.tar.gz", hash = "sha256:ba9d0c1e3e37aaadd4b5678449eb08176770e0fc227e769b6ce747df3ceea531"},
+    {file = "sphinx_tabs-3.4.5-py3-none-any.whl", hash = "sha256:92cc9473e2ecf1828ca3f6617d0efc0aa8acb06b08c56ba29d1413f2f0f6cf09"},
+]
+
+[[package]]
+name = "sphinx-togglebutton"
+version = "0.3.2"
+summary = "Toggle page content and collapse admonitions in Sphinx."
+groups = ["docs"]
+dependencies = [
+    "docutils",
+    "setuptools",
+    "sphinx",
+    "wheel",
+]
+files = [
+    {file = "sphinx-togglebutton-0.3.2.tar.gz", hash = "sha256:ab0c8b366427b01e4c89802d5d078472c427fa6e9d12d521c34fa0442559dc7a"},
+    {file = "sphinx_togglebutton-0.3.2-py3-none-any.whl", hash = "sha256:9647ba7874b7d1e2d43413d8497153a85edc6ac95a3fea9a75ef9c1e08aaae2b"},
 ]
 
 [[package]]
 name = "sphinx-toolbox"
 version = "3.5.0"
 requires_python = ">=3.7"
 summary = "Box of handy tools for Sphinx 🧰 📔"
+groups = ["docs"]
 dependencies = [
     "apeye>=0.4.0",
     "autodocsumm>=0.2.0",
     "beautifulsoup4>=4.9.1",
     "cachecontrol[filecache]>=0.13.0",
     "dict2css>=0.2.3",
     "docutils>=0.16",
@@ -1856,447 +1901,203 @@
 ]
 
 [[package]]
 name = "sphinxcontrib-applehelp"
 version = "1.0.4"
 requires_python = ">=3.8"
 summary = "sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books"
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-applehelp-1.0.4.tar.gz", hash = "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"},
     {file = "sphinxcontrib_applehelp-1.0.4-py3-none-any.whl", hash = "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228"},
 ]
 
 [[package]]
 name = "sphinxcontrib-devhelp"
 version = "1.0.2"
 requires_python = ">=3.5"
 summary = "sphinxcontrib-devhelp is a sphinx extension which outputs Devhelp document."
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-devhelp-1.0.2.tar.gz", hash = "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"},
     {file = "sphinxcontrib_devhelp-1.0.2-py2.py3-none-any.whl", hash = "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e"},
 ]
 
 [[package]]
 name = "sphinxcontrib-htmlhelp"
 version = "2.0.1"
 requires_python = ">=3.8"
 summary = "sphinxcontrib-htmlhelp is a sphinx extension which renders HTML help files"
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-htmlhelp-2.0.1.tar.gz", hash = "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff"},
     {file = "sphinxcontrib_htmlhelp-2.0.1-py3-none-any.whl", hash = "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"},
 ]
 
 [[package]]
 name = "sphinxcontrib-jsmath"
 version = "1.0.1"
 requires_python = ">=3.5"
 summary = "A sphinx extension which renders display math in HTML via JavaScript"
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-jsmath-1.0.1.tar.gz", hash = "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"},
     {file = "sphinxcontrib_jsmath-1.0.1-py2.py3-none-any.whl", hash = "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178"},
 ]
 
 [[package]]
 name = "sphinxcontrib-qthelp"
 version = "1.0.3"
 requires_python = ">=3.5"
 summary = "sphinxcontrib-qthelp is a sphinx extension which outputs QtHelp document."
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-qthelp-1.0.3.tar.gz", hash = "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72"},
     {file = "sphinxcontrib_qthelp-1.0.3-py2.py3-none-any.whl", hash = "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"},
 ]
 
 [[package]]
 name = "sphinxcontrib-serializinghtml"
 version = "1.1.5"
 requires_python = ">=3.5"
 summary = "sphinxcontrib-serializinghtml is a sphinx extension which outputs \"serialized\" HTML files (json and pickle)."
+groups = ["docs"]
 files = [
     {file = "sphinxcontrib-serializinghtml-1.1.5.tar.gz", hash = "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"},
     {file = "sphinxcontrib_serializinghtml-1.1.5-py2.py3-none-any.whl", hash = "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd"},
 ]
 
 [[package]]
-name = "sqlalchemy"
-version = "2.0.21"
-requires_python = ">=3.7"
-summary = "Database Abstraction Library"
-dependencies = [
-    "greenlet!=0.4.17; platform_machine == \"aarch64\" or (platform_machine == \"ppc64le\" or (platform_machine == \"x86_64\" or (platform_machine == \"amd64\" or (platform_machine == \"AMD64\" or (platform_machine == \"win32\" or platform_machine == \"WIN32\")))))",
-    "typing-extensions>=4.2.0",
-]
-files = [
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1e7dc99b23e33c71d720c4ae37ebb095bebebbd31a24b7d99dfc4753d2803ede"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:7f0c4ee579acfe6c994637527c386d1c22eb60bc1c1d36d940d8477e482095d4"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3f7d57a7e140efe69ce2d7b057c3f9a595f98d0bbdfc23fd055efdfbaa46e3a5"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7ca38746eac23dd7c20bec9278d2058c7ad662b2f1576e4c3dbfcd7c00cc48fa"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:3cf229704074bce31f7f47d12883afee3b0a02bb233a0ba45ddbfe542939cca4"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:fb87f763b5d04a82ae84ccff25554ffd903baafba6698e18ebaf32561f2fe4aa"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-win32.whl", hash = "sha256:89e274604abb1a7fd5c14867a412c9d49c08ccf6ce3e1e04fffc068b5b6499d4"},
-    {file = "SQLAlchemy-2.0.21-cp310-cp310-win_amd64.whl", hash = "sha256:e36339a68126ffb708dc6d1948161cea2a9e85d7d7b0c54f6999853d70d44430"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:bf8eebccc66829010f06fbd2b80095d7872991bfe8415098b9fe47deaaa58063"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b977bfce15afa53d9cf6a632482d7968477625f030d86a109f7bdfe8ce3c064a"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6ff3dc2f60dbf82c9e599c2915db1526d65415be323464f84de8db3e361ba5b9"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:44ac5c89b6896f4740e7091f4a0ff2e62881da80c239dd9408f84f75a293dae9"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:87bf91ebf15258c4701d71dcdd9c4ba39521fb6a37379ea68088ce8cd869b446"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:b69f1f754d92eb1cc6b50938359dead36b96a1dcf11a8670bff65fd9b21a4b09"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-win32.whl", hash = "sha256:af520a730d523eab77d754f5cf44cc7dd7ad2d54907adeb3233177eeb22f271b"},
-    {file = "SQLAlchemy-2.0.21-cp311-cp311-win_amd64.whl", hash = "sha256:141675dae56522126986fa4ca713739d00ed3a6f08f3c2eb92c39c6dfec463ce"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b4eae01faee9f2b17f08885e3f047153ae0416648f8e8c8bd9bc677c5ce64be9"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:3eb7c03fe1cd3255811cd4e74db1ab8dca22074d50cd8937edf4ef62d758cdf4"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c2d494b6a2a2d05fb99f01b84cc9af9f5f93bf3e1e5dbdafe4bed0c2823584c1"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b19ae41ef26c01a987e49e37c77b9ad060c59f94d3b3efdfdbf4f3daaca7b5fe"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:fc6b15465fabccc94bf7e38777d665b6a4f95efd1725049d6184b3a39fd54880"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:014794b60d2021cc8ae0f91d4d0331fe92691ae5467a00841f7130fe877b678e"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-win32.whl", hash = "sha256:0268256a34806e5d1c8f7ee93277d7ea8cc8ae391f487213139018b6805aeaf6"},
-    {file = "SQLAlchemy-2.0.21-cp38-cp38-win_amd64.whl", hash = "sha256:73c079e21d10ff2be54a4699f55865d4b275fd6c8bd5d90c5b1ef78ae0197301"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:785e2f2c1cb50d0a44e2cdeea5fd36b5bf2d79c481c10f3a88a8be4cfa2c4615"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:c111cd40910ffcb615b33605fc8f8e22146aeb7933d06569ac90f219818345ef"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c9cba4e7369de663611ce7460a34be48e999e0bbb1feb9130070f0685e9a6b66"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50a69067af86ec7f11a8e50ba85544657b1477aabf64fa447fd3736b5a0a4f67"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ccb99c3138c9bde118b51a289d90096a3791658da9aea1754667302ed6564f6e"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:513fd5b6513d37e985eb5b7ed89da5fd9e72354e3523980ef00d439bc549c9e9"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-win32.whl", hash = "sha256:f9fefd6298433b6e9188252f3bff53b9ff0443c8fde27298b8a2b19f6617eeb9"},
-    {file = "SQLAlchemy-2.0.21-cp39-cp39-win_amd64.whl", hash = "sha256:2e617727fe4091cedb3e4409b39368f424934c7faa78171749f704b49b4bb4ce"},
-    {file = "SQLAlchemy-2.0.21-py3-none-any.whl", hash = "sha256:ea7da25ee458d8f404b93eb073116156fd7d8c2a776d8311534851f28277b4ce"},
-    {file = "SQLAlchemy-2.0.21.tar.gz", hash = "sha256:05b971ab1ac2994a14c56b35eaaa91f86ba080e9ad481b20d99d77f381bb6258"},
-]
-
-[[package]]
 name = "tabulate"
 version = "0.9.0"
 requires_python = ">=3.7"
 summary = "Pretty-print tabular data"
+groups = ["docs"]
 files = [
     {file = "tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
     {file = "tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
 ]
 
 [[package]]
-name = "time-machine"
-version = "2.13.0"
+name = "termcolor"
+version = "2.4.0"
 requires_python = ">=3.8"
-summary = "Travel through time in your tests."
-dependencies = [
-    "python-dateutil",
-]
+summary = "ANSI color formatting for output in terminal"
+groups = ["test"]
 files = [
-    {file = "time_machine-2.13.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:685d98593f13649ad5e7ce3e58efe689feca1badcf618ba397d3ab877ee59326"},
-    {file = "time_machine-2.13.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:ccbce292380ebf63fb9a52e6b03d91677f6a003e0c11f77473efe3913a75f289"},
-    {file = "time_machine-2.13.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:679cbf9b15bfde1654cf48124128d3fbe52f821fa158a98fcee5fe7e05db1917"},
-    {file = "time_machine-2.13.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a26bdf3462d5f12a4c1009fdbe54366c6ef22c7b6f6808705b51dedaaeba8296"},
-    {file = "time_machine-2.13.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dabb3b155819811b4602f7e9be936e2024e20dc99a90f103e36b45768badf9c3"},
-    {file = "time_machine-2.13.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:0db97f92be3efe0ac62fd3f933c91a78438cef13f283b6dfc2ee11123bfd7d8a"},
-    {file = "time_machine-2.13.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:12eed2e9171c85b703d75c985dab2ecad4fe7025b7d2f842596fce1576238ece"},
-    {file = "time_machine-2.13.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:bdfe4a7f033e6783c3e9a7f8d8fc0b115367330762e00a03ff35fedf663994f3"},
-    {file = "time_machine-2.13.0-cp310-cp310-win32.whl", hash = "sha256:3a7a0a49ce50d9c306c4343a7d6a3baa11092d4399a4af4355c615ccc321a9d3"},
-    {file = "time_machine-2.13.0-cp310-cp310-win_amd64.whl", hash = "sha256:1812e48c6c58707db9988445a219a908a710ea065b2cc808d9a50636291f27d4"},
-    {file = "time_machine-2.13.0-cp310-cp310-win_arm64.whl", hash = "sha256:5aee23cd046abf9caeddc982113e81ba9097a01f3972e9560f5ed64e3495f66d"},
-    {file = "time_machine-2.13.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e9a9d150e098be3daee5c9f10859ab1bd14a61abebaed86e6d71f7f18c05b9d7"},
-    {file = "time_machine-2.13.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:2bd4169b808745d219a69094b3cb86006938d45e7293249694e6b7366225a186"},
-    {file = "time_machine-2.13.0-cp311-cp311-macosx_13_0_arm64.whl", hash = "sha256:8d526cdcaca06a496877cfe61cc6608df2c3a6fce210e076761964ebac7f77cc"},
-    {file = "time_machine-2.13.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cfef4ebfb4f055ce3ebc7b6c1c4d0dbfcffdca0e783ad8c6986c992915a57ed3"},
-    {file = "time_machine-2.13.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9f128db8997c3339f04f7f3946dd9bb2a83d15e0a40d35529774da1e9e501511"},
-    {file = "time_machine-2.13.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21bef5854d49b62e2c33848b5c3e8acf22a3b46af803ef6ff19529949cb7cf9f"},
-    {file = "time_machine-2.13.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:32b71e50b07f86916ac04bd1eefc2bd2c93706b81393748b08394509ee6585dc"},
-    {file = "time_machine-2.13.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:1ac8ff145c63cd0dcfd9590fe694b5269aacbc130298dc7209b095d101f8cdde"},
-    {file = "time_machine-2.13.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:19a3b10161c91ca8e0fd79348665cca711fd2eac6ce336ff9e6b447783817f93"},
-    {file = "time_machine-2.13.0-cp311-cp311-win32.whl", hash = "sha256:5f87787d562e42bf1006a87eb689814105b98c4d5545874a281280d0f8b9a2d9"},
-    {file = "time_machine-2.13.0-cp311-cp311-win_amd64.whl", hash = "sha256:62fd14a80b8b71726e07018628daaee0a2e00937625083f96f69ed6b8e3304c0"},
-    {file = "time_machine-2.13.0-cp311-cp311-win_arm64.whl", hash = "sha256:e9935aff447f5400a2665ab10ed2da972591713080e1befe1bb8954e7c0c7806"},
-    {file = "time_machine-2.13.0-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:34dcdbbd25c1e124e17fe58050452960fd16a11f9d3476aaa87260e28ecca0fd"},
-    {file = "time_machine-2.13.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:e58d82fe0e59d6e096ada3281d647a2e7420f7da5453b433b43880e1c2e8e0c5"},
-    {file = "time_machine-2.13.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:71acbc1febbe87532c7355eca3308c073d6e502ee4ce272b5028967847c8e063"},
-    {file = "time_machine-2.13.0-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:dec0ec2135a4e2a59623e40c31d6e8a8ae73305ade2634380e4263d815855750"},
-    {file = "time_machine-2.13.0-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4e3a2611f8788608ebbcb060a5e36b45911bc3b8adc421b1dc29d2c81786ce4d"},
-    {file = "time_machine-2.13.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:42ef5349135626ad6cd889a0a81400137e5c6928502b0817ea9e90bb10702000"},
-    {file = "time_machine-2.13.0-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:6c16d90a597a8c2d3ce22d6be2eb3e3f14786974c11b01886e51b3cf0d5edaf7"},
-    {file = "time_machine-2.13.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4f2ae8d0e359b216b695f1e7e7256f208c390db0480601a439c5dd1e1e4e16ce"},
-    {file = "time_machine-2.13.0-cp312-cp312-win32.whl", hash = "sha256:f5fa9610f7e73fff42806a2ed8b06d862aa59ce4d178a52181771d6939c3e237"},
-    {file = "time_machine-2.13.0-cp312-cp312-win_amd64.whl", hash = "sha256:02b33a8c19768c94f7ffd6aa6f9f64818e88afce23250016b28583929d20fb12"},
-    {file = "time_machine-2.13.0-cp312-cp312-win_arm64.whl", hash = "sha256:0cc116056a8a2a917a4eec85661dfadd411e0d8faae604ef6a0e19fe5cd57ef1"},
-    {file = "time_machine-2.13.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:de01f33aa53da37530ad97dcd17e9affa25a8df4ab822506bb08101bab0c2673"},
-    {file = "time_machine-2.13.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:67fa45cd813821e4f5bec0ac0820869e8e37430b15509d3f5fad74ba34b53852"},
-    {file = "time_machine-2.13.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d4a2d3db2c3b8e519d5ef436cd405abd33542a7b7761fb05ef5a5f782a8ce0b1"},
-    {file = "time_machine-2.13.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7558622a62243be866a7e7c41da48eacd82c874b015ecf67d18ebf65ca3f7436"},
-    {file = "time_machine-2.13.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ab04cf4e56e1ee65bee2adaa26a04695e92eb1ed1ccc65fbdafd0d114399595a"},
-    {file = "time_machine-2.13.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:b0c8f24ae611a58782773af34dd356f1f26756272c04be2be7ea73b47e5da37d"},
-    {file = "time_machine-2.13.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4ca20f85a973a4ca8b00cf466cd72c27ccc72372549b138fd48d7e70e5a190ab"},
-    {file = "time_machine-2.13.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:9fad549521c4c13bdb1e889b2855a86ec835780d534ffd8f091c2647863243be"},
-    {file = "time_machine-2.13.0-cp38-cp38-win32.whl", hash = "sha256:20205422fcf2caf9a7488394587df86e5b54fdb315c1152094fbb63eec4e9304"},
-    {file = "time_machine-2.13.0-cp38-cp38-win_amd64.whl", hash = "sha256:2dc76ee55a7d915a55960a726ceaca7b9097f67e4b4e681ef89871bcf98f00be"},
-    {file = "time_machine-2.13.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:7693704c0f2f6b9beed912ff609781edf5fcf5d63aff30c92be4093e09d94b8e"},
-    {file = "time_machine-2.13.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:918f8389de29b4f41317d121f1150176fae2cdb5fa41f68b2aee0b9dc88df5c3"},
-    {file = "time_machine-2.13.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5fe3fda5fa73fec74278912e438fce1612a79c36fd0cc323ea3dc2d5ce629f31"},
-    {file = "time_machine-2.13.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5c6245db573863b335d9ca64b3230f623caf0988594ae554c0c794e7f80e3e66"},
-    {file = "time_machine-2.13.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e433827eccd6700a34a2ab28fd9361ff6e4d4923f718d2d1dac6d1dcd9d54da6"},
-    {file = "time_machine-2.13.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:924377d398b1c48e519ad86a71903f9f36117f69e68242c99fb762a2465f5ad2"},
-    {file = "time_machine-2.13.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:66fb3877014dca0b9286b0f06fa74062357bd23f2d9d102d10e31e0f8fa9b324"},
-    {file = "time_machine-2.13.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0c9829b2edfcf6b5d72a6ff330d4380f36a937088314c675531b43d3423dd8af"},
-    {file = "time_machine-2.13.0-cp39-cp39-win32.whl", hash = "sha256:1a22be4df364f49a507af4ac9ea38108a0105f39da3f9c60dce62d6c6ea4ccdc"},
-    {file = "time_machine-2.13.0-cp39-cp39-win_amd64.whl", hash = "sha256:88601de1da06c7cab3d5ed3d5c3801ef683366e769e829e96383fdab6ae2fe42"},
-    {file = "time_machine-2.13.0-cp39-cp39-win_arm64.whl", hash = "sha256:3c87856105dcb25b5bbff031d99f06ef4d1c8380d096222e1bc63b496b5258e6"},
-    {file = "time_machine-2.13.0.tar.gz", hash = "sha256:c23b2408e3adcedec84ea1131e238f0124a5bc0e491f60d1137ad7239b37c01a"},
+    {file = "termcolor-2.4.0-py3-none-any.whl", hash = "sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63"},
+    {file = "termcolor-2.4.0.tar.gz", hash = "sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a"},
 ]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
+groups = ["docs", "linting", "test"]
+marker = "python_version < \"3.11\""
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tornado"
-version = "6.3.3"
+version = "6.4"
 requires_python = ">= 3.8"
 summary = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
+groups = ["docs"]
+marker = "python_version > \"2.7\""
 files = [
-    {file = "tornado-6.3.3-cp38-abi3-macosx_10_9_universal2.whl", hash = "sha256:502fba735c84450974fec147340016ad928d29f1e91f49be168c0a4c18181e1d"},
-    {file = "tornado-6.3.3-cp38-abi3-macosx_10_9_x86_64.whl", hash = "sha256:805d507b1f588320c26f7f097108eb4023bbaa984d63176d1652e184ba24270a"},
-    {file = "tornado-6.3.3-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1bd19ca6c16882e4d37368e0152f99c099bad93e0950ce55e71daed74045908f"},
-    {file = "tornado-6.3.3-cp38-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7ac51f42808cca9b3613f51ffe2a965c8525cb1b00b7b2d56828b8045354f76a"},
-    {file = "tornado-6.3.3-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:71a8db65160a3c55d61839b7302a9a400074c9c753040455494e2af74e2501f2"},
-    {file = "tornado-6.3.3-cp38-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:ceb917a50cd35882b57600709dd5421a418c29ddc852da8bcdab1f0db33406b0"},
-    {file = "tornado-6.3.3-cp38-abi3-musllinux_1_1_i686.whl", hash = "sha256:7d01abc57ea0dbb51ddfed477dfe22719d376119844e33c661d873bf9c0e4a16"},
-    {file = "tornado-6.3.3-cp38-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:9dc4444c0defcd3929d5c1eb5706cbe1b116e762ff3e0deca8b715d14bf6ec17"},
-    {file = "tornado-6.3.3-cp38-abi3-win32.whl", hash = "sha256:65ceca9500383fbdf33a98c0087cb975b2ef3bfb874cb35b8de8740cf7f41bd3"},
-    {file = "tornado-6.3.3-cp38-abi3-win_amd64.whl", hash = "sha256:22d3c2fa10b5793da13c807e6fc38ff49a4f6e1e3868b0a6f4164768bb8e20f5"},
-    {file = "tornado-6.3.3.tar.gz", hash = "sha256:e7d8db41c0181c80d76c982aacc442c0783a2c54d6400fe028954201a2e032fe"},
+    {file = "tornado-6.4-cp38-abi3-macosx_10_9_universal2.whl", hash = "sha256:02ccefc7d8211e5a7f9e8bc3f9e5b0ad6262ba2fbb683a6443ecc804e5224ce0"},
+    {file = "tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl", hash = "sha256:27787de946a9cffd63ce5814c33f734c627a87072ec7eed71f7fc4417bb16263"},
+    {file = "tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f7894c581ecdcf91666a0912f18ce5e757213999e183ebfc2c3fdbf4d5bd764e"},
+    {file = "tornado-6.4-cp38-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e43bc2e5370a6a8e413e1e1cd0c91bedc5bd62a74a532371042a18ef19e10579"},
+    {file = "tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212"},
+    {file = "tornado-6.4-cp38-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:fd03192e287fbd0899dd8f81c6fb9cbbc69194d2074b38f384cb6fa72b80e9c2"},
+    {file = "tornado-6.4-cp38-abi3-musllinux_1_1_i686.whl", hash = "sha256:88b84956273fbd73420e6d4b8d5ccbe913c65d31351b4c004ae362eba06e1f78"},
+    {file = "tornado-6.4-cp38-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:71ddfc23a0e03ef2df1c1397d859868d158c8276a0603b96cf86892bff58149f"},
+    {file = "tornado-6.4-cp38-abi3-win32.whl", hash = "sha256:6f8a6c77900f5ae93d8b4ae1196472d0ccc2775cc1dfdc9e7727889145c45052"},
+    {file = "tornado-6.4-cp38-abi3-win_amd64.whl", hash = "sha256:10aeaa8006333433da48dec9fe417877f8bcc21f48dda8d661ae79da357b2a63"},
+    {file = "tornado-6.4.tar.gz", hash = "sha256:72291fa6e6bc84e626589f1c29d90a5a6d593ef5ae68052ee2ef000dfd273dee"},
 ]
 
 [[package]]
-name = "types-docutils"
-version = "0.20.0.3"
-summary = "Typing stubs for docutils"
+name = "types-click"
+version = "7.1.8"
+summary = "Typing stubs for click"
+groups = ["linting"]
 files = [
-    {file = "types-docutils-0.20.0.3.tar.gz", hash = "sha256:4928e790f42b99d5833990f99c8dd9fa9f16825f6ed30380ca981846d36870cd"},
-    {file = "types_docutils-0.20.0.3-py3-none-any.whl", hash = "sha256:a930150d8e01a9170f9bca489f46808ddebccdd8bc1e47c07968a77e49fb9321"},
+    {file = "types-click-7.1.8.tar.gz", hash = "sha256:b6604968be6401dc516311ca50708a0a28baa7a0cb840efd7412f0dbbff4e092"},
+    {file = "types_click-7.1.8-py3-none-any.whl", hash = "sha256:8cb030a669e2e927461be9827375f83c16b8178c365852c060a34e24871e7e81"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.8.0"
+version = "4.11.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
+groups = ["default", "docs", "linting", "test"]
 files = [
-    {file = "typing_extensions-4.8.0-py3-none-any.whl", hash = "sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0"},
-    {file = "typing_extensions-4.8.0.tar.gz", hash = "sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "urllib3"
-version = "2.0.5"
-requires_python = ">=3.7"
-summary = "HTTP library with thread-safe connection pooling, file post, and more."
-files = [
-    {file = "urllib3-2.0.5-py3-none-any.whl", hash = "sha256:ef16afa8ba34a1f989db38e1dbbe0c302e4289a47856990d0682e374563ce35e"},
-    {file = "urllib3-2.0.5.tar.gz", hash = "sha256:13abf37382ea2ce6fb744d4dad67838eec857c9f4f57009891805e0b5e123594"},
-]
-
-[[package]]
-name = "uvicorn"
-version = "0.23.2"
+version = "2.2.1"
 requires_python = ">=3.8"
-summary = "The lightning-fast ASGI server."
-dependencies = [
-    "click>=7.0",
-    "h11>=0.8",
-    "typing-extensions>=4.0; python_version < \"3.11\"",
-]
+summary = "HTTP library with thread-safe connection pooling, file post, and more."
+groups = ["docs"]
 files = [
-    {file = "uvicorn-0.23.2-py3-none-any.whl", hash = "sha256:1f9be6558f01239d4fdf22ef8126c39cb1ad0addf76c40e760549d2c2f43ab53"},
-    {file = "uvicorn-0.23.2.tar.gz", hash = "sha256:4d3cc12d7727ba72b64d12d3cc7743124074c0a69f7b201512fc50c3e3f1569a"},
-]
-
-[[package]]
-name = "uvicorn"
-version = "0.23.2"
-extras = ["standard"]
-requires_python = ">=3.8"
-summary = "The lightning-fast ASGI server."
-dependencies = [
-    "colorama>=0.4; sys_platform == \"win32\"",
-    "httptools>=0.5.0",
-    "python-dotenv>=0.13",
-    "pyyaml>=5.1",
-    "uvicorn==0.23.2",
-    "uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != \"win32\" and (sys_platform != \"cygwin\" and platform_python_implementation != \"PyPy\")",
-    "watchfiles>=0.13",
-    "websockets>=10.4",
-]
-files = [
-    {file = "uvicorn-0.23.2-py3-none-any.whl", hash = "sha256:1f9be6558f01239d4fdf22ef8126c39cb1ad0addf76c40e760549d2c2f43ab53"},
-    {file = "uvicorn-0.23.2.tar.gz", hash = "sha256:4d3cc12d7727ba72b64d12d3cc7743124074c0a69f7b201512fc50c3e3f1569a"},
-]
-
-[[package]]
-name = "uvloop"
-version = "0.17.0"
-requires_python = ">=3.7"
-summary = "Fast implementation of asyncio event loop on top of libuv"
-files = [
-    {file = "uvloop-0.17.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:ce9f61938d7155f79d3cb2ffa663147d4a76d16e08f65e2c66b77bd41b356718"},
-    {file = "uvloop-0.17.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:68532f4349fd3900b839f588972b3392ee56042e440dd5873dfbbcd2cc67617c"},
-    {file = "uvloop-0.17.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0949caf774b9fcefc7c5756bacbbbd3fc4c05a6b7eebc7c7ad6f825b23998d6d"},
-    {file = "uvloop-0.17.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ff3d00b70ce95adce264462c930fbaecb29718ba6563db354608f37e49e09024"},
-    {file = "uvloop-0.17.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:a5abddb3558d3f0a78949c750644a67be31e47936042d4f6c888dd6f3c95f4aa"},
-    {file = "uvloop-0.17.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8efcadc5a0003d3a6e887ccc1fb44dec25594f117a94e3127954c05cf144d811"},
-    {file = "uvloop-0.17.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:3378eb62c63bf336ae2070599e49089005771cc651c8769aaad72d1bd9385a7c"},
-    {file = "uvloop-0.17.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6aafa5a78b9e62493539456f8b646f85abc7093dd997f4976bb105537cf2635e"},
-    {file = "uvloop-0.17.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c686a47d57ca910a2572fddfe9912819880b8765e2f01dc0dd12a9bf8573e539"},
-    {file = "uvloop-0.17.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:864e1197139d651a76c81757db5eb199db8866e13acb0dfe96e6fc5d1cf45fc4"},
-    {file = "uvloop-0.17.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:2a6149e1defac0faf505406259561bc14b034cdf1d4711a3ddcdfbaa8d825a05"},
-    {file = "uvloop-0.17.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6708f30db9117f115eadc4f125c2a10c1a50d711461699a0cbfaa45b9a78e376"},
-    {file = "uvloop-0.17.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:a4aee22ece20958888eedbad20e4dbb03c37533e010fb824161b4f05e641f738"},
-    {file = "uvloop-0.17.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:307958f9fc5c8bb01fad752d1345168c0abc5d62c1b72a4a8c6c06f042b45b20"},
-    {file = "uvloop-0.17.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3ebeeec6a6641d0adb2ea71dcfb76017602ee2bfd8213e3fcc18d8f699c5104f"},
-    {file = "uvloop-0.17.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1436c8673c1563422213ac6907789ecb2b070f5939b9cbff9ef7113f2b531595"},
-    {file = "uvloop-0.17.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:8887d675a64cfc59f4ecd34382e5b4f0ef4ae1da37ed665adba0c2badf0d6578"},
-    {file = "uvloop-0.17.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:3db8de10ed684995a7f34a001f15b374c230f7655ae840964d51496e2f8a8474"},
-    {file = "uvloop-0.17.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:7d37dccc7ae63e61f7b96ee2e19c40f153ba6ce730d8ba4d3b4e9738c1dccc1b"},
-    {file = "uvloop-0.17.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:cbbe908fda687e39afd6ea2a2f14c2c3e43f2ca88e3a11964b297822358d0e6c"},
-    {file = "uvloop-0.17.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3d97672dc709fa4447ab83276f344a165075fd9f366a97b712bdd3fee05efae8"},
-    {file = "uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f1e507c9ee39c61bfddd79714e4f85900656db1aec4d40c6de55648e85c2799c"},
-    {file = "uvloop-0.17.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c092a2c1e736086d59ac8e41f9c98f26bbf9b9222a76f21af9dfe949b99b2eb9"},
-    {file = "uvloop-0.17.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:30babd84706115626ea78ea5dbc7dd8d0d01a2e9f9b306d24ca4ed5796c66ded"},
-    {file = "uvloop-0.17.0.tar.gz", hash = "sha256:0ddf6baf9cf11a1a22c71487f39f15b2cf78eb5bde7e5b45fbb99e8a9d91b9e1"},
+    {file = "urllib3-2.2.1-py3-none-any.whl", hash = "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d"},
+    {file = "urllib3-2.2.1.tar.gz", hash = "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.24.5"
+version = "20.26.1"
 requires_python = ">=3.7"
 summary = "Virtual Python Environment builder"
+groups = ["linting"]
 dependencies = [
     "distlib<1,>=0.3.7",
     "filelock<4,>=3.12.2",
-    "platformdirs<4,>=3.9.1",
+    "platformdirs<5,>=3.9.1",
 ]
 files = [
-    {file = "virtualenv-20.24.5-py3-none-any.whl", hash = "sha256:b80039f280f4919c77b30f1c23294ae357c4c8701042086e3fc005963e4e537b"},
-    {file = "virtualenv-20.24.5.tar.gz", hash = "sha256:e8361967f6da6fbdf1426483bfe9fca8287c242ac0bc30429905721cefbff752"},
-]
-
-[[package]]
-name = "watchfiles"
-version = "0.20.0"
-requires_python = ">=3.7"
-summary = "Simple, modern and high performance file watching and code reload in python."
-dependencies = [
-    "anyio>=3.0.0",
-]
-files = [
-    {file = "watchfiles-0.20.0-cp37-abi3-macosx_10_7_x86_64.whl", hash = "sha256:3796312bd3587e14926013612b23066912cf45a14af71cf2b20db1c12dadf4e9"},
-    {file = "watchfiles-0.20.0-cp37-abi3-macosx_11_0_arm64.whl", hash = "sha256:d0002d81c89a662b595645fb684a371b98ff90a9c7d8f8630c82f0fde8310458"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:570848706440373b4cd8017f3e850ae17f76dbdf1e9045fc79023b11e1afe490"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9a0351d20d03c6f7ad6b2e8a226a5efafb924c7755ee1e34f04c77c3682417fa"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:007dcc4a401093010b389c044e81172c8a2520dba257c88f8828b3d460c6bb38"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0d82dbc1832da83e441d112069833eedd4cf583d983fb8dd666fbefbea9d99c0"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:99f4c65fd2fce61a571b2a6fcf747d6868db0bef8a934e8ca235cc8533944d95"},
-    {file = "watchfiles-0.20.0-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5392dd327a05f538c56edb1c6ebba6af91afc81b40822452342f6da54907bbdf"},
-    {file = "watchfiles-0.20.0-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:08dc702529bb06a2b23859110c214db245455532da5eaea602921687cfcd23db"},
-    {file = "watchfiles-0.20.0-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:7d4e66a857621584869cfbad87039e65dadd7119f0d9bb9dbc957e089e32c164"},
-    {file = "watchfiles-0.20.0-cp37-abi3-win32.whl", hash = "sha256:a03d1e6feb7966b417f43c3e3783188167fd69c2063e86bad31e62c4ea794cc5"},
-    {file = "watchfiles-0.20.0-cp37-abi3-win_amd64.whl", hash = "sha256:eccc8942bcdc7d638a01435d915b913255bbd66f018f1af051cd8afddb339ea3"},
-    {file = "watchfiles-0.20.0-cp37-abi3-win_arm64.whl", hash = "sha256:b17d4176c49d207865630da5b59a91779468dd3e08692fe943064da260de2c7c"},
-    {file = "watchfiles-0.20.0-pp38-pypy38_pp73-macosx_10_7_x86_64.whl", hash = "sha256:d97db179f7566dcf145c5179ddb2ae2a4450e3a634eb864b09ea04e68c252e8e"},
-    {file = "watchfiles-0.20.0-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:835df2da7a5df5464c4a23b2d963e1a9d35afa422c83bf4ff4380b3114603644"},
-    {file = "watchfiles-0.20.0-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:608cd94a8767f49521901aff9ae0c92cc8f5a24d528db7d6b0295290f9d41193"},
-    {file = "watchfiles-0.20.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:89d1de8218874925bce7bb2ae9657efc504411528930d7a83f98b1749864f2ef"},
-    {file = "watchfiles-0.20.0-pp39-pypy39_pp73-macosx_10_7_x86_64.whl", hash = "sha256:13f995d5152a8ba4ed7c2bbbaeee4e11a5944defc7cacd0ccb4dcbdcfd78029a"},
-    {file = "watchfiles-0.20.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:9b5c8d3be7b502f8c43a33c63166ada8828dbb0c6d49c8f9ce990a96de2f5a49"},
-    {file = "watchfiles-0.20.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e43af4464daa08723c04b43cf978ab86cc55c684c16172622bdac64b34e36af0"},
-    {file = "watchfiles-0.20.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:87d9e1f75c4f86c93d73b5bd1ebe667558357548f11b4f8af4e0e272f79413ce"},
-    {file = "watchfiles-0.20.0.tar.gz", hash = "sha256:728575b6b94c90dd531514677201e8851708e6e4b5fe7028ac506a200b622019"},
+    {file = "virtualenv-20.26.1-py3-none-any.whl", hash = "sha256:7aa9982a728ae5892558bff6a2839c00b9ed145523ece2274fad6f414690ae75"},
+    {file = "virtualenv-20.26.1.tar.gz", hash = "sha256:604bfdceaeece392802e6ae48e69cec49168b9c5f4a44e483963f9242eb0e78b"},
 ]
 
 [[package]]
 name = "webencodings"
 version = "0.5.1"
 summary = "Character encoding aliases for legacy web content"
+groups = ["docs"]
 files = [
     {file = "webencodings-0.5.1-py2.py3-none-any.whl", hash = "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78"},
     {file = "webencodings-0.5.1.tar.gz", hash = "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"},
 ]
 
 [[package]]
-name = "websockets"
-version = "11.0.3"
-requires_python = ">=3.7"
-summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
+name = "wheel"
+version = "0.43.0"
+requires_python = ">=3.8"
+summary = "A built-package format for Python"
+groups = ["docs"]
 files = [
-    {file = "websockets-11.0.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:3ccc8a0c387629aec40f2fc9fdcb4b9d5431954f934da3eaf16cdc94f67dbfac"},
-    {file = "websockets-11.0.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d67ac60a307f760c6e65dad586f556dde58e683fab03323221a4e530ead6f74d"},
-    {file = "websockets-11.0.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:84d27a4832cc1a0ee07cdcf2b0629a8a72db73f4cf6de6f0904f6661227f256f"},
-    {file = "websockets-11.0.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffd7dcaf744f25f82190856bc26ed81721508fc5cbf2a330751e135ff1283564"},
-    {file = "websockets-11.0.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7622a89d696fc87af8e8d280d9b421db5133ef5b29d3f7a1ce9f1a7bf7fcfa11"},
-    {file = "websockets-11.0.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bceab846bac555aff6427d060f2fcfff71042dba6f5fca7dc4f75cac815e57ca"},
-    {file = "websockets-11.0.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:54c6e5b3d3a8936a4ab6870d46bdd6ec500ad62bde9e44462c32d18f1e9a8e54"},
-    {file = "websockets-11.0.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:41f696ba95cd92dc047e46b41b26dd24518384749ed0d99bea0a941ca87404c4"},
-    {file = "websockets-11.0.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:86d2a77fd490ae3ff6fae1c6ceaecad063d3cc2320b44377efdde79880e11526"},
-    {file = "websockets-11.0.3-cp310-cp310-win32.whl", hash = "sha256:2d903ad4419f5b472de90cd2d40384573b25da71e33519a67797de17ef849b69"},
-    {file = "websockets-11.0.3-cp310-cp310-win_amd64.whl", hash = "sha256:1d2256283fa4b7f4c7d7d3e84dc2ece74d341bce57d5b9bf385df109c2a1a82f"},
-    {file = "websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
-    {file = "websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
-    {file = "websockets-11.0.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b58cbf0697721120866820b89f93659abc31c1e876bf20d0b3d03cef14faf84d"},
-    {file = "websockets-11.0.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:660e2d9068d2bedc0912af508f30bbeb505bbbf9774d98def45f68278cea20d3"},
-    {file = "websockets-11.0.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c1f0524f203e3bd35149f12157438f406eff2e4fb30f71221c8a5eceb3617b6b"},
-    {file = "websockets-11.0.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:def07915168ac8f7853812cc593c71185a16216e9e4fa886358a17ed0fd9fcf6"},
-    {file = "websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
-    {file = "websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
-    {file = "websockets-11.0.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:01f5567d9cf6f502d655151645d4e8b72b453413d3819d2b6f1185abc23e82dd"},
-    {file = "websockets-11.0.3-cp311-cp311-win32.whl", hash = "sha256:e1459677e5d12be8bbc7584c35b992eea142911a6236a3278b9b5ce3326f282c"},
-    {file = "websockets-11.0.3-cp311-cp311-win_amd64.whl", hash = "sha256:e7837cb169eca3b3ae94cc5787c4fed99eef74c0ab9506756eea335e0d6f3ed8"},
-    {file = "websockets-11.0.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:fb06eea71a00a7af0ae6aefbb932fb8a7df3cb390cc217d51a9ad7343de1b8d0"},
-    {file = "websockets-11.0.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8a34e13a62a59c871064dfd8ffb150867e54291e46d4a7cf11d02c94a5275bae"},
-    {file = "websockets-11.0.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4841ed00f1026dfbced6fca7d963c4e7043aa832648671b5138008dc5a8f6d99"},
-    {file = "websockets-11.0.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a073fc9ab1c8aff37c99f11f1641e16da517770e31a37265d2755282a5d28aa"},
-    {file = "websockets-11.0.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:68b977f21ce443d6d378dbd5ca38621755f2063d6fdb3335bda981d552cfff86"},
-    {file = "websockets-11.0.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e1a99a7a71631f0efe727c10edfba09ea6bee4166a6f9c19aafb6c0b5917d09c"},
-    {file = "websockets-11.0.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:bee9fcb41db2a23bed96c6b6ead6489702c12334ea20a297aa095ce6d31370d0"},
-    {file = "websockets-11.0.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:4b253869ea05a5a073ebfdcb5cb3b0266a57c3764cf6fe114e4cd90f4bfa5f5e"},
-    {file = "websockets-11.0.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:1553cb82942b2a74dd9b15a018dce645d4e68674de2ca31ff13ebc2d9f283788"},
-    {file = "websockets-11.0.3-cp38-cp38-win32.whl", hash = "sha256:f61bdb1df43dc9c131791fbc2355535f9024b9a04398d3bd0684fc16ab07df74"},
-    {file = "websockets-11.0.3-cp38-cp38-win_amd64.whl", hash = "sha256:03aae4edc0b1c68498f41a6772d80ac7c1e33c06c6ffa2ac1c27a07653e79d6f"},
-    {file = "websockets-11.0.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:777354ee16f02f643a4c7f2b3eff8027a33c9861edc691a2003531f5da4f6bc8"},
-    {file = "websockets-11.0.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8c82f11964f010053e13daafdc7154ce7385ecc538989a354ccc7067fd7028fd"},
-    {file = "websockets-11.0.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3580dd9c1ad0701169e4d6fc41e878ffe05e6bdcaf3c412f9d559389d0c9e016"},
-    {file = "websockets-11.0.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6f1a3f10f836fab6ca6efa97bb952300b20ae56b409414ca85bff2ad241d2a61"},
-    {file = "websockets-11.0.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df41b9bc27c2c25b486bae7cf42fccdc52ff181c8c387bfd026624a491c2671b"},
-    {file = "websockets-11.0.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:279e5de4671e79a9ac877427f4ac4ce93751b8823f276b681d04b2156713b9dd"},
-    {file = "websockets-11.0.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:1fdf26fa8a6a592f8f9235285b8affa72748dc12e964a5518c6c5e8f916716f7"},
-    {file = "websockets-11.0.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:69269f3a0b472e91125b503d3c0b3566bda26da0a3261c49f0027eb6075086d1"},
-    {file = "websockets-11.0.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:97b52894d948d2f6ea480171a27122d77af14ced35f62e5c892ca2fae9344311"},
-    {file = "websockets-11.0.3-cp39-cp39-win32.whl", hash = "sha256:c7f3cb904cce8e1be667c7e6fef4516b98d1a6a0635a58a57528d577ac18a128"},
-    {file = "websockets-11.0.3-cp39-cp39-win_amd64.whl", hash = "sha256:c792ea4eabc0159535608fc5658a74d1a81020eb35195dd63214dcf07556f67e"},
-    {file = "websockets-11.0.3-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:f2e58f2c36cc52d41f2659e4c0cbf7353e28c8c9e63e30d8c6d3494dc9fdedcf"},
-    {file = "websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:de36fe9c02995c7e6ae6efe2e205816f5f00c22fd1fbf343d4d18c3d5ceac2f5"},
-    {file = "websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0ac56b661e60edd453585f4bd68eb6a29ae25b5184fd5ba51e97652580458998"},
-    {file = "websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
-    {file = "websockets-11.0.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:42cc5452a54a8e46a032521d7365da775823e21bfba2895fb7b77633cce031bb"},
-    {file = "websockets-11.0.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:e6316827e3e79b7b8e7d8e3b08f4e331af91a48e794d5d8b099928b6f0b85f20"},
-    {file = "websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8531fdcad636d82c517b26a448dcfe62f720e1922b33c81ce695d0edb91eb931"},
-    {file = "websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c114e8da9b475739dde229fd3bc6b05a6537a88a578358bc8eb29b4030fac9c9"},
-    {file = "websockets-11.0.3-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e063b1865974611313a3849d43f2c3f5368093691349cf3c7c8f8f75ad7cb280"},
-    {file = "websockets-11.0.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:92b2065d642bf8c0a82d59e59053dd2fdde64d4ed44efe4870fa816c1232647b"},
-    {file = "websockets-11.0.3-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:0ee68fe502f9031f19d495dae2c268830df2760c0524cbac5d759921ba8c8e82"},
-    {file = "websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dcacf2c7a6c3a84e720d1bb2b543c675bf6c40e460300b628bab1b1efc7c034c"},
-    {file = "websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b67c6f5e5a401fc56394f191f00f9b3811fe843ee93f4a70df3c389d1adf857d"},
-    {file = "websockets-11.0.3-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1d5023a4b6a5b183dc838808087033ec5df77580485fc533e7dab2567851b0a4"},
-    {file = "websockets-11.0.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:ed058398f55163a79bb9f06a90ef9ccc063b204bb346c4de78efc5d15abfe602"},
-    {file = "websockets-11.0.3-py3-none-any.whl", hash = "sha256:6681ba9e7f8f3b19440921e99efbb40fc89f26cd71bf539e45d8c8a25c976dc6"},
-    {file = "websockets-11.0.3.tar.gz", hash = "sha256:88fc51d9a26b10fc331be344f1781224a375b78488fc343620184e95a4b27016"},
+    {file = "wheel-0.43.0-py3-none-any.whl", hash = "sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81"},
+    {file = "wheel-0.43.0.tar.gz", hash = "sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.17.0"
+version = "3.18.1"
 requires_python = ">=3.8"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
+groups = ["default", "docs"]
+marker = "python_version < \"3.10\""
 files = [
-    {file = "zipp-3.17.0-py3-none-any.whl", hash = "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31"},
-    {file = "zipp-3.17.0.tar.gz", hash = "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"},
+    {file = "zipp-3.18.1-py3-none-any.whl", hash = "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b"},
+    {file = "zipp-3.18.1.tar.gz", hash = "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"},
 ]
```

### Comparing `litestar_asyncpg-0.1.3/.github/workflows/cd.yaml` & `litestar_asyncpg-0.2.0/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/.github/workflows/ci.yaml` & `litestar_asyncpg-0.2.0/.github/workflows/ci.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 
 jobs:
   validate:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - name: Install Pre-Commit
         run: python -m pip install pre-commit && pre-commit install
 
       - name: Load cached Pre-Commit Dependencies
         id: cached-pre-commit-dependencies
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ~/.cache/pre-commit/
           key: pre-commit|${{ env.pythonLocation }}|${{ hashFiles('.pre-commit-config.yaml') }}
 
       - name: Execute Pre-Commit
         run: pre-commit run --show-diff-on-failure --color=always --all-files
 
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: true
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     timeout-minutes: 30
     defaults:
       run:
         shell: bash
     steps:
       - name: Check out repository
         uses: actions/checkout@v4
@@ -48,27 +48,27 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: pdm install
 
       - name: Test
-        run: pdm run pytest -m "" -n auto
+        run: pdm run pytest -m ""
 
   build-docs:
     needs:
       - validate
     if: github.event_name == 'pull_request'
     runs-on: ubuntu-latest
     steps:
       - name: Check out repository
         uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: pdm-project/setup-pdm@v3
         name: Set up PDM
         with:
           python-version: "3.11"
@@ -81,13 +81,13 @@
 
       - name: Save PR number
         env:
           PR_NUMBER: ${{ github.event.number }}
         run: echo $PR_NUMBER > .pr_number
 
       - name: Upload artifact
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: docs-preview
           path: |
             docs/_build/html
             .pr_number
```

### Comparing `litestar_asyncpg-0.1.3/.github/workflows/docs-preview.yaml` & `litestar_asyncpg-0.2.0/.github/workflows/docs-preview.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -14,41 +14,41 @@
       pull-requests: write
 
     steps:
       - name: Check out repository
         uses: actions/checkout@v4
 
       - name: Download artifact
-        uses: dawidd6/action-download-artifact@v2
+        uses: dawidd6/action-download-artifact@v3
         with:
           workflow_conclusion: success
           run_id: ${{ github.event.workflow_run.id }}
           path: docs-preview
           name: docs-preview
 
       - name: Set PR number
         run: echo "PR_NUMBER=$(cat docs-preview/.pr_number)" >> $GITHUB_ENV
 
       - name: Deploy docs preview
         uses: JamesIves/github-pages-deploy-action@v4
         with:
           folder: docs-preview/docs/_build/html
           token: ${{ secrets.DOCS_PREVIEW_DEPLOY_TOKEN }}
-          repository-name: cofin/litestar-asyncpg-docs-preview
+          repository-name: litestar-org/litestar-asyncpg-docs-preview
           clean: false
           target-folder: ${{ env.PR_NUMBER }}
           branch: gh-pages
 
-      - uses: actions/github-script@v6
+      - uses: actions/github-script@v7
         env:
           PR_NUMBER: ${{ env.PR_NUMBER }}
         with:
           script: |
             const issue_number = process.env.PR_NUMBER
-            const body = "Documentation preview will be available shortly at https://cofin.github.io/advanced-alchemy-docs-preview/" + issue_number
+            const body = "Documentation preview will be available shortly at https://litestar-org.github.io/litestar-asyncpg-docs-preview/" + issue_number
 
             const opts = github.rest.issues.listComments.endpoint.merge({
               owner: context.repo.owner,
               repo: context.repo.repo,
               issue_number: issue_number,
             });
```

### Comparing `litestar_asyncpg-0.1.3/.github/workflows/docs.yaml` & `litestar_asyncpg-0.2.0/.github/workflows/docs.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   docs:
     permissions:
       contents: write
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: pdm-project/setup-pdm@v3
         name: Set up PDM
         with:
           python-version: "3.11"
```

### Comparing `litestar_asyncpg-0.1.3/.github/workflows/publish.yaml` & `litestar_asyncpg-0.2.0/.github/workflows/publish.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     permissions:
       id-token: write
     environment: release
     steps:
       - name: Check out repository
         uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: pdm-project/setup-pdm@v3
         name: Set up PDM
         with:
           python-version: "3.11"
```

### Comparing `litestar_asyncpg-0.1.3/docs/Makefile` & `litestar_asyncpg-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/docs/conf.py` & `litestar_asyncpg-0.2.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 html_css_files = ["css/custom.css"]
 html_show_sourcelink = True
 html_title = "Docs"
 html_favicon = "_static/logo.png"
 html_logo = "_static/logo.png"
 html_context = {
     "source_type": "github",
-    "source_user": "cofin",
+    "source_user": "litestar-org",
     "source_repo": project.replace("_", "-"),
 }
 
 brand_colors = {
     "--brand-primary": {"rgb": "245, 0, 87", "hex": "#f50057"},
     "--brand-secondary": {"rgb": "32, 32, 32", "hex": "#202020"},
     "--brand-tertiary": {"rgb": "161, 173, 161", "hex": "#A1ADA1"},
@@ -105,19 +105,19 @@
     "--brand-dark": {"rgb": "0, 0, 0", "hex": "#000000"},
     "--brand-light": {"rgb": "235, 221, 221", "hex": "#ebdddd"},
 }
 
 html_theme_options = {
     "logo_target": "/",
     "announcement": "This documentation is currently under development.",
-    "github_url": "https://github.com/cofin/litestar-asyncpg",
+    "github_url": "https://github.com/litestar-org/litestar-asyncpg",
     "nav_links": [
-        {"title": "Home", "url": "https://cofin.github.io/litesatr-asyncpg/"},
-        {"title": "Docs", "url": "https://cofin.github.io/litesatr-asyncpg/latest/"},
-        {"title": "Code", "url": "https://github.com/cofin/litestar-asyncpg"},
+        {"title": "Home", "url": "https://litestar-org.github.io/litesatr-asyncpg/"},
+        {"title": "Docs", "url": "https://litestar-org.github.io/litesatr-asyncpg/latest/"},
+        {"title": "Code", "url": "https://github.com/litestar-org/litestar-asyncpg"},
     ],
     "light_css_variables": {
         # RGB
         "--sy-rc-theme": brand_colors["--brand-primary"]["rgb"],
         "--sy-rc-text": brand_colors["--brand-primary"]["rgb"],
         "--sy-rc-invert": brand_colors["--brand-primary"]["rgb"],
         # "--sy-rc-bg": brand_colors["--brand-secondary"]["rgb"],
```

### Comparing `litestar_asyncpg-0.1.3/docs/fix_missing_references.py` & `litestar_asyncpg-0.2.0/docs/fix_missing_references.py`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/docs/index.rst` & `litestar_asyncpg-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/examples/basic.py` & `litestar_asyncpg-0.2.0/examples/basic.py`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/litestar_asyncpg/config.py` & `litestar_asyncpg-0.2.0/litestar_asyncpg/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, TypeVar, cast
+from typing import TYPE_CHECKING, Optional, TypeVar, Union, cast
 
 from asyncpg import Record
 from asyncpg import create_pool as asyncpg_create_pool
-from asyncpg.connection import Connection
-from asyncpg.pool import Pool, PoolConnectionProxy
+from asyncpg.connection import Connection, ConnectionMeta
+from asyncpg.pool import Pool, PoolConnectionProxy, PoolConnectionProxyMeta
 from litestar.constants import HTTP_DISCONNECT, HTTP_RESPONSE_START, WEBSOCKET_CLOSE, WEBSOCKET_DISCONNECT
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.serialization import decode_json, encode_json
 from litestar.types import Empty
-from litestar.utils import delete_litestar_scope_state, get_litestar_scope_state, set_litestar_scope_state
 from litestar.utils.dataclass import simple_asdict
 
+from litestar_asyncpg._utils import delete_scope_state, get_scope_state, set_scope_state
+
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from collections.abc import AsyncGenerator, Callable, Coroutine
     from typing import Any
 
     from litestar import Litestar
     from litestar.datastructures.state import State
     from litestar.types import BeforeMessageSendHookHandler, EmptyType, Message, Scope
 
 
-SESSION_SCOPE_KEY = "_asyncpg_db_connection"
+CONNECTION_SCOPE_KEY = "_asyncpg_db_connection"
 SESSION_TERMINUS_ASGI_EVENTS = {HTTP_RESPONSE_START, HTTP_DISCONNECT, WEBSOCKET_DISCONNECT, WEBSOCKET_CLOSE}
 T = TypeVar("T")
 
 
-async def default_before_send_handler(message: Message, scope: Scope) -> None:  # noqa: ARG001
+async def default_before_send_handler(message: Message, scope: Scope) -> None:
     """Handle closing and cleaning up sessions before sending.
 
     Args:
         message: ASGI-``Message``
         scope: An ASGI-``Scope``
 
     Returns:
         None
     """
-    session = cast("Connection | PoolConnectionProxy | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
-    if session is not None:
-        delete_litestar_scope_state(scope, SESSION_SCOPE_KEY)
-
+    session = cast("Union[PoolConnectionProxy,Connection,None]", get_scope_state(scope, CONNECTION_SCOPE_KEY))
+    if session  is not None and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
+        delete_scope_state(scope, CONNECTION_SCOPE_KEY)
 
 def serializer(value: Any) -> str:
     """Serialize JSON field values.
 
     Args:
         value: Any json serializable value.
 
@@ -103,14 +103,18 @@
 
     pool_config: PoolConfig | None = None
     """Asyncpg Pool configuration"""
     pool_app_state_key: str = "db_pool"
     """Key under which to store the asyncpg pool in the application :class:`State <.datastructures.State>`
     instance.
     """
+    pool_dependency_key: str = "db_pool"
+    """Key under which to store the asyncpg Pool in the application dependency injection map.    """
+    connection_dependency_key: str = "db_connection"
+    """Key under which to store the asyncpg Pool in the application dependency injection map.    """
     before_send_handler: BeforeMessageSendHookHandler = default_before_send_handler
     """Handler to call before the ASGI message is sent.
 
     The handler should handle closing the session stored in the ASGI scope, if it's still open, and committing and
     uncommitted data.
     """
     json_deserializer: Callable[[str], Any] = decode_json
@@ -142,15 +146,21 @@
     @property
     def signature_namespace(self) -> dict[str, Any]:
         """Return the plugin's signature namespace.
 
         Returns:
             A string keyed dict of names to be added to the namespace for signature forward reference resolution.
         """
-        return {"Connection": Connection, "Pool": Pool, "PoolConnectionProxy": PoolConnectionProxy}
+        return {
+            "Connection": Connection,
+            "Pool": Pool,
+            "PoolConnectionProxy": PoolConnectionProxy,
+            "PoolConnectionProxyMeta": PoolConnectionProxyMeta,
+            "ConnectionMeta": ConnectionMeta,
+        }
 
     async def create_pool(self) -> Pool:
         """Return a pool. If none exists yet, create one.
 
         Returns:
             Getter that returns the pool instance used by the plugin.
         """
@@ -161,17 +171,15 @@
             msg = "One of 'pool_config' or 'pool_instance' must be provided."
             raise ImproperlyConfiguredException(msg)
 
         pool_config = self.pool_config_dict
         self.pool_instance = await asyncpg_create_pool(**pool_config)
         if self.pool_instance is None:
             msg = "Could not configure the 'pool_instance'. Please check your configuration."
-            raise ImproperlyConfiguredException(
-                msg,
-            )
+            raise ImproperlyConfiguredException(    msg        )
         return self.pool_instance
 
     @asynccontextmanager
     async def lifespan(
         self,
         app: Litestar,
     ) -> AsyncGenerator[None, None]:
@@ -194,24 +202,24 @@
         """
         return cast("Pool", state.get(self.pool_app_state_key))
 
     async def provide_connection(
         self,
         state: State,
         scope: Scope,
-    ) -> AsyncGenerator[Connection | PoolConnectionProxy, None]:
+    ) -> AsyncGenerator[Union[PoolConnectionProxy,Connection], None]:  # noqa: UP007
         """Create a connection instance.
 
         Args:
             state: The ``Litestar.state`` instance.
             scope: The current connection's scope.
 
         Returns:
             A connection instance.
         """
-        connection = cast("Connection | PoolConnectionProxy | None", get_litestar_scope_state(scope, SESSION_SCOPE_KEY))
+        connection = cast("Optional[Union[PoolConnectionProxy,Connection]]", get_scope_state(scope, CONNECTION_SCOPE_KEY))
         if connection is None:
             pool = cast("Pool", state.get(self.pool_app_state_key))
 
             async with pool.acquire() as connection:
-                set_litestar_scope_state(scope, SESSION_SCOPE_KEY, connection)
+                set_scope_state(scope, CONNECTION_SCOPE_KEY, connection)
                 yield connection
```

### Comparing `litestar_asyncpg-0.1.3/litestar_asyncpg/plugin.py` & `litestar_asyncpg-0.2.0/litestar_asyncpg/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
         Args:
             app_config: The :class:`AppConfig <.config.app.AppConfig>` instance.
         """
 
         app_config.dependencies.update(
             {
-                "db_pool": Provide(self._config.provide_pool, sync_to_thread=False),
-                "db_connection": Provide(self._config.provide_connection),
+                self._config.pool_dependency_key: Provide(self._config.provide_pool, sync_to_thread=False),
+                self._config.connection_dependency_key: Provide(self._config.provide_connection),
             },
         )
         app_config.type_encoders = {pgproto.UUID: str, **(app_config.type_encoders or {})}
         app_config.before_send.append(self._config.before_send_handler)
         app_config.lifespan.append(self._config.lifespan)
         app_config.signature_namespace.update(self._config.signature_namespace)
```

### Comparing `litestar_asyncpg-0.1.3/.gitignore` & `litestar_asyncpg-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `litestar_asyncpg-0.1.3/LICENSE` & `litestar_asyncpg-0.2.0/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Cody Fincher
+Copyright (c) 2024 Litestar Organization
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

