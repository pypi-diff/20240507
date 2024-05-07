# Comparing `tmp/openmeter-1.0.0b67.tar.gz` & `tmp/openmeter-1.0.0b69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmeter-1.0.0b67.tar", max compression
+gzip compressed data, was "openmeter-1.0.0b69.tar", max compression
```

## Comparing `openmeter-1.0.0b67.tar` & `openmeter-1.0.0b69.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1260 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/README.md
--rw-r--r--   0        0        0      837 2024-05-07 12:40:54.738790 openmeter-1.0.0b67/pyproject.toml
--rw-r--r--   0        0        0      702 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/__init__.py
--rw-r--r--   0        0        0     3982 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_client.py
--rw-r--r--   0        0        0     1807 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_operations/__init__.py
--rw-r--r--   0        0        0    90468 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_operations/_operations.py
--rw-r--r--   0        0        0     4874 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-07 12:40:32.666726 openmeter-1.0.0b67/src/openmeter/_patch.py
--rw-r--r--   0        0        0    78873 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/_serialization.py
--rw-r--r--   0        0        0      851 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/_vendor.py
--rw-r--r--   0        0        0      702 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/__init__.py
--rw-r--r--   0        0        0     4100 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_client.py
--rw-r--r--   0        0        0     1817 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_operations/__init__.py
--rw-r--r--   0        0        0    78762 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_operations/_operations.py
--rw-r--r--   0        0        0      674 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_patch.py
--rw-r--r--   0        0        0      862 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/aio/_vendor.py
--rw-r--r--   0        0        0       26 2024-05-07 12:40:32.670727 openmeter-1.0.0b67/src/openmeter/py.typed
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b67/PKG-INFO
+-rw-r--r--   0        0        0     1260 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/README.md
+-rw-r--r--   0        0        0      837 2024-05-07 20:26:51.065208 openmeter-1.0.0b69/pyproject.toml
+-rw-r--r--   0        0        0      702 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/__init__.py
+-rw-r--r--   0        0        0     3982 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_client.py
+-rw-r--r--   0        0        0     1807 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_operations/__init__.py
+-rw-r--r--   0        0        0   178032 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_operations/_operations.py
+-rw-r--r--   0        0        0     4874 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_patch.py
+-rw-r--r--   0        0        0    78873 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_serialization.py
+-rw-r--r--   0        0        0      851 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/_vendor.py
+-rw-r--r--   0        0        0      702 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/__init__.py
+-rw-r--r--   0        0        0     4100 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_client.py
+-rw-r--r--   0        0        0     1817 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_operations/__init__.py
+-rw-r--r--   0        0        0   156302 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_operations/_operations.py
+-rw-r--r--   0        0        0      674 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_patch.py
+-rw-r--r--   0        0        0      862 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/aio/_vendor.py
+-rw-r--r--   0        0        0       26 2024-05-07 20:16:13.000000 openmeter-1.0.0b69/src/openmeter/py.typed
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b69/PKG-INFO
```

### Comparing `openmeter-1.0.0b67/README.md` & `openmeter-1.0.0b69/README.md`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/pyproject.toml` & `openmeter-1.0.0b69/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmeter"
-version = "v1.0.0-beta.67"
+version = "v1.0.0-beta.69"
 description = "Client for OpenMeter: Real-Time and Scalable Usage Metering"
 authors = ["Andras Toth <4157749+tothandras@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/openmeter/openmeter"
 homepage = "https://openmeter.io"
 keywords = [
```

### Comparing `openmeter-1.0.0b67/src/openmeter/__init__.py` & `openmeter-1.0.0b69/src/openmeter/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_client.py` & `openmeter-1.0.0b69/src/openmeter/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_configuration.py` & `openmeter-1.0.0b69/src/openmeter/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_operations/__init__.py` & `openmeter-1.0.0b69/src/openmeter/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_operations/_operations.py` & `openmeter-1.0.0b69/src/openmeter/aio/_operations/_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,383 +14,64 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.rest import HttpRequest, HttpResponse
-from azure.core.tracing.decorator import distributed_trace
+from azure.core.rest import AsyncHttpResponse, HttpRequest
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
-from .._serialization import Serializer
+from ..._operations._operations import (
+    build_create_credit_grant_request,
+    build_create_feature_request,
+    build_create_ledger_request,
+    build_create_meter_request,
+    build_create_portal_token_request,
+    build_delete_feature_request,
+    build_delete_meter_request,
+    build_delete_subject_request,
+    build_get_credit_balance_request,
+    build_get_credit_grant_request,
+    build_get_credit_history_request,
+    build_get_feature_request,
+    build_get_meter_request,
+    build_get_subject_request,
+    build_ingest_events_request,
+    build_invalidate_portal_tokens_request,
+    build_list_credit_grants_by_ledger_request,
+    build_list_credit_grants_request,
+    build_list_events_request,
+    build_list_features_request,
+    build_list_ledgers_request,
+    build_list_meter_subjects_request,
+    build_list_meters_request,
+    build_list_portal_tokens_request,
+    build_list_subjects_request,
+    build_query_meter_request,
+    build_query_portal_meter_request,
+    build_reset_credit_request,
+    build_upsert_subject_request,
+    build_void_credit_grant_request,
+)
 from .._vendor import ClientMixinABC
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_list_events_request(
-    *,
-    from_parameter: Optional[datetime.datetime] = None,
-    to: Optional[datetime.datetime] = None,
-    limit: int = 100,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/events"
-
-    # Construct parameters
-    if from_parameter is not None:
-        _params["from"] = _SERIALIZER.query("from_parameter", from_parameter, "iso-8601")
-    if to is not None:
-        _params["to"] = _SERIALIZER.query("to", to, "iso-8601")
-    if limit is not None:
-        _params["limit"] = _SERIALIZER.query("limit", limit, "int", maximum=100, minimum=1)
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_ingest_events_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/events"
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
-def build_list_meters_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters"
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_create_meter_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters"
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
-def build_get_meter_request(meter_id_or_slug: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters/{meterIdOrSlug}"
-    path_format_arguments = {
-        "meterIdOrSlug": _SERIALIZER.url("meter_id_or_slug", meter_id_or_slug, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_delete_meter_request(meter_id_or_slug: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters/{meterIdOrSlug}"
-    path_format_arguments = {
-        "meterIdOrSlug": _SERIALIZER.url("meter_id_or_slug", meter_id_or_slug, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
-
-
-def build_query_meter_request(
-    meter_id_or_slug: str,
-    *,
-    from_parameter: Optional[datetime.datetime] = None,
-    to: Optional[datetime.datetime] = None,
-    window_size: Optional[str] = None,
-    window_time_zone: str = "UTC",
-    subject: Optional[List[str]] = None,
-    filter_group_by: Optional[Dict[str, str]] = None,
-    group_by: Optional[List[str]] = None,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, text/csv, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters/{meterIdOrSlug}/query"
-    path_format_arguments = {
-        "meterIdOrSlug": _SERIALIZER.url("meter_id_or_slug", meter_id_or_slug, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    if from_parameter is not None:
-        _params["from"] = _SERIALIZER.query("from_parameter", from_parameter, "iso-8601")
-    if to is not None:
-        _params["to"] = _SERIALIZER.query("to", to, "iso-8601")
-    if window_size is not None:
-        _params["windowSize"] = _SERIALIZER.query("window_size", window_size, "str")
-    if window_time_zone is not None:
-        _params["windowTimeZone"] = _SERIALIZER.query("window_time_zone", window_time_zone, "str")
-    if subject is not None:
-        _params["subject"] = _SERIALIZER.query("subject", subject, "[str]")
-    if filter_group_by is not None:
-        _params["filterGroupBy"] = _SERIALIZER.query("filter_group_by", filter_group_by, "{str}")
-    if group_by is not None:
-        _params["groupBy"] = _SERIALIZER.query("group_by", group_by, "[str]")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_list_meter_subjects_request(meter_id_or_slug: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/meters/{meterIdOrSlug}/subjects"
-    path_format_arguments = {
-        "meterIdOrSlug": _SERIALIZER.url("meter_id_or_slug", meter_id_or_slug, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_create_portal_token_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/portal/tokens"
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
-def build_list_portal_tokens_request(*, limit: int = 25, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/portal/tokens"
-
-    # Construct parameters
-    if limit is not None:
-        _params["limit"] = _SERIALIZER.query("limit", limit, "int", maximum=100, minimum=1)
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_invalidate_portal_tokens_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/portal/tokens/invalidate"
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
-def build_list_subjects_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/subjects"
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_upsert_subject_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/subjects"
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
-def build_get_subject_request(subject_id_or_key: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/subjects/{subjectIdOrKey}"
-    path_format_arguments = {
-        "subjectIdOrKey": _SERIALIZER.url("subject_id_or_key", subject_id_or_key, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_delete_subject_request(subject_id_or_key: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/subjects/{subjectIdOrKey}"
-    path_format_arguments = {
-        "subjectIdOrKey": _SERIALIZER.url("subject_id_or_key", subject_id_or_key, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
-
-
-def build_query_portal_meter_request(
-    meter_slug: str,
-    *,
-    from_parameter: Optional[datetime.datetime] = None,
-    to: Optional[datetime.datetime] = None,
-    window_size: Optional[str] = None,
-    window_time_zone: str = "UTC",
-    filter_group_by: Optional[Dict[str, str]] = None,
-    group_by: Optional[List[str]] = None,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json, text/csv, application/problem+json")
-
-    # Construct URL
-    _url = "/api/v1/portal/meters/{meterSlug}/query"
-    path_format_arguments = {
-        "meterSlug": _SERIALIZER.url("meter_slug", meter_slug, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    if from_parameter is not None:
-        _params["from"] = _SERIALIZER.query("from_parameter", from_parameter, "iso-8601")
-    if to is not None:
-        _params["to"] = _SERIALIZER.query("to", to, "iso-8601")
-    if window_size is not None:
-        _params["windowSize"] = _SERIALIZER.query("window_size", window_size, "str")
-    if window_time_zone is not None:
-        _params["windowTimeZone"] = _SERIALIZER.query("window_time_zone", window_time_zone, "str")
-    if filter_group_by is not None:
-        _params["filterGroupBy"] = _SERIALIZER.query("filter_group_by", filter_group_by, "{str}")
-    if group_by is not None:
-        _params["groupBy"] = _SERIALIZER.query("group_by", group_by, "[str]")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-class ClientOperationsMixin(ClientMixinABC):
-    @distributed_trace
-    def list_events(
+class ClientOperationsMixin(ClientMixinABC):  # pylint: disable=too-many-public-methods
+    @distributed_trace_async
+    async def list_events(
         self,
         *,
         from_parameter: Optional[datetime.datetime] = None,
         to: Optional[datetime.datetime] = None,
         limit: int = 100,
         **kwargs: Any
     ) -> List[JSON]:
@@ -461,38 +142,38 @@
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def ingest_events(  # pylint: disable=inconsistent-return-statements
+    async def ingest_events(  # pylint: disable=inconsistent-return-statements
         self, body: JSON, *, content_type: str = "application/cloudevents+json", **kwargs: Any
     ) -> None:
         # pylint: disable=line-too-long
         """Ingest events.
 
         Ingests an event or batch of events following the CloudEvents specification.
 
@@ -530,15 +211,15 @@
                     "dataschema": "str",  # Optional. Identifies the schema that data adheres to.
                     "time": "2020-02-20 00:00:00"  # Optional. Timestamp of when the occurrence
                       happened. Must adhere to RFC 3339.
                 }
         """
 
     @overload
-    def ingest_events(  # pylint: disable=inconsistent-return-statements
+    async def ingest_events(  # pylint: disable=inconsistent-return-statements
         self, body: List[JSON], *, content_type: str = "application/cloudevents-batch+json", **kwargs: Any
     ) -> None:
         # pylint: disable=line-too-long
         """Ingest events.
 
         Ingests an event or batch of events following the CloudEvents specification.
 
@@ -578,16 +259,16 @@
                           adheres to.
                         "time": "2020-02-20 00:00:00"  # Optional. Timestamp of when the
                           occurrence happened. Must adhere to RFC 3339.
                     }
                 ]
         """
 
-    @distributed_trace
-    def ingest_events(  # pylint: disable=inconsistent-return-statements
+    @distributed_trace_async
+    async def ingest_events(  # pylint: disable=inconsistent-return-statements
         self, body: Union[JSON, List[JSON]], **kwargs: Any
     ) -> None:
         # pylint: disable=line-too-long
         """Ingest events.
 
         Ingests an event or batch of events following the CloudEvents specification.
 
@@ -652,31 +333,31 @@
             json=_json,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
-    @distributed_trace
-    def list_meters(self, **kwargs: Any) -> List[JSON]:
+    @distributed_trace_async
+    async def list_meters(self, **kwargs: Any) -> List[JSON]:
         # pylint: disable=line-too-long
         """List meters.
 
         List meters.
 
         :return: list of JSON object
         :rtype: list[JSON]
@@ -727,38 +408,38 @@
         _request = build_list_meters_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def create_meter(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+    async def create_meter(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """☁ Create meter.
 
         *Available in OpenMeter Cloud.*
         *In the open-source version, meters are created in the configuration file.*
 
         Create a meter.
@@ -819,15 +500,15 @@
                       and MAX aggregations is a number or a string that can be parsed to a number. For
                       UNIQUE_COUNT aggregation, the ingested value must be a string. For COUNT
                       aggregation the valueProperty is ignored.
                 }
         """
 
     @overload
-    def create_meter(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+    async def create_meter(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """☁ Create meter.
 
         *Available in OpenMeter Cloud.*
         *In the open-source version, meters are created in the configuration file.*
 
         Create a meter.
@@ -864,16 +545,16 @@
                       from the ingested event's data property. The ingested value for SUM, AVG, MIN,
                       and MAX aggregations is a number or a string that can be parsed to a number. For
                       UNIQUE_COUNT aggregation, the ingested value must be a string. For COUNT
                       aggregation the valueProperty is ignored.
                 }
         """
 
-    @distributed_trace
-    def create_meter(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+    @distributed_trace_async
+    async def create_meter(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """☁ Create meter.
 
         *Available in OpenMeter Cloud.*
         *In the open-source version, meters are created in the configuration file.*
 
         Create a meter.
@@ -963,38 +644,38 @@
             content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
-    @distributed_trace
-    def get_meter(self, meter_id_or_slug: str, **kwargs: Any) -> JSON:
+    @distributed_trace_async
+    async def get_meter(self, meter_id_or_slug: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get meter.
 
         Get meter by ID or slug.
 
         :param meter_id_or_slug: A unique identifier for the meter. Required.
         :type meter_id_or_slug: str
@@ -1045,38 +726,38 @@
             meter_id_or_slug=meter_id_or_slug,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
-    @distributed_trace
-    def delete_meter(  # pylint: disable=inconsistent-return-statements
+    @distributed_trace_async
+    async def delete_meter(  # pylint: disable=inconsistent-return-statements
         self, meter_id_or_slug: str, **kwargs: Any
     ) -> None:
         """☁ Delete meter.
 
         *Available in OpenMeter Cloud.*
 
         Delete a meter by ID or slug.
@@ -1105,31 +786,31 @@
             meter_id_or_slug=meter_id_or_slug,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
-    @distributed_trace
-    def query_meter(
+    @distributed_trace_async
+    async def query_meter(
         self,
         meter_id_or_slug: str,
         *,
         from_parameter: Optional[datetime.datetime] = None,
         to: Optional[datetime.datetime] = None,
         window_size: Optional[str] = None,
         window_time_zone: str = "UTC",
@@ -1154,15 +835,16 @@
          entirety of the specified period for each subject and group. Known values are: "MINUTE",
          "HOUR", and "DAY". Default value is None.
         :paramtype window_size: str
         :keyword window_time_zone: The value is the name of the time zone as defined in the IANA Time
          Zone Database (http://www.iana.org/time-zones).
          If not specified, the UTC timezone will be used. Default value is "UTC".
         :paramtype window_time_zone: str
-        :keyword subject: Filtering and group by multiple subjects.
+        :keyword subject: Filtering by multiple subjects.
+
          Usage: ?subject=customer-1&subject=customer-2. Default value is None.
         :paramtype subject: list[str]
         :keyword filter_group_by: Default value is None.
         :paramtype filter_group_by: dict[str, str]
         :keyword group_by: If not specified a single aggregate will be returned for each subject and
          time window.
          ``subject`` is a reserved group by value. Default value is None.
@@ -1219,23 +901,23 @@
             group_by=group_by,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.status_code == 200:
             if response.content:
                 deserialized = response.json()
             else:
@@ -1248,16 +930,16 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[JSON, str], deserialized), {})  # type: ignore
 
         return cast(Union[JSON, str], deserialized)  # type: ignore
 
-    @distributed_trace
-    def list_meter_subjects(self, meter_id_or_slug: str, **kwargs: Any) -> List[str]:
+    @distributed_trace_async
+    async def list_meter_subjects(self, meter_id_or_slug: str, **kwargs: Any) -> List[str]:
         """List meter subjects.
 
         List subjects for a meter.
 
         :param meter_id_or_slug: A unique identifier for the meter. Required.
         :type meter_id_or_slug: str
         :return: list of str
@@ -1290,38 +972,38 @@
             meter_id_or_slug=meter_id_or_slug,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[str], deserialized), {})  # type: ignore
 
         return cast(List[str], deserialized)  # type: ignore
 
     @overload
-    def create_portal_token(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+    async def create_portal_token(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
         """Create portal token.
 
         Create a consumer portal token.
 
         :param body: The portal token to create. Required.
         :type body: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
@@ -1360,15 +1042,17 @@
                     "expiresAt": "2020-02-20 00:00:00",  # Optional.
                     "id": "str",  # Optional.
                     "token": "str"  # Optional. The token is only returned at creation.
                 }
         """
 
     @overload
-    def create_portal_token(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+    async def create_portal_token(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
         """Create portal token.
 
         Create a consumer portal token.
 
         :param body: The portal token to create. Required.
         :type body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
@@ -1392,16 +1076,16 @@
                     "expired": bool,  # Optional.
                     "expiresAt": "2020-02-20 00:00:00",  # Optional.
                     "id": "str",  # Optional.
                     "token": "str"  # Optional. The token is only returned at creation.
                 }
         """
 
-    @distributed_trace
-    def create_portal_token(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+    @distributed_trace_async
+    async def create_portal_token(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
         """Create portal token.
 
         Create a consumer portal token.
 
         :param body: The portal token to create. Is either a JSON type or a IO[bytes] type. Required.
         :type body: JSON or IO[bytes]
         :return: JSON object
@@ -1468,38 +1152,38 @@
             content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
-    @distributed_trace
-    def list_portal_tokens(self, *, limit: int = 25, **kwargs: Any) -> List[JSON]:
+    @distributed_trace_async
+    async def list_portal_tokens(self, *, limit: int = 25, **kwargs: Any) -> List[JSON]:
         """☁ List portal tokens.
 
         *Available in OpenMeter Cloud.*
 
         List consumer portal tokens.
 
         :keyword limit: Number of portal tokens to return. Default is 25. Default value is 25.
@@ -1546,38 +1230,38 @@
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
+    async def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
         self, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> None:
         """☁ Invalidate portal tokens.
 
         *Available in OpenMeter Cloud.*
 
         Invalidates consumer portal tokens by ID or subject.
@@ -1598,15 +1282,15 @@
                 body = {
                     "id": "str",  # Optional. Invalidate a portal token by ID.
                     "subject": "str"  # Optional. Invalidate all portal tokens for a subject.
                 }
         """
 
     @overload
-    def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
+    async def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
         self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> None:
         """☁ Invalidate portal tokens.
 
         *Available in OpenMeter Cloud.*
 
         Invalidates consumer portal tokens by ID or subject.
@@ -1617,16 +1301,16 @@
          Default value is "application/json".
         :paramtype content_type: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace
-    def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
+    @distributed_trace_async
+    async def invalidate_portal_tokens(  # pylint: disable=inconsistent-return-statements
         self, body: Union[JSON, IO[bytes]], **kwargs: Any
     ) -> None:
         """☁ Invalidate portal tokens.
 
         *Available in OpenMeter Cloud.*
 
         Invalidates consumer portal tokens by ID or subject.
@@ -1677,31 +1361,31 @@
             content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
-    @distributed_trace
-    def list_subjects(self, **kwargs: Any) -> List[JSON]:
+    @distributed_trace_async
+    async def list_subjects(self, **kwargs: Any) -> List[JSON]:
         """☁ List subjects.
 
         *Available in OpenMeter Cloud.*
 
         List subjects.
 
         :return: list of JSON object
@@ -1742,38 +1426,40 @@
         _request = build_list_subjects_request(
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def upsert_subject(self, body: List[JSON], *, content_type: str = "application/json", **kwargs: Any) -> List[JSON]:
+    async def upsert_subject(
+        self, body: List[JSON], *, content_type: str = "application/json", **kwargs: Any
+    ) -> List[JSON]:
         """☁ Upsert subject.
 
         *Available in OpenMeter Cloud.*
 
         Upserts a subject. Creates or updates subject.
         If the subject doesn't exist, it will be created.
         If the subject exists, it will be partially updated with the provided fields.
@@ -1818,15 +1504,17 @@
                         },
                         "stripeCustomerId": "str"  # Optional.
                     }
                 ]
         """
 
     @overload
-    def upsert_subject(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> List[JSON]:
+    async def upsert_subject(
+        self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> List[JSON]:
         """☁ Upsert subject.
 
         *Available in OpenMeter Cloud.*
 
         Upserts a subject. Creates or updates subject.
         If the subject doesn't exist, it will be created.
         If the subject exists, it will be partially updated with the provided fields.
@@ -1855,16 +1543,16 @@
                             "str": {}  # Optional. Dictionary of :code:`<any>`.
                         },
                         "stripeCustomerId": "str"  # Optional.
                     }
                 ]
         """
 
-    @distributed_trace
-    def upsert_subject(self, body: Union[List[JSON], IO[bytes]], **kwargs: Any) -> List[JSON]:
+    @distributed_trace_async
+    async def upsert_subject(self, body: Union[List[JSON], IO[bytes]], **kwargs: Any) -> List[JSON]:
         """☁ Upsert subject.
 
         *Available in OpenMeter Cloud.*
 
         Upserts a subject. Creates or updates subject.
         If the subject doesn't exist, it will be created.
         If the subject exists, it will be partially updated with the provided fields.
@@ -1923,38 +1611,38 @@
             content=_content,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
-    @distributed_trace
-    def get_subject(self, subject_id_or_key: str, **kwargs: Any) -> JSON:
+    @distributed_trace_async
+    async def get_subject(self, subject_id_or_key: str, **kwargs: Any) -> JSON:
         """☁ Get subject.
 
         *Available in OpenMeter Cloud.*
 
         Get subject by ID or key.
 
         :param subject_id_or_key: A unique identifier for a subject. Required.
@@ -1996,38 +1684,38 @@
             subject_id_or_key=subject_id_or_key,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.content:
             deserialized = response.json()
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
-    @distributed_trace
-    def delete_subject(  # pylint: disable=inconsistent-return-statements
+    @distributed_trace_async
+    async def delete_subject(  # pylint: disable=inconsistent-return-statements
         self, subject_id_or_key: str, **kwargs: Any
     ) -> None:
         """☁ Delete subject.
 
         *Available in OpenMeter Cloud.*
 
         Delete a subject by ID or key.
@@ -2057,31 +1745,31 @@
             subject_id_or_key=subject_id_or_key,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
-    @distributed_trace
-    def query_portal_meter(
+    @distributed_trace_async
+    async def query_portal_meter(
         self,
         meter_slug: str,
         *,
         from_parameter: Optional[datetime.datetime] = None,
         to: Optional[datetime.datetime] = None,
         window_size: Optional[str] = None,
         window_time_zone: str = "UTC",
@@ -2166,23 +1854,23 @@
             group_by=group_by,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 200]:
             if _stream:
-                response.read()  # Load the body in memory and close the socket
+                await response.read()  # Load the body in memory and close the socket
             map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if response.status_code == 200:
             if response.content:
                 deserialized = response.json()
             else:
@@ -2194,7 +1882,1696 @@
             else:
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[JSON, str], deserialized), {})  # type: ignore
 
         return cast(Union[JSON, str], deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def list_features(self, **kwargs: Any) -> List[JSON]:
+        # pylint: disable=line-too-long
+        """List features.
+
+        List features.
+
+        :return: list of JSON object
+        :rtype: list[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "meterSlug": "str",  # The meter that the feature is associated with
+                          and decreases grants by usage. Required.
+                        "name": "str",  # The name of the feature. Required.
+                        "archived": bool,  # Optional. If the feature is archived, it will
+                          not be used for grants or usage.
+                        "id": "str",  # Optional. Readonly unique ULID identifier of the
+                          feature.
+                        "meterGroupByFilters": {
+                            "str": "str"  # Optional. Optional meter group by filters.
+                              Useful if the meter scope is broader than what feature tracks.
+                        }
+                    }
+                ]
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
+
+        _request = build_list_features_request(
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
+
+        return cast(List[JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create_feature(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create feature.
+
+        Creates a feature.
+
+        :param body: The feature to create. Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+        """
+
+    @overload
+    async def create_feature(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create feature.
+
+        Creates a feature.
+
+        :param body: The feature to create. Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 201
+                response == {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+        """
+
+    @distributed_trace_async
+    async def create_feature(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create feature.
+
+        Creates a feature.
+
+        :param body: The feature to create. Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            501: HttpResponseError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_create_feature_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get_feature(self, feature_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get feature.
+
+        Get feature by key.
+
+        :param feature_id: A unique ULID identifier for a feature. Required.
+        :type feature_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "meterSlug": "str",  # The meter that the feature is associated with and
+                      decreases grants by usage. Required.
+                    "name": "str",  # The name of the feature. Required.
+                    "archived": bool,  # Optional. If the feature is archived, it will not be
+                      used for grants or usage.
+                    "id": "str",  # Optional. Readonly unique ULID identifier of the feature.
+                    "meterGroupByFilters": {
+                        "str": "str"  # Optional. Optional meter group by filters. Useful if
+                          the meter scope is broader than what feature tracks.
+                    }
+                }
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_get_feature_request(
+            feature_id=feature_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def delete_feature(  # pylint: disable=inconsistent-return-statements
+        self, feature_id: str, **kwargs: Any
+    ) -> None:
+        """Delete feature.
+
+        Delete a feature by key.
+
+        :param feature_id: A unique ULID identifier for a feature. Required.
+        :type feature_id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_delete_feature_request(
+            feature_id=feature_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
+
+    @distributed_trace_async
+    async def list_ledgers(
+        self, *, subject: Optional[List[str]] = None, limit: int = 1000, offset: Optional[int] = None, **kwargs: Any
+    ) -> List[JSON]:
+        """List the already defined ledgers.
+
+        List the already defined ledgers.
+
+        :keyword subject: Query a specific ledger. Default value is None.
+        :paramtype subject: list[str]
+        :keyword limit: Number of ledgers to return. Default value is 1000.
+        :paramtype limit: int
+        :keyword offset: Start returning ledgers from this offset. Default value is None.
+        :paramtype offset: int
+        :return: list of JSON object
+        :rtype: list[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "id": "str",  # Readonly unique ULID identifier of the ledger.
+                          Required.
+                        "subject": "str",  # The metering subject this ledger used to track
+                          credits for. Required.
+                        "metadata": {
+                            "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                        }
+                    }
+                ]
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
+
+        _request = build_list_ledgers_request(
+            subject=subject,
+            limit=limit,
+            offset=offset,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
+
+        return cast(List[JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create_ledger(self, body: JSON, *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+        """Creates the specified ledger.
+
+        Create or update the specified ledger.
+
+        :param body: The ledger to be created. Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "subject": "str",  # The metering subject this ledger used to track credits
+                      for. Required.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
+                    "subject": "str",  # The metering subject this ledger used to track credits
+                      for. Required.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    }
+                }
+        """
+
+    @overload
+    async def create_ledger(self, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any) -> JSON:
+        """Creates the specified ledger.
+
+        Create or update the specified ledger.
+
+        :param body: The ledger to be created. Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 201
+                response == {
+                    "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
+                    "subject": "str",  # The metering subject this ledger used to track credits
+                      for. Required.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    }
+                }
+        """
+
+    @distributed_trace_async
+    async def create_ledger(self, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        """Creates the specified ledger.
+
+        Create or update the specified ledger.
+
+        :param body: The ledger to be created. Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "subject": "str",  # The metering subject this ledger used to track credits
+                      for. Required.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
+                    "subject": "str",  # The metering subject this ledger used to track credits
+                      for. Required.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    }
+                }
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_create_ledger_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get_credit_balance(
+        self, ledger_id: str, *, time: Optional[datetime.datetime] = None, **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the balance of a specific subject.
+
+        Get the balance of a specific subject.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :keyword time: Point of time to query balances: date-time in RFC 3339 format. Defaults to now.
+         Default value is None.
+        :paramtype time: ~datetime.datetime
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "grants": [
+                        {
+                            "amount": 0.0,  # The amount to grant. Can be positive or
+                              negative number. Required.
+                            "effectiveAt": "2020-02-20 00:00:00",  # The effective date.
+                              Required.
+                            "expiration": {
+                                "count": 0,  # The expiration period count like 12
+                                  months. Required.
+                                "duration": "str"  # The expiration period duration
+                                  like month. Required. Known values are: "HOUR", "DAY", "WEEK",
+                                  "MONTH", and "YEAR".
+                            },
+                            "featureID": "str",  # The unique feature ULID that the grant
+                              is associated with, if any. Required.
+                            "id": "str",  # Readonly unique ULID identifier of the grant.
+                              Required.
+                            "subject": "str",  # The subject to grant the amount to.
+                              Required.
+                            "type": "str",  # The grant type:   * ``USAGE`` - Increase
+                              balance by the amount in the unit of the associated meter. Required.
+                              "USAGE"
+                            "balance": 0.0,  # Optional. The balance of the grant.
+                            "expiresAt": "2020-02-20 00:00:00",  # Optional. The
+                              expiration date of the grant.
+                            "metadata": {
+                                "str": "str"  # Optional. Dictionary of
+                                  :code:`<string>`.
+                            },
+                            "priority": 1,  # Optional. Default value is 1. The priority
+                              of the grant. Grants with higher priority are applied first. Priority is
+                              a positive decimal numbers. With lower numbers indicating higher
+                              importance. For example, a priority of 1 is more urgent than a priority
+                              of 2. When there are several grants available for the same subject, the
+                              system selects the grant with the highest priority. In cases where credit
+                              grants share the same priority level, the grant closest to its expiration
+                              will be used first. In the case of two credits have identical priorities
+                              and expiration dates, the system will use the grant that was created
+                              first.
+                            "rollover": {
+                                "type": "str",  # The rollover type to use:   *
+                                  ``REMAINING_AMOUNT`` - Rollover remaining amount. *
+                                  ``ORIGINAL_AMOUNT`` - Rollover re-applies the full grant amount.
+                                  Required. Known values are: "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
+                                "maxAmount": 0.0  # Optional. Maximum amount to
+                                  rollover.
+                            }
+                        }
+                    ],
+                    "features": [
+                        {
+                            "meterSlug": "str",  # The meter that the feature is
+                              associated with and decreases grants by usage. Required.
+                            "name": "str",  # The name of the feature. Required.
+                            "archived": bool,  # Optional. If the feature is archived, it
+                              will not be used for grants or usage.
+                            "balance": 0.0,  # Optional. The balance of the feature.
+                            "id": "str",  # Optional. Readonly unique ULID identifier of
+                              the feature.
+                            "meterGroupByFilters": {
+                                "str": "str"  # Optional. Optional meter group by
+                                  filters. Useful if the meter scope is broader than what feature
+                                  tracks.
+                            }
+                        }
+                    ]
+                }
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_get_credit_balance_request(
+            ledger_id=ledger_id,
+            time=time,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get_credit_history(
+        self,
+        ledger_id: str,
+        *,
+        from_parameter: datetime.datetime,
+        limit: int = 1000,
+        to: Optional[datetime.datetime] = None,
+        **kwargs: Any
+    ) -> List[JSON]:
+        """Get credit ledger.
+
+        Get credit ledger for a specific subject.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :keyword from_parameter: Start of time range to query ledger: date-time in RFC 3339 format.
+         Required.
+        :paramtype from_parameter: ~datetime.datetime
+        :keyword limit: Number of entries to return. Default value is 1000.
+        :paramtype limit: int
+        :keyword to: End of time range to query ledger: date-time in RFC 3339 format. Defaults to now.
+         Default value is None.
+        :paramtype to: ~datetime.datetime
+        :return: list of JSON object
+        :rtype: list[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "id": "str",  # Readonly unique ULID identifier of the ledger entry.
+                          Required.
+                        "time": "2020-02-20 00:00:00",  # The time the ledger entry was
+                          created. Required.
+                        "type": "str",  # Required. Known values are: "GRANT", "VOID",
+                          "RESET", and "GRANT_USAGE".
+                        "amount": 0.0,  # Optional. The amount to apply. Can be positive or
+                          negative number. If applicable.
+                        "period": {
+                            "from": "2020-02-20 00:00:00",  # Period start time where the
+                              amount was applied. If applicable. Required.
+                            "to": "2020-02-20 00:00:00"  # Period end time where the
+                              amount was applied. If applicable. Required.
+                        }
+                    }
+                ]
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
+
+        _request = build_get_credit_history_request(
+            ledger_id=ledger_id,
+            from_parameter=from_parameter,
+            limit=limit,
+            to=to,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
+
+        return cast(List[JSON], deserialized)  # type: ignore
+
+    @overload
+    async def reset_credit(
+        self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Reset credit balance.
+
+        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        rollover configuration.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: Details for the reset. Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                      cannot be in the future. Required.
+                    "id": "str"  # Readonly unique ULID identifier of the reset. Required.
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                      cannot be in the future. Required.
+                    "id": "str"  # Readonly unique ULID identifier of the reset. Required.
+                }
+        """
+
+    @overload
+    async def reset_credit(
+        self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Reset credit balance.
+
+        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        rollover configuration.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: Details for the reset. Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 201
+                response == {
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                      cannot be in the future. Required.
+                    "id": "str"  # Readonly unique ULID identifier of the reset. Required.
+                }
+        """
+
+    @distributed_trace_async
+    async def reset_credit(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        """Reset credit balance.
+
+        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        rollover configuration.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: Details for the reset. Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                      cannot be in the future. Required.
+                    "id": "str"  # Readonly unique ULID identifier of the reset. Required.
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                      cannot be in the future. Required.
+                    "id": "str"  # Readonly unique ULID identifier of the reset. Required.
+                }
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_reset_credit_request(
+            ledger_id=ledger_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def list_credit_grants(
+        self, *, ledger_id: Optional[str] = None, limit: int = 1000, **kwargs: Any
+    ) -> List[JSON]:
+        # pylint: disable=line-too-long
+        """List credit grants for multiple ledgers.
+
+        List credit grants for multiple ledgers.
+
+        :keyword ledger_id: Filtering and group by multiple subjects.
+
+         Usage: ``?ledgerID=01HX6VK5C498B3ABY9PR1069PP``. Default value is None.
+        :paramtype ledger_id: str
+        :keyword limit: Number of entries to return. Default value is 1000.
+        :paramtype limit: int
+        :return: list of JSON object
+        :rtype: list[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "amount": 0.0,  # The amount to grant. Can be positive or negative
+                          number. Required.
+                        "effectiveAt": "2020-02-20 00:00:00",  # The effective date.
+                          Required.
+                        "expiration": {
+                            "count": 0,  # The expiration period count like 12 months.
+                              Required.
+                            "duration": "str"  # The expiration period duration like
+                              month. Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and
+                              "YEAR".
+                        },
+                        "featureID": "str",  # The unique feature ULID that the grant is
+                          associated with, if any. Required.
+                        "id": "str",  # Readonly unique ULID identifier of the grant.
+                          Required.
+                        "subject": "str",  # The subject to grant the amount to. Required.
+                        "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by
+                          the amount in the unit of the associated meter. Required. "USAGE"
+                        "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date
+                          of the grant.
+                        "metadata": {
+                            "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                        },
+                        "priority": 1,  # Optional. Default value is 1. The priority of the
+                          grant. Grants with higher priority are applied first. Priority is a positive
+                          decimal numbers. With lower numbers indicating higher importance. For
+                          example, a priority of 1 is more urgent than a priority of 2. When there are
+                          several grants available for the same subject, the system selects the grant
+                          with the highest priority. In cases where credit grants share the same
+                          priority level, the grant closest to its expiration will be used first. In
+                          the case of two credits have identical priorities and expiration dates, the
+                          system will use the grant that was created first.
+                        "rollover": {
+                            "type": "str",  # The rollover type to use:   *
+                              ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
+                              Rollover re-applies the full grant amount. Required. Known values are:
+                              "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
+                            "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                        }
+                    }
+                ]
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
+
+        _request = build_list_credit_grants_request(
+            ledger_id=ledger_id,
+            limit=limit,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
+
+        return cast(List[JSON], deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def list_credit_grants_by_ledger(self, ledger_id: str, *, limit: int = 1000, **kwargs: Any) -> List[JSON]:
+        # pylint: disable=line-too-long
+        """List credit grants.
+
+        List credit grants for a specific ledger.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :keyword limit: Number of entries to return. Default value is 1000.
+        :paramtype limit: int
+        :return: list of JSON object
+        :rtype: list[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "amount": 0.0,  # The amount to grant. Can be positive or negative
+                          number. Required.
+                        "effectiveAt": "2020-02-20 00:00:00",  # The effective date.
+                          Required.
+                        "expiration": {
+                            "count": 0,  # The expiration period count like 12 months.
+                              Required.
+                            "duration": "str"  # The expiration period duration like
+                              month. Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and
+                              "YEAR".
+                        },
+                        "featureID": "str",  # The unique feature ULID that the grant is
+                          associated with, if any. Required.
+                        "id": "str",  # Readonly unique ULID identifier of the grant.
+                          Required.
+                        "subject": "str",  # The subject to grant the amount to. Required.
+                        "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by
+                          the amount in the unit of the associated meter. Required. "USAGE"
+                        "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date
+                          of the grant.
+                        "metadata": {
+                            "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                        },
+                        "priority": 1,  # Optional. Default value is 1. The priority of the
+                          grant. Grants with higher priority are applied first. Priority is a positive
+                          decimal numbers. With lower numbers indicating higher importance. For
+                          example, a priority of 1 is more urgent than a priority of 2. When there are
+                          several grants available for the same subject, the system selects the grant
+                          with the highest priority. In cases where credit grants share the same
+                          priority level, the grant closest to its expiration will be used first. In
+                          the case of two credits have identical priorities and expiration dates, the
+                          system will use the grant that was created first.
+                        "rollover": {
+                            "type": "str",  # The rollover type to use:   *
+                              ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
+                              Rollover re-applies the full grant amount. Required. Known values are:
+                              "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
+                            "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                        }
+                    }
+                ]
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
+
+        _request = build_list_credit_grants_by_ledger_request(
+            ledger_id=ledger_id,
+            limit=limit,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
+
+        return cast(List[JSON], deserialized)  # type: ignore
+
+    @overload
+    async def create_credit_grant(
+        self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create credit grant.
+
+        Creates a credit grant.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: The credit grant to create. Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "subject": "str",  # The subject to grant the amount to. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date of the
+                      grant.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+        """
+
+    @overload
+    async def create_credit_grant(
+        self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Create credit grant.
+
+        Creates a credit grant.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: The credit grant to create. Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 201
+                response == {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "subject": "str",  # The subject to grant the amount to. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date of the
+                      grant.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+        """
+
+    @distributed_trace_async
+    async def create_credit_grant(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Create credit grant.
+
+        Creates a credit grant.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param body: The credit grant to create. Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+
+                # response body for status code(s): 201
+                response == {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "subject": "str",  # The subject to grant the amount to. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date of the
+                      grant.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+        """
+        error_map = {
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            400: HttpResponseError,
+            401: lambda response: ClientAuthenticationError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_create_credit_grant_request(
+            ledger_id=ledger_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [201]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def get_credit_grant(self, ledger_id: str, credit_grant_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get credit grant.
+
+        Get credit by key.
+
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :param credit_grant_id: A unique identifier for a credit grant. Required.
+        :type credit_grant_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "amount": 0.0,  # The amount to grant. Can be positive or negative number.
+                      Required.
+                    "effectiveAt": "2020-02-20 00:00:00",  # The effective date. Required.
+                    "expiration": {
+                        "count": 0,  # The expiration period count like 12 months. Required.
+                        "duration": "str"  # The expiration period duration like month.
+                          Required. Known values are: "HOUR", "DAY", "WEEK", "MONTH", and "YEAR".
+                    },
+                    "featureID": "str",  # The unique feature ULID that the grant is associated
+                      with, if any. Required.
+                    "id": "str",  # Readonly unique ULID identifier of the grant. Required.
+                    "subject": "str",  # The subject to grant the amount to. Required.
+                    "type": "str",  # The grant type:   * ``USAGE`` - Increase balance by the
+                      amount in the unit of the associated meter. Required. "USAGE"
+                    "expiresAt": "2020-02-20 00:00:00",  # Optional. The expiration date of the
+                      grant.
+                    "metadata": {
+                        "str": "str"  # Optional. Dictionary of :code:`<string>`.
+                    },
+                    "priority": 1,  # Optional. Default value is 1. The priority of the grant.
+                      Grants with higher priority are applied first. Priority is a positive decimal
+                      numbers. With lower numbers indicating higher importance. For example, a priority
+                      of 1 is more urgent than a priority of 2. When there are several grants available
+                      for the same subject, the system selects the grant with the highest priority. In
+                      cases where credit grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two credits have identical
+                      priorities and expiration dates, the system will use the grant that was created
+                      first.
+                    "rollover": {
+                        "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
+                          - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
+                          full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
+                          "ORIGINAL_AMOUNT".
+                        "maxAmount": 0.0  # Optional. Maximum amount to rollover.
+                    }
+                }
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_get_credit_grant_request(
+            ledger_id=ledger_id,
+            credit_grant_id=credit_grant_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if response.content:
+            deserialized = response.json()
+        else:
+            deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def void_credit_grant(  # pylint: disable=inconsistent-return-statements
+        self, credit_grant_id: str, ledger_id: str, **kwargs: Any
+    ) -> None:
+        """Void credit grant.
+
+        Void a credit grant by ID. Partially or fully used credits cannot be voided.
+        Voided credits won't be applied to the subject's balance anymore.
+
+        :param credit_grant_id: A unique identifier for a credit grant. Required.
+        :type credit_grant_id: str
+        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :type ledger_id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+            401: lambda response: ClientAuthenticationError(response=response),
+            404: lambda response: ResourceNotFoundError(response=response),
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        _request = build_void_credit_grant_request(
+            credit_grant_id=credit_grant_id,
+            ledger_id=ledger_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `openmeter-1.0.0b67/src/openmeter/_operations/_patch.py` & `openmeter-1.0.0b69/src/openmeter/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_patch.py` & `openmeter-1.0.0b69/src/openmeter/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_serialization.py` & `openmeter-1.0.0b69/src/openmeter/_serialization.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/_vendor.py` & `openmeter-1.0.0b69/src/openmeter/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/__init__.py` & `openmeter-1.0.0b69/src/openmeter/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_client.py` & `openmeter-1.0.0b69/src/openmeter/aio/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_configuration.py` & `openmeter-1.0.0b69/src/openmeter/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_operations/__init__.py` & `openmeter-1.0.0b69/src/openmeter/aio/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_operations/_patch.py` & `openmeter-1.0.0b69/src/openmeter/aio/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_patch.py` & `openmeter-1.0.0b69/src/openmeter/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/src/openmeter/aio/_vendor.py` & `openmeter-1.0.0b69/src/openmeter/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b67/PKG-INFO` & `openmeter-1.0.0b69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmeter
-Version: 1.0.0b67
+Version: 1.0.0b69
 Summary: Client for OpenMeter: Real-Time and Scalable Usage Metering
 Home-page: https://openmeter.io
 License: Apache-2.0
 Keywords: openmeter,api,client,usage,usage-based,metering,ai,aggregation,real-time,billing,cloud
 Author: Andras Toth
 Author-email: 4157749+tothandras@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```
