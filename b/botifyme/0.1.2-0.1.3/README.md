# Comparing `tmp/botifyme-0.1.2.tar.gz` & `tmp/botifyme-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botifyme-0.1.2.tar", max compression
+gzip compressed data, was "botifyme-0.1.3.tar", max compression
```

## Comparing `botifyme-0.1.2.tar` & `botifyme-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.2/LICENSE
--rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-02-22 03:29:19.474406 botifyme-0.1.2/botifyme/__init__.py
--rw-r--r--   0        0        0       61 2024-02-22 03:29:19.474873 botifyme-0.1.2/botifyme/cli/__init__.py
--rw-r--r--   0        0        0     1612 2024-02-22 03:29:19.475154 botifyme-0.1.2/botifyme/cli/common.py
--rw-r--r--   0        0        0     1117 2024-02-22 03:29:19.475523 botifyme-0.1.2/botifyme/cli/root.py
--rw-r--r--   0        0        0     2440 2024-02-22 17:49:39.110473 botifyme-0.1.2/botifyme/cli/worker.py
--rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.2/botifyme/registry.py
--rw-r--r--   0        0        0        0 2024-02-22 03:29:19.476068 botifyme-0.1.2/botifyme/utils/__init__.py
--rw-r--r--   0        0        0     3533 2024-02-23 02:37:51.479797 botifyme-0.1.2/botifyme/utils/tools.py
--rw-r--r--   0        0        0      826 2024-02-23 05:52:21.900837 botifyme-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 botifyme-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.3/LICENSE
+-rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.3/README.md
+-rw-r--r--   0        0        0      162 2024-04-23 20:15:22.599781 botifyme-0.1.3/botifyme/__init__.py
+-rw-r--r--   0        0        0     3008 2024-05-04 06:02:47.290817 botifyme-0.1.3/botifyme/__main__.py
+-rw-r--r--   0        0        0     1438 2024-04-23 20:15:22.599920 botifyme-0.1.3/botifyme/agent.py
+-rw-r--r--   0        0        0    11826 2024-05-04 06:02:47.291215 botifyme-0.1.3/botifyme/config.py
+-rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.3/botifyme/registry.py
+-rw-r--r--   0        0        0     4075 2024-05-03 05:36:25.537048 botifyme-0.1.3/botifyme/runtime.py
+-rw-r--r--   0        0        0      475 2024-04-23 20:15:22.600500 botifyme-0.1.3/botifyme/utils/__init__.py
+-rw-r--r--   0        0        0     3533 2024-03-14 23:09:57.824589 botifyme-0.1.3/botifyme/utils/tools.py
+-rw-r--r--   0        0        0     3640 2024-04-23 22:21:27.280737 botifyme-0.1.3/botifyme/workflow.py
+-rw-r--r--   0        0        0      869 2024-05-06 23:14:46.509546 botifyme-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 botifyme-0.1.3/PKG-INFO
```

### Comparing `botifyme-0.1.2/LICENSE` & `botifyme-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.2/botifyme/registry.py` & `botifyme-0.1.3/botifyme/registry.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.2/botifyme/utils/tools.py` & `botifyme-0.1.3/botifyme/utils/tools.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.2/pyproject.toml` & `botifyme-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botifyme"
-version = "0.1.2"
+version = "0.1.3"
 description = "Toolkit for building Autonomous AI agents"
 authors = ["Arun Reddy <arun@botifyme.dev>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -16,14 +16,16 @@
 httpx = "^0.26.0"
 toml = "^0.10.2"
 autoregistry = "^1.1.2"
 docstring-parser = "^0.15"
 loguru = "^0.7.2"
 python-dotenv = "^1.0.1"
 python-slugify = "^8.0.4"
+pydantic = "^2.7.0"
+cloudpickle = "^3.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `botifyme-0.1.2/PKG-INFO` & `botifyme-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: botifyme
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolkit for building Autonomous AI agents
 License: Apache-2.0
 Author: Arun Reddy
 Author-email: arun@botifyme.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autoregistry (>=1.1.2,<2.0.0)
+Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.1.2,<2.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
```

