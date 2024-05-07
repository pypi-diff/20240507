# Comparing `tmp/orloj-0.1.1.tar.gz` & `tmp/orloj-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orloj-0.1.1.tar", max compression
+gzip compressed data, was "orloj-0.1.2.tar", max compression
```

## Comparing `orloj-0.1.1.tar` & `orloj-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2023-12-06 15:48:59.770410 orloj-0.1.1/LICENSE
--rw-r--r--   0        0        0     2531 2023-12-06 18:19:16.137771 orloj-0.1.1/README.md
--rw-r--r--   0        0        0      465 2023-12-06 18:35:07.056296 orloj-0.1.1/orloj/__init__.py
--rw-r--r--   0        0        0     1992 2023-12-06 18:35:07.056259 orloj-0.1.1/orloj/core.py
--rw-r--r--   0        0        0      922 2023-12-06 18:35:07.056180 orloj-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3209 1970-01-01 00:00:00.000000 orloj-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-12-06 15:48:59.770410 orloj-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3730 2023-12-07 09:35:41.847561 orloj-0.1.2/README.md
+-rw-r--r--   0        0        0      471 2024-05-07 05:31:23.277165 orloj-0.1.2/orloj/__init__.py
+-rw-r--r--   0        0        0     1998 2024-05-07 05:31:29.130410 orloj-0.1.2/orloj/core.py
+-rw-r--r--   0        0        0      921 2024-05-07 05:26:14.825068 orloj-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 orloj-0.1.2/PKG-INFO
```

### Comparing `orloj-0.1.1/LICENSE` & `orloj-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orloj-0.1.1/orloj/core.py` & `orloj-0.1.2/orloj/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3.9
 # coding:utf-8
-# Copyright (C) 2023 All rights reserved.
+# Copyright (C) 2023-2024 All rights reserved.
 # FILENAME:    ~~/orloj/core.py
-# VERSION: 	   0.1.1
-# CREATED: 	   2023-12-06 21:54
-# AUTHOR: 	   Sitt Guruvanich <aekazitt+github@gmail.com>
+# VERSION:     0.1.2
+# CREATED:     2023-12-06 21:54
+# AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 """Module defining `OrlojMiddleware` class
 """
```

### Comparing `orloj-0.1.1/pyproject.toml` & `orloj-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 [tool.poetry]
 authors = ['Sitt Guruvanich <aekazitt+github@gmail.com>']
 description = 'Scheduler middleware for ASGI frameworks'
 license = 'MIT'
 name = 'orloj'
 packages = [{include='orloj'}]
 readme = 'README.md'
-version = '0.1.1'
+version = '0.1.2'
 
 
 [tool.poetry.dependencies]
 APScheduler = '>=3.10.4,<4.0.0'
 python = '^3.8'
-starlette = '<0.28.0'
+starlette = '<0.37.2'
 
 
 [tool.poetry.group.dev]
 optional = true
 
 
 [tool.poetry.group.dev.dependencies]
@@ -45,8 +45,7 @@
 [tool.poetry.group.examples]
 optional = true
 
 
 [tool.poetry.group.examples.dependencies]
 fastapi = '^0.104.0'
 uvicorn = '^0.15.0'
-
```

### Comparing `orloj-0.1.1/PKG-INFO` & `orloj-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 Metadata-Version: 2.1
 Name: orloj
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scheduler middleware for ASGI frameworks
 License: MIT
 Author: Sitt Guruvanich
 Author-email: aekazitt+github@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: APScheduler (>=3.10.4,<4.0.0)
-Requires-Dist: starlette (<0.28.0)
+Requires-Dist: starlette (<0.37.2)
 Description-Content-Type: text/markdown
 
 # Orloj
 
 [![Format](https://img.shields.io/pypi/format/orloj)](https://pypi.org/project/orloj)
 [![Python version](https://img.shields.io/pypi/pyversions/orloj)](https://pypi.org/project/orloj)
 [![License](https://img.shields.io/pypi/l/orloj)](https://pypi.org/project/orloj)
 [![Top](https://img.shields.io/github/languages/top/aekasitt/orloj)](.)
 [![Languages](https://img.shields.io/github/languages/count/aekasitt/orloj)](.)
 [![Size](https://img.shields.io/github/repo-size/aekasitt/orloj)](.)
 [![Last commit](https://img.shields.io/github/last-commit/aekasitt/orloj/master)](.)
 
 [![Orloj banner](static/orloj-banner.svg)](static/orloj-banner.svg)
 
-## Getting Started
+## Getting started
+
+You can use `orloj` simply by installing via `pip` on your Terminal.
+
+```sh
+pip install orloj
+```
+
+or alternatively when using [poetry](https://python-poetry.org) package manager as such:
+
+```sh
+poetry add orloj
+```
+
+And then you can begin using `OrlojMiddleware` in your ASGI project as such
+
+```python
+...
+from orloj import OrlojMiddleware
+
+def action() -> None:
+  """Action to be called by scheduler"""
+
+app.add_middleware(OrlojMiddleware, interval=3, job=action)  # Schedules for 3 second interval
+...
+```
 
 The following example shows you how to setup `OrlojMiddleware` to run scheduled tasks alongside
 your [FastAPI](https://github.com/tiangolo/fastapi) application.
 
 ```python
 from fastapi import FastAPI
 from logging import Logger, getLogger
@@ -61,14 +86,24 @@
   """
   return "OK"
 
 app.add_middleware(OrlojMiddleware, interval=3, job=hello_name, name="Igor")
 app.add_middleware(OrlojMiddleware, interval=6, job=hello_world)
 ```
 
+## Dependencies
+
+* [APScheduler](https://github.com/agronholm/apscheduler)
+  [![PyPI](https://img.shields.io/badge/PyPI-3775A9?logo=pypi&logoColor=white)](https://pypi.org/project/APScheduler)
+  [![Docs](https://img.shields.io/readthedocs/apscheduler?logo=readthedocs)](https://apscheduler.readthedocs.io/en/3.x)
+
+* [starlette](https://www.starlette.io)
+  [![PyPI](https://img.shields.io/badge/PyPI-3775A9?logo=pypi&logoColor=white)](https://pypi.org/project/starlette)
+  [![Docs](https://img.shields.io/badge/MkDocs-526CFE?logo=materialformkdocs&logoColor=white)](https://www.starlette.io)
+
 ## Contributions
 
 To contribute to the project, fork the repository and clone to your local device and development
 dependencies including three extra libraries not included in final builds as such:
 
 * [black](https://github.com/psf/black) - The uncompromising Python code formatter 
 * [mypy](https://github.com/python/mypy) - Optional static typing for Python
@@ -79,12 +114,13 @@
 ```bash
 pip install --user poetry
 poetry install --with dev
 ```
 
 ## Acknowledgements
 
+* [APScheduler Web Examples](https://github.com/agronholm/apscheduler/tree/master/examples/web)
 * [Wikimedia Commons - File:Prague Astronomical Clock.svg](https://commons.wikimedia.org/wiki/File:Prague_Astronomical_Clock.svg)
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

