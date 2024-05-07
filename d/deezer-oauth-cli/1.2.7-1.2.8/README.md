# Comparing `tmp/deezer_oauth_cli-1.2.7.tar.gz` & `tmp/deezer_oauth_cli-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_oauth_cli-1.2.7.tar", max compression
+gzip compressed data, was "deezer_oauth_cli-1.2.8.tar", max compression
```

## Comparing `deezer_oauth_cli-1.2.7.tar` & `deezer_oauth_cli-1.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/LICENSE
--rw-r--r--   0        0        0     5506 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/README.md
--rw-r--r--   0        0        0     3412 2024-04-09 21:59:22.043886 deezer_oauth_cli-1.2.7/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-09 21:59:22.043886 deezer_oauth_cli-1.2.7/src/deezer_oauth/__init__.py
--rw-r--r--   0        0        0       53 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/__main__.py
--rw-r--r--   0        0        0     1833 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/client.py
--rw-r--r--   0        0        0      115 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/constants.py
--rw-r--r--   0        0        0     1003 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/files.py
--rw-r--r--   0        0        0     1044 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/main.py
--rw-r--r--   0        0        0        0 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/py.typed
--rw-r--r--   0        0        0     3238 2024-04-09 21:59:18.631894 deezer_oauth_cli-1.2.7/src/deezer_oauth/server.py
--rw-r--r--   0        0        0     6989 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/LICENSE
+-rw-r--r--   0        0        0     5506 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/README.md
+-rw-r--r--   0        0        0     3414 2024-05-07 16:55:17.216796 deezer_oauth_cli-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 16:55:17.216796 deezer_oauth_cli-1.2.8/src/deezer_oauth/__init__.py
+-rw-r--r--   0        0        0       53 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/__main__.py
+-rw-r--r--   0        0        0     1833 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/client.py
+-rw-r--r--   0        0        0      115 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/constants.py
+-rw-r--r--   0        0        0     1003 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/files.py
+-rw-r--r--   0        0        0     1044 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/py.typed
+-rw-r--r--   0        0        0     3238 2024-05-07 16:55:14.204769 deezer_oauth_cli-1.2.8/src/deezer_oauth/server.py
+-rw-r--r--   0        0        0     6976 1970-01-01 00:00:00.000000 deezer_oauth_cli-1.2.8/PKG-INFO
```

### Comparing `deezer_oauth_cli-1.2.7/LICENSE` & `deezer_oauth_cli-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/README.md` & `deezer_oauth_cli-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/pyproject.toml` & `deezer_oauth_cli-1.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-oauth-cli"
-version = "1.2.7"
+version = "1.2.8"
 description = "A small CLI to quickly obtain an API token for Deezer API."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/deezer-oauth-cli"
 documentation = "https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md"
 classifiers = [
@@ -26,17 +26,17 @@
 "Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.scripts]
 deezer-oauth = "deezer_oauth.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.27"
+requests = ">=2.27"
 rich = ">=10"
-typer = {extras = ["all"], version = "^0.12.0"}
+typer = {extras = ["all"], version = ">=0.12.0"}
 
 [tool.poetry.group.dev.dependencies]
 pyfakefs = "^5.0"
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.6"
 responses = "^0.25.0"
```

### Comparing `deezer_oauth_cli-1.2.7/src/deezer_oauth/client.py` & `deezer_oauth_cli-1.2.8/src/deezer_oauth/client.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/src/deezer_oauth/files.py` & `deezer_oauth_cli-1.2.8/src/deezer_oauth/files.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/src/deezer_oauth/main.py` & `deezer_oauth_cli-1.2.8/src/deezer_oauth/main.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/src/deezer_oauth/server.py` & `deezer_oauth_cli-1.2.8/src/deezer_oauth/server.py`

 * *Files identical despite different names*

### Comparing `deezer_oauth_cli-1.2.7/PKG-INFO` & `deezer_oauth_cli-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-oauth-cli
-Version: 1.2.7
+Version: 1.2.8
 Summary: A small CLI to quickly obtain an API token for Deezer API.
 Home-page: https://github.com/browniebroke/deezer-oauth-cli
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: requests (>=2.27,<3.0)
+Requires-Dist: requests (>=2.27)
 Requires-Dist: rich (>=10)
-Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
+Requires-Dist: typer[all] (>=0.12.0)
 Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues
 Project-URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/README.md
 Project-URL: Mastodon, https://fosstodon.org/@browniebroke
 Project-URL: Repository, https://github.com/browniebroke/deezer-oauth-cli
 Project-URL: Twitter, https://twitter.com/_BrunoAlla
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.2.7 Summary: A small
+Metadata-Version: 2.1 Name: deezer-oauth-cli Version: 1.2.8 Summary: A small
 CLI to quickly obtain an API token for Deezer API. Home-page: https://
 github.com/browniebroke/deezer-oauth-cli License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: requests
-(>=2.27,<3.0) Requires-Dist: rich (>=10) Requires-Dist: typer[all]
-(>=0.12.0,<0.13.0) Project-URL: Bug Tracker, https://github.com/browniebroke/
-deezer-oauth-cli/issues Project-URL: Changelog, https://github.com/
-browniebroke/deezer-oauth-cli/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://github.com/browniebroke/deezer-oauth-cli/blob/main/
-README.md Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-
-URL: Repository, https://github.com/browniebroke/deezer-oauth-cli Project-URL:
-Twitter, https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown
-# Deezer OAuth CLI
+Topic :: Software Development :: Libraries Requires-Dist: requests (>=2.27)
+Requires-Dist: rich (>=10) Requires-Dist: typer[all] (>=0.12.0) Project-URL:
+Bug Tracker, https://github.com/browniebroke/deezer-oauth-cli/issues Project-
+URL: Changelog, https://github.com/browniebroke/deezer-oauth-cli/blob/main/
+CHANGELOG.md Project-URL: Documentation, https://github.com/browniebroke/
+deezer-oauth-cli/blob/main/README.md Project-URL: Mastodon, https://
+fosstodon.org/@browniebroke Project-URL: Repository, https://github.com/
+browniebroke/deezer-oauth-cli Project-URL: Twitter, https://twitter.com/
+_BrunoAlla Description-Content-Type: text/markdown # Deezer OAuth CLI
                      _[_C_I_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_r_o_w_n_i_e_b_r_o_k_e_/_d_e_e_z_e_r_-_o_a_u_t_h_-_c_l_i --- A
 small CLI to quickly obtain an API token for the Deezer API. Obtaining API
 token to develop API applications can be complicated and sometimes feel like a
 chicken and egg situation: it's hard to play with the API without a token, but
```

