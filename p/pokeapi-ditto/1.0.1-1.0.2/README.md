# Comparing `tmp/pokeapi_ditto-1.0.1.tar.gz` & `tmp/pokeapi_ditto-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokeapi_ditto-1.0.1.tar", max compression
+gzip compressed data, was "pokeapi_ditto-1.0.2.tar", max compression
```

## Comparing `pokeapi_ditto-1.0.1.tar` & `pokeapi_ditto-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11347 2024-05-06 20:43:28.157792 pokeapi_ditto-1.0.1/LICENSE
--rw-r--r--   0        0        0      742 2024-05-07 10:44:08.246518 pokeapi_ditto-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-06 20:43:28.159792 pokeapi_ditto-1.0.1/pokeapi_ditto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/__init__.py
--rw-r--r--   0        0        0     3014 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/analyze.py
--rw-r--r--   0        0        0     3292 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/clone.py
--rw-r--r--   0        0        0     4987 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/models.py
--rw-r--r--   0        0        0     1899 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/transform.py
--rw-r--r--   0        0        0      584 2024-05-06 20:43:28.162793 pokeapi_ditto-1.0.1/pokeapi_ditto/common.py
--rw-r--r--   0        0        0     1712 2024-05-06 20:43:28.162793 pokeapi_ditto-1.0.1/pokeapi_ditto/main.py
--rw-r--r--   0        0        0     1312 2024-05-07 10:42:36.452721 pokeapi_ditto-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 pokeapi_ditto-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-05-06 20:43:28.157792 pokeapi_ditto-1.0.2/LICENSE
+-rw-r--r--   0        0        0      848 2024-05-07 13:57:31.504424 pokeapi_ditto-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 20:43:28.159792 pokeapi_ditto-1.0.2/pokeapi_ditto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.2/pokeapi_ditto/commands/__init__.py
+-rw-r--r--   0        0        0     3014 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.2/pokeapi_ditto/commands/analyze.py
+-rw-r--r--   0        0        0     3292 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.2/pokeapi_ditto/commands/clone.py
+-rw-r--r--   0        0        0     4987 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.2/pokeapi_ditto/commands/models.py
+-rw-r--r--   0        0        0     1899 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.2/pokeapi_ditto/commands/transform.py
+-rw-r--r--   0        0        0      584 2024-05-06 20:43:28.162793 pokeapi_ditto-1.0.2/pokeapi_ditto/common.py
+-rw-r--r--   0        0        0     1704 2024-05-07 13:57:37.266915 pokeapi_ditto-1.0.2/pokeapi_ditto/main.py
+-rw-r--r--   0        0        0     1404 2024-05-07 13:57:37.279910 pokeapi_ditto-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 pokeapi_ditto-1.0.2/PKG-INFO
```

### Comparing `pokeapi_ditto-1.0.1/LICENSE` & `pokeapi_ditto-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/analyze.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/clone.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/commands/clone.py`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/models.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/commands/models.py`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/transform.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/commands/transform.py`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/common.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/common.py`

 * *Files identical despite different names*

### Comparing `pokeapi_ditto-1.0.1/pokeapi_ditto/main.py` & `pokeapi_ditto-1.0.2/pokeapi_ditto/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse
 import sys
-
-import pkg_resources
+import importlib.metadata
 
 from pokeapi_ditto.commands import analyze, clone, transform
 
 
 class Ditto(object):
     def __init__(self):
         parser = argparse.ArgumentParser()
         parser.add_argument(
             "--version",
             action="version",
-            version=pkg_resources.get_distribution("pokeapi-ditto").version,
+            version=importlib.metadata.version('pokeapi-ditto'),
         )
         subparsers = parser.add_subparsers(dest="command")
 
         clone_args = subparsers.add_parser("clone")
         clone_args.add_argument("--src-url", type=str, default="http://localhost/")
         clone_args.add_argument("--dest-dir", type=str, default="./data")
         clone_args.add_argument("--select", nargs="+", default=[])
```

### Comparing `pokeapi_ditto-1.0.1/pyproject.toml` & `pokeapi_ditto-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokeapi-ditto"
-version = "1.0.1"
+version = "1.0.2"
 description = "Ditto is a command line tool for performing meta operations over PokéAPI data."
 license = "Apache-2.0"
 authors = ["Sargun Vohra <sargun.vohra@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PokeAPI/ditto"
 repository = "https://github.com/PokeAPI/ditto.git"
 documentation = "https://github.com/PokeAPI/ditto"
@@ -13,14 +13,16 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.scripts]
 ditto = "pokeapi_ditto.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pokeapi_ditto-1.0.1/PKG-INFO` & `pokeapi_ditto-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokeapi-ditto
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ditto is a command line tool for performing meta operations over PokéAPI data.
 Home-page: https://github.com/PokeAPI/ditto
 License: Apache-2.0
 Keywords: pokeapi,ditto,pokemon
 Author: Sargun Vohra
 Author-email: sargun.vohra@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -22,15 +22,15 @@
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Requires-Dist: yarl (>=1.9,<2.0)
 Project-URL: Documentation, https://github.com/PokeAPI/ditto
 Project-URL: Repository, https://github.com/PokeAPI/ditto.git
 Description-Content-Type: text/markdown
 
-# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/132.svg' height='50px'/></a>
+# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/132.svg' height='50px'/></a> [![PyPI - Version](https://img.shields.io/pypi/v/pokeapi-ditto)](https://pypi.org/project/pokeapi-ditto/)
 
 This repository contains:
 
  - `ditto clone`: a script to crawl an instance of PokeAPI and download all data
  - `ditto analyze`: a script to generate a JSON schema of the above data
  - `ditto transform`: a script to apply a new base url to the above data and schema
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pokeapi-ditto Version: 1.0.1 Summary: Ditto is a
+Metadata-Version: 2.1 Name: pokeapi-ditto Version: 1.0.2 Summary: Ditto is a
 command line tool for performing meta operations over PokÃ©API data. Home-page:
 https://github.com/PokeAPI/ditto License: Apache-2.0 Keywords:
 pokeapi,ditto,pokemon Author: Sargun Vohra Author-email: sargun.vohra@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -10,15 +10,16 @@
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: 3.6 Requires-Dist: genson (>=1.2,<2.0) Requires-Dist:
 odictliteral (>=1.0,<2.0) Requires-Dist: requests (>=2.31,<3.0) Requires-Dist:
 tqdm (>=4.66,<5.0) Requires-Dist: yarl (>=1.9,<2.0) Project-URL: Documentation,
 https://github.com/PokeAPI/ditto Project-URL: Repository, https://github.com/
 PokeAPI/ditto.git Description-Content-Type: text/markdown # Ditto _[_h_t_t_p_s_:_/_/
 _r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_P_o_k_e_A_P_I_/_s_p_r_i_t_e_s_/_m_a_s_t_e_r_/_s_p_r_i_t_e_s_/_p_o_k_e_m_o_n_/_o_t_h_e_r_/_d_r_e_a_m_-
-_w_o_r_l_d_/_1_3_2_._s_v_g_]This repository contains: - `ditto clone`: a script to crawl an
-instance of PokeAPI and download all data - `ditto analyze`: a script to
-generate a JSON schema of the above data - `ditto transform`: a script to apply
-a new base url to the above data and schema ## Usage ```sh pip install pokeapi-
-ditto ditto --help ``` ## Development ```sh poetry install poetry run ditto --
-help ``` ## Docker You should have a PokeApi server running on `localhost:80`.
-```sh # runs clone, analyze, and transform all in one step docker-compose up --
-build ```
+_w_o_r_l_d_/_1_3_2_._s_v_g_][![PyPI - Version](https://img.shields.io/pypi/v/pokeapi-ditto)]
+(https://pypi.org/project/pokeapi-ditto/) This repository contains: - `ditto
+clone`: a script to crawl an instance of PokeAPI and download all data - `ditto
+analyze`: a script to generate a JSON schema of the above data - `ditto
+transform`: a script to apply a new base url to the above data and schema ##
+Usage ```sh pip install pokeapi-ditto ditto --help ``` ## Development ```sh
+poetry install poetry run ditto --help ``` ## Docker You should have a PokeApi
+server running on `localhost:80`. ```sh # runs clone, analyze, and transform
+all in one step docker-compose up --build ```
```

