# Comparing `tmp/nipe_py-0.0.1.tar.gz` & `tmp/nipe_py-0.0.2.tar.gz`

## Comparing `nipe_py-0.0.1.tar` & `nipe_py-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.cruft.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 nipe_py-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.configs/arch-torrc
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.configs/centos-torrc
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.configs/debian-torrc
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.configs/fedora-torrc
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.configs/void-torrc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/release-drafter.yml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/workflows/draft.yml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.1/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.1/assets/demo.gif
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nipe_py-0.0.1/docs/index.md
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/py.typed
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/engine/Restart.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/engine/Start.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/engine/Stop.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/utils/Device.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/utils/Install.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.0.1/src/nipe_py/utils/Status.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.0.1/LICENSE
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 nipe_py-0.0.1/README.md
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 nipe_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 nipe_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.cruft.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nipe_py-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/arch-torrc
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/centos-torrc
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/debian-torrc
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/fedora-torrc
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/void-torrc
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/release-drafter.yml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/draft.yml
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.2/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.2/assets/demo.gif
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 nipe_py-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Restart.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Start.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Stop.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Device.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Install.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Status.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 nipe_py-0.0.2/README.md
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 nipe_py-0.0.2/PKG-INFO
```

### Comparing `nipe_py-0.0.1/.cruft.json` & `nipe_py-0.0.2/.cruft.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941176470588236%*

 * *Differences: {"'context'": "{'cookiecutter': {'github_username': 'aviksaikat', 'repository_name': "*

 * *              "'aviksaikat/nipe_py', 'repository_url': 'https://github.com/aviksaikat/nipe_py', "*

 * *              "'docs_url': 'https://aviksaikat.github.io/nipe_py/'}}"}*

```diff
@@ -5,23 +5,23 @@
         "cookiecutter": {
             "_template": "https://github.com/frankie567/cookiecutter-hipster-pypackage",
             "asyncio": "N",
             "dist_name": "nipe_py",
             "docs_color_accent": "deep purple",
             "docs_color_primary": "deep purple",
             "docs_icon": "material/library",
-            "docs_url": "https://avik_saikat.github.io/nipe_py/",
+            "docs_url": "https://aviksaikat.github.io/nipe_py/",
             "email": "king.arthur@camelot.bt",
             "full_name": "Saikat Karmakar",
-            "github_username": "avik_saikat",
+            "github_username": "aviksaikat",
             "open_source_license": "MIT license",
             "package_name": "nipe_py",
             "project_name": "nipe_py",
             "project_short_description": "",
             "python_version": "3.11",
-            "repository_name": "avik_saikat/nipe_py",
-            "repository_url": "https://github.com/avik_saikat/nipe_py"
+            "repository_name": "aviksaikat/nipe_py",
+            "repository_url": "https://github.com/aviksaikat/nipe_py"
         }
     },
     "directory": null,
     "template": "https://github.com/frankie567/cookiecutter-hipster-pypackage"
 }
```

### Comparing `nipe_py-0.0.1/mkdocs.yml` & `nipe_py-0.0.2/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 site_name: nipe_py
 site_description: 
 
-repo_url: https://github.com/avik_saikat/nipe_py
-repo_name: avik_saikat/nipe_py
+repo_url: https://github.com/aviksaikat/nipe_py
+repo_name: aviksaikat/nipe_py
 
 theme:
     name: material
     icon:
         logo: material/library
     palette:
         # Palette toggle for automatic mode
```

### Comparing `nipe_py-0.0.1/.github/release-drafter.yml` & `nipe_py-0.0.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `nipe_py-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/.github/workflows/documentation.yml` & `nipe_py-0.0.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/.github/workflows/release.yml` & `nipe_py-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/assets/banner.png` & `nipe_py-0.0.2/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/assets/demo.gif` & `nipe_py-0.0.2/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/docs/index.md` & `nipe_py-0.0.2/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 ---
 
-**Documentation**: <a href="https://avik_saikat.github.io/nipe_py/" target="_blank">https://avik_saikat.github.io/nipe_py/</a>
+**Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
-**Source Code**: <a href="https://github.com/avik_saikat/nipe_py" target="_blank">https://github.com/avik_saikat/nipe_py</a>
+**Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
 
 Python version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # nipe_py
                             [../assets/banner.png]
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
 py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
 aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/
-_a_v_i_k___s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k___s_a_i_k_a_t_/
-_n_i_p_e___p_y --- Python version of [nipe](https://github.com/htrgouvea/nipe): An
-engine to make Tor Network your default gateway. ## Installation ```sh pip
-install nipe_py ``` ## Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: install Install
-dependencies restart Restart the Nipe circuit start Start routing status See
-status stop Stop routing ``` ## Demo ![](../assets/demo.gif) ## License This
-project is licensed under the terms of the MIT license.
+nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
+_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
+version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
+Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
+Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
+help Show this message and exit. Commands: install Install dependencies restart
+Restart the Nipe circuit start Start routing status See status stop Stop
+routing ``` ## Demo ![](../assets/demo.gif) ## License This project is licensed
+under the terms of the MIT license.
```

### Comparing `nipe_py-0.0.1/src/nipe_py/main.py` & `nipe_py-0.0.2/src/nipe_py/main.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/src/nipe_py/engine/Start.py` & `nipe_py-0.0.2/src/nipe_py/engine/Start.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/src/nipe_py/engine/Stop.py` & `nipe_py-0.0.2/src/nipe_py/engine/Stop.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/src/nipe_py/utils/Device.py` & `nipe_py-0.0.2/src/nipe_py/utils/Device.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/src/nipe_py/utils/Install.py` & `nipe_py-0.0.2/src/nipe_py/utils/Install.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/src/nipe_py/utils/Status.py` & `nipe_py-0.0.2/src/nipe_py/utils/Status.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/.gitignore` & `nipe_py-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/LICENSE` & `nipe_py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.1/README.md` & `nipe_py-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 ---
 
-**Documentation**: <a href="https://avik_saikat.github.io/nipe_py/" target="_blank">https://avik_saikat.github.io/nipe_py/</a>
+**Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
-**Source Code**: <a href="https://github.com/avik_saikat/nipe_py" target="_blank">https://github.com/avik_saikat/nipe_py</a>
+**Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
 
 Python version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # nipe_py
                              [./assets/banner.png]
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
 py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
 aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/
-_a_v_i_k___s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k___s_a_i_k_a_t_/
-_n_i_p_e___p_y --- Python version of [nipe](https://github.com/htrgouvea/nipe): An
-engine to make Tor Network your default gateway. ## Installation ```sh pip
-install nipe_py ``` ## Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: install Install
-dependencies restart Restart the Nipe circuit start Start routing status See
-status stop Stop routing ``` ## Demo ![](./assets/demo.gif) ## License This
-project is licensed under the terms of the MIT license.
+nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
+_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
+version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
+Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
+Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
+help Show this message and exit. Commands: install Install dependencies restart
+Restart the Nipe circuit start Start routing status See status stop Stop
+routing ``` ## Demo ![](./assets/demo.gif) ## License This project is licensed
+under the terms of the MIT license.
```

### Comparing `nipe_py-0.0.1/pyproject.toml` & `nipe_py-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 dependencies = [
   "requests",
   "rich",
   "click"
 ]
 
 [project.urls]
-Documentation = "https://avik_saikat.github.io/nipe_py/"
-Source = "https://github.com/avik_saikat/nipe_py"
+Documentation = "https://aviksaikat.github.io/nipe_py/"
+Source = "https://github.com/aviksaikat/nipe_py"
 
 # mypy
 [tool.mypy]
 exclude = ["build/", "dist/", "docs/", "tests/*"]
 check_untyped_defs = true
 plugins = ["pydantic.mypy"]
```

### Comparing `nipe_py-0.0.1/PKG-INFO` & `nipe_py-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: nipe_py
-Version: 0.0.1
+Version: 0.0.2
 Summary: An engine to make Tor Network your default gateway.
-Project-URL: Documentation, https://avik_saikat.github.io/nipe_py/
-Project-URL: Source, https://github.com/avik_saikat/nipe_py
+Project-URL: Documentation, https://aviksaikat.github.io/nipe_py/
+Project-URL: Source, https://github.com/aviksaikat/nipe_py
 Author-email: nipe_py <saikickkarma@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024, Saikat Karmakar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -50,17 +50,17 @@
 
 
 
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 ---
 
-**Documentation**: <a href="https://avik_saikat.github.io/nipe_py/" target="_blank">https://avik_saikat.github.io/nipe_py/</a>
+**Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
-**Source Code**: <a href="https://github.com/avik_saikat/nipe_py" target="_blank">https://github.com/avik_saikat/nipe_py</a>
+**Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
 
 Python version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.3 Name: nipe_py Version: 0.0.1 Summary: An engine to make
+Metadata-Version: 2.3 Name: nipe_py Version: 0.0.2 Summary: An engine to make
 Tor Network your default gateway. Project-URL: Documentation, https://
-avik_saikat.github.io/nipe_py/ Project-URL: Source, https://github.com/
-avik_saikat/nipe_py Author-email: nipe_py
+aviksaikat.github.io/nipe_py/ Project-URL: Source, https://github.com/
+aviksaikat/nipe_py Author-email: nipe_py
 protonmail.com> License: MIT License Copyright (c) 2024, Saikat Karmakar
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions: The above copyright notice and this
@@ -25,16 +25,16 @@
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.9 Requires-
 Dist: click Requires-Dist: requests Requires-Dist: rich Description-Content-
 Type: text/markdown # nipe_py
                              [./assets/banner.png]
 [![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
 py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
 aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/
-_a_v_i_k___s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k___s_a_i_k_a_t_/
-_n_i_p_e___p_y --- Python version of [nipe](https://github.com/htrgouvea/nipe): An
-engine to make Tor Network your default gateway. ## Installation ```sh pip
-install nipe_py ``` ## Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND
-[ARGS]... Options: --help Show this message and exit. Commands: install Install
-dependencies restart Restart the Nipe circuit start Start routing status See
-status stop Stop routing ``` ## Demo ![](./assets/demo.gif) ## License This
-project is licensed under the terms of the MIT license.
+nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
+_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
+version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
+Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
+Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
+help Show this message and exit. Commands: install Install dependencies restart
+Restart the Nipe circuit start Start routing status See status stop Stop
+routing ``` ## Demo ![](./assets/demo.gif) ## License This project is licensed
+under the terms of the MIT license.
```

