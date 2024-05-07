# Comparing `tmp/pynpc-0.2.2.tar.gz` & `tmp/pynpc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynpc-0.2.2.tar", max compression
+gzip compressed data, was "pynpc-0.3.0.tar", max compression
```

## Comparing `pynpc-0.2.2.tar` & `pynpc-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1063 2024-02-27 09:21:33.759607 pynpc-0.2.2/LICENSE
--rw-r--r--   0        0        0     1749 2024-02-27 09:21:33.759607 pynpc-0.2.2/README.md
--rw-r--r--   0        0        0      189 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/__init__.py
--rw-r--r--   0        0        0    10282 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/console.py
--rw-r--r--   0        0        0    18949 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/archetypes.res.json
--rw-r--r--   0        0        0     8252 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/archetypes.txt
--rw-r--r--   0        0        0    80611 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/cards.res.json
--rw-r--r--   0        0        0     8363 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/fantasy-professions.res.json
--rw-r--r--   0        0        0      843 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/fantasy-professions.txt
--rw-r--r--   0        0        0     3176 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/idiosyncrasies.res.json
--rw-r--r--   0        0        0      662 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/idiosyncrasies.txt
--rw-r--r--   0        0        0      739 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/name-corruption-pattern.json
--rw-r--r--   0        0        0     3240 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/personalities.res.json
--rw-r--r--   0        0        0    24985 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/phobia.res.json
--rw-r--r--   0        0        0     9672 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/data/phobia.txt
--rw-r--r--   0        0        0     2892 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/name_corruptor.py
--rw-r--r--   0        0        0     8917 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/npc.py
--rw-r--r--   0        0        0      733 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/skills.py
--rw-r--r--   0        0        0     2877 2024-02-27 09:21:33.759607 pynpc-0.2.2/pynpc/utils.py
--rw-r--r--   0        0        0     7336 2024-02-27 09:22:10.139405 pynpc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 pynpc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-07 09:02:55.106720 pynpc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1749 2024-05-07 09:02:55.106720 pynpc-0.3.0/README.md
+-rw-r--r--   0        0        0      189 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/__init__.py
+-rw-r--r--   0        0        0    10282 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/console.py
+-rw-r--r--   0        0        0    18949 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/archetypes.res.json
+-rw-r--r--   0        0        0     8252 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/archetypes.txt
+-rw-r--r--   0        0        0    80611 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/cards.res.json
+-rw-r--r--   0        0        0     8363 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/fantasy-professions.res.json
+-rw-r--r--   0        0        0      843 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/fantasy-professions.txt
+-rw-r--r--   0        0        0     3176 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/idiosyncrasies.res.json
+-rw-r--r--   0        0        0      662 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/idiosyncrasies.txt
+-rw-r--r--   0        0        0      739 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/name-corruption-pattern.json
+-rw-r--r--   0        0        0     3240 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/personalities.res.json
+-rw-r--r--   0        0        0    24985 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/phobia.res.json
+-rw-r--r--   0        0        0     9672 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/data/phobia.txt
+-rw-r--r--   0        0        0     2892 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/name_corruptor.py
+-rw-r--r--   0        0        0     8917 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/npc.py
+-rw-r--r--   0        0        0      733 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/skills.py
+-rw-r--r--   0        0        0     2877 2024-05-07 09:02:55.110720 pynpc-0.3.0/pynpc/utils.py
+-rw-r--r--   0        0        0     7337 2024-05-07 09:03:30.510697 pynpc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 pynpc-0.3.0/PKG-INFO
```

### Comparing `pynpc-0.2.2/LICENSE` & `pynpc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/README.md` & `pynpc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/console.py` & `pynpc-0.3.0/pynpc/console.py`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/archetypes.res.json` & `pynpc-0.3.0/pynpc/data/archetypes.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/archetypes.txt` & `pynpc-0.3.0/pynpc/data/archetypes.txt`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/cards.res.json` & `pynpc-0.3.0/pynpc/data/cards.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/fantasy-professions.res.json` & `pynpc-0.3.0/pynpc/data/fantasy-professions.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/fantasy-professions.txt` & `pynpc-0.3.0/pynpc/data/fantasy-professions.txt`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/idiosyncrasies.res.json` & `pynpc-0.3.0/pynpc/data/idiosyncrasies.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/idiosyncrasies.txt` & `pynpc-0.3.0/pynpc/data/idiosyncrasies.txt`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/name-corruption-pattern.json` & `pynpc-0.3.0/pynpc/data/name-corruption-pattern.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/personalities.res.json` & `pynpc-0.3.0/pynpc/data/personalities.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/phobia.res.json` & `pynpc-0.3.0/pynpc/data/phobia.res.json`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/data/phobia.txt` & `pynpc-0.3.0/pynpc/data/phobia.txt`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/name_corruptor.py` & `pynpc-0.3.0/pynpc/name_corruptor.py`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/npc.py` & `pynpc-0.3.0/pynpc/npc.py`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/skills.py` & `pynpc-0.3.0/pynpc/skills.py`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pynpc/utils.py` & `pynpc-0.3.0/pynpc/utils.py`

 * *Files identical despite different names*

### Comparing `pynpc-0.2.2/pyproject.toml` & `pynpc-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 [tool.poetry]
 name = "pynpc"
-version = "0.2.2"
+version = "0.3.0"
 description = "Generate simple NPCs for table top role playing games"
 authors = ["Dr Yann Golanski <github@kierun.org>"]
 keywords = ["ttrpg", "rpg", "generate", "NPC"]
 license = "MIT"
 homepage = "https://github.com/kierun/pynpc"
 repository = "https://github.com/kierun/pynpc"
 readme = "README.md"
 packages = [{ include = "pynpc" }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-rich = "^13.7.0"
+rich = "^13.7.1"
 click = "^8.1.7"
 click-help-colors = "^0.9.4"
 pendulum = "^3.0.0"
 structlog = ">=23.3,<25.0"
 requests = "^2.31.0"
-types-requests = "^2.31.0.20240218"
-orjson = "^3.9.15"
+types-requests = "^2.31.0.20240406"
+orjson = "^3.10.3"
 mimesis = "^14.0.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 typer-config = { extras = ["all"], version = "^1.4.0" }
 unidecode = "^1.3.8"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.12.1,<25.0.0"
 isort = "^5.13.2"
-pytest = ">=8.0.2"
-mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.11"
+pytest = ">=8.2.0"
+mkdocs = "^1.6.0"
+mkdocs-material = "^9.5.21"
 mkdocstrings = "^0.24.0"
-mypy = "^1.8.0"
-pre-commit = "^3.6.2"
-coverage = "^7.4.3"
-bandit = "^1.7.7"
+mypy = "^1.10.0"
+pre-commit = "^3.7.0"
+coverage = "^7.5.1"
+bandit = "^1.7.8"
 pytest-skip-slow = "^0.0.5"
-commitizen = "^3.16.0"
+commitizen = "^3.25.0"
 python-semantic-release = "^8.7.0"
 pytest-cov = "^4.1.0"
 pydocstyle = "^6.3.0"
 ruff = "^0.2.1"
 dlint = "^0.14.1"
 pytest-sugar = "^0.9.7"
-requests-mock = "^1.11.0"
+requests-mock = "^1.12.1"
 ptpython = "^3.0.26"
 pdbpp = "^0.10.3"
 poetry-plugin-up = "^0.7.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pynpc-0.2.2/PKG-INFO` & `pynpc-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpc
-Version: 0.2.2
+Version: 0.3.0
 Summary: Generate simple NPCs for table top role playing games
 Home-page: https://github.com/kierun/pynpc
 License: MIT
 Keywords: ttrpg,rpg,generate,NPC
 Author: Dr Yann Golanski
 Author-email: github@kierun.org
 Requires-Python: >=3.10,<4.0
@@ -12,22 +12,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.4,<0.10.0)
 Requires-Dist: mimesis (>=14.0.0,<15.0.0)
-Requires-Dist: orjson (>=3.9.15,<4.0.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: structlog (>=23.3,<25.0)
 Requires-Dist: typer-config[all] (>=1.4.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
-Requires-Dist: types-requests (>=2.31.0.20240218,<3.0.0.0)
+Requires-Dist: types-requests (>=2.31.0.20240406,<3.0.0.0)
 Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Project-URL: Repository, https://github.com/kierun/pynpc
 Description-Content-Type: text/markdown
 
 # pynpc
 
 [![PyPi status](https://img.shields.io/pypi/status/pynpc)](https://img.shields.io/pypi/status/pynpc)
```

