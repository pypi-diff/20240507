# Comparing `tmp/nipe_py-0.1.0.tar.gz` & `tmp/nipe_py-0.1.1.tar.gz`

## Comparing `nipe_py-0.1.0.tar` & `nipe_py-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.cruft.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nipe_py-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/arch-torrc
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/centos-torrc
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/debian-torrc
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/fedora-torrc
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.configs/void-torrc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/draft.yml
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.0/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.0/assets/demo.gif
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/index.md
--rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/assets/banner.png
--rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.0/docs/assets/demo.gif
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/py.typed
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Restart.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Start.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/engine/Stop.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Device.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Install.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.1.0/src/nipe_py/utils/Status.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.1.0/LICENSE
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nipe_py-0.1.0/README.md
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 nipe_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.cruft.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nipe_py-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.configs/arch-torrc
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.configs/centos-torrc
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.configs/debian-torrc
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.configs/fedora-torrc
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.configs/void-torrc
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/release-drafter.yml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/workflows/draft.yml
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.1/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.1/assets/demo.gif
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 nipe_py-0.1.1/docs/index.md
+-rw-r--r--   0        0        0    19649 2020-02-02 00:00:00.000000 nipe_py-0.1.1/docs/assets/banner.png
+-rw-r--r--   0        0        0   109143 2020-02-02 00:00:00.000000 nipe_py-0.1.1/docs/assets/demo.gif
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/engine/Restart.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/engine/Start.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/engine/Stop.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/utils/Device.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/utils/Install.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nipe_py-0.1.1/src/nipe_py/utils/Status.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nipe_py-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 nipe_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nipe_py-0.1.1/README.md
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 nipe_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 nipe_py-0.1.1/PKG-INFO
```

### Comparing `nipe_py-0.1.0/.cruft.json` & `nipe_py-0.1.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/mkdocs.yml` & `nipe_py-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/.github/release-drafter.yml` & `nipe_py-0.1.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nipe_py-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/.github/workflows/documentation.yml` & `nipe_py-0.1.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/.github/workflows/release.yml` & `nipe_py-0.1.1/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
   push:
     branches: ["main"]
   pull_request:
     branches: ["main"]
 
 jobs:
   test:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python_version: ["3.9", "3.10", "3.11", "3.12"]
+        os: [ubuntu-latest]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python_version }}
@@ -23,14 +24,15 @@
       run: |
         python -m pip install --upgrade pip
         pip install hatch
         hatch env create
     - name: Test
       run: |
         sudo $(which hatch) run nipe --help | grep "Start routing" > /dev/null
+
   release:
     runs-on: ubuntu-latest
     needs: test
     environment: release
     # if: startsWith(github.ref, 'refs/heads/main/')
     permissions:
         contents: write
```

### Comparing `nipe_py-0.1.0/assets/banner.png` & `nipe_py-0.1.1/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/assets/demo.gif` & `nipe_py-0.1.1/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/docs/index.md` & `nipe_py-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # nipe_py
 
 <p align="center">
-    <img src="../assets/banner.png">
+    <img src="./assets/banner.png">
 </p>
 
-<center>
 
-[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
+<div align="center">
 
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
 [![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 
-</center>
+</div>
 
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
@@ -45,12 +45,12 @@
   restart  Restart the Nipe circuit
   start    Start routing
   status   See status
   stop     Stop routing
 ```
 
 ## Demo
-![](../assets/demo.gif)
+![](./assets/demo.gif)
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the [MIT](./LICENSE) license.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # nipe_py
-                            [../assets/banner.png]
+                             [./assets/banner.png]
                 [![Python](https://img.shields.io/badge/Python-
 3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
  [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
   (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
            badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
 Actions&logoColor=white)](https://github.com/features/actions) [![PyPI version]
 (https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
@@ -13,10 +13,10 @@
                      aviksaikat/nipe_py/blob/main/LICENSE)
 --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
 github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 ## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
 Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
 exit. Commands: install Install dependencies restart Restart the Nipe circuit
-start Start routing status See status stop Stop routing ``` ## Demo ![](../
-assets/demo.gif) ## License This project is licensed under the terms of the MIT
-license.
+start Start routing status See status stop Stop routing ``` ## Demo ![](./
+assets/demo.gif) ## License This project is licensed under the terms of the
+[MIT](./LICENSE) license.
```

### Comparing `nipe_py-0.1.0/docs/assets/banner.png` & `nipe_py-0.1.1/docs/assets/banner.png`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/docs/assets/demo.gif` & `nipe_py-0.1.1/docs/assets/demo.gif`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/main.py` & `nipe_py-0.1.1/src/nipe_py/main.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/engine/Start.py` & `nipe_py-0.1.1/src/nipe_py/engine/Start.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/engine/Stop.py` & `nipe_py-0.1.1/src/nipe_py/engine/Stop.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/utils/Device.py` & `nipe_py-0.1.1/src/nipe_py/utils/Device.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/utils/Install.py` & `nipe_py-0.1.1/src/nipe_py/utils/Install.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/src/nipe_py/utils/Status.py` & `nipe_py-0.1.1/src/nipe_py/utils/Status.py`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/.gitignore` & `nipe_py-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/LICENSE` & `nipe_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/README.md` & `nipe_py-0.1.1/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # nipe_py
 
 <p align="center">
-    <img src="./assets/banner.png">
+    <img src="https://github.com/Aviksaikat/nipe_py/assets/banner.png">
 </p>
 
+<center>
 
+[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
-<div align="center">
 
-[![Python](https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-Actions&logoColor=white)](https://github.com/features/actions)
 
 [![PyPI version](https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nipe_py)](https://pypi.org/project/nipe_py/)
 [![GitHub license](https://img.shields.io/github/license/aviksaikat/nipe_py?style=flat&color=1573D5)](https://github.com/aviksaikat/nipe_py/blob/main/LICENSE)
 
-</div>
+</center>
 
 ---
 
 **Documentation**: <a href="https://aviksaikat.github.io/nipe_py/" target="_blank">https://aviksaikat.github.io/nipe_py/</a>
 
 **Source Code**: <a href="https://github.com/aviksaikat/nipe_py" target="_blank">https://github.com/aviksaikat/nipe_py</a>
 
@@ -45,12 +45,12 @@
   restart  Restart the Nipe circuit
   start    Start routing
   status   See status
   stop     Stop routing
 ```
 
 ## Demo
-![](./assets/demo.gif)
+![](https://github.com/Aviksaikat/nipe_py/assets/demo.gif)
 
 ## License
 
-This project is licensed under the terms of the [MIT](./LICENSE) license.
+This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # nipe_py
-                             [./assets/banner.png]
+           [https://github.com/Aviksaikat/nipe_py/assets/banner.png]
                 [![Python](https://img.shields.io/badge/Python-
 3776AB.svg?style=flat&logo=Python&logoColor=white)](https://www.python.org/) [!
  [Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)]
   (https://github.com/pypa/hatch) [![GitHub Actions](https://img.shields.io/
            badge/GitHub%20Actions-2088FF.svg?style=flat&logo=GitHub-
 Actions&logoColor=white)](https://github.com/features/actions) [![PyPI version]
 (https://img.shields.io/pypi/v/nipe_py.svg)](https://pypi.org/project/nipe_py)
@@ -13,10 +13,10 @@
                      aviksaikat/nipe_py/blob/main/LICENSE)
 --- **Documentation**: _h_t_t_p_s_:_/_/_a_v_i_k_s_a_i_k_a_t_._g_i_t_h_u_b_._i_o_/_n_i_p_e___p_y_/ **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_v_i_k_s_a_i_k_a_t_/_n_i_p_e___p_y --- Python version of [nipe](https://
 github.com/htrgouvea/nipe): An engine to make Tor Network your default gateway.
 ## Installation ```sh pip install nipe_py ``` ## Usage ```sh $ nipe --help
 Usage: nipe [OPTIONS] COMMAND [ARGS]... Options: --help Show this message and
 exit. Commands: install Install dependencies restart Restart the Nipe circuit
-start Start routing status See status stop Stop routing ``` ## Demo ![](./
-assets/demo.gif) ## License This project is licensed under the terms of the
-[MIT](./LICENSE) license.
+start Start routing status See status stop Stop routing ``` ## Demo ![](https:/
+/github.com/Aviksaikat/nipe_py/assets/demo.gif) ## License This project is
+licensed under the terms of the MIT license.
```

### Comparing `nipe_py-0.1.0/pyproject.toml` & `nipe_py-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipe_py-0.1.0/PKG-INFO` & `nipe_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipe_py
-Version: 0.1.0
+Version: 0.1.1
 Summary: An engine to make Tor Network your default gateway.
 Project-URL: Documentation, https://aviksaikat.github.io/nipe_py/
 Project-URL: Source, https://github.com/aviksaikat/nipe_py
 Author-email: nipe_py <saikickkarma@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024, Saikat Karmakar
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: nipe_py Version: 0.1.0 Summary: An engine to make
+Metadata-Version: 2.3 Name: nipe_py Version: 0.1.1 Summary: An engine to make
 Tor Network your default gateway. Project-URL: Documentation, https://
 aviksaikat.github.io/nipe_py/ Project-URL: Source, https://github.com/
 aviksaikat/nipe_py Author-email: nipe_py
 protonmail.com> License: MIT License Copyright (c) 2024, Saikat Karmakar
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

