# Comparing `tmp/nipe_py-0.0.2.tar.gz` & `tmp/nipe_py-0.0.3.tar.gz`

## Comparing `nipe_py-0.0.2.tar` & `nipe_py-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.cruft.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.editorconfig
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nipe_py-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/arch-torrc
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/centos-torrc
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/debian-torrc
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/fedora-torrc
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.configs/void-torrc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/release-drafter.yml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/draft.yml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.2/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.2/assets/demo.gif
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 nipe_py-0.0.2/docs/index.md
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/py.typed
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Restart.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Start.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/engine/Stop.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Device.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Install.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.0.2/src/nipe_py/utils/Status.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.0.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.0.2/LICENSE
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 nipe_py-0.0.2/README.md
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 nipe_py-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.cruft.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.editorconfig
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nipe_py-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/arch-torrc
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/centos-torrc
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/debian-torrc
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/fedora-torrc
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.configs/void-torrc
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/release-drafter.yml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/draft.yml
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.3/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.3/assets/demo.gif
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/index.md
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.0.3/docs/assets/demo.gif
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Restart.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Start.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/engine/Stop.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Device.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Install.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.0.3/src/nipe_py/utils/Status.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 nipe_py-0.0.3/README.md
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 nipe_py-0.0.3/PKG-INFO
```

### Comparing `nipe_py-0.0.2/.cruft.json` & `nipe_py-0.0.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/mkdocs.yml` & `nipe_py-0.0.3/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -52,11 +52,11 @@
                 import:
                     - https://docs.python.org/3.11/objects.inv
                 options:
                     docstring_style: google
 
 watch:
     - docs
-    - nipe_py
+    - src/nipe_py
 
 nav:
     - About: index.md
```

### Comparing `nipe_py-0.0.2/.github/release-drafter.yml` & `nipe_py-0.0.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `nipe_py-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/.github/workflows/documentation.yml` & `nipe_py-0.0.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/.github/workflows/release.yml` & `nipe_py-0.0.3/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     - name: Build
       run: |
         hatch build
     - name: Publish 📦 to Test PyPI
       if: startsWith(github.ref, 'refs/heads/main')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        skip_existing: true
+        skip-existing: true
         user: __token__
         password: ${{ secrets.TEST_PYPI_SECRECT }}
         packages-dir: dist/
         repository-url: https://test.pypi.org/legacy/
     - name: Publish 📦 to PyPI
       if: startsWith(github.ref, 'refs/heads/main')
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `nipe_py-0.0.2/assets/banner.png` & `nipe_py-0.0.3/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/assets/demo.gif` & `nipe_py-0.0.3/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/docs/index.md` & `nipe_py-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # nipe_py
 
 <p align="center">
-    <img src="../assets/banner.png">
+    <img src="./assets/banner.png">
 </p>
 
 
 
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
+<div align="center">
+
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
+
+[![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
+
+</div>
+
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
@@ -37,12 +45,12 @@
   restart  Restart the Nipe circuit
   start    Start routing
   status   See status
   stop     Stop routing
 ```
 
 ## Demo
-![](../assets/demo.gif)
+![](./assets/demo.gif)
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,14 +1,25 @@
 # nipe_py
-                            [../assets/banner.png]
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
-py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
-aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
-_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
-version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
-Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
-Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
-help Show this message and exit. Commands: install Install dependencies restart
-Restart the Nipe circuit start Start routing status See status stop Stop
-routing ``` ## Demo ![](../assets/demo.gif) ## License This project is licensed
-under the terms of the MIT license.
+                             [./assets/banner.png]
+                [![Python](https://img.shields.io/badge/Python-
+3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
+ [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
+  (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
+           badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
+   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
+                     (https://img.shields.io/badge/Pytest-
+    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
+  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+(https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
+(https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
+github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
+                     aviksaikat/nipe_py/blob/main/LICENSE)
+--- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
+github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
+## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
+Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
+exit. Commands: install Install dependencies restart Restart the Nipe circuit
+start Start routing status See status stop Stop routing ``` ## Demo ![](./
+assets/demo.gif) ## License This project is licensed under the terms of the MIT
+license.
```

### Comparing `nipe_py-0.0.2/src/nipe_py/main.py` & `nipe_py-0.0.3/src/nipe_py/main.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/src/nipe_py/engine/Start.py` & `nipe_py-0.0.3/src/nipe_py/engine/Start.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/src/nipe_py/engine/Stop.py` & `nipe_py-0.0.3/src/nipe_py/engine/Stop.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/src/nipe_py/utils/Device.py` & `nipe_py-0.0.3/src/nipe_py/utils/Device.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/src/nipe_py/utils/Install.py` & `nipe_py-0.0.3/src/nipe_py/utils/Install.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/src/nipe_py/utils/Status.py` & `nipe_py-0.0.3/src/nipe_py/utils/Status.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/.gitignore` & `nipe_py-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/LICENSE` & `nipe_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/README.md` & `nipe_py-0.0.3/docs/index.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # nipe_py
 
 <p align="center">
-    <img src="./assets/banner.png">
+    <img src="../assets/banner.png">
 </p>
 
+<center>
 
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
 
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
+
+
+[![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
+
+</center>
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
@@ -37,12 +44,12 @@
   restart  Restart the Nipe circuit
   start    Start routing
   status   See status
   stop     Stop routing
 ```
 
 ## Demo
-![](./assets/demo.gif)
+![](../assets/demo.gif)
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,14 +1,25 @@
 # nipe_py
-                             [./assets/banner.png]
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
-py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
-aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
-_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
-version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
-Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
-Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
-help Show this message and exit. Commands: install Install dependencies restart
-Restart the Nipe circuit start Start routing status See status stop Stop
-routing ``` ## Demo ![](./assets/demo.gif) ## License This project is licensed
-under the terms of the MIT license.
+                            [../assets/banner.png]
+                [![Python](https://img.shields.io/badge/Python-
+3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
+ [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
+  (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
+           badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
+   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
+                     (https://img.shields.io/badge/Pytest-
+    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
+  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+(https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
+(https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
+github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
+                     aviksaikat/nipe_py/blob/main/LICENSE)
+--- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
+github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
+## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
+Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
+exit. Commands: install Install dependencies restart Restart the Nipe circuit
+start Start routing status See status stop Stop routing ``` ## Demo ![](../
+assets/demo.gif) ## License This project is licensed under the terms of the MIT
+license.
```

### Comparing `nipe_py-0.0.2/pyproject.toml` & `nipe_py-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.0.2/PKG-INFO` & `nipe_py-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipe_py
-Version: 0.0.2
+Version: 0.0.3
 Summary: An engine to make Tor Network your default gateway.
 Project-URL: Documentation, https://aviksaikat.github.io/nipe_py/
 Project-URL: Source, https://github.com/aviksaikat/nipe_py
 Author-email: nipe_py <saikickkarma@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024, Saikat Karmakar
@@ -46,16 +46,24 @@
 
 <p align="center">
     <img src="./assets/banner.png">
 </p>
 
 
 
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/py/nipe_py)
+<div align="center">
+
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions) [![Pytest](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg)
+
+[![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
+
+</div>
+
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: nipe_py Version: 0.0.2 Summary: An engine to make
+Metadata-Version: 2.3 Name: nipe_py Version: 0.0.3 Summary: An engine to make
 Tor Network your default gateway. Project-URL: Documentation, https://
 aviksaikat.github.io/nipe_py/ Project-URL: Source, https://github.com/
 aviksaikat/nipe_py Author-email: nipe_py
 protonmail.com> License: MIT License Copyright (c) 2024, Saikat Karmakar
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -22,19 +22,30 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.9 Requires-
 Dist: click Requires-Dist: requests Requires-Dist: rich Description-Content-
 Type: text/markdown # nipe_py
                              [./assets/banner.png]
-[![PyPI version](https://badge.fury.io/py/nipe_py.svg)](https://badge.fury.io/
-py/nipe_py) [![GitHub license](https://img.shields.io/github/license/
-aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/
-nipe_py/blob/main/LICENSE) --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/
-_n_i_p_e___p_y_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python
-version of [nipe](https://github.com/htrgouvea/nipe): An engine to make Tor
-Network your default gateway. ## Installation ```sh pip install nipe_py ``` ##
-Usage ```sh $ nipe --help Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --
-help Show this message and exit. Commands: install Install dependencies restart
-Restart the Nipe circuit start Start routing status See status stop Stop
-routing ``` ## Demo ![](./assets/demo.gif) ## License This project is licensed
-under the terms of the MIT license.
+                [![Python](https://img.shields.io/badge/Python-
+3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
+ [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
+  (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
+           badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
+   Actions&logoColor=white)](https://github.com/features/actions) [![Pytest]
+                     (https://img.shields.io/badge/Pytest-
+    0A9EDC.svg?style=flat&logo=Pytest&logoColor=white)](https://github.com/
+  aviksaikat/nipe_py/actions/workflows/tests.yml/badge.svg) [![PyPI version]
+(https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
+  [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)]
+(https://pypi.org/project/nipe_py/) [![GitHub license](https://img.shields.io/
+github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/
+                     aviksaikat/nipe_py/blob/main/LICENSE)
+--- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
+github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
+## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
+Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
+exit. Commands: install Install dependencies restart Restart the Nipe circuit
+start Start routing status See status stop Stop routing ``` ## Demo ![](./
+assets/demo.gif) ## License This project is licensed under the terms of the MIT
+license.
```

