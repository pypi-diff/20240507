# Comparing `tmp/st-paywall-0.1.6.tar.gz` & `tmp/st_paywall-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-paywall-0.1.6.tar", last modified: Wed Nov  1 03:44:36 2023, max compression
+gzip compressed data, was "st_paywall-0.1.7.tar", last modified: Tue May  7 17:31:44 2024, max compression
```

## Comparing `st-paywall-0.1.6.tar` & `st_paywall-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-11-01 03:44:36.218254 st-paywall-0.1.6/
--rw-r--r--   0 trichards   (501) staff       (20)     1068 2023-11-01 02:41:41.000000 st-paywall-0.1.6/LICENSE
--rw-r--r--   0 trichards   (501) staff       (20)     3547 2023-11-01 03:44:36.217914 st-paywall-0.1.6/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     3166 2023-07-28 21:28:03.000000 st-paywall-0.1.6/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      417 2023-11-01 03:44:28.000000 st-paywall-0.1.6/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-11-01 03:44:36.218314 st-paywall-0.1.6/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-11-01 03:44:36.211439 st-paywall-0.1.6/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-11-01 03:44:36.215089 st-paywall-0.1.6/src/st_paywall/
--rw-r--r--   0 trichards   (501) staff       (20)       45 2023-07-28 21:28:03.000000 st-paywall-0.1.6/src/st_paywall/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     3149 2023-11-01 03:42:55.000000 st-paywall-0.1.6/src/st_paywall/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1414 2023-07-28 21:28:03.000000 st-paywall-0.1.6/src/st_paywall/buymeacoffee_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     3132 2023-11-01 03:40:43.000000 st-paywall-0.1.6/src/st_paywall/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1746 2023-11-01 03:42:55.000000 st-paywall-0.1.6/src/st_paywall/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-11-01 03:44:36.217404 st-paywall-0.1.6/src/st_paywall.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     3547 2023-11-01 03:44:36.000000 st-paywall-0.1.6/src/st_paywall.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      377 2023-11-01 03:44:36.000000 st-paywall-0.1.6/src/st_paywall.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-11-01 03:44:36.000000 st-paywall-0.1.6/src/st_paywall.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       43 2023-11-01 03:44:36.000000 st-paywall-0.1.6/src/st_paywall.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       11 2023-11-01 03:44:36.000000 st-paywall-0.1.6/src/st_paywall.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.780587 st_paywall-0.1.7/
+-rw-r--r--   0 trichards   (501) staff       (20)     1068 2024-03-24 02:06:46.000000 st_paywall-0.1.7/LICENSE
+-rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-07 17:31:44.780159 st_paywall-0.1.7/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     3166 2023-09-24 19:23:05.000000 st_paywall-0.1.7/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      417 2024-05-07 17:30:19.000000 st_paywall-0.1.7/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2024-05-07 17:31:44.780639 st_paywall-0.1.7/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.773295 st_paywall-0.1.7/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.776184 st_paywall-0.1.7/src/st_paywall/
+-rw-r--r--   0 trichards   (501) staff       (20)       45 2023-09-24 19:23:05.000000 st_paywall-0.1.7/src/st_paywall/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     3149 2024-03-24 02:06:49.000000 st_paywall-0.1.7/src/st_paywall/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1414 2023-09-24 19:23:05.000000 st_paywall-0.1.7/src/st_paywall/buymeacoffee_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     3112 2024-05-07 17:30:19.000000 st_paywall-0.1.7/src/st_paywall/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1746 2024-03-24 02:06:49.000000 st_paywall-0.1.7/src/st_paywall/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2024-05-07 17:31:44.779658 st_paywall-0.1.7/src/st_paywall.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     3547 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      377 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       43 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       11 2024-05-07 17:31:44.000000 st_paywall-0.1.7/src/st_paywall.egg-info/top_level.txt
```

### Comparing `st-paywall-0.1.6/LICENSE` & `st_paywall-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.6/PKG-INFO` & `st_paywall-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler Richards <tylerjrichards@gmail.com>
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stripe
 Requires-Dist: httpx-oauth
 Requires-Dist: pyjwt
-Requires-Dist: streamlit>=1.27.0
+Requires-Dist: streamlit>=1.30.0
 
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
```

### Comparing `st-paywall-0.1.6/README.md` & `st_paywall-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.6/src/st_paywall/aggregate_auth.py` & `st_paywall-0.1.7/src/st_paywall/aggregate_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.6/src/st_paywall/buymeacoffee_auth.py` & `st_paywall-0.1.7/src/st_paywall/buymeacoffee_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.6/src/st_paywall/google_auth.py` & `st_paywall-0.1.7/src/st_paywall/google_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,21 +77,21 @@
     token = await client.get_access_token(code, redirect_url)
     return token
 
 
 def get_access_token_from_query_params(
     client: GoogleOAuth2, redirect_url: str
 ) -> OAuth2Token:
-    query_params = st.experimental_get_query_params()
+    query_params = st.query_params.get_all()
     code = query_params["code"][0]
     token = asyncio.run(
         get_access_token(client=client, redirect_url=redirect_url, code=code)
     )
     # Clear query params
-    st.experimental_set_query_params()
+    st.query_params.clear()
     return token
 
 
 def show_login_button(
     text: Optional[str] = "Login with Google", color="#FD504D", sidebar: bool = True
 ):
     authorization_url = asyncio.run(
```

### Comparing `st-paywall-0.1.6/src/st_paywall/stripe_auth.py` & `st_paywall-0.1.7/src/st_paywall/stripe_auth.py`

 * *Files identical despite different names*

### Comparing `st-paywall-0.1.6/src/st_paywall.egg-info/PKG-INFO` & `st_paywall-0.1.7/src/st_paywall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: st-paywall
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler Richards <tylerjrichards@gmail.com>
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stripe
 Requires-Dist: httpx-oauth
 Requires-Dist: pyjwt
-Requires-Dist: streamlit>=1.27.0
+Requires-Dist: streamlit>=1.30.0
 
 [![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 Author: [@tylerjrichards](https://twitter.com/tylerjrichards)
```

