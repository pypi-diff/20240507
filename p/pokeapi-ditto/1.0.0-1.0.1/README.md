# Comparing `tmp/pokeapi-ditto-1.0.0.tar.gz` & `tmp/pokeapi_ditto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokeapi-ditto-1.0.0.tar", last modified: Mon Aug 10 10:35:03 2020, max compression
+gzip compressed data, was "pokeapi_ditto-1.0.1.tar", max compression
```

## Comparing `pokeapi-ditto-1.0.0.tar` & `pokeapi_ditto-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11347 2020-08-06 14:08:20.058780 pokeapi-ditto-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-08-10 08:49:07.799035 pokeapi-ditto-1.0.0/pokeapi_ditto/__init__.py
--rw-r--r--   0        0        0        0 2020-08-10 08:49:07.800024 pokeapi-ditto-1.0.0/pokeapi_ditto/commands/__init__.py
--rw-r--r--   0        0        0     3014 2020-08-10 08:49:07.801069 pokeapi-ditto-1.0.0/pokeapi_ditto/commands/analyze.py
--rw-r--r--   0        0        0     3292 2020-08-10 08:49:07.802021 pokeapi-ditto-1.0.0/pokeapi_ditto/commands/clone.py
--rw-r--r--   0        0        0     4987 2020-08-10 08:49:07.803022 pokeapi-ditto-1.0.0/pokeapi_ditto/commands/models.py
--rw-r--r--   0        0        0     1899 2020-08-10 08:49:07.806026 pokeapi-ditto-1.0.0/pokeapi_ditto/commands/transform.py
--rw-r--r--   0        0        0      584 2020-08-10 08:49:07.807050 pokeapi-ditto-1.0.0/pokeapi_ditto/common.py
--rw-r--r--   0        0        0     1712 2020-08-10 08:49:07.808025 pokeapi-ditto-1.0.0/pokeapi_ditto/main.py
--rw-r--r--   0        0        0     1257 2020-08-10 08:49:07.809026 pokeapi-ditto-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      698 2020-08-10 08:49:07.798023 pokeapi-ditto-1.0.0/README.md
--rw-r--r--   0        0        0     1656 2020-08-10 10:35:03.931696 pokeapi-ditto-1.0.0/setup.py
--rw-r--r--   0        0        0     1776 2020-08-10 10:35:03.932696 pokeapi-ditto-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-05-06 20:43:28.157792 pokeapi_ditto-1.0.1/LICENSE
+-rw-r--r--   0        0        0      742 2024-05-07 10:44:08.246518 pokeapi_ditto-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 20:43:28.159792 pokeapi_ditto-1.0.1/pokeapi_ditto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/__init__.py
+-rw-r--r--   0        0        0     3014 2024-05-06 20:43:28.160792 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/analyze.py
+-rw-r--r--   0        0        0     3292 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/clone.py
+-rw-r--r--   0        0        0     4987 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/models.py
+-rw-r--r--   0        0        0     1899 2024-05-06 20:43:28.161791 pokeapi_ditto-1.0.1/pokeapi_ditto/commands/transform.py
+-rw-r--r--   0        0        0      584 2024-05-06 20:43:28.162793 pokeapi_ditto-1.0.1/pokeapi_ditto/common.py
+-rw-r--r--   0        0        0     1712 2024-05-06 20:43:28.162793 pokeapi_ditto-1.0.1/pokeapi_ditto/main.py
+-rw-r--r--   0        0        0     1312 2024-05-07 10:42:36.452721 pokeapi_ditto-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 pokeapi_ditto-1.0.1/PKG-INFO
```

### Comparing `pokeapi-ditto-1.0.0/LICENSE` & `pokeapi_ditto-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/commands/analyze.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/commands/clone.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/clone.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/commands/models.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/models.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/commands/transform.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/commands/transform.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/common.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/common.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pokeapi_ditto/main.py` & `pokeapi_ditto-1.0.1/pokeapi_ditto/main.py`

 * *Files identical despite different names*

### Comparing `pokeapi-ditto-1.0.0/pyproject.toml` & `pokeapi_ditto-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokeapi-ditto"
-version = "1.0.0"
+version = "1.0.1"
 description = "Ditto is a command line tool for performing meta operations over PokéAPI data."
 license = "Apache-2.0"
 authors = ["Sargun Vohra <sargun.vohra@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PokeAPI/ditto"
 repository = "https://github.com/PokeAPI/ditto.git"
 documentation = "https://github.com/PokeAPI/ditto"
@@ -12,36 +12,37 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.scripts]
 ditto = "pokeapi_ditto.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-requests = "^2.19"
-genson = "^1.0"
-tqdm = "^4.26"
+python = "^3.10"
+requests = "^2.31"
+genson = "^1.2"
+tqdm = "^4.66"
 odictliteral = "^1.0"
-yarl = "^1.2"
+yarl = "^1.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^3.0"
-flake8 = "^3.5"
-black = "^18.3-alpha.0"
-isort = "^4.3"
+pytest = "^8.2"
+flake8 = "^7.0"
+black = "^24.4"
+isort = "^5.13"
 
 [tool.black]
 line-length = 88
-py36 = true
+target-version = ['py310']
 
 [tool.isort]
 skip = [".venv", "venv", ".git", "__pycache__", "dist", "data"]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 combine_as_imports = true
```

### Comparing `pokeapi-ditto-1.0.0/README.md` & `pokeapi_ditto-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://veekun.com/dex/media/pokemon/global-link/132.png' height=50px/></a>
+# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/132.svg' height='50px'/></a>
 
 This repository contains:
 
  - `ditto clone`: a script to crawl an instance of PokeAPI and download all data
  - `ditto analyze`: a script to generate a JSON schema of the above data
  - `ditto transform`: a script to apply a new base url to the above data and schema
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-# Ditto _[_h_t_t_p_s_:_/_/_v_e_e_k_u_n_._c_o_m_/_d_e_x_/_m_e_d_i_a_/_p_o_k_e_m_o_n_/_g_l_o_b_a_l_-_l_i_n_k_/_1_3_2_._p_n_g_]This
-repository contains: - `ditto clone`: a script to crawl an instance of PokeAPI
-and download all data - `ditto analyze`: a script to generate a JSON schema of
-the above data - `ditto transform`: a script to apply a new base url to the
-above data and schema ## Usage ```sh pip install pokeapi-ditto ditto --help ```
-## Development ```sh poetry install poetry run ditto --help ``` ## Docker You
-should have a PokeApi server running on `localhost:80`. ```sh # runs clone,
-analyze, and transform all in one step docker-compose up --build ```
+# Ditto _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_P_o_k_e_A_P_I_/_s_p_r_i_t_e_s_/_m_a_s_t_e_r_/_s_p_r_i_t_e_s_/
+_p_o_k_e_m_o_n_/_o_t_h_e_r_/_d_r_e_a_m_-_w_o_r_l_d_/_1_3_2_._s_v_g_]This repository contains: - `ditto clone`: a
+script to crawl an instance of PokeAPI and download all data - `ditto analyze`:
+a script to generate a JSON schema of the above data - `ditto transform`: a
+script to apply a new base url to the above data and schema ## Usage ```sh pip
+install pokeapi-ditto ditto --help ``` ## Development ```sh poetry install
+poetry run ditto --help ``` ## Docker You should have a PokeApi server running
+on `localhost:80`. ```sh # runs clone, analyze, and transform all in one step
+docker-compose up --build ```
```

### Comparing `pokeapi-ditto-1.0.0/PKG-INFO` & `pokeapi_ditto-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: pokeapi-ditto
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ditto is a command line tool for performing meta operations over PokéAPI data.
 Home-page: https://github.com/PokeAPI/ditto
 License: Apache-2.0
 Keywords: pokeapi,ditto,pokemon
 Author: Sargun Vohra
 Author-email: sargun.vohra@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: genson (>=1.0,<2.0)
+Requires-Dist: genson (>=1.2,<2.0)
 Requires-Dist: odictliteral (>=1.0,<2.0)
-Requires-Dist: requests (>=2.19,<3.0)
-Requires-Dist: tqdm (>=4.26,<5.0)
-Requires-Dist: yarl (>=1.2,<2.0)
+Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: tqdm (>=4.66,<5.0)
+Requires-Dist: yarl (>=1.9,<2.0)
 Project-URL: Documentation, https://github.com/PokeAPI/ditto
 Project-URL: Repository, https://github.com/PokeAPI/ditto.git
 Description-Content-Type: text/markdown
 
-# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://veekun.com/dex/media/pokemon/global-link/132.png' height=50px/></a>
+# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/132.svg' height='50px'/></a>
 
 This repository contains:
 
  - `ditto clone`: a script to crawl an instance of PokeAPI and download all data
  - `ditto analyze`: a script to generate a JSON schema of the above data
  - `ditto transform`: a script to apply a new base url to the above data and schema
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: pokeapi-ditto Version: 1.0.0 Summary: Ditto is a
+Metadata-Version: 2.1 Name: pokeapi-ditto Version: 1.0.1 Summary: Ditto is a
 command line tool for performing meta operations over PokÃ©API data. Home-page:
 https://github.com/PokeAPI/ditto License: Apache-2.0 Keywords:
 pokeapi,ditto,pokemon Author: Sargun Vohra Author-email: sargun.vohra@gmail.com
-Requires-Python: >=3.6,<4.0 Classifier: Development Status :: 5 - Production/
+Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Requires-Dist: genson
-(>=1.0,<2.0) Requires-Dist: odictliteral (>=1.0,<2.0) Requires-Dist: requests
-(>=2.19,<3.0) Requires-Dist: tqdm (>=4.26,<5.0) Requires-Dist: yarl
-(>=1.2,<2.0) Project-URL: Documentation, https://github.com/PokeAPI/ditto
-Project-URL: Repository, https://github.com/PokeAPI/ditto.git Description-
-Content-Type: text/markdown # Ditto _[_h_t_t_p_s_:_/_/_v_e_e_k_u_n_._c_o_m_/_d_e_x_/_m_e_d_i_a_/_p_o_k_e_m_o_n_/
-_g_l_o_b_a_l_-_l_i_n_k_/_1_3_2_._p_n_g_]This repository contains: - `ditto clone`: a script to
-crawl an instance of PokeAPI and download all data - `ditto analyze`: a script
-to generate a JSON schema of the above data - `ditto transform`: a script to
-apply a new base url to the above data and schema ## Usage ```sh pip install
-pokeapi-ditto ditto --help ``` ## Development ```sh poetry install poetry run
-ditto --help ``` ## Docker You should have a PokeApi server running on
-`localhost:80`. ```sh # runs clone, analyze, and transform all in one step
-docker-compose up --build ```
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3.6 Requires-Dist: genson (>=1.2,<2.0) Requires-Dist:
+odictliteral (>=1.0,<2.0) Requires-Dist: requests (>=2.31,<3.0) Requires-Dist:
+tqdm (>=4.66,<5.0) Requires-Dist: yarl (>=1.9,<2.0) Project-URL: Documentation,
+https://github.com/PokeAPI/ditto Project-URL: Repository, https://github.com/
+PokeAPI/ditto.git Description-Content-Type: text/markdown # Ditto _[_h_t_t_p_s_:_/_/
+_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_P_o_k_e_A_P_I_/_s_p_r_i_t_e_s_/_m_a_s_t_e_r_/_s_p_r_i_t_e_s_/_p_o_k_e_m_o_n_/_o_t_h_e_r_/_d_r_e_a_m_-
+_w_o_r_l_d_/_1_3_2_._s_v_g_]This repository contains: - `ditto clone`: a script to crawl an
+instance of PokeAPI and download all data - `ditto analyze`: a script to
+generate a JSON schema of the above data - `ditto transform`: a script to apply
+a new base url to the above data and schema ## Usage ```sh pip install pokeapi-
+ditto ditto --help ``` ## Development ```sh poetry install poetry run ditto --
+help ``` ## Docker You should have a PokeApi server running on `localhost:80`.
+```sh # runs clone, analyze, and transform all in one step docker-compose up --
+build ```
```

