# Comparing `tmp/iaptoolkit-0.0.4.3.tar.gz` & `tmp/iaptoolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaptoolkit-0.0.4.3.tar", max compression
+gzip compressed data, was "iaptoolkit-0.0.5.tar", max compression
```

## Comparing `iaptoolkit-0.0.4.3.tar` & `iaptoolkit-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/LICENSE
--rwxr-xr-x   0        0        0     1343 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/README.md
--rwxr-xr-x   0        0        0     1012 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/pyproject.toml
--rw-r--r--   0        0        0       77 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/__init__.py
--rw-r--r--   0        0        0      522 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/constants.py
--rw-r--r--   0        0        0     1507 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/exceptions.py
--rw-r--r--   0        0        0     4041 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/headers.py
--rw-r--r--   0        0        0      931 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/__init__.py
--rw-r--r--   0        0        0     7750 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/service_account.py
--rw-r--r--   0        0        0     1330 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/structs.py
--rw-r--r--   0        0        0     2689 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/token_datastore.py
--rw-r--r--   0        0        0        0 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/utils/__init__.py
--rw-r--r--   0        0        0     1477 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/utils/urls.py
--rw-r--r--   0        0        0      817 2024-04-22 11:07:06.984136 iaptoolkit-0.0.4.3/src/iaptoolkit/vars.py
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 iaptoolkit-0.0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     1343 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/README.md
+-rwxr-xr-x   0        0        0     1010 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/constants.py
+-rw-r--r--   0        0        0     1507 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/exceptions.py
+-rw-r--r--   0        0        0     4041 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/headers.py
+-rw-r--r--   0        0        0      931 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/__init__.py
+-rw-r--r--   0        0        0     8135 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/service_account.py
+-rw-r--r--   0        0        0     1330 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/structs.py
+-rw-r--r--   0        0        0     2689 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/tokens/token_datastore.py
+-rw-r--r--   0        0        0        0 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     1477 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/utils/urls.py
+-rw-r--r--   0        0        0      817 2024-05-07 11:17:27.221503 iaptoolkit-0.0.5/src/iaptoolkit/vars.py
+-rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 iaptoolkit-0.0.5/PKG-INFO
```

### Comparing `iaptoolkit-0.0.4.3/LICENSE` & `iaptoolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/README.md` & `iaptoolkit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/pyproject.toml` & `iaptoolkit-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iaptoolkit"
-version = "0.0.4.3"
+version = "0.0.5"
 description = "Library of common utils for interacting with Identity-Aware Proxies"
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -20,15 +20,15 @@
 target-version = ['py311']
 include = '\.pyi?$'
 
 # ================================
 # Dependencies
 [tool.poetry.dependencies]
 python = "^3.11"
-google-auth = "^2.26.2"
+google-auth = "^2.29.0"
 requests = "^2.31.0"
 pytest = "^7.4.4"
 toml = "^0.10.2"
 kvcommon = "^0.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
```

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/constants.py` & `iaptoolkit-0.0.5/src/iaptoolkit/constants.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/exceptions.py` & `iaptoolkit-0.0.5/src/iaptoolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/headers.py` & `iaptoolkit-0.0.5/src/iaptoolkit/headers.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/__init__.py` & `iaptoolkit-0.0.5/src/iaptoolkit/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/service_account.py` & `iaptoolkit-0.0.5/src/iaptoolkit/tokens/service_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,22 @@
             )
         return credentials
 
     @staticmethod
     def _get_fresh_token(iap_client_id: str) -> TokenStruct:
         google_credentials = ServiceAccount._get_fresh_credentials(iap_client_id)
         id_token: str = str(google_credentials.token)
-        return TokenStruct(id_token=id_token, expiry=google_credentials.expiry)
+
+        # Google lib uses deprecated 'utcfromtimestamp' func as of v2.29.x
+        # e.g.: datetime.datetime.utcfromtimestamp(payload["exp"])
+        # This creates a TZ-naive datetime in UTC from a POSIX timestamp.
+        # Python datetimes assume local TZ, and we want to explicitly only work in UTC here.
+        token_expiry = google_credentials.expiry.replace(tzinfo=datetime.timezone.utc)
+
+        return TokenStruct(id_token=id_token, expiry=token_expiry)
 
     @staticmethod
     def get_token(
         iap_client_id: str, bypass_cached: bool = False, attempts: int = 0
     ) -> TokenRefreshStruct:
         """Retrieves an OIDC token for the current environment either from environment variable or from
         metadata service.
```

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/structs.py` & `iaptoolkit-0.0.5/src/iaptoolkit/tokens/structs.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/tokens/token_datastore.py` & `iaptoolkit-0.0.5/src/iaptoolkit/tokens/token_datastore.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/utils/urls.py` & `iaptoolkit-0.0.5/src/iaptoolkit/utils/urls.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/src/iaptoolkit/vars.py` & `iaptoolkit-0.0.5/src/iaptoolkit/vars.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.0.4.3/PKG-INFO` & `iaptoolkit-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: iaptoolkit
-Version: 0.0.4.3
+Version: 0.0.5
 Summary: Library of common utils for interacting with Identity-Aware Proxies
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: google-auth (>=2.26.2,<3.0.0)
+Requires-Dist: google-auth (>=2.29.0,<3.0.0)
 Requires-Dist: kvcommon (>=0.1.0,<0.2.0)
 Requires-Dist: pytest (>=7.4.4,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # IAP Toolkit
```

