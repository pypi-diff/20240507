# Comparing `tmp/unkey_py-0.7.1.tar.gz` & `tmp/unkey_py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unkey_py-0.7.1.tar", max compression
+gzip compressed data, was "unkey_py-0.7.2.tar", max compression
```

## Comparing `unkey_py-0.7.1.tar` & `unkey_py-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2024-02-04 16:23:59.235586 unkey_py-0.7.1/LICENSE
--rw-r--r--   0        0        0     1872 2024-02-04 16:23:59.235586 unkey_py-0.7.1/README.md
--rw-r--r--   0        0        0     2311 2024-02-04 16:23:59.235586 unkey_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1732 2024-02-04 16:23:59.307586 unkey_py-0.7.1/unkey/__init__.py
--rw-r--r--   0        0        0      643 2024-02-04 16:23:59.235586 unkey_py-0.7.1/unkey/__main__.py
--rw-r--r--   0        0        0     2511 2024-02-04 16:23:59.235586 unkey_py-0.7.1/unkey/client.py
--rw-r--r--   0        0        0      332 2024-02-04 16:23:59.235586 unkey_py-0.7.1/unkey/constants.py
--rw-r--r--   0        0        0     5076 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/decorators.py
--rw-r--r--   0        0        0      656 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/errors.py
--rw-r--r--   0        0        0      365 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/models/__init__.py
--rw-r--r--   0        0        0      822 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/models/apis.py
--rw-r--r--   0        0        0     1627 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/models/base.py
--rw-r--r--   0        0        0      942 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/models/http.py
--rw-r--r--   0        0        0     4915 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/models/keys.py
--rw-r--r--   0        0        0        0 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/py.typed
--rw-r--r--   0        0        0     2230 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/result.py
--rw-r--r--   0        0        0     2303 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/routes.py
--rw-r--r--   0        0        0     4505 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/serializer.py
--rw-r--r--   0        0        0      151 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/services/__init__.py
--rw-r--r--   0        0        0     2030 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/services/apis.py
--rw-r--r--   0        0        0     1323 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/services/base.py
--rw-r--r--   0        0        0     4717 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/services/http.py
--rw-r--r--   0        0        0     8375 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/services/keys.py
--rw-r--r--   0        0        0     1658 2024-02-04 16:23:59.239586 unkey_py-0.7.1/unkey/undefined.py
--rw-r--r--   0        0        0     3009 1970-01-01 00:00:00.000000 unkey_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-07 00:31:51.065612 unkey_py-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1939 2024-05-07 00:31:51.065612 unkey_py-0.7.2/README.md
+-rw-r--r--   0        0        0     2311 2024-05-07 00:31:51.069613 unkey_py-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1732 2024-05-07 00:31:51.145613 unkey_py-0.7.2/unkey/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/__main__.py
+-rw-r--r--   0        0        0     2701 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/client.py
+-rw-r--r--   0        0        0      332 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/constants.py
+-rw-r--r--   0        0        0     5017 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/decorators.py
+-rw-r--r--   0        0        0      656 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/errors.py
+-rw-r--r--   0        0        0      365 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/models/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/models/apis.py
+-rw-r--r--   0        0        0     1627 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/models/base.py
+-rw-r--r--   0        0        0      942 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/models/http.py
+-rw-r--r--   0        0        0     4915 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/models/keys.py
+-rw-r--r--   0        0        0        0 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/py.typed
+-rw-r--r--   0        0        0     2230 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/result.py
+-rw-r--r--   0        0        0     2303 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/routes.py
+-rw-r--r--   0        0        0     4505 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/serializer.py
+-rw-r--r--   0        0        0      151 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/services/__init__.py
+-rw-r--r--   0        0        0     2030 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/services/apis.py
+-rw-r--r--   0        0        0     1323 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/services/base.py
+-rw-r--r--   0        0        0     4717 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/services/http.py
+-rw-r--r--   0        0        0     8375 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/services/keys.py
+-rw-r--r--   0        0        0     2913 2024-05-07 00:31:51.069613 unkey_py-0.7.2/unkey/undefined.py
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 unkey_py-0.7.2/PKG-INFO
```

### Comparing `unkey_py-0.7.1/LICENSE` & `unkey_py-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/README.md` & `unkey_py-0.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,7 +74,9 @@
 
 unkey.py is open to contributions. Check out the
 [contributing guide](https://github.com/Jonxslays/unkey.py/blob/master/CONTRIBUTING.md) to learn how.
 
 ## License
 
 unkey.py is licensed under the [GPLv3 License](https://github.com/Jonxslays/unkey.py/blob/master/LICENSE).
+
+The `unkey.undefined` module is licensed under the `MIT License`.
```

### Comparing `unkey_py-0.7.1/pyproject.toml` & `unkey_py-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unkey.py"
-version = "0.7.1"
+version = "0.7.2"
 description = "An asynchronous Python SDK for unkey.dev."
 authors = ["Jonxslays"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/unkey.py"
 repository = "https://github.com/Jonxslays/unkey.py"
 packages = [{ include = "unkey" }, { include = "unkey/py.typed" }]
```

### Comparing `unkey_py-0.7.1/unkey/__init__.py` & `unkey_py-0.7.2/unkey/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "unkey.py"
-__version__: Final[str] = "0.7.1"
+__version__: Final[str] = "0.7.2"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous Python SDK for unkey.dev."
 __url__: Final[str] = "https://github.com/Jonxslays/unkey.py"
 __docs__: Final[str] = "https://jonxslays.github.io/unkey.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "GPL-3.0"
-__git_sha__: Final[str] = "[024513f]"
+__git_sha__: Final[str] = "[8f161fb]"
 
 from . import client
 from . import decorators
 from . import constants
 from . import errors
 from . import models
 from . import result
```

### Comparing `unkey_py-0.7.1/unkey/__main__.py` & `unkey_py-0.7.2/unkey/__main__.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/client.py` & `unkey_py-0.7.2/unkey/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 
     def __init_service(self, service: t.Type[ServiceT]) -> ServiceT:
         if not issubclass(service, services.BaseService):
             raise TypeError(f"{service.__name__!r} can not be initialized as a service.")
 
         return service(self._http, self._serializer)  # type: ignore[return-value]
 
+    async def __aenter__(self) -> Client:
+        await self.start()
+        return self
+
+    async def __aexit__(self, *_args: t.Any, **_kwargs: t.Any) -> None:
+        await self.close()
+
     @property
     def keys(self) -> services.KeyService:
         """The key service used to make key related requests."""
         return self._keys
 
     @property
     def apis(self) -> services.ApiService:
```

### Comparing `unkey_py-0.7.1/unkey/decorators.py` & `unkey_py-0.7.2/unkey/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 DecoratorT = CallableT[CallbackT]
 VerificationResponseT = Union[T, Any]
 ExtractorT = Callable[[Tuple[Any], Dict[str, Any]], Optional[str]]
 """The type of a callback used to extract the api key from the decorated
 functions `*args` and `**kwargs`.
 """
 
-InvalidKeyHandlerT = Optional[Callable[[Dict[str, Any], Optional[models.ApiKeyVerification]], Any]]
+InvalidKeyHandlerT = Callable[[Dict[str, Any], Optional[models.ApiKeyVerification]], Any]
 """The type of a callback used to handle cases where the key was invalid."""
 
-ExcHandlerT = Optional[Callable[[Exception], Any]]
+ExcHandlerT = Callable[[Exception], Any]
 """The type of a callback used to handle exceptions during verification."""
 
 
 def protected(
     api_id: str,
     key_extractor: ExtractorT,
-    on_invalid_key: InvalidKeyHandlerT = None,
-    on_exc: ExcHandlerT = None,
+    on_invalid_key: Optional[InvalidKeyHandlerT] = None,
+    on_exc: Optional[ExcHandlerT] = None,
 ) -> DecoratorT:
     """A framework agnostic second order decorator that is used to protect
     api routes with Unkey key verification.
 
     !!! info
 
         An endpoint decorated with this decorator guarantees that once the
@@ -78,15 +78,14 @@
         A function that replaces the decorated function, and performs Unkey
             key verification prior to calling the decorated function.
             If the key could not be parsed or was invalid, a dictionary
             containing "code" and "message" keys will be returned, unless
             altered by `on_invalid_key` if it was passed. If verification
             succeeds the original functions return value is returned.
     """
-    _client = client.Client()
 
     def _on_invalid_key(
         data: Dict[str, Any], verification: Optional[models.ApiKeyVerification] = None
     ) -> Any:
         if on_invalid_key:
             return on_invalid_key(data, verification)
 
@@ -104,17 +103,16 @@
         @functools.wraps(func)
         async def inner(*args: Any, **kwargs: Any) -> VerificationResponseT[T]:
             try:
                 if not (key := key_extractor(*args, **kwargs)):
                     message = "Failed to extract API key"
                     return _on_invalid_key({"code": None, "message": message})
 
-                await _client.start()
-                result = await _client.keys.verify_key(key, api_id)
-                await _client.close()
+                async with client.Client() as c:
+                    result = await c.keys.verify_key(key, api_id)
 
                 if result.is_err:
                     err = result.unwrap_err()
                     code = (err.code or models.ErrorCode.Unknown).value
                     return _on_invalid_key({"code": code, "message": err.message})
 
                 verification = result.unwrap()
```

### Comparing `unkey_py-0.7.1/unkey/errors.py` & `unkey_py-0.7.2/unkey/errors.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/models/apis.py` & `unkey_py-0.7.2/unkey/models/apis.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/models/base.py` & `unkey_py-0.7.2/unkey/models/base.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/models/http.py` & `unkey_py-0.7.2/unkey/models/http.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/models/keys.py` & `unkey_py-0.7.2/unkey/models/keys.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/result.py` & `unkey_py-0.7.2/unkey/result.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/routes.py` & `unkey_py-0.7.2/unkey/routes.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/serializer.py` & `unkey_py-0.7.2/unkey/serializer.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/services/apis.py` & `unkey_py-0.7.2/unkey/services/apis.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/services/base.py` & `unkey_py-0.7.2/unkey/services/base.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/services/http.py` & `unkey_py-0.7.2/unkey/services/http.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/unkey/services/keys.py` & `unkey_py-0.7.2/unkey/services/keys.py`

 * *Files identical despite different names*

### Comparing `unkey_py-0.7.1/PKG-INFO` & `unkey_py-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unkey.py
-Version: 0.7.1
+Version: 0.7.2
 Summary: An asynchronous Python SDK for unkey.dev.
 Home-page: https://github.com/Jonxslays/unkey.py
 License: GPL-3.0-only
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -103,7 +103,9 @@
 unkey.py is open to contributions. Check out the
 [contributing guide](https://github.com/Jonxslays/unkey.py/blob/master/CONTRIBUTING.md) to learn how.
 
 ## License
 
 unkey.py is licensed under the [GPLv3 License](https://github.com/Jonxslays/unkey.py/blob/master/LICENSE).
 
+The `unkey.undefined` module is licensed under the `MIT License`.
+
```

