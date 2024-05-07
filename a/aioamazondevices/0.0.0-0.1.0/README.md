# Comparing `tmp/aioamazondevices-0.0.0.tar.gz` & `tmp/aioamazondevices-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioamazondevices-0.0.0.tar", max compression
+gzip compressed data, was "aioamazondevices-0.1.0.tar", max compression
```

## Comparing `aioamazondevices-0.0.0.tar` & `aioamazondevices-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    11346 2024-04-24 16:23:44.504487 aioamazondevices-0.0.0/LICENSE
--rw-r--r--   0        0        0     3588 2024-04-24 16:23:44.504487 aioamazondevices-0.0.0/README.md
--rw-r--r--   0        0        0     2264 2024-04-24 16:23:45.316486 aioamazondevices-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       55 2024-04-24 16:23:45.320485 aioamazondevices-0.0.0/src/aioamazondevices/__init__.py
--rw-r--r--   0        0        0      118 2024-04-24 16:23:44.504487 aioamazondevices-0.0.0/src/aioamazondevices/main.py
--rw-r--r--   0        0        0        0 2024-04-24 16:23:44.504487 aioamazondevices-0.0.0/src/aioamazondevices/py.typed
--rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 aioamazondevices-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3588 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/README.md
+-rw-r--r--   0        0        0     2296 2024-05-07 20:46:52.609484 aioamazondevices-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-05-07 20:46:52.617484 aioamazondevices-0.1.0/src/aioamazondevices/__init__.py
+-rw-r--r--   0        0        0     8856 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/api.py
+-rw-r--r--   0        0        0     1089 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/const.py
+-rw-r--r--   0        0        0      444 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/py.typed
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 aioamazondevices-0.1.0/PKG-INFO
```

### Comparing `aioamazondevices-0.0.0/LICENSE` & `aioamazondevices-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioamazondevices-0.0.0/README.md` & `aioamazondevices-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aioamazondevices-0.0.0/pyproject.toml` & `aioamazondevices-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioamazondevices"
-version = "0.0.0"
+version = "0.1.0"
 description = "Python library to control Amazon devices"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aioamazondevices"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -19,15 +19,17 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chemelli74/aioamazondevices/issues"
 "Changelog" = "https://github.com/chemelli74/aioamazondevices/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-aiohttp = "*"
+beautifulsoup4 = "*"
+httpx = "*"
+orjson = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1"
 pytest-cov = "^5.0"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
```

### Comparing `aioamazondevices-0.0.0/PKG-INFO` & `aioamazondevices-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioamazondevices
-Version: 0.0.0
+Version: 0.1.0
 Summary: Python library to control Amazon devices
 Home-page: https://github.com/chemelli74/aioamazondevices
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,17 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: aiohttp
+Requires-Dist: beautifulsoup4
+Requires-Dist: httpx
+Requires-Dist: orjson
 Project-URL: Bug Tracker, https://github.com/chemelli74/aioamazondevices/issues
 Project-URL: Changelog, https://github.com/chemelli74/aioamazondevices/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/chemelli74/aioamazondevices
 Description-Content-Type: text/markdown
 
 # aioamazondevices
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: aioamazondevices Version: 0.0.0 Summary: Python
+Metadata-Version: 2.1 Name: aioamazondevices Version: 0.1.0 Summary: Python
 library to control Amazon devices Home-page: https://github.com/chemelli74/
 aioamazondevices License: Apache Software License 2.0 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries Requires-Dist: aiohttp
-Project-URL: Bug Tracker, https://github.com/chemelli74/aioamazondevices/issues
-Project-URL: Changelog, https://github.com/chemelli74/aioamazondevices/blob/
-main/CHANGELOG.md Project-URL: Repository, https://github.com/chemelli74/
+Classifier: Topic :: Software Development :: Libraries Requires-Dist:
+beautifulsoup4 Requires-Dist: httpx Requires-Dist: orjson Project-URL: Bug
+Tracker, https://github.com/chemelli74/aioamazondevices/issues Project-URL:
+Changelog, https://github.com/chemelli74/aioamazondevices/blob/main/
+CHANGELOG.md Project-URL: Repository, https://github.com/chemelli74/
 aioamazondevices Description-Content-Type: text/markdown # aioamazondevices
                      _[_C_I_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_h_e_m_e_l_l_i_7_4_/_a_i_o_a_m_a_z_o_n_d_e_v_i_c_e_s_ --- Python
 library to control Amazon devices ## Installation Install this via pip (or your
 favourite package manager): `pip install aioamazondevices` ## Usage Start by
```

