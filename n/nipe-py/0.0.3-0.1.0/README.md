# Comparing `tmp/nipe_py-0.0.3.tar.gz` & `tmp/nipe_py-0.1.0.tar.gz`

## Comparing `nipe_py-0.0.3.tar` & `nipe_py-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.cruft.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.editorconfig
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nipe_py-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/arch-torrc
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/centos-torrc
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/debian-torrc
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/fedora-torrc
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/void-torrc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/release-drafter.yml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/draft.yml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.3/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.3/assets/demo.gif
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/index.md
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/assets/demo.gif
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/py.typed
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Restart.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Start.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Stop.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Device.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Install.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Status.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.0.3/LICENSE
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nipe_py-0.0.3/README.md
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 nipe_py-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.cruft.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.editorconfig
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nipe_py-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/arch-torrc
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/centos-torrc
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/debian-torrc
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/fedora-torrc
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/void-torrc
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/draft.yml
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.0/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.0/assets/demo.gif
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/index.md
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/assets/demo.gif
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Restart.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Start.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Stop.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Device.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Install.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Status.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nipe_py-0.1.0/README.md
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 nipe_py-0.1.0/PKG-INFO
```

### Comparing `nipe_py-0.0.3/.cruft.json` & `nipe_py-0.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/mkdocs.yml` & `nipe_py-0.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/.github/release-drafter.yml` & `nipe_py-0.1.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `nipe_py-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/.github/workflows/documentation.yml` & `nipe_py-0.1.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/.github/workflows/release.yml` & `nipe_py-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/assets/banner.png` & `nipe_py-0.1.0/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/assets/demo.gif` & `nipe_py-0.1.0/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/docs/index.md` & `nipe_py-0.1.0/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 <p align="center">
     <img src="../assets/banner.png">
 </p>
 
 <center>
 
-[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
 
 
 [![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 
 </center>
+
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
```

#### html2text {}

```diff
@@ -1,18 +1,15 @@
 # nipe_py
                             [../assets/banner.png]
                 [![Python](https://img.shields.io/badge/Python-
 3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
  [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
   (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
            badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
-   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
-                     (https://img.shields.io/badge/Pytest-
-    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
-  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+Actions&logoColor=white)](https://github.com/features/actions) [![PyPI version]
 (https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
 (https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
 github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
                      aviksaikat/nipe_py/blob/main/LICENSE)
 --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
```

### Comparing `nipe_py-0.0.3/docs/assets/banner.png` & `nipe_py-0.1.0/docs/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/docs/assets/demo.gif` & `nipe_py-0.1.0/docs/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/main.py` & `nipe_py-0.1.0/src/nipe_py/main.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/engine/Start.py` & `nipe_py-0.1.0/src/nipe_py/engine/Start.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/engine/Stop.py` & `nipe_py-0.1.0/src/nipe_py/engine/Stop.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/utils/Device.py` & `nipe_py-0.1.0/src/nipe_py/utils/Device.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/utils/Install.py` & `nipe_py-0.1.0/src/nipe_py/utils/Install.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/src/nipe_py/utils/Status.py` & `nipe_py-0.1.0/src/nipe_py/utils/Status.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/.gitignore` & `nipe_py-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/LICENSE` & `nipe_py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/README.md` & `nipe_py-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <img src="./assets/banner.png">
 </p>
 
 
 
 <div align="center">
 
-[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
 [![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 
 </div>
 
@@ -49,8 +49,8 @@
 ```
 
 ## Demo
 ![](./assets/demo.gif)
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the [MIT](./LICENSE) license.
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
 # nipe_py
                              [./assets/banner.png]
                 [![Python](https://img.shields.io/badge/Python-
 3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
  [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
   (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
            badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
-   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
-                     (https://img.shields.io/badge/Pytest-
-    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
-  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+Actions&logoColor=white)](https://github.com/features/actions) [![PyPI version]
 (https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
 (https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
 github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
                      aviksaikat/nipe_py/blob/main/LICENSE)
 --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
 github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 ## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
 Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
 exit. Commands: install Install dependencies restart Restart the Nipe circuit
 start Start routing status See status stop Stop routing ``` ## Demo ![](./
-assets/demo.gif) ## License This project is licensed under the terms of the MIT
-license.
+assets/demo.gif) ## License This project is licensed under the terms of the
+[MIT](./LICENSE) license.
```

### Comparing `nipe_py-0.0.3/pyproject.toml` & `nipe_py-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.3/PKG-INFO` & `nipe_py-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipe_py
-Version: 0.0.3
+Version: 0.1.0
 Summary: An engine to make Tor Network your default gateway.
 Project-URL: Documentation, https://aviksaikat.github.io/nipe_py/
 Project-URL: Source, https://github.com/aviksaikat/nipe_py
 Author-email: nipe_py <saikickkarma@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024, Saikat Karmakar
@@ -48,15 +48,15 @@
     <img src="./assets/banner.png">
 </p>
 
 
 
 <div align="center">
 
-[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
 [![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 
 </div>
 
@@ -93,8 +93,8 @@
 ```
 
 ## Demo
 ![](./assets/demo.gif)
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the [MIT](./LICENSE) license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: nipe_py Version: 0.0.3 Summary: An engine to make
+Metadata-Version: 2.3 Name: nipe_py Version: 0.1.0 Summary: An engine to make
 Tor Network your default gateway. Project-URL: Documentation, https://
 aviksaikat.github.io/nipe_py/ Project-URL: Source, https://github.com/
 aviksaikat/nipe_py Author-email: nipe_py
 protonmail.com> License: MIT License Copyright (c) 2024, Saikat Karmakar
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -27,25 +27,22 @@
 Type: text/markdown # nipe_py
                              [./assets/banner.png]
                 [![Python](https://img.shields.io/badge/Python-
 3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
  [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
   (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
            badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
-   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
-                     (https://img.shields.io/badge/Pytest-
-    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
-  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+Actions&logoColor=white)](https://github.com/features/actions) [![PyPI version]
 (https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
   [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
 (https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
 github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
                      aviksaikat/nipe_py/blob/main/LICENSE)
 --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
 github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 ## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
 Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
 exit. Commands: install Install dependencies restart Restart the Nipe circuit
 start Start routing status See status stop Stop routing ``` ## Demo ![](./
-assets/demo.gif) ## License This project is licensed under the terms of the MIT
-license.
+assets/demo.gif) ## License This project is licensed under the terms of the
+[MIT](./LICENSE) license.
```

