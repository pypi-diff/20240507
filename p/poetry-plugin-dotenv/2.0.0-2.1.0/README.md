# Comparing `tmp/poetry_plugin_dotenv-2.0.0.tar.gz` & `tmp/poetry_plugin_dotenv-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-2.0.0.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-2.1.0.tar", max compression
```

## Comparing `poetry_plugin_dotenv-2.0.0.tar` & `poetry_plugin_dotenv-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-05-06 20:55:24.914678 poetry_plugin_dotenv-2.0.0/LICENSE
--rw-r--r--   0        0        0     9687 2024-05-06 20:55:24.914678 poetry_plugin_dotenv-2.0.0/README.md
--rw-r--r--   0        0        0     6906 2024-05-06 20:55:45.866966 poetry_plugin_dotenv-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      778 2024-05-06 20:55:45.866966 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/config.py
--rw-r--r--   0        0        0      335 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5421 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6005 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1572 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     1558 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/logger.py
--rw-r--r--   0        0        0     1999 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-06 21:02:52.390435 poetry_plugin_dotenv-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9687 2024-05-06 21:02:52.390435 poetry_plugin_dotenv-2.1.0/README.md
+-rw-r--r--   0        0        0     6955 2024-05-06 21:03:13.318497 poetry_plugin_dotenv-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-05-06 21:03:13.318497 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     1558 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:02:52.402435 poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.0/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-2.0.0/LICENSE` & `poetry_plugin_dotenv-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/README.md` & `poetry_plugin_dotenv-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/pyproject.toml` & `poetry_plugin_dotenv-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "2.0.0"
+version = "2.1.0"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
@@ -32,14 +32,15 @@
   "Environment :: Other Environment",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Scientific/Engineering",
   "Natural Language :: English",
@@ -127,15 +128,15 @@
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "semver"
 version_provider = "poetry"
-allowed_prefixes = ["build", "tests", "Merge", "Initial", "0", "1"]
+allowed_prefixes = ["build", "tests", "Merge", "Initial", "0", "1", "2"]
 
 [tool.isort]
 profile = "black"
 line_length = 100
 lines_after_imports = 2
 lines_between_types = 1
 atomic = false
```

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/config.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/config.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/logger.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/logger.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-2.1.0/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.0.0/PKG-INFO` & `poetry_plugin_dotenv-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 2.0.0
+Version: 2.1.0
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.0 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
```

