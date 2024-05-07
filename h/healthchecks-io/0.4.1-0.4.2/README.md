# Comparing `tmp/healthchecks_io-0.4.1.tar.gz` & `tmp/healthchecks_io-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthchecks_io-0.4.1.tar", max compression
+gzip compressed data, was "healthchecks_io-0.4.2.tar", max compression
```

## Comparing `healthchecks_io-0.4.1.tar` & `healthchecks_io-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/LICENSE
--rw-r--r--   0        0        0     1089 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/LICENSE.rst
--rw-r--r--   0        0        0     3170 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/README.rst
--rw-r--r--   0        0        0     2471 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1378 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/__init__.py
--rw-r--r--   0        0        0      228 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/__init__.py
--rw-r--r--   0        0        0    10427 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/_abstract.py
--rw-r--r--   0        0        0    20246 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/async_client.py
--rw-r--r--   0        0        0     6673 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/check_trap.py
--rw-r--r--   0        0        0      885 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/exceptions.py
--rw-r--r--   0        0        0    19690 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/sync_client.py
--rw-r--r--   0        0        0        0 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/py.typed
--rw-r--r--   0        0        0      394 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/__init__.py
--rw-r--r--   0        0        0      602 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/badges.py
--rw-r--r--   0        0        0     9557 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/checks.py
--rw-r--r--   0        0        0      470 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/integrations.py
--rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 healthchecks_io-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-07 21:25:36.193451 healthchecks_io-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1089 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/LICENSE.rst
+-rw-r--r--   0        0        0     3170 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/README.rst
+-rw-r--r--   0        0        0     2483 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1378 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/__init__.py
+-rw-r--r--   0        0        0    10427 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/_abstract.py
+-rw-r--r--   0        0        0    20246 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/async_client.py
+-rw-r--r--   0        0        0     6673 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/check_trap.py
+-rw-r--r--   0        0        0      885 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/exceptions.py
+-rw-r--r--   0        0        0    19690 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/client/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/py.typed
+-rw-r--r--   0        0        0      394 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/schemas/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/schemas/badges.py
+-rw-r--r--   0        0        0     9557 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/schemas/checks.py
+-rw-r--r--   0        0        0      470 2024-05-07 21:25:36.197450 healthchecks_io-0.4.2/src/healthchecks_io/schemas/integrations.py
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 healthchecks_io-0.4.2/PKG-INFO
```

### Comparing `healthchecks_io-0.4.1/LICENSE` & `healthchecks_io-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/LICENSE.rst` & `healthchecks_io-0.4.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/README.rst` & `healthchecks_io-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/pyproject.toml` & `healthchecks_io-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "healthchecks_io"
-version = "0.4.1"
+version = "0.4.2"
 description = "A python client package for Healthchecks.io API"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/andrewthetechie/py-healthchecks.io"
 repository = "https://github.com/andrewthetechie/py-healthchecks.io"
 documentation = "https://py-healthchecks.io.readthedocs.io"
@@ -24,31 +24,31 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/andrewthetechie/py-healthchecks.io/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 httpx = ">=0.23.0,<0.25.0"
-croniter = "^1.1.0"
+croniter = ">=1.1,<3.0"
 pytz = ">=2021.3,<2024.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 coverage = {extras = ["toml"], version = "^7.1"}
-safety = "^2.3.5"
+safety = ">=2.3.5,<4.0.0"
 mypy = "^1.0"
 xdoctest = {extras = ["colors"], version = "^1.1.1"}
-sphinx = ">=4.3.2,<6.0.0"
+sphinx = ">=4.3.2,<8.0.0"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^2.21.0"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.4.0"
 pyupgrade = "^3.3.1"
 furo = ">=2021.11.12"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 types-croniter = ">=1.3.2,<3.0.0"
 types-pytz = ">=2022.7.1,<2024.0.0"
 pytest-asyncio = ">=0.20.3,<0.24.0"
 respx = ">=0.20.1,<0.22.0"
 pytest-mock = "^3.10.0"
 pytest-lazy-fixture = "^0.6.3"
 pytest-xdist = "^3.2.0"
```

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/__init__.py` & `healthchecks_io-0.4.2/src/healthchecks_io/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Py Healthchecks.Io."""
 
 # set by poetry-dynamic-versioning
-__version__ = "0.4.1"  # noqa: E402
+__version__ = "0.4.2"  # noqa: E402
 
 from .client import AsyncClient  # noqa: F401, E402
 from .client import Client  # noqa: F401, E402
 from .client import CheckTrap  # noqa: F401, E402
 from .client.exceptions import BadAPIRequestError  # noqa: F401, E402
 from .client.exceptions import CheckNotFoundError  # noqa: F401, E402
 from .client.exceptions import HCAPIAuthError  # noqa: F401, E402
```

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/client/_abstract.py` & `healthchecks_io-0.4.2/src/healthchecks_io/client/_abstract.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/client/async_client.py` & `healthchecks_io-0.4.2/src/healthchecks_io/client/async_client.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/client/check_trap.py` & `healthchecks_io-0.4.2/src/healthchecks_io/client/check_trap.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/client/exceptions.py` & `healthchecks_io-0.4.2/src/healthchecks_io/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/client/sync_client.py` & `healthchecks_io-0.4.2/src/healthchecks_io/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/schemas/badges.py` & `healthchecks_io-0.4.2/src/healthchecks_io/schemas/badges.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/src/healthchecks_io/schemas/checks.py` & `healthchecks_io-0.4.2/src/healthchecks_io/schemas/checks.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.1/PKG-INFO` & `healthchecks_io-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthchecks_io
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python client package for Healthchecks.io API
 Home-page: https://github.com/andrewthetechie/py-healthchecks.io
 License: MIT
 Author: Andrew Herrington
 Author-email: andrew.the.techie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: croniter (>=1.1.0,<2.0.0)
+Requires-Dist: croniter (>=1.1,<3.0)
 Requires-Dist: httpx (>=0.23.0,<0.25.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pytz (>=2021.3,<2024.0)
 Project-URL: Changelog, https://github.com/andrewthetechie/py-healthchecks.io/releases
 Project-URL: Documentation, https://py-healthchecks.io.readthedocs.io
 Project-URL: Repository, https://github.com/andrewthetechie/py-healthchecks.io
 Description-Content-Type: text/x-rst
```

