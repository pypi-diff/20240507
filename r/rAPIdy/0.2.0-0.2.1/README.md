# Comparing `tmp/rapidy-0.2.0.tar.gz` & `tmp/rapidy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidy-0.2.0.tar", max compression
+gzip compressed data, was "rapidy-0.2.1.tar", max compression
```

## Comparing `rapidy-0.2.0.tar` & `rapidy-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1079 2024-04-22 08:38:32.528691 rapidy-0.2.0/LICENSE
--rw-r--r--   0        0        0    19477 2024-05-03 20:23:55.332530 rapidy-0.2.0/README.md
--rw-r--r--   0        0        0     5921 2024-05-03 20:54:52.580860 rapidy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7822 2024-04-30 11:15:43.280798 rapidy-0.2.0/rapidy/__init__.py
--rw-r--r--   0        0        0    12717 2024-04-22 03:22:22.724232 rapidy-0.2.0/rapidy/_annotation_container.py
--rw-r--r--   0        0        0     9154 2024-04-22 03:22:22.724232 rapidy-0.2.0/rapidy/_annotation_extractor.py
--rw-r--r--   0        0        0     4382 2024-04-22 08:38:32.528691 rapidy-0.2.0/rapidy/_client_errors.py
--rw-r--r--   0        0        0     9279 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/_extractors.py
--rw-r--r--   0        0        0     7400 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_fields.py
--rw-r--r--   0        0        0      627 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/_parsers.py
--rw-r--r--   0        0        0      474 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_request_params_base.py
--rw-r--r--   0        0        0     2565 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_validators.py
--rw-r--r--   0        0        0      614 2024-04-22 08:38:32.528691 rapidy-0.2.0/rapidy/_version.py
--rw-r--r--   0        0        0      285 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/constants.py
--rw-r--r--   0        0        0     3496 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/hdrs.py
--rw-r--r--   0        0        0      290 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/media_types.py
--rw-r--r--   0        0        0      169 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/__init__.py
--rw-r--r--   0        0        0      929 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/_api_errors.py
--rw-r--r--   0        0        0     4463 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/mypy/_type_helpers.py
--rw-r--r--   0        0        0      146 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/_version.py
--rw-r--r--   0        0        0     5485 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/plugin.py
--rw-r--r--   0        0        0        7 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/py.typed
--rw-r--r--   0        0        0    11108 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/request_params.py
--rw-r--r--   0        0        0      218 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/streams.py
--rw-r--r--   0        0        0     2363 2024-05-02 21:51:29.755968 rapidy-0.2.0/rapidy/typedefs.py
--rw-r--r--   0        0        0     9009 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web.py
--rw-r--r--   0        0        0     8310 2024-05-02 22:30:37.509688 rapidy-0.2.0/rapidy/web_app.py
--rw-r--r--   0        0        0    12391 2024-05-02 21:51:29.755968 rapidy-0.2.0/rapidy/web_exceptions.py
--rw-r--r--   0        0        0      140 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web_middlewares.py
--rw-r--r--   0        0        0      130 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web_request.py
--rw-r--r--   0        0        0     2483 2024-05-02 22:30:37.510688 rapidy-0.2.0/rapidy/web_response.py
--rw-r--r--   0        0        0     2926 2024-04-22 03:22:22.726232 rapidy-0.2.0/rapidy/web_routedef.py
--rw-r--r--   0        0        0      350 2024-04-22 03:22:22.726232 rapidy-0.2.0/rapidy/web_runner.py
--rw-r--r--   0        0        0     5682 2024-04-22 08:38:32.529691 rapidy-0.2.0/rapidy/web_urldispatcher.py
--rw-r--r--   0        0        0    20927 1970-01-01 00:00:00.000000 rapidy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-22 08:38:32.528691 rapidy-0.2.1/LICENSE
+-rw-r--r--   0        0        0    19477 2024-05-03 20:23:55.332530 rapidy-0.2.1/README.md
+-rw-r--r--   0        0        0     5921 2024-05-07 20:37:17.601436 rapidy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7822 2024-05-07 20:28:28.108186 rapidy-0.2.1/rapidy/__init__.py
+-rw-r--r--   0        0        0    13191 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/_annotation_container.py
+-rw-r--r--   0        0        0     9154 2024-04-22 03:22:22.724232 rapidy-0.2.1/rapidy/_annotation_extractor.py
+-rw-r--r--   0        0        0     4382 2024-04-22 08:38:32.528691 rapidy-0.2.1/rapidy/_client_errors.py
+-rw-r--r--   0        0        0     9279 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/_extractors.py
+-rw-r--r--   0        0        0     6045 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/_fields.py
+-rw-r--r--   0        0        0      627 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/_parsers.py
+-rw-r--r--   0        0        0      474 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/_request_params_base.py
+-rw-r--r--   0        0        0     2565 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/_validators.py
+-rw-r--r--   0        0        0      614 2024-04-22 08:38:32.528691 rapidy-0.2.1/rapidy/_version.py
+-rw-r--r--   0        0        0     1011 2024-05-07 20:13:27.764531 rapidy-0.2.1/rapidy/_web_request_validation.py
+-rw-r--r--   0        0        0      285 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/constants.py
+-rw-r--r--   0        0        0     3496 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/hdrs.py
+-rw-r--r--   0        0        0      290 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/media_types.py
+-rw-r--r--   0        0        0      169 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/_api_errors.py
+-rw-r--r--   0        0        0     4463 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/mypy/_type_helpers.py
+-rw-r--r--   0        0        0      146 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/_version.py
+-rw-r--r--   0        0        0     5485 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/plugin.py
+-rw-r--r--   0        0        0        7 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/py.typed
+-rw-r--r--   0        0        0    11108 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/request_params.py
+-rw-r--r--   0        0        0      218 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/streams.py
+-rw-r--r--   0        0        0     2363 2024-05-02 21:51:29.755968 rapidy-0.2.1/rapidy/typedefs.py
+-rw-r--r--   0        0        0     9009 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web.py
+-rw-r--r--   0        0        0     7956 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/web_app.py
+-rw-r--r--   0        0        0    12391 2024-05-02 21:51:29.755968 rapidy-0.2.1/rapidy/web_exceptions.py
+-rw-r--r--   0        0        0      140 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web_middlewares.py
+-rw-r--r--   0        0        0      130 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web_request.py
+-rw-r--r--   0        0        0     2483 2024-05-02 22:30:37.510688 rapidy-0.2.1/rapidy/web_response.py
+-rw-r--r--   0        0        0     2926 2024-04-22 03:22:22.726232 rapidy-0.2.1/rapidy/web_routedef.py
+-rw-r--r--   0        0        0      350 2024-04-22 03:22:22.726232 rapidy-0.2.1/rapidy/web_runner.py
+-rw-r--r--   0        0        0     5801 2024-05-07 20:12:13.910385 rapidy-0.2.1/rapidy/web_urldispatcher.py
+-rw-r--r--   0        0        0    20927 1970-01-01 00:00:00.000000 rapidy-0.2.1/PKG-INFO
```

### Comparing `rapidy-0.2.0/LICENSE` & `rapidy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/README.md` & `rapidy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/pyproject.toml` & `rapidy-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rAPIdy"
-version = "0.2.0"
+version = "0.2.1"
 description = "rAPIdy - write quickly - write beautifully"
 authors = [
     "Daniil Grois <daniil.grois@gmail.com>",
     "Lev Zaplatin <lev@zaplatin.dev>",
 ]
 keywords = [
     "rAPIdy",
```

### Comparing `rapidy-0.2.0/rapidy/__init__.py` & `rapidy-0.2.1/rapidy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 from typing import Tuple, TYPE_CHECKING
 
 from aiohttp.client import (
     BaseConnector as BaseConnector,
     ClientConnectionError as ClientConnectionError,
     ClientConnectorCertificateError as ClientConnectorCertificateError,
```

### Comparing `rapidy-0.2.0/rapidy/_annotation_container.py` & `rapidy-0.2.1/rapidy/_annotation_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,38 +11,41 @@
 from rapidy._client_errors import _create_handler_attr_info_msg, _create_handler_info_msg, ExtractError
 from rapidy._fields import ModelField
 from rapidy._validators import validate_request_param_data
 from rapidy.request_params import create_param_model_field_by_request_param, ParamFieldInfo, ParamType, ValidateType
 from rapidy.typedefs import Handler, MethodHandler, Middleware, NoArgAnyCallable, ValidateReturn
 
 
+# FIXME: I don't like this solution as it is being used now.
+#  We need to mark handlers somehow so that we don't have
+#  to check them every time for issubclass(handler, AbstractView) or isinstance(handler, FunctionType).
 class HandlerEnumType(str, Enum):
     func = 'func'
     method = 'method'
     middleware = 'middleware'
 
     @property
     def is_func(self) -> bool:
         return self == self.func
 
-    @property
-    def is_method(self) -> bool:
-        return self == self.method
-
 
 class AnnotationContainerAddFieldError(TypeError):
     pass
 
 
 class RequestFieldAlreadyExistError(Exception):
-    _base_err_msg = 'Error during attribute definition in the handler - request param defined twice.'
+    _base_err_msg = (
+        'Error during attribute definition in the handler - request param defined twice.'
+        'The error may be because the first attribute of the handler is not annotated.'
+        'By default, `rAPIdy` will pass `web.Request` to the first attribute if it has no type annotation.'
+    )
 
     def __init__(self, *args: Any, handler: Any):
         super().__init__(
-            f'{self._base_err_msg} {_create_handler_info_msg(handler)}',
+            f'\n\n{self._base_err_msg} {_create_handler_info_msg(handler)}',
             *args,
         )
 
 
 class AttributeAlreadyExistError(KeyError):
     pass
 
@@ -274,18 +277,14 @@
     @property
     def request_param_name(self) -> str:
         if not self._request_exists or not self._request_param_name:
             raise
 
         return self._request_param_name
 
-    @property
-    def is_method_container(self) -> bool:
-        return self._handler_type.is_method
-
     def add_param(
             self,
             name: str,
             annotation: Type[Any],
             field_info: ParamFieldInfo,
             default: Any,
             default_factory: Optional[NoArgAnyCallable],
@@ -338,23 +337,28 @@
 def create_annotation_container(
         handler: Union[FunctionType, Middleware],
         handler_type: HandlerEnumType,
 ) -> AnnotationContainer:
     container = AnnotationContainer(handler=handler, handler_type=handler_type)
 
     endpoint_signature = inspect.signature(handler)
-    signature_params = endpoint_signature.parameters
+    signature_params = endpoint_signature.parameters.items()
+
+    num_of_extracted_signatures = 0
+
+    for param_name, param in signature_params:
+        num_of_extracted_signatures += 1
 
-    for param_name, param in signature_params.items():
         try:
             annotation, param_field_info, default = extract_handler_attr_annotations(param=param, handler=handler)
         except NotParameterError:
             if handler_type.is_func:
                 if not get_args(param.annotation):
-                    if issubclass(Request, param.annotation):
+                    # FIXME: Fix the processing logic for the 1-st attribute to return a specific error
+                    if issubclass(Request, param.annotation) or num_of_extracted_signatures == 1:
                         container.set_request_field(param_name)
 
             continue
 
         if isinstance(param_field_info, ParamFieldInfo):
             try:
                 container.add_param(
@@ -362,11 +366,12 @@
                     field_info=param_field_info,
                     name=param_name,
                     default=default,
                     default_factory=param_field_info.default_factory,
                 )
             except AnnotationContainerAddFieldError as annotation_container_add_field_error:
                 raise RequestParamError(handler=handler) from annotation_container_add_field_error
+
         else:  # pragma: no cover
             raise
 
     return container
```

### Comparing `rapidy-0.2.0/rapidy/_annotation_extractor.py` & `rapidy-0.2.1/rapidy/_annotation_extractor.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/_client_errors.py` & `rapidy-0.2.1/rapidy/_client_errors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/_extractors.py` & `rapidy-0.2.1/rapidy/_extractors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/_fields.py` & `rapidy-0.2.1/rapidy/_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, TYPE_CHECKING, Union
+from typing import Any, Dict, Optional, Tuple, Type, TYPE_CHECKING, Union
 
 from pydantic import ValidationError
 from pydantic.fields import FieldInfo as FieldInfo
 from typing_extensions import Annotated
 
-from rapidy._client_errors import RequestErrorModel
+from rapidy._client_errors import _regenerate_error_with_loc
 from rapidy._request_params_base import ParamType, ValidateType
 from rapidy.constants import PYDANTIC_V1, PYDANTIC_V2
 from rapidy.typedefs import NoArgAnyCallable, Required, Undefined, ValidateReturn
 
 
 class ParamFieldInfo(FieldInfo, ABC):
     param_type: ParamType
@@ -37,15 +37,14 @@
         if not extractor:
             raise
 
 
 if PYDANTIC_V1:  # noqa: C901
     from pydantic import BaseConfig  # noqa: WPS433
     from pydantic.class_validators import Validator as Validator  # noqa: WPS433
-    from pydantic.error_wrappers import ErrorWrapper  # noqa: WPS433
     from pydantic.fields import ModelField as PydanticModelField  # noqa: WPS433
     from pydantic.schema import get_annotation_from_field_info  # noqa: WPS433
 
     if TYPE_CHECKING:  # pragma: no cover
         from pydantic.fields import BoolUndefined
 
     class ModelField(PydanticModelField):
@@ -102,63 +101,22 @@
             return ModelField(**kwargs)
         except Exception:
             raise Exception(
                 'Invalid args for annotated request field! '
                 f'Hint: check that {type_} is a valid Pydantic field type. ',
             ) from None
 
-    def _regenerate_error_with_loc(
-            *,
-            errors: Sequence[Any],
-            loc_prefix: Tuple[Union[str, int], ...],
-    ) -> List[Dict[str, Any]]:
-        return [
-            {
-                **err,
-                'loc': loc_prefix + err.get('loc', ()),
-            }
-            for err in _normalize_errors(errors)
-        ]
-
-    def _normalize_errors(errors: Sequence[Any]) -> List[Dict[str, Any]]:
-        use_errors: List[Any] = []
-        for error in errors:
-            if isinstance(error, ErrorWrapper):
-                new_errors = ValidationError(
-                    errors=[error],
-                    model=RequestErrorModel,
-                ).errors()
-                use_errors.extend(new_errors)
-            elif isinstance(error, list):
-                use_errors.extend(_normalize_errors(error))
-            else:
-                use_errors.append(error)
-        return use_errors
-
 elif PYDANTIC_V2:
     from dataclasses import dataclass  # noqa: WPS433
 
     from pydantic import TypeAdapter  # noqa: WPS433
 
     def get_annotation_from_field_info(annotation: Any, field_info: FieldInfo, field_name: str) -> Any:  # noqa: WPS440
         return annotation
 
-    def _regenerate_error_with_loc(  # noqa: WPS440
-            *,
-            errors: Sequence[Any],
-            loc_prefix: Tuple[Union[str, int], ...],
-    ) -> List[Dict[str, Any]]:
-        return [
-            {
-                **err,
-                'loc': loc_prefix + err.get('loc', ()),
-            }
-            for err in errors
-        ]
-
     @dataclass
     class ModelField:  # type: ignore[no-redef]  # noqa: WPS440
         name: str
         field_info: FieldInfo
         rapid_param_type: ParamType
 
         @property
```

### Comparing `rapidy-0.2.0/rapidy/_parsers.py` & `rapidy-0.2.1/rapidy/_parsers.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/_validators.py` & `rapidy-0.2.1/rapidy/_validators.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/_version.py` & `rapidy-0.2.1/rapidy/_version.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/hdrs.py` & `rapidy-0.2.1/rapidy/hdrs.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/mypy/_api_errors.py` & `rapidy-0.2.1/rapidy/mypy/_api_errors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/mypy/_type_helpers.py` & `rapidy-0.2.1/rapidy/mypy/_type_helpers.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/mypy/plugin.py` & `rapidy-0.2.1/rapidy/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/request_params.py` & `rapidy-0.2.1/rapidy/request_params.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/typedefs.py` & `rapidy-0.2.1/rapidy/typedefs.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/web.py` & `rapidy-0.2.1/rapidy/web.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/web_app.py` & `rapidy-0.2.1/rapidy/web_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import asyncio
 import logging
 import warnings
 from functools import partial, update_wrapper
-from typing import Any, cast, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple
+from types import FunctionType
+from typing import Any, Dict, Iterable, Iterator, Mapping, Optional, Tuple
 
-from aiohttp.abc import AbstractMatchInfo
+from aiohttp.abc import AbstractMatchInfo, AbstractView
 from aiohttp.log import web_logger
 from aiohttp.web_app import Application as AiohttpApplication, CleanupError
 from aiohttp.web_middlewares import _fix_request_current_app
 from aiohttp.web_urldispatcher import MatchInfoError
 
 from rapidy import hdrs
 from rapidy._annotation_container import AnnotationContainer, create_annotation_container, HandlerEnumType
-from rapidy._client_errors import _normalize_errors
+from rapidy._web_request_validation import _validate_request
 from rapidy.constants import CLIENT_MAX_SIZE
 from rapidy.typedefs import Handler, Middleware
-from rapidy.web_exceptions import HTTPValidationFailure
 from rapidy.web_request import Request
 from rapidy.web_response import StreamResponse
-from rapidy.web_urldispatcher import UrlDispatcher
+from rapidy.web_urldispatcher import StaticResource, UrlDispatcher
 
 __all__ = (
     'Application',
     'CleanupError',
 )
 
 
@@ -90,15 +90,15 @@
                     DeprecationWarning,
                     stacklevel=2,
                 )
                 yield middleware, False
 
         yield _fix_request_current_app(self), True
 
-    async def _handle(self, request: Request) -> StreamResponse:  # noqa: C901  # FIXME: refactor
+    async def _handle(self, request: Request) -> StreamResponse:  # noqa: C901 WPS212  # FIXME: refactor
         loop = asyncio.get_event_loop()
         debug = loop.get_debug()
         match_info = await self._router.resolve(request)
         if debug:  # pragma: no cover
             if not isinstance(match_info, AbstractMatchInfo):
                 raise TypeError(
                     'match_info should be AbstractMatchInfo '
@@ -117,19 +117,22 @@
 
         if resp is None:
             handler = match_info.handler
 
             if isinstance(match_info, MatchInfoError):
                 return await handler(request)
 
-            annotation_container = match_info.route.get_method_container(request.method)
-
             if self._run_middlewares:
-                async def w_handler(request: Request) -> StreamResponse:  # noqa: WPS442
-                    return await self._get_handler_response(request, handler, annotation_container)
+                # FIXME: refactor
+                if isinstance(match_info.route.resource, StaticResource):
+                    async def w_handler(request: Request) -> StreamResponse:  # noqa: WPS442
+                        return await handler(request)
+                else:
+                    async def w_handler(request: Request) -> StreamResponse:  # noqa: WPS440 WPS442
+                        return await self._get_handler_response(request, handler)
 
                 for app in match_info.apps[::-1]:
                     for middleware, new_style in app._middlewares_handlers:
                         if new_style:
                             validated_request_data_for_middleware = await self._validate_request_for_middleware(
                                 app=app, request=request, middleware=middleware,
                             )
@@ -139,71 +142,54 @@
                             )
                         else:
                             w_handler = await middleware(app, w_handler)
 
                 resp = await w_handler(request)
 
             else:
-                return await self._get_handler_response(request, handler, annotation_container)
+                # FIXME: refactor
+                if isinstance(match_info.route.resource, StaticResource):
+                    return await handler(request)
+                else:
+                    return await self._get_handler_response(request, handler)
 
         return resp
 
     async def _get_handler_response(
             self,
             request: Request,
             handler: Handler,
-            annotation_container: AnnotationContainer,
     ) -> StreamResponse:
-        validate_request_data_for_handler = await self._validate_request_for_handler(
-            request=request,
-            annotation_container=annotation_container,
-        )
+        if isinstance(handler, FunctionType):
+            annotation_container = request._match_info.route.get_method_container(request.method)
 
-        if annotation_container.is_method_container:
-            return await handler(request, **validate_request_data_for_handler)
+            validate_request_data_for_handler = await _validate_request(
+                request=request,
+                annotation_container=annotation_container,
+                errors_response_field_name=self._client_errors_response_field_name,
+            )
 
-        if annotation_container.request_exists:
-            validate_request_data_for_handler[annotation_container.request_param_name] = request
+            if annotation_container.request_exists:
+                validate_request_data_for_handler[annotation_container.request_param_name] = request
 
-        return await handler(**validate_request_data_for_handler)
+            return await handler(**validate_request_data_for_handler)
 
-    async def _validate_request_for_handler(
-            self,
-            request: Request,
-            annotation_container: AnnotationContainer,
-    ) -> Dict[str, Any]:
-        return await self._validate_request(annotation_container=annotation_container, request=request)
+        if issubclass(handler, AbstractView):  # type: ignore[arg-type]
+            return await handler(request)
+
+        raise ValueError('Unknown handler type')
 
     async def _validate_request_for_middleware(
             self,
             app: 'Application',
             request: Request,
             middleware: Middleware,
     ) -> Dict[str, Any]:
         annotation_container = app._get_middleware_annotation_container(middleware)
         if annotation_container:
-            return await self._validate_request(annotation_container=annotation_container, request=request)
-
-        return {}
-
-    async def _validate_request(
-            self,
-            annotation_container: AnnotationContainer,
-            request: Request,
-    ) -> Dict[str, Any]:
-        values: Dict[str, Any] = {}
-        errors: List[Dict[str, Any]] = []
-
-        for param_container in annotation_container:
-            param_values, param_errors = await param_container.get_request_data(request)
-            if param_errors:
-                errors += param_errors
-            else:
-                values.update(cast(Dict[str, Any], param_values))
-
-        if errors:
-            raise HTTPValidationFailure(
-                validation_failure_field_name=self._client_errors_response_field_name,
-                errors=_normalize_errors(errors),
+            return await _validate_request(
+                request=request,
+                annotation_container=annotation_container,
+                errors_response_field_name=self._client_errors_response_field_name,
             )
 
-        return values
+        return {}
```

### Comparing `rapidy-0.2.0/rapidy/web_exceptions.py` & `rapidy-0.2.1/rapidy/web_exceptions.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/web_response.py` & `rapidy-0.2.1/rapidy/web_response.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/web_routedef.py` & `rapidy-0.2.1/rapidy/web_routedef.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.0/rapidy/web_urldispatcher.py` & `rapidy-0.2.1/rapidy/web_urldispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC
 from types import FunctionType
-from typing import Any, Awaitable, Callable, cast, Optional, Type, Union
+from typing import Awaitable, Callable, cast, Optional, Type, Union
 
 from aiohttp.abc import AbstractView
-from aiohttp.web_request import Request
 from aiohttp.web_response import StreamResponse
 from aiohttp.web_urldispatcher import (
     _requote_path,
     AbstractResource,
     AbstractRoute,
     DynamicResource as AioHTTPDynamicResource,
     PlainResource as AioHTTPPlainResource,
@@ -19,14 +18,15 @@
     UrlDispatcher as AioHTTPUrlDispatcher,
     UrlMappingMatchInfo,
     View as AioHTTPView,
 )
 
 from rapidy import hdrs
 from rapidy._annotation_container import AnnotationContainer, create_annotation_container, HandlerEnumType
+from rapidy._web_request_validation import _validate_request
 from rapidy.typedefs import Handler, HandlerType, MethodHandler
 
 __all__ = [
     'UrlDispatcher',
     'UrlMappingMatchInfo',
     'AbstractResource',
     'Resource',
@@ -148,25 +148,27 @@
         expect_handler: Optional[_ExpectHandler] = None,
     ) -> AbstractRoute:
         resource = self.add_resource(path, name=name)
         return resource.add_route(method, handler, expect_handler=expect_handler)
 
 
 class View(AioHTTPView):
-    def __init__(self, request: Request, **request_validated_data: Any) -> None:
-        super().__init__(request)
-        self._request_validated_data = request_validated_data
-
     async def _iter(self) -> StreamResponse:
         if self.request.method not in hdrs.METH_ALL:  # aiohttp code  # pragma: no cover
             self._raise_allowed_methods()
 
         method: Optional[MethodHandler] = getattr(self, self.request.method.lower(), None)
         if method is None:  # aiohttp code  # pragma: no cover
             self._raise_allowed_methods()
 
         method = cast(MethodHandler, method)
 
-        ret = await method(**self._request_validated_data)
+        validated_data = await _validate_request(
+            request=self.request,
+            annotation_container=self._request.match_info.route.get_method_container(self.request.method),
+            errors_response_field_name=self._request.app._client_errors_response_field_name,
+        )
+
+        ret = await method(**validated_data)
 
         assert isinstance(ret, StreamResponse)
         return ret
```

### Comparing `rapidy-0.2.0/PKG-INFO` & `rapidy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rAPIdy
-Version: 0.2.0
+Version: 0.2.1
 Summary: rAPIdy - write quickly - write beautifully
 License: MIT
 Keywords: rAPIdy,aiohttp,pydantic,api,fast,http server,Daniil Grois,Lev Zaplatin
 Author: Daniil Grois
 Author-email: daniil.grois@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
```

