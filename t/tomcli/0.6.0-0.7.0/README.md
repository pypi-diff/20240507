# Comparing `tmp/tomcli-0.6.0.tar.gz` & `tmp/tomcli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcli-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tomcli-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tomcli-0.6.0.tar` & `tomcli-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      616 2023-12-16 07:35:28.578052 tomcli-0.6.0/.builds/docs.yml
--rw-r--r--   0        0        0      775 2023-12-16 07:34:56.746163 tomcli-0.6.0/.builds/main.yml
--rw-r--r--   0        0        0      634 2024-03-28 23:00:35.979103 tomcli-0.6.0/.builds/mockbuild-epel9.yml
--rw-r--r--   0        0        0      639 2024-03-28 23:00:29.520125 tomcli-0.6.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      251 2023-08-31 05:40:26.140196 tomcli-0.6.0/.copr/Makefile
--rw-r--r--   0        0        0      183 2024-03-28 23:09:34.789234 tomcli-0.6.0/.gitignore
--rw-r--r--   0        0        0      150 2023-12-16 07:09:40.400329 tomcli-0.6.0/.reuse/dep5
--rw-r--r--   0        0        0     1675 2023-08-31 05:40:26.140196 tomcli-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1101 2023-12-22 02:01:11.818644 tomcli-0.6.0/LICENSE
-lrwxr-xr-x   0        0        0        0 2023-12-22 02:01:11.825644 tomcli-0.6.0/LICENSES/MIT.txt -> ../LICENSE
--rw-r--r--   0        0        0     2769 2024-03-28 23:10:09.961110 tomcli-0.6.0/NEWS.md
--rw-r--r--   0        0        0     3771 2023-12-16 20:15:53.207081 tomcli-0.6.0/README.md
--rw-r--r--   0        0        0     2343 2023-12-16 20:55:32.286301 tomcli-0.6.0/compgen.py
--rwxr-xr-x   0        0        0      912 2023-04-14 16:27:01.804916 tomcli-0.6.0/contrib/fedoraify.py
-lrwxr-xr-x   0        0        0        0 2023-12-16 07:09:40.516328 tomcli-0.6.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      529 2023-12-16 07:09:40.517328 tomcli-0.6.0/doc/mkdocs_mangen.py
-lrwxr-xr-x   0        0        0        0 2023-12-16 07:09:40.517328 tomcli-0.6.0/doc/news.md -> ../NEWS.md
--rw-r--r--   0        0        0      189 2023-12-16 07:09:40.517328 tomcli-0.6.0/doc/requirements.in
--rw-r--r--   0        0        0      473 2023-12-16 21:39:12.694171 tomcli-0.6.0/doc/tomcli-formatters.1.scd
--rw-r--r--   0        0        0      902 2023-12-16 07:03:51.206529 tomcli-0.6.0/doc/tomcli-get.1.scd
--rw-r--r--   0        0        0     2089 2023-12-16 21:19:49.446168 tomcli-0.6.0/doc/tomcli-set-lists.1.scd
--rw-r--r--   0        0        0     1654 2023-12-16 21:20:43.971975 tomcli-0.6.0/doc/tomcli-set.1.scd
--rw-r--r--   0        0        0      980 2023-12-16 21:22:34.494586 tomcli-0.6.0/doc/tomcli.1.scd
--rw-r--r--   0        0        0     1516 2023-12-16 21:24:53.172097 tomcli-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0     5741 2024-03-28 22:46:49.924829 tomcli-0.6.0/noxfile.py
--rw-r--r--   0        0        0     2983 2024-03-28 22:46:58.435801 tomcli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      972 2024-03-28 23:09:38.594220 tomcli-0.6.0/ruff.toml
--rw-r--r--   0        0        0      204 2024-03-28 23:10:04.354130 tomcli-0.6.0/src/tomcli/__init__.py
--rw-r--r--   0        0        0      181 2023-12-16 07:03:48.733538 tomcli-0.6.0/src/tomcli/__main__.py
--rw-r--r--   0        0        0     5557 2024-01-26 07:25:16.723043 tomcli-0.6.0/src/tomcli/_peekable.py
--rw-r--r--   0        0        0       82 2023-11-27 06:19:42.217982 tomcli-0.6.0/src/tomcli/cli/__init__.py
--rw-r--r--   0        0        0     5627 2023-12-16 20:46:47.601113 tomcli-0.6.0/src/tomcli/cli/_util.py
--rw-r--r--   0        0        0      957 2023-12-14 02:42:21.100931 tomcli-0.6.0/src/tomcli/cli/formatters.py
--rw-r--r--   0        0        0     2201 2024-01-26 07:25:04.111104 tomcli-0.6.0/src/tomcli/cli/get.py
--rw-r--r--   0        0        0      560 2024-01-26 07:25:16.651043 tomcli-0.6.0/src/tomcli/cli/main.py
--rw-r--r--   0        0        0    12845 2024-03-28 22:54:33.250333 tomcli-0.6.0/src/tomcli/cli/set.py
--rw-r--r--   0        0        0     1865 2023-12-02 03:09:19.984105 tomcli-0.6.0/src/tomcli/formatters/__init__.py
--rw-r--r--   0        0        0     1651 2023-12-13 16:47:14.317265 tomcli-0.6.0/src/tomcli/formatters/builtin.py
--rw-r--r--   0        0        0        0 2023-08-31 05:36:11.986530 tomcli-0.6.0/src/tomcli/py.typed
--rw-r--r--   0        0        0     5983 2023-08-31 07:04:33.173107 tomcli-0.6.0/src/tomcli/toml.py
--rw-r--r--   0        0        0      116 2023-08-31 05:36:11.984530 tomcli-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1653 2023-08-31 07:04:33.283106 tomcli-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     3051 2023-12-13 16:46:19.278487 tomcli-0.6.0/tests/test_data/pyproject.toml
--rw-r--r--   0        0        0      123 2023-04-14 16:27:01.816916 tomcli-0.6.0/tests/test_data/test1.toml
--rw-r--r--   0        0        0      202 2023-09-01 03:29:40.186027 tomcli-0.6.0/tests/test_data/test2.toml
--rw-r--r--   0        0        0     1270 2023-11-26 20:17:49.576053 tomcli-0.6.0/tests/test_formatters_builtin.py
--rw-r--r--   0        0        0      852 2023-12-14 02:42:21.101931 tomcli-0.6.0/tests/test_main.py
--rw-r--r--   0        0        0     2604 2023-12-14 02:42:21.101931 tomcli-0.6.0/tests/test_tomcli_get.py
--rw-r--r--   0        0        0     7069 2024-03-28 22:41:23.242941 tomcli-0.6.0/tests/test_tomcli_set.py
--rw-r--r--   0        0        0     1446 2023-08-31 07:04:33.505105 tomcli-0.6.0/tests/test_toml.py
--rw-r--r--   0        0        0      112 2024-03-28 23:00:15.917172 tomcli-0.6.0/tomcli.rpmlintrc
--rw-r--r--   0        0        0     3658 2024-03-28 23:10:09.367112 tomcli-0.6.0/tomcli.spec
--rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 tomcli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      616 2023-12-16 07:35:28.578052 tomcli-0.7.0/.builds/docs.yml
+-rw-r--r--   0        0        0      775 2023-12-16 07:34:56.746163 tomcli-0.7.0/.builds/main.yml
+-rw-r--r--   0        0        0      634 2024-03-28 23:00:35.979103 tomcli-0.7.0/.builds/mockbuild-epel9.yml
+-rw-r--r--   0        0        0      639 2024-03-28 23:00:29.520125 tomcli-0.7.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      251 2023-08-31 05:40:26.140196 tomcli-0.7.0/.copr/Makefile
+-rw-r--r--   0        0        0      183 2024-03-28 23:09:34.789234 tomcli-0.7.0/.gitignore
+-rw-r--r--   0        0        0      150 2023-12-16 07:09:40.400329 tomcli-0.7.0/.reuse/dep5
+-rw-r--r--   0        0        0     1675 2023-08-31 05:40:26.140196 tomcli-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1101 2023-12-22 02:01:11.818644 tomcli-0.7.0/LICENSE
+lrwxr-xr-x   0        0        0        0 2023-12-22 02:01:11.825644 tomcli-0.7.0/LICENSES/MIT.txt -> ../LICENSE
+-rw-r--r--   0        0        0     2995 2024-05-06 23:34:50.754364 tomcli-0.7.0/NEWS.md
+-rw-r--r--   0        0        0     3771 2023-12-16 20:15:53.207081 tomcli-0.7.0/README.md
+-rw-r--r--   0        0        0     2343 2023-12-16 20:55:32.286301 tomcli-0.7.0/compgen.py
+-rwxr-xr-x   0        0        0      912 2023-04-14 16:27:01.804916 tomcli-0.7.0/contrib/fedoraify.py
+lrwxr-xr-x   0        0        0        0 2023-12-16 07:09:40.516328 tomcli-0.7.0/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      529 2023-12-16 07:09:40.517328 tomcli-0.7.0/doc/mkdocs_mangen.py
+lrwxr-xr-x   0        0        0        0 2023-12-16 07:09:40.517328 tomcli-0.7.0/doc/news.md -> ../NEWS.md
+-rw-r--r--   0        0        0      189 2023-12-16 07:09:40.517328 tomcli-0.7.0/doc/requirements.in
+-rw-r--r--   0        0        0      473 2023-12-16 21:39:12.694171 tomcli-0.7.0/doc/tomcli-formatters.1.scd
+-rw-r--r--   0        0        0      902 2023-12-16 07:03:51.206529 tomcli-0.7.0/doc/tomcli-get.1.scd
+-rw-r--r--   0        0        0     2089 2023-12-16 21:19:49.446168 tomcli-0.7.0/doc/tomcli-set-lists.1.scd
+-rw-r--r--   0        0        0     1657 2024-04-30 22:16:30.769304 tomcli-0.7.0/doc/tomcli-set.1.scd
+-rw-r--r--   0        0        0      980 2023-12-16 21:22:34.494586 tomcli-0.7.0/doc/tomcli.1.scd
+-rw-r--r--   0        0        0     1516 2023-12-16 21:24:53.172097 tomcli-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0     5966 2024-05-06 22:40:46.465340 tomcli-0.7.0/noxfile.py
+-rw-r--r--   0        0        0     3255 2024-05-06 22:48:21.996031 tomcli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      972 2024-03-28 23:09:38.594220 tomcli-0.7.0/ruff.toml
+-rw-r--r--   0        0        0      204 2024-05-06 23:34:47.337386 tomcli-0.7.0/src/tomcli/__init__.py
+-rw-r--r--   0        0        0      181 2023-12-16 07:03:48.733538 tomcli-0.7.0/src/tomcli/__main__.py
+-rw-r--r--   0        0        0     5557 2024-01-26 07:25:16.723043 tomcli-0.7.0/src/tomcli/_peekable.py
+-rw-r--r--   0        0        0       82 2023-11-27 06:19:42.217982 tomcli-0.7.0/src/tomcli/cli/__init__.py
+-rw-r--r--   0        0        0     5833 2024-05-06 19:36:05.336306 tomcli-0.7.0/src/tomcli/cli/_util.py
+-rw-r--r--   0        0        0      957 2023-12-14 02:42:21.100931 tomcli-0.7.0/src/tomcli/cli/formatters.py
+-rw-r--r--   0        0        0     2201 2024-01-26 07:25:04.111104 tomcli-0.7.0/src/tomcli/cli/get.py
+-rw-r--r--   0        0        0      560 2024-01-26 07:25:16.651043 tomcli-0.7.0/src/tomcli/cli/main.py
+-rw-r--r--   0        0        0    12917 2024-05-06 19:46:19.045771 tomcli-0.7.0/src/tomcli/cli/set.py
+-rw-r--r--   0        0        0     1865 2023-12-02 03:09:19.984105 tomcli-0.7.0/src/tomcli/formatters/__init__.py
+-rw-r--r--   0        0        0     2451 2024-05-06 22:42:44.259014 tomcli-0.7.0/src/tomcli/formatters/builtin.py
+-rw-r--r--   0        0        0        0 2023-08-31 05:36:11.986530 tomcli-0.7.0/src/tomcli/py.typed
+-rw-r--r--   0        0        0     5983 2023-08-31 07:04:33.173107 tomcli-0.7.0/src/tomcli/toml.py
+-rw-r--r--   0        0        0      116 2023-08-31 05:36:11.984530 tomcli-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1653 2023-08-31 07:04:33.283106 tomcli-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     3051 2023-12-13 16:46:19.278487 tomcli-0.7.0/tests/test_data/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-04-14 16:27:01.816916 tomcli-0.7.0/tests/test_data/test1.toml
+-rw-r--r--   0        0        0      202 2023-09-01 03:29:40.186027 tomcli-0.7.0/tests/test_data/test2.toml
+-rw-r--r--   0        0        0     1655 2024-05-06 20:07:02.284675 tomcli-0.7.0/tests/test_formatters_builtin.py
+-rw-r--r--   0        0        0      982 2024-05-06 22:51:53.269389 tomcli-0.7.0/tests/test_main.py
+-rw-r--r--   0        0        0     2604 2023-12-14 02:42:21.101931 tomcli-0.7.0/tests/test_tomcli_get.py
+-rw-r--r--   0        0        0     7069 2024-03-28 22:41:23.242941 tomcli-0.7.0/tests/test_tomcli_set.py
+-rw-r--r--   0        0        0     1446 2023-08-31 07:04:33.505105 tomcli-0.7.0/tests/test_toml.py
+-rw-r--r--   0        0        0      112 2024-03-28 23:00:15.917172 tomcli-0.7.0/tomcli.rpmlintrc
+-rw-r--r--   0        0        0     3732 2024-05-06 23:34:50.235367 tomcli-0.7.0/tomcli.spec
+-rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 tomcli-0.7.0/PKG-INFO
```

### Comparing `tomcli-0.6.0/.builds/docs.yml` & `tomcli-0.7.0/.builds/docs.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/.builds/main.yml` & `tomcli-0.7.0/.builds/main.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/.builds/mockbuild-epel9.yml` & `tomcli-0.7.0/.builds/mockbuild-epel9.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/.builds/mockbuild.yml` & `tomcli-0.7.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/CONTRIBUTING.md` & `tomcli-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/LICENSE` & `tomcli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/NEWS.md` & `tomcli-0.7.0/NEWS.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 SPDX-License-Identifier: MIT
 -->
 
 NEWS
 =======
 
+## 0.7.0 - 2024-05-06 <a id='0.7.0'></a>
+
+### Added
+
+- `cli set del`: allow removing multiple keys in one invocation
+- `formatters`: add `-F newline-keys` and `-F newline-values`
+
+### Removed
+
+- Remove support for Python 3.8
+
 ## 0.6.0 - 2024-03-28 <a id='0.6.0'></a>
 
 ### Added
 
 - `cli main`: add command description
 - `cli set`: allow passing multiple values to the append command
 - `cli`: support `python -m tomcli`
```

### Comparing `tomcli-0.6.0/README.md` & `tomcli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/compgen.py` & `tomcli-0.7.0/compgen.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/contrib/fedoraify.py` & `tomcli-0.7.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/doc/mkdocs_mangen.py` & `tomcli-0.7.0/doc/mkdocs_mangen.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/doc/tomcli-get.1.scd` & `tomcli-0.7.0/doc/tomcli-get.1.scd`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/doc/tomcli-set-lists.1.scd` & `tomcli-0.7.0/doc/tomcli-set-lists.1.scd`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/doc/tomcli-set.1.scd` & `tomcli-0.7.0/doc/tomcli-set.1.scd`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 ```
 
 ## del
 
 Delete a value from a TOML file
 
 ```
-tomcli-set [GLOBAL OPTIONS] PATH del SELECTOR [OPTIONS]
+tomcli-set [GLOBAL OPTIONS] PATH del [OPTIONS] SELECTOR...
 tomcli-set ... del --help
 ```
 
 ## true / false
 
 Set a value in a TOML file to *true* or *false*.
```

### Comparing `tomcli-0.6.0/doc/tomcli.1.scd` & `tomcli-0.7.0/doc/tomcli.1.scd`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/mkdocs.yml` & `tomcli-0.7.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/noxfile.py` & `tomcli-0.7.0/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import glob
 import os
+from collections.abc import Sequence
 from glob import iglob
 from pathlib import Path
 from shutil import copy2
+from typing import Any, Union
 
 import nox
 
+StrPath = Union[str, "os.PathLike[str]"]
 IN_CI = "JOB_ID" in os.environ or "CI" in os.environ
 ALLOW_EDITABLE = os.environ.get("ALLOW_EDITABLE", str(not IN_CI)).lower() in (
     "1",
     "true",
 )
 
 PROJECT = "tomcli"
@@ -31,28 +34,28 @@
 
 nox.options.sessions = (*LINT_SESSIONS, "covtest")
 
 
 # Helpers
 
 
-def install(session: nox.Session, *args, editable=False, **kwargs):
+def install(session: nox.Session, *args: str, editable: bool = False, **kwargs: Any):
     if editable and ALLOW_EDITABLE:
         args = ("-e", *args)
     session.install(*args, **kwargs)
 
 
-def git(session: nox.Session, *args, **kwargs):
+def git(session: nox.Session, *args: StrPath, **kwargs: Any):
     return session.run("git", *args, **kwargs, external=True)
 
 
 # General
 
 
-@nox.session(python=["3.8", "3.9", "3.10", "3.11", "3.12"])
+@nox.session(python=["3.9", "3.10", "3.11", "3.12"])
 def test(session: nox.Session):
     packages: list[str] = [".[all,tomli,test]"]
     env: dict[str, str] = {}
     tmp = Path(session.create_tmp())
 
     if any(i.startswith("--cov") for i in session.posargs):
         packages.extend(("coverage[toml]", "pytest-cov"))
@@ -107,14 +110,15 @@
     session.run("isort", *posargs, *LINT_FILES)
 
 
 @nox.session
 def typing(session: nox.Session):
     install(session, ".[typing]", "-r", "doc/requirements.in", editable=True)
     session.run("mypy", *LINT_FILES)
+    session.run("basedpyright", f"src/{PROJECT}", "noxfile.py")
 
 
 @nox.session
 def bump(session: nox.Session):
     version = session.posargs[0]
 
     install(session, RELEASERR, "fclogr", "flit")
@@ -174,15 +178,15 @@
     dest = tmp / SPECFILE
     copy2(SPECFILE, dest)
     session.run("python", "contrib/fedoraify.py", str(dest))
     session.run("copr-cli", "build", "--nowait", f"gotmax23/{PROJECT}", str(dest))
 
 
 @nox.session
-def srpm(session: nox.Session, posargs=None):
+def srpm(session: nox.Session, posargs: Sequence[StrPath] | None = None):
     install(session, "fclogr")
     posargs = posargs or session.posargs
     session.run("fclogr", "--debug", "dev-srpm", *posargs, SPECFILE)
 
 
 @nox.session
 def mockbuild(session: nox.Session):
```

### Comparing `tomcli-0.6.0/pyproject.toml` & `tomcli-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "tomcli"
 dynamic = ["version"]
 description = 'CLI for working with TOML files. Pronounced "tom clee."'
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license.text = "MIT"
 authors = [
   { name = "Maxwell G", email = "maxwell@gtmx.me" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 dependencies = [
@@ -52,18 +51,21 @@
     "reuse",
 ]
 formatters = [
     "black>=24",
     "isort",
 ]
 typing = [
+    "basedpyright",
     "tomcli[tomli]",
     "tomcli[tomlkit]",
     "mypy",
     "pytest",
+    # Always install tomli
+    "tomli",
     "typing_extensions",
     # For checking noxfile.py
     "nox",
 ]
 test = [
     "pytest",
 ]
@@ -88,15 +90,17 @@
 "tomcli-get" = "tomcli.cli.get:app"
 "tomcli-set" = "tomcli.cli.set:app"
 "tomcli-formatters" = "tomcli.cli.formatters:APP"
 
 [project.entry-points."tomcli.formatters"]
 default = "tomcli.formatters.builtin:default_formatter"
 json = "tomcli.formatters.builtin:json_formatter"
+newline-keys = "tomcli.formatters.builtin:newline_keys_formatter"
 newline-list = "tomcli.formatters.builtin:newline_list_formatter"
+newline-values = "tomcli.formatters.builtin:newline_values_formatter"
 string = "tomcli.formatters.builtin:string_formatter"
 toml = "tomcli.formatters.builtin:toml_formatter"
 
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
@@ -133,7 +137,13 @@
     'if TYPE_CHECKING:',
     'if t\.TYPE_CHECKING:',
     '@(abc\.)?abstractmethod',
     '@overload',
     'except ImportError:',
 ]
 
+[tool.basedpyright]
+typeCheckingMode = "strict"
+reportPrivateUsage = false
+ignore = [
+    "src/tomcli/_peekable.py",
+]
```

### Comparing `tomcli-0.6.0/ruff.toml` & `tomcli-0.7.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/_peekable.py` & `tomcli-0.7.0/src/tomcli/_peekable.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/cli/_util.py` & `tomcli-0.7.0/src/tomcli/cli/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         msg = f"Invalid selector part: `{part}`. Expected {expected} but got `{but}`."
         raise ValueError(msg)
 
     for character in it:
         if character == quote:
             # Don't allow something like `"ab"c.d`.
             if it.peek(...) not in (".", ...):
+                quote = cast(str, quote)
                 _err(quote + parts + quote + it.peek(), "`.` or end")
             quote = None
             # Short circuit. We know the next is a "."
             yield parts
             parts = ""
             next(it, ...)
         elif quote is None and character == ".":
@@ -137,15 +138,15 @@
 def add_args_and_help(
     *params: SharedArg | Any,
 ) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
     def inner(func: Callable[_P, _T]) -> Callable[_P, _T]:
         helps: list[str] = []
         for param in reversed(params):
             param(func)
-            metavar = func.__click_params__[-1].make_metavar()  # type: ignore[attr-defined]
+            metavar = func.__click_params__[-1].make_metavar().removesuffix("...")  # type: ignore[attr-defined]
             phelp = f"* {metavar}"
             if isinstance(param, SharedArg) and param.help:
                 phelp += f": {param.help}"
             helps.append(phelp)
         helps.reverse()
         func.__doc__ = dedent(func.__doc__) + "\n\n" if func.__doc__ else ""
         func.__doc__ += "\n\n".join(helps)
@@ -168,14 +169,18 @@
         help="Path to a TOML file to read. Use '-' to read from stdin."
         " Set to `...` when calling `--help` for a subcommand",
     ),
     selector=SharedArg(
         click.argument("selector"),
         help=SELECTOR_HELP,
     ),
+    selectors=SharedArg(
+        click.argument("selectors", metavar="SELECTOR...", nargs=-1, required=True),
+        help=SELECTOR_HELP,
+    ),
     formatter=click.option("-F", "--formatter", default=DEFAULT_FORMATTER),
     version=click.version_option(_ver, message="%(version)s"),
 )
 
 
 __all__ = (
     "DEFAULT_CONTEXT_SETTINGS",
```

### Comparing `tomcli-0.6.0/src/tomcli/cli/formatters.py` & `tomcli-0.7.0/src/tomcli/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/cli/get.py` & `tomcli-0.7.0/src/tomcli/cli/get.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/cli/main.py` & `tomcli-0.7.0/src/tomcli/cli/main.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/cli/set.py` & `tomcli-0.7.0/src/tomcli/cli/set.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,28 +100,29 @@
     Subcommands for creating and modifying lists
     """
     ...
 
 
 @cli.command(name="del")
 @click.pass_context
-@add_args_and_help(SHARED_PARAMS.selector)
+@add_args_and_help(SHARED_PARAMS.selectors)
 def delete(
     ctx: click.Context,
-    selector: str,
+    selectors: Sequence[str],
 ):
     """
     Delete a value from a TOML file.
     """
     modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     fun_msg = "Thank you for your patronage, but we won't delete the whole file."
-    set_type(
-        callback=operator.delitem, fun_msg=fun_msg, modder=modder, selector=selector
-    )
+    for selector in selectors:
+        set_type(
+            callback=operator.delitem, fun_msg=fun_msg, modder=modder, selector=selector
+        )
 
 
 @cli.command(name="str")
 @click.pass_context
 @add_args_and_help(SHARED_PARAMS.selector, click.argument("value"))
 def string(ctx: click.Context, selector: str, value: str):
     """
@@ -266,14 +267,15 @@
 def _append_callback(cur: MutableMapping[str, Any], part: str, value: list[Any]):
     lst = cur.get(part)
     if not isinstance(lst, MutableSequence):
         fatal(
             "You can only append values to an existing list."
             " Use the 'list' subcommand to create a new list"
         )
+    lst = cast("MutableSequence[Any]", lst)
     lst.extend(value)
 
 
 _LISTS_COMMON_ARGS = SimpleNamespace(
     pattern=SharedArg(
         click.argument("pattern"),
         help="Pattern against which to match strings",
@@ -434,15 +436,15 @@
         else:
             cur = {"data": cur}
             parts = ["data"]
     for idx, part in enumerate(parts):
         if idx + 1 == len(parts):
             break
         if part not in cur and default is not ...:
-            cur[part] = cast("Callable[[], Any]", default)()
+            cur[part] = default()
         cur = cur[part]
     if value is ...:
         callback(cur, part)  # type: ignore[call-arg]
     else:
         callback(cur, part, typ(value))  # type: ignore[call-arg]
     if selector == ".":
         data = data["data"]
```

### Comparing `tomcli-0.6.0/src/tomcli/formatters/__init__.py` & `tomcli-0.7.0/src/tomcli/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/src/tomcli/toml.py` & `tomcli-0.7.0/src/tomcli/toml.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tests/conftest.py` & `tomcli-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tests/test_data/pyproject.toml` & `tomcli-0.7.0/tests/test_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tests/test_main.py` & `tomcli-0.7.0/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,23 @@
 default
 	Use the `toml` formatter if the object is a Mapping and fall back to
 	`string`.
 
 json
 	Return the JSON representation of the object
 
+newline-keys
+	Return a newline-separated list of Mapping keys
+
 newline-list
 	Return a newline separated list
 
+newline-values
+	Return a newline-separated list of Mapping values
+
 string
 	Print the Python str() representation of the object
 
 toml
 	Return the TOML mapping of the object
 
 """
```

### Comparing `tomcli-0.6.0/tests/test_tomcli_get.py` & `tomcli-0.7.0/tests/test_tomcli_get.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tests/test_tomcli_set.py` & `tomcli-0.7.0/tests/test_tomcli_set.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tests/test_toml.py` & `tomcli-0.7.0/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.6.0/tomcli.spec` & `tomcli-0.7.0/tomcli.spec`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 %define py3_test_envvars %{shrink:
 PYTHONPATH=%{buildroot}%{python3_sitelib}
 PATH=%{buildroot}%{_bindir}:${PATH}
 }
 %endif
 
 Name:           tomcli
-Version:        0.6.0
+Version:        0.7.0
 Release:        1%{?dist}
 Summary:        CLI for working with TOML files. Pronounced "tom clee."
 
 License:        MIT
 URL:            https://sr.ht/~gotmax23/tomcli
 %global furl    https://git.sr.ht/~gotmax23/tomcli
 Source0:        %{furl}/refs/download/v%{version}/tomcli-%{version}.tar.gz
@@ -132,14 +132,17 @@
 %{bash_completions_dir}/tomcli*
 %{fish_completions_dir}/tomcli*.fish
 %{zsh_completions_dir}/_tomcli*
 %{_mandir}/man1/tomcli*.1*
 
 
 %changelog
+* Mon May 06 2024 Maxwell G <maxwell@gtmx.me> - 0.7.0-1
+- Release 0.7.0.
+
 * Thu Mar 28 2024 Maxwell G <maxwell@gtmx.me> - 0.6.0-1
 - Release 0.6.0.
 
 * Thu Dec 14 2023 Maxwell G <maxwell@gtmx.me> - 0.5.0-1
 - Release 0.5.0.
 
 * Sat Dec 02 2023 Maxwell G <maxwell@gtmx.me> - 0.4.0-1
```

### Comparing `tomcli-0.6.0/PKG-INFO` & `tomcli-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tomcli
-Version: 0.6.0
+Version: 0.7.0
 Summary: CLI for working with TOML files. Pronounced "tom clee."
 Author-email: Maxwell G <maxwell@gtmx.me>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: click
 Requires-Dist: importlib_metadata; python_version<'3.11'
@@ -27,18 +26,20 @@
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: black>=24 ; extra == "formatters"
 Requires-Dist: isort ; extra == "formatters"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: tomli  ; extra == "tomli" and ( python_version<'3.11')
 Requires-Dist: tomli_w ; extra == "tomli"
 Requires-Dist: tomlkit ; extra == "tomlkit"
+Requires-Dist: basedpyright ; extra == "typing"
 Requires-Dist: tomcli[tomli] ; extra == "typing"
 Requires-Dist: tomcli[tomlkit] ; extra == "typing"
 Requires-Dist: mypy ; extra == "typing"
 Requires-Dist: pytest ; extra == "typing"
+Requires-Dist: tomli ; extra == "typing"
 Requires-Dist: typing_extensions ; extra == "typing"
 Requires-Dist: nox ; extra == "typing"
 Project-URL: Changelog, https://tomcli.gtmx.me/news/
 Project-URL: Documentation, https://tomcli.gtmx.me
 Project-URL: Homepage, https://tomcli.gtmx.me
 Project-URL: Mailing List, https://lists.sr.ht/~gotmax23/tomcli
 Project-URL: Source, https://git.sr.ht/~gotmax23/tomcli
```

