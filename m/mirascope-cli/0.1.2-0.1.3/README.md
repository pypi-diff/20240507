# Comparing `tmp/mirascope_cli-0.1.2.tar.gz` & `tmp/mirascope_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope_cli-0.1.2.tar", max compression
+gzip compressed data, was "mirascope_cli-0.1.3.tar", max compression
```

## Comparing `mirascope_cli-0.1.2.tar` & `mirascope_cli-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0     7529 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/docs/README.md
--rw-r--r--   0        0        0       98 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/__init__.py
--rw-r--r--   0        0        0     4212 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/status.py
--rw-r--r--   0        0        0     2800 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/constants.py
--rw-r--r--   0        0        0      980 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/enums.py
--rw-r--r--   0        0        0       86 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1556 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/main.py
--rw-r--r--   0        0        0        0 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/py.typed
--rw-r--r--   0        0        0     1582 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/schemas.py
--rw-r--r--   0        0        0    26969 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/utils.py
--rw-r--r--   0        0        0     1804 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8319 1970-01-01 00:00:00.000000 mirascope_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7529 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/docs/README.md
+-rw-r--r--   0        0        0       98 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/__init__.py
+-rw-r--r--   0        0        0     4212 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/status.py
+-rw-r--r--   0        0        0     2800 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/constants.py
+-rw-r--r--   0        0        0      980 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/enums.py
+-rw-r--r--   0        0        0       86 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1556 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/py.typed
+-rw-r--r--   0        0        0     1582 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/schemas.py
+-rw-r--r--   0        0        0    26969 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/mirascope_cli/utils.py
+-rw-r--r--   0        0        0     1802 2024-05-06 23:04:13.909639 mirascope_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8319 1970-01-01 00:00:00.000000 mirascope_cli-0.1.3/PKG-INFO
```

### Comparing `mirascope_cli-0.1.2/LICENSE` & `mirascope_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/docs/README.md` & `mirascope_cli-0.1.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/commands/add.py` & `mirascope_cli-0.1.3/mirascope_cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/commands/init.py` & `mirascope_cli-0.1.3/mirascope_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/commands/remove.py` & `mirascope_cli-0.1.3/mirascope_cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/commands/status.py` & `mirascope_cli-0.1.3/mirascope_cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/commands/use.py` & `mirascope_cli-0.1.3/mirascope_cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/enums.py` & `mirascope_cli-0.1.3/mirascope_cli/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/generic/prompt_template.j2` & `mirascope_cli-0.1.3/mirascope_cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/main.py` & `mirascope_cli-0.1.3/mirascope_cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/schemas.py` & `mirascope_cli-0.1.3/mirascope_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/mirascope_cli/utils.py` & `mirascope_cli-0.1.3/mirascope_cli/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.2/pyproject.toml` & `mirascope_cli-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirascope-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "The Mirascope Command Line Interface"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
@@ -14,18 +14,18 @@
 [tool.poetry.scripts]
 mirascope = 'mirascope_cli.main:app'
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pydantic = "^2.0.2"
 typer = { version = ">=0.9.0,<1.0.0", extras = ["all"] }
-Jinja2 = "^3.1.3"
+Jinja2 = "^3.1.4"
 
 [tool.poetry.group.dev.dependencies]
-# mirascope = ">=0.9.1,<1.0.0"
+mirascope = ">=0.9.1,<1.0.0"
 mypy = "^1.6.1"
 pytest = "^7.4.0"
 ruff = "^0.1.5"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `mirascope_cli-0.1.2/PKG-INFO` & `mirascope_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mirascope-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Mirascope Command Line Interface
 Home-page: https://github.com/Mirascope/mirascope-cli
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: Jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<1.0.0)
 Project-URL: Repository, https://github.com/Mirascope/mirascope-cli
 Description-Content-Type: text/markdown
 
 # Using the Mirascope CLI
```

