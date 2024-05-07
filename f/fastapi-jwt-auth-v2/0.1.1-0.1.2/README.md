# Comparing `tmp/fastapi_jwt_auth_v2-0.1.1.tar.gz` & `tmp/fastapi_jwt_auth_v2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_jwt_auth_v2-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_jwt_auth_v2-0.1.2.tar", max compression
```

## Comparing `fastapi_jwt_auth_v2-0.1.1.tar` & `fastapi_jwt_auth_v2-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2024-02-10 15:13:03.669050 fastapi_jwt_auth_v2-0.1.1/LICENSE
--rw-r--r--   0        0        0     1702 2024-02-10 15:13:03.669050 fastapi_jwt_auth_v2-0.1.1/README.md
--rw-r--r--   0        0        0      147 2024-02-10 15:13:03.673050 fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/__init__.py
--rw-r--r--   0        0        0     4957 2024-03-20 13:59:25.989766 fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/auth_config.py
--rw-r--r--   0        0        0    36416 2024-03-20 13:59:26.697682 fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/auth_jwt.py
--rw-r--r--   0        0        0     4300 2024-03-20 13:59:26.401717 fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/config.py
--rw-r--r--   0        0        0     2233 2024-03-20 13:59:26.361722 fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/exceptions.py
--rw-r--r--   0        0        0      647 2024-03-20 14:13:13.846183 fastapi_jwt_auth_v2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 fastapi_jwt_auth_v2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-07 18:04:51.220820 fastapi_jwt_auth_v2-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1702 2024-05-07 18:04:51.220820 fastapi_jwt_auth_v2-0.1.2/README.md
+-rw-r--r--   0        0        0      147 2024-02-10 15:13:03.673050 fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/__init__.py
+-rw-r--r--   0        0        0     4957 2024-03-20 13:59:25.989766 fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/auth_config.py
+-rw-r--r--   0        0        0    36416 2024-03-20 13:59:26.697682 fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/auth_jwt.py
+-rw-r--r--   0        0        0     4300 2024-03-20 13:59:26.401717 fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/config.py
+-rw-r--r--   0        0        0     2233 2024-03-20 13:59:26.361722 fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/exceptions.py
+-rw-r--r--   0        0        0      549 2024-05-07 18:30:49.743880 fastapi_jwt_auth_v2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 fastapi_jwt_auth_v2-0.1.2/PKG-INFO
```

### Comparing `fastapi_jwt_auth_v2-0.1.1/LICENSE` & `fastapi_jwt_auth_v2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/README.md` & `fastapi_jwt_auth_v2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/auth_config.py` & `fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/auth_jwt.py` & `fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/config.py` & `fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/fastapi_jwt_auth/exceptions.py` & `fastapi_jwt_auth_v2-0.1.2/fastapi_jwt_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jwt_auth_v2-0.1.1/pyproject.toml` & `fastapi_jwt_auth_v2-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 [tool.poetry]
 name = "fastapi-jwt-auth-v2"
-packages = [
-    {include = "fastapi_jwt_auth"}
-]
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Daniel Chico <chico@generalsoftwareinc.com>"]
 readme = "README.md"
-
+packages = [
+    { include = "fastapi_jwt_auth" },
+]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.12"
+fastapi = "^0.111.0"
 pyjwt = "^2.8.0"
-fastapi = "^0.110.0"
 
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.1.1"
-httpx = "^0.27.0"
-pydantic-settings = "^2.2.1"
+pytest = "^8.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
-autoflake = "^2.3.1"
-isort = "^5.13.2"
-black = "^24.3.0"
-
-[tool.poetry.group.asymmetric.dependencies]
-cryptography = "^42.0.5"
+uvicorn = "^0.29.0"
+cryptography = "^42.0.7"
+pydantic-settings = "^2.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_jwt_auth_v2-0.1.1/PKG-INFO` & `fastapi_jwt_auth_v2-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi-jwt-auth-v2
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Daniel Chico
 Author-email: chico@generalsoftwareinc.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   FastAPI JWT Auth V2
 </h1>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: fastapi-jwt-auth-v2 Version: 0.1.1 Summary: Author:
+Metadata-Version: 2.1 Name: fastapi-jwt-auth-v2 Version: 0.1.2 Summary: Author:
 Daniel Chico Author-email: chico@generalsoftwareinc.com Requires-Python:
->=3.11,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: fastapi
-(>=0.110.0,<0.111.0) Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Description-Content-
+>=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.12 Requires-Dist: fastapi
+(>=0.111.0,<0.112.0) Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Description-Content-
 Type: text/markdown
 ************ FFaassttAAPPII JJWWTT AAuutthh VV22 ************
 ![Tests](https://github.com/DanielChico/fastapi-jwt-auth-v2/workflows/Tests/
 badge.svg) [![Coverage Status](https://coveralls.io/repos/github/DanielChico/
 fastapi-jwt-auth-v2/badge.svg?branch=master)](https://coveralls.io/github/
 DanielChico/fastapi-jwt-auth-v2?branch=master) [![PyPI version](https://
 badge.fury.io/py/fastapi-jwt-auth-v2.svg)](https://badge.fury.io/py/fastapi-
```

