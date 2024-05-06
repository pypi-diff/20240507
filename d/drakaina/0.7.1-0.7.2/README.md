# Comparing `tmp/drakaina-0.7.1.tar.gz` & `tmp/drakaina-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.1.tar", max compression
+gzip compressed data, was "drakaina-0.7.2.tar", max compression
```

## Comparing `drakaina-0.7.1.tar` & `drakaina-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     9452 2024-05-06 18:37:59.533917 drakaina-0.7.1/drakaina/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.1/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.1/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.1/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.1/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.1/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      351 2024-05-06 19:02:29.664147 drakaina-0.7.1/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     8986 2024-05-06 18:57:08.110107 drakaina-0.7.1/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.1/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18281 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.1/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.1/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.1/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7749 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     1991 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/middleware/exception.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.1/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12943 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.1/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     8028 2024-05-06 18:37:59.534916 drakaina-0.7.1/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    14864 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.1/drakaina/serializers.py
--rw-r--r--   0        0        0    34083 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/types.py
--rw-r--r--   0        0        0     6193 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/utils.py
--rw-r--r--   0        0        0     8288 2024-05-06 18:37:59.535920 drakaina-0.7.1/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.1/LICENSE
--rw-r--r--   0        0        0     2703 2024-05-06 19:02:47.259023 drakaina-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6992 2024-05-06 18:37:59.533917 drakaina-0.7.1/README.md
--rw-r--r--   0        0        0     8512 1970-01-01 00:00:00.000000 drakaina-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     9452 2024-05-06 18:37:59.533917 drakaina-0.7.2/drakaina/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.2/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.2/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.2/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.2/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.2/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-06 19:02:29.664147 drakaina-0.7.2/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     8970 2024-05-06 19:36:29.872629 drakaina-0.7.2/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.2/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18281 2024-05-06 18:37:59.534916 drakaina-0.7.2/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.2/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.2/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.2/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7749 2024-05-06 18:37:59.534916 drakaina-0.7.2/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1991 2024-05-06 18:37:59.534916 drakaina-0.7.2/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.2/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12943 2024-05-06 18:37:59.534916 drakaina-0.7.2/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.2/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     8028 2024-05-06 18:37:59.534916 drakaina-0.7.2/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    14864 2024-05-06 18:37:59.535920 drakaina-0.7.2/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.2/drakaina/serializers.py
+-rw-r--r--   0        0        0    34083 2024-05-06 18:37:59.535920 drakaina-0.7.2/drakaina/types.py
+-rw-r--r--   0        0        0     6193 2024-05-06 18:37:59.535920 drakaina-0.7.2/drakaina/utils.py
+-rw-r--r--   0        0        0     8288 2024-05-06 18:37:59.535920 drakaina-0.7.2/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2684 2024-05-06 19:58:12.500005 drakaina-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6992 2024-05-06 18:37:59.533917 drakaina-0.7.2/README.md
+-rw-r--r--   0        0        0     8462 1970-01-01 00:00:00.000000 drakaina-0.7.2/PKG-INFO
```

### Comparing `drakaina-0.7.1/drakaina/__init__.py` & `drakaina-0.7.2/drakaina/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/contrib/django/__init__.py` & `drakaina-0.7.2/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/contrib/django/middleware.py` & `drakaina-0.7.2/drakaina/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/contrib/django/views.py` & `drakaina-0.7.2/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.2/drakaina/contrib/jwt/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                     raise error
                 else:
                     token_payload = decode_jwt_token(
                         token=token,
                         algorithms=self._algorithms,
                         verify_key=self.__verify_key,
                         verify=False,
-                        decode_options=self._decode_options,
+                        decode_options=None,
                         verify_values=self._verify_values,
                         leeway=self._leeway,
                     )
                     token_is_valid = environ.get(ENV_IS_AUTHENTICATED, False)
 
             if callable(self.is_revoked):
                 if self.is_revoked(environ, token_payload):
```

### Comparing `drakaina-0.7.1/drakaina/contrib/jwt/types.py` & `drakaina-0.7.2/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.2/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/exceptions.py` & `drakaina-0.7.2/drakaina/exceptions.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/middleware/base.py` & `drakaina-0.7.2/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/middleware/cors.py` & `drakaina-0.7.2/drakaina/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/middleware/exception.py` & `drakaina-0.7.2/drakaina/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.2/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/registries.py` & `drakaina-0.7.2/drakaina/registries.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/rpc_protocols/base.py` & `drakaina-0.7.2/drakaina/rpc_protocols/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.2/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/serializers.py` & `drakaina-0.7.2/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/types.py` & `drakaina-0.7.2/drakaina/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/utils.py` & `drakaina-0.7.2/drakaina/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/drakaina/wsgi.py` & `drakaina-0.7.2/drakaina/wsgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/LICENSE` & `drakaina-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/pyproject.toml` & `drakaina-0.7.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.1"
+version = "0.7.2"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -20,15 +20,15 @@
 homepage  = "https://gitlab.com/tau_lex/drakaina"
 repository = "https://gitlab.com/tau_lex/drakaina"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 typing-extensions = "^4.6.2"
 msgpack = { version = "^1.0.5", optional = true }
 orjson = { version = "^3.8.14", optional = true }
 ujson = { version = "^5.7.0", optional = true }
 pyjwt = { version = "^2.7.0", optional = true }
 docstring-parser = { version = "^0.15", optional = true }
 
@@ -39,32 +39,31 @@
 msgpack = ["msgpack"]
 docs = ["docstring-parser"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["d"], version = "^22.12.0"}
-pre-commit = "^3.3.2"
-ruff = "^0.0.269"
-msgpack = "^1.0.4"
-orjson = "^3.8.6"
-pytest = "^7.3.1"
-ujson = "^5.7.0"
-pyjwt = "^2.7.0"
+black = {extras = ["d"], version = "^24.4.2"}
+pre-commit = "^3.7.0"
+ruff = "^0.1.15"
+msgpack = "^1.0.8"
+orjson = "^3.10.3"
+ujson = "^5.9.0"
+pyjwt = "^2.8.0"
 django = ">=3.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.1"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.1.0"
-httpx = "^0.23.3"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-cov = "^5.0.0"
+httpx = "^0.27.0"
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 testpaths = "tests"
 addopts = "-vl --cov=drakaina --cov-report term-missing --tb=auto --capture=sys"
 
 [tool.ruff]
@@ -90,20 +89,20 @@
 
 # Same as Black.
 line-length = 80
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py39"]
 line-length = 80
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drakaina-0.7.1/README.md` & `drakaina-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.1/PKG-INFO` & `drakaina-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.1
+Version: 0.7.2
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Provides-Extra: docs
```

