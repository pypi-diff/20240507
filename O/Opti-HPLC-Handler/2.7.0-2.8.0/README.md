# Comparing `tmp/opti_hplc_handler-2.7.0.tar.gz` & `tmp/opti_hplc_handler-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opti_hplc_handler-2.7.0.tar", last modified: Mon May  6 06:49:57 2024, max compression
+gzip compressed data, was "opti_hplc_handler-2.8.0.tar", last modified: Tue May  7 07:53:49 2024, max compression
```

## Comparing `opti_hplc_handler-2.7.0.tar` & `opti_hplc_handler-2.8.0.tar`

### file list

```diff
@@ -1,30 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 06:49:43.000000 opti_hplc_handler-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:49:57.678278 opti_hplc_handler-2.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.670278 opti_hplc_handler-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 06:49:43.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_api_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_module_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_gradient_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_method_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 06:49:57.000000 opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:49:57.674278 opti_hplc_handler-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_instrument_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    50054 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_module_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_proxy_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-06 06:49:34.000000 opti_hplc_handler-2.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.316170 opti_hplc_handler-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-07 07:53:49.316170 opti_hplc_handler-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 07:53:33.000000 opti_hplc_handler-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:53:49.316170 opti_hplc_handler-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.308169 opti_hplc_handler-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.312169 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 07:53:33.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.312169 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.312169 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/empower_implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.312169 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/alter_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/method_generators/ramp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/applications/revert_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_api_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15927 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_module_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.312169 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/validate_gradient_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/validate_method_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.316170 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-07 07:53:49.000000 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 07:53:49.000000 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:53:49.000000 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 07:53:49.000000 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 07:53:49.000000 opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:53:49.316170 opti_hplc_handler-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/tests/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/tests/test_instrument_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50054 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/tests/test_module_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23590 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/tests/test_proxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-07 07:53:23.000000 opti_hplc_handler-2.8.0/tests/test_utils.py
```

### Comparing `opti_hplc_handler-2.7.0/LICENSE` & `opti_hplc_handler-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/PKG-INFO` & `opti_hplc_handler-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.7.0
+Version: 2.8.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
@@ -65,14 +65,16 @@
 Provides-Extra: release
 Requires-Dist: bumpver==2023.1125; extra == "release"
 Provides-Extra: build
 Requires-Dist: build==1.0.3; extra == "build"
 Provides-Extra: doc
 Requires-Dist: pylint==3.0.2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
+Provides-Extra: examples
+Requires-Dist: python-dotenv==1.0.1; extra == "examples"
 
 # OptiHPLCHandler
 
 <a href="https://pypi.python.org/pypi/Opti-HPLC-Handler"><img src="https://img.shields.io/pypi/v/Opti-HPLC-Handler.svg" alt="PyPI Version"></a>
 <a href="https://zenodo.org/doi/10.5281/zenodo.8386699"><img src="https://zenodo.org/badge/673355902.svg" alt="Zenodo DOI"></a>
 <a href="https://github.com/novonordisk-research/OptiHPLCHandler/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/Opti-HPLC-Handler.svg" alt="License"></a>
 <a href="https://pepy.tech/project/opti-hplc-handler"><img src="https://img.shields.io/pypi/dm/Opti-HPLC-Handler.svg" alt="PyPI Downloads"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.7.0 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.8.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
@@ -37,25 +37,26 @@
 "dev" Requires-Dist: isort==5.12.0; extra == "dev" Provides-Extra: test
 Requires-Dist: pytest==8.0.0; extra == "test" Requires-Dist: pytest-cov==4.1.0;
 extra == "test" Provides-Extra: lint Requires-Dist: black[jupyter]==23.3.0;
 extra == "lint" Requires-Dist: flake8==7.0.0; extra == "lint" Requires-Dist:
 isort==5.12.0; extra == "lint" Provides-Extra: release Requires-Dist:
 bumpver==2023.1125; extra == "release" Provides-Extra: build Requires-Dist:
 build==1.0.3; extra == "build" Provides-Extra: doc Requires-Dist:
-pylint==3.0.2; extra == "doc" Requires-Dist: sphinx==7.2.6; extra == "doc" #
-OptiHPLCHandler _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_Z_e_n_o_d_o_ _D_O_I_]_[_L_i_c_e_n_s_e_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_S_o_u_r_c_e_ _c_o_d_e
-_o_n_ _G_i_t_H_u_b_]Simplified proxy API for interacting with the Waters Empower Web API.
-It aims to make putting data into and getting data out of Empower easy, with
-the aim of automating running samples. It will not feature changing data
-already in Empower. ## Using the package The package can be installed into a
-Python environment with the command ``` pip install Opti-HPLC-Handler ``` You
-can then import package and start an `EmpowerHandler`. You need to select the
-Empower project to log in to. Note that the user logging in needs to have
-access to both that project, and the project `Mobile`. ```python from
-OptiHPLCHandler import EmpowerHandler handler=EmpowerHandler
+pylint==3.0.2; extra == "doc" Requires-Dist: sphinx==7.2.6; extra == "doc"
+Provides-Extra: examples Requires-Dist: python-dotenv==1.0.1; extra ==
+"examples" # OptiHPLCHandler _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_Z_e_n_o_d_o_ _D_O_I_]_[_L_i_c_e_n_s_e_]_[_P_y_P_I
+_D_o_w_n_l_o_a_d_s_]_[_S_o_u_r_c_e_ _c_o_d_e_ _o_n_ _G_i_t_H_u_b_]Simplified proxy API for interacting with the
+Waters Empower Web API. It aims to make putting data into and getting data out
+of Empower easy, with the aim of automating running samples. It will not
+feature changing data already in Empower. ## Using the package The package can
+be installed into a Python environment with the command ``` pip install Opti-
+HPLC-Handler ``` You can then import package and start an `EmpowerHandler`. You
+need to select the Empower project to log in to. Note that the user logging in
+needs to have access to both that project, and the project `Mobile`. ```python
+from OptiHPLCHandler import EmpowerHandler handler=EmpowerHandler
 ( project="project", address="https://API_url.com:3076",
 allow_login_without_context_manager=True, ) ``` Your username will be auto-
 detected. Add the argument `username` to circumvent this auto-detection.
 `EmpowerHandler` will first try to find a password for Empower for the
 `username` in the OS's system keyring, e.g. Windows Credential Locker. If it
 can't access a system keyring, or the keyring does not contain the relevant
 key, you will be prompted you for the password. The password will only be used
```

### Comparing `opti_hplc_handler-2.7.0/README.md` & `opti_hplc_handler-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/pyproject.toml` & `opti_hplc_handler-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Opti_HPLC_Handler"
-version = "2.7.0"
+version = "2.8.0"
 description = "Simplified proxy API for interacting with the Waters Empower Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Søren Furbo", email="srfu@novonordisk.com" },
 ]
@@ -50,14 +50,17 @@
 build = [
   "build==1.0.3",
 ]
 doc = [
   "pylint==3.0.2",
   "sphinx==7.2.6",
 ]
+examples = [
+  "python-dotenv==1.0.1",
+]
 
 
 [project.urls]
 Repository = "https://github.com/novonordisk-research/OptiHPLCHandler.git"
 
 [build-system]
 requires = ["setuptools>=0.64.0", "wheel"]
@@ -90,15 +93,15 @@
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
 
 [tool.bumpver]
-current_version = "2.7.0"
+current_version = "2.8.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_api_core.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_api_core.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_handler.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_handler.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_instrument_method.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_instrument_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             is passed, the instrument method definition will be extracted.
         :param use_sample_manager_oven: If True, both sample manager oven and column
             manager oven will be used. If False, only column manager oven will be used.
         """
         self.column_oven_method_list: list[ColumnOvenMethod] = []
         self.module_method_list: list[EmpowerModuleMethod] = []
         self.solvent_handler_method: Optional[SolventManagerMethod] = None
+        self.sample_handler_method: Optional[SampleManagerMethod] = None
 
         if use_sample_manager_oven:
             oven_type_tuple = (ColumnManagerMethod, SampleManagerMethod)
         else:
             oven_type_tuple = (ColumnManagerMethod,)
 
         if isinstance(method_definition, dict) and "results" in method_definition:
@@ -79,14 +80,16 @@
                 self.column_oven_method_list.append(module_method)
             if isinstance(module_method, SolventManagerMethod):
                 if self.solvent_handler_method is not None:
                     raise ValueError(
                         "Multiple solvent managers found in instrument method."
                     )
                 self.solvent_handler_method = module_method
+            if isinstance(module_method, SampleManagerMethod):
+                self.sample_handler_method = module_method
 
     @property
     def current_method(self):
         """The current method definition."""
         method = dict(self.original_method)
         method["methodName"] = self.method_name
         method["modules"] = [
@@ -110,14 +113,21 @@
     def column_temperature(self, temperature: float):
         if len(self.column_oven_method_list) == 0:
             raise ValueError("No column oven found in instrument method.")
         for module in self.column_oven_method_list:
             module.column_temperature = temperature
 
     @property
+    def sample_temperature(self):
+        """The sample temperature for the relevant sample oven(s) if any are present."""
+        if self.sample_handler_method is None:
+            raise ValueError("No sample manager found in instrument method.")
+        return self.sample_handler_method.sample_temperature
+
+    @property
     def gradient_table(self) -> List[dict]:
         """The gradient table, if a solvent manager module method is present."""
         if self.solvent_handler_method is None:
             raise ValueError(
                 "Can't get gradient table, "
                 "no solvent manager found in instrument method."
             )
```

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/empower_module_method.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/empower_module_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -161,38 +161,49 @@
     Attributes in addition to the ones from EmpowerModuleMethod:
 
     :ivar column_temperature: The column temperature.
 
     :meta private:
     """
 
-    TEMPERATURE_KEY: str
+    column_temperature_key: str
 
     @property
     def column_temperature(self) -> str:
         """
         The column temperature. If a float is given, it will be rounded to 1 decimal.
         """
-        return self[self.TEMPERATURE_KEY]
+        return self[self.column_temperature_key]
 
     @column_temperature.setter
     def column_temperature(self, value: Union[str, float]) -> None:
-        self[self.TEMPERATURE_KEY] = self._round(value, decimal_digits=1)
+        self[self.column_temperature_key] = self._round(value, decimal_digits=1)
 
 
 class SampleManagerMethod(ColumnOvenMethod):
     """Class for module methods that control a sample manager."""
 
-    TEMPERATURE_KEY = "ColumnTemperature"
+    column_temperature_key = "ColumnTemperature"
+
+    sample_temperature_key = "SampleTemperature"
+
+    @property
+    def sample_temperature(self) -> str:
+        """The sample temperature."""
+        return self[self.sample_temperature_key]
+
+    @sample_temperature.setter
+    def sample_temperature(self, value: Union[str, float]) -> None:
+        self[self.sample_temperature_key] = self._round(value, decimal_digits=1)
 
 
 class ColumnManagerMethod(ColumnOvenMethod):
     """Class for module methods that control a column manager."""
 
-    TEMPERATURE_KEY = "SetColumnTemperature"
+    column_temperature_key = "SetColumnTemperature"
 
 
 class SolventManagerMethod(EmpowerModuleMethod):
     """
     Parent class for module methods that control a solvent manager. Specific instrument
     types should subclass this class and set the following class attributes:
     valve_tag_prefix, valve_tag_suffix, and solvent_lines.
@@ -333,15 +344,15 @@
     """
     Factory function for creating an EmpowerModuleMethod from a method definition. The
     method definition should contain at least a name key, which is used to determine
     which subclass should be created. If the name key is not present or the name is not
     recognized, a generic EmpowerModuleMethod will be created.
     """
     try:
-        if method_definition["name"] in ["rAcquityFTN"]:
+        if method_definition["name"] in ["rAcquityFTN", "AcquityFTN", "AcquitySMDI"]:
             logger.debug("Creating SampleManagerMethod")
             return SampleManagerMethod(method_definition)
         if method_definition["name"] in ["AcquityCM", "ACQ-CM"]:
             logger.debug("Creating ColumnManagerMethod")
             return ColumnManagerMethod(method_definition)
         if method_definition["name"] in ["AcquityBSM", "ACQ-BSM", "rAcquityBSM"]:
             logger.debug("Creating BSMMethod")
```

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/data_types.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/data_types.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_gradient_table.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/validate_gradient_table.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/src/OptiHPLCHandler/utils/validate_method_name.py` & `opti_hplc_handler-2.8.0/src/OptiHPLCHandler/utils/validate_method_name.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO` & `opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Opti_HPLC_Handler
-Version: 2.7.0
+Version: 2.8.0
 Summary: Simplified proxy API for interacting with the Waters Empower Web API.
 Author-email: Søren Furbo <srfu@novonordisk.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, novonordisk-research
         
         Redistribution and use in source and binary forms, with or without
@@ -65,14 +65,16 @@
 Provides-Extra: release
 Requires-Dist: bumpver==2023.1125; extra == "release"
 Provides-Extra: build
 Requires-Dist: build==1.0.3; extra == "build"
 Provides-Extra: doc
 Requires-Dist: pylint==3.0.2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
+Provides-Extra: examples
+Requires-Dist: python-dotenv==1.0.1; extra == "examples"
 
 # OptiHPLCHandler
 
 <a href="https://pypi.python.org/pypi/Opti-HPLC-Handler"><img src="https://img.shields.io/pypi/v/Opti-HPLC-Handler.svg" alt="PyPI Version"></a>
 <a href="https://zenodo.org/doi/10.5281/zenodo.8386699"><img src="https://zenodo.org/badge/673355902.svg" alt="Zenodo DOI"></a>
 <a href="https://github.com/novonordisk-research/OptiHPLCHandler/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/Opti-HPLC-Handler.svg" alt="License"></a>
 <a href="https://pepy.tech/project/opti-hplc-handler"><img src="https://img.shields.io/pypi/dm/Opti-HPLC-Handler.svg" alt="PyPI Downloads"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.7.0 Summary:
+Metadata-Version: 2.1 Name: Opti_HPLC_Handler Version: 2.8.0 Summary:
 Simplified proxy API for interacting with the Waters Empower Web API. Author-
 email: SÃ¸ren Furbo
 novonordisk.com> License: BSD 3-Clause License Copyright (c) 2023, novonordisk-
 research Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
@@ -37,25 +37,26 @@
 "dev" Requires-Dist: isort==5.12.0; extra == "dev" Provides-Extra: test
 Requires-Dist: pytest==8.0.0; extra == "test" Requires-Dist: pytest-cov==4.1.0;
 extra == "test" Provides-Extra: lint Requires-Dist: black[jupyter]==23.3.0;
 extra == "lint" Requires-Dist: flake8==7.0.0; extra == "lint" Requires-Dist:
 isort==5.12.0; extra == "lint" Provides-Extra: release Requires-Dist:
 bumpver==2023.1125; extra == "release" Provides-Extra: build Requires-Dist:
 build==1.0.3; extra == "build" Provides-Extra: doc Requires-Dist:
-pylint==3.0.2; extra == "doc" Requires-Dist: sphinx==7.2.6; extra == "doc" #
-OptiHPLCHandler _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_Z_e_n_o_d_o_ _D_O_I_]_[_L_i_c_e_n_s_e_]_[_P_y_P_I_ _D_o_w_n_l_o_a_d_s_]_[_S_o_u_r_c_e_ _c_o_d_e
-_o_n_ _G_i_t_H_u_b_]Simplified proxy API for interacting with the Waters Empower Web API.
-It aims to make putting data into and getting data out of Empower easy, with
-the aim of automating running samples. It will not feature changing data
-already in Empower. ## Using the package The package can be installed into a
-Python environment with the command ``` pip install Opti-HPLC-Handler ``` You
-can then import package and start an `EmpowerHandler`. You need to select the
-Empower project to log in to. Note that the user logging in needs to have
-access to both that project, and the project `Mobile`. ```python from
-OptiHPLCHandler import EmpowerHandler handler=EmpowerHandler
+pylint==3.0.2; extra == "doc" Requires-Dist: sphinx==7.2.6; extra == "doc"
+Provides-Extra: examples Requires-Dist: python-dotenv==1.0.1; extra ==
+"examples" # OptiHPLCHandler _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_Z_e_n_o_d_o_ _D_O_I_]_[_L_i_c_e_n_s_e_]_[_P_y_P_I
+_D_o_w_n_l_o_a_d_s_]_[_S_o_u_r_c_e_ _c_o_d_e_ _o_n_ _G_i_t_H_u_b_]Simplified proxy API for interacting with the
+Waters Empower Web API. It aims to make putting data into and getting data out
+of Empower easy, with the aim of automating running samples. It will not
+feature changing data already in Empower. ## Using the package The package can
+be installed into a Python environment with the command ``` pip install Opti-
+HPLC-Handler ``` You can then import package and start an `EmpowerHandler`. You
+need to select the Empower project to log in to. Note that the user logging in
+needs to have access to both that project, and the project `Mobile`. ```python
+from OptiHPLCHandler import EmpowerHandler handler=EmpowerHandler
 ( project="project", address="https://API_url.com:3076",
 allow_login_without_context_manager=True, ) ``` Your username will be auto-
 detected. Add the argument `username` to circumvent this auto-detection.
 `EmpowerHandler` will first try to find a password for Empower for the
 `username` in the OS's system keyring, e.g. Windows Credential Locker. If it
 can't access a system keyring, or the keyring does not contain the relevant
 key, you will be prompted you for the password. The password will only be used
```

### Comparing `opti_hplc_handler-2.7.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt` & `opti_hplc_handler-2.8.0/src/Opti_HPLC_Handler.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 README.md
 pyproject.toml
 src/OptiHPLCHandler/__init__.py
 src/OptiHPLCHandler/empower_api_core.py
 src/OptiHPLCHandler/empower_handler.py
 src/OptiHPLCHandler/empower_instrument_method.py
 src/OptiHPLCHandler/empower_module_method.py
+src/OptiHPLCHandler/applications/__init__.py
+src/OptiHPLCHandler/applications/generate_basic_robustness_methods.py
+src/OptiHPLCHandler/applications/revert_method.py
+src/OptiHPLCHandler/applications/empower_implementation/empower_tools.py
+src/OptiHPLCHandler/applications/method_generators/add_isocratic_segment.py
+src/OptiHPLCHandler/applications/method_generators/alter_strong_eluent_pct.py
+src/OptiHPLCHandler/applications/method_generators/alter_temperature.py
+src/OptiHPLCHandler/applications/method_generators/condense_gradient_table.py
+src/OptiHPLCHandler/applications/method_generators/ramp_method.py
 src/OptiHPLCHandler/utils/__init__.py
 src/OptiHPLCHandler/utils/data_types.py
 src/OptiHPLCHandler/utils/validate_gradient_table.py
 src/OptiHPLCHandler/utils/validate_method_name.py
 src/Opti_HPLC_Handler.egg-info/PKG-INFO
 src/Opti_HPLC_Handler.egg-info/SOURCES.txt
 src/Opti_HPLC_Handler.egg-info/dependency_links.txt
```

### Comparing `opti_hplc_handler-2.7.0/tests/test_core_api.py` & `opti_hplc_handler-2.8.0/tests/test_core_api.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/tests/test_instrument_method.py` & `opti_hplc_handler-2.8.0/tests/test_instrument_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     def test_initialisation_multiple_oven_types(self):
         method_definition = self.example["response-BSM-TUV-CM-Acq.json"]
         method = EmpowerInstrumentMethod(
             method_definition, use_sample_manager_oven=True
         )
         assert len(method.column_oven_method_list) == 2
 
+    def test_sample_manager_method(self):
+        method_definition = self.example["response-BSM-TUV-CM-Acq.json"]
+        method = EmpowerInstrumentMethod(method_definition)
+        assert method.sample_temperature == "20.0"
+
     def test_original_method(self):
         for method_definition in self.example.values():
             method = EmpowerInstrumentMethod(method_definition)
             assert isinstance(method.original_method, dict)
             assert method.original_method == method_definition["results"][0]
 
     def test_original_method_immutable(self):
```

### Comparing `opti_hplc_handler-2.7.0/tests/test_module_method.py` & `opti_hplc_handler-2.8.0/tests/test_module_method.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/tests/test_proxy_api.py` & `opti_hplc_handler-2.8.0/tests/test_proxy_api.py`

 * *Files identical despite different names*

### Comparing `opti_hplc_handler-2.7.0/tests/test_utils.py` & `opti_hplc_handler-2.8.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
-from src.OptiHPLCHandler.utils import (
+from OptiHPLCHandler.utils import (
     append_truncate_method_name,
     make_method_name_string_compatible_with_empower,
 )
-from src.OptiHPLCHandler.utils.validate_gradient_table import validate_gradient_table
+from OptiHPLCHandler.utils.validate_gradient_table import validate_gradient_table
 
 
 class TestUtils(unittest.TestCase):
     def test_make_method_name_string_compatible_with_empower(self):
         method_name = "Test.Method-Name"
         expected_result = "Test_MethodmName"
         assert (
```

