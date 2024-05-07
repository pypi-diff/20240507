# Comparing `tmp/sag-py-fastapi-health-0.1.3.tar.gz` & `tmp/sag_py_fastapi_health-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-fastapi-health-0.1.3.tar", last modified: Tue May 23 17:25:31 2023, max compression
+gzip compressed data, was "sag_py_fastapi_health-0.1.4.tar", last modified: Tue May  7 09:26:53 2024, max compression
```

## Comparing `sag-py-fastapi-health-0.1.3.tar` & `sag_py_fastapi_health-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:25:31.000000 sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:25:31.247773 sag-py-fastapi-health-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_checks_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_checks_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_prtg_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-23 17:25:22.000000 sag-py-fastapi-health-0.1.3/tests/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:53.428548 sag_py_fastapi_health-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-07 09:26:53.428548 sag_py_fastapi_health-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:53.424548 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:53.424548 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:53.424548 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-07 09:26:53.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 09:26:53.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:26:53.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 09:26:53.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 09:26:53.000000 sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 09:26:53.428548 sag_py_fastapi_health-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:26:53.424548 sag_py_fastapi_health-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/tests/test_checks_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/tests/test_checks_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/tests/test_json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/tests/test_prtg_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-07 09:26:49.000000 sag_py_fastapi_health-0.1.4/tests/test_router.py
```

### Comparing `sag-py-fastapi-health-0.1.3/LICENSE.txt` & `sag_py_fastapi_health-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/PKG-INFO` & `sag_py_fastapi_health-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
@@ -14,16 +14,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: fastapi>=0.109.1
+Requires-Dist: pydantic>=1.9
+Requires-Dist: aiohttp[speedups]<4,>=3
+Requires-Dist: typing-extensions>=4.0.0
+Provides-Extra: dev
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_fastapi_health
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
 
 Add health check endpoints to fastapi (similar to the ones dotnet core has)
```

### Comparing `sag-py-fastapi-health-0.1.3/README.md` & `sag_py_fastapi_health-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/http.py` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/http.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/checks/storage.py` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/checks/storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/formatter.py` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/models.py` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/models.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health/router.py` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health/router.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/PKG-INFO` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-fastapi-health
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for fastapi health checks
 Home-page: https://github.com/SamhammerAG/sag_py_fastapi_health
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_fastapi_health
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_fastapi_health/issues
@@ -14,16 +14,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: fastapi>=0.109.1
+Requires-Dist: pydantic>=1.9
+Requires-Dist: aiohttp[speedups]<4,>=3
+Requires-Dist: typing-extensions>=4.0.0
+Provides-Extra: dev
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_fastapi_health
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
 
 Add health check endpoints to fastapi (similar to the ones dotnet core has)
```

### Comparing `sag-py-fastapi-health-0.1.3/sag_py_fastapi_health.egg-info/SOURCES.txt` & `sag_py_fastapi_health-0.1.4/sag_py_fastapi_health.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 sag_py_fastapi_health.egg-info/PKG-INFO
 sag_py_fastapi_health.egg-info/SOURCES.txt
 sag_py_fastapi_health.egg-info/dependency_links.txt
 sag_py_fastapi_health.egg-info/requires.txt
 sag_py_fastapi_health.egg-info/top_level.txt
 sag_py_fastapi_health/checks/__init__.py
 sag_py_fastapi_health/checks/http.py
+sag_py_fastapi_health/checks/py.typed
 sag_py_fastapi_health/checks/storage.py
 tests/test_checks_http.py
 tests/test_checks_storage.py
 tests/test_json_formatter.py
 tests/test_prtg_formatter.py
 tests/test_router.py
```

### Comparing `sag-py-fastapi-health-0.1.3/setup.py` & `sag_py_fastapi_health-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-fastapi-health",
-    version="0.1.3",
+    version="0.1.4",
     description="A library for fastapi health checks",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_fastapi_health",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-fastapi-health-0.1.3/tests/test_checks_http.py` & `sag_py_fastapi_health-0.1.4/tests/test_checks_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 import mock
 import pytest
 from aiohttp import ClientResponse
 from aiohttp.helpers import TimerNoop
 from yarl import URL
 
 from sag_py_fastapi_health.checks.http import HttpCheck
@@ -11,15 +12,15 @@
 @pytest.mark.asyncio
 async def test__HttpCheck__with_ok_result(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
     response = ClientResponse(
         "get",
         URL("http://localhost/test"),
         request_info=mock.Mock(),
-        writer=mock.Mock(),
+        writer=None,  # type: ignore [arg-type]
         continue100=None,
         timer=TimerNoop(),
         traces=[],
         loop=mock.Mock(),
         session=mock.Mock(),
     )
     response.status = 200
@@ -37,15 +38,15 @@
 @pytest.mark.asyncio
 async def test__HttpCheck__with_no_content_result(monkeypatch: pytest.MonkeyPatch) -> None:
     # Arrange
     response = ClientResponse(
         "get",
         URL("http://localhost/test"),
         request_info=mock.Mock(),
-        writer=mock.Mock(),
+        writer=None,  # type: ignore [arg-type]
         continue100=None,
         timer=TimerNoop(),
         traces=[],
         loop=mock.Mock(),
         session=mock.Mock(),
     )
     response.status = 204
```

### Comparing `sag-py-fastapi-health-0.1.3/tests/test_checks_storage.py` & `sag_py_fastapi_health-0.1.4/tests/test_checks_storage.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/tests/test_json_formatter.py` & `sag_py_fastapi_health-0.1.4/tests/test_json_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/tests/test_prtg_formatter.py` & `sag_py_fastapi_health-0.1.4/tests/test_prtg_formatter.py`

 * *Files identical despite different names*

### Comparing `sag-py-fastapi-health-0.1.3/tests/test_router.py` & `sag_py_fastapi_health-0.1.4/tests/test_router.py`

 * *Files identical despite different names*

