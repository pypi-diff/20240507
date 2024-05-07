# Comparing `tmp/django_contract_tester-1.3.1.tar.gz` & `tmp/django_contract_tester-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_contract_tester-1.3.1.tar", max compression
+gzip compressed data, was "django_contract_tester-1.3.2.tar", max compression
```

## Comparing `django_contract_tester-1.3.1.tar` & `django_contract_tester-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      598 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1500 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/LICENSE
--rw-r--r--   0        0        0     8081 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/README.md
--rw-r--r--   0        0        0      577 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/case_testers.py
--rw-r--r--   0        0        0     4032 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/clients.py
--rw-r--r--   0        0        0      426 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/config.py
--rw-r--r--   0        0        0     2923 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/constants.py
--rw-r--r--   0        0        0      762 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/exceptions.py
--rw-r--r--   0        0        0    11261 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/loaders.py
--rw-r--r--   0        0        0        0 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/py.typed
--rw-r--r--   0        0        0     1918 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/response_handler.py
--rw-r--r--   0        0        0      856 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/response_handler_factory.py
--rw-r--r--   0        0        0    26740 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/schema_tester.py
--rw-r--r--   0        0        0     2197 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/utils.py
--rw-r--r--   0        0        0     8559 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/validators.py
--rw-r--r--   0        0        0     4045 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    10900 1970-01-01 00:00:00.000000 django_contract_tester-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      598 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1500 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/LICENSE
+-rw-r--r--   0        0        0     8081 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/README.md
+-rw-r--r--   0        0        0      577 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/__init__.py
+-rw-r--r--   0        0        0     1133 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/case_testers.py
+-rw-r--r--   0        0        0     4032 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/clients.py
+-rw-r--r--   0        0        0      426 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/config.py
+-rw-r--r--   0        0        0     3029 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/constants.py
+-rw-r--r--   0        0        0      762 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/exceptions.py
+-rw-r--r--   0        0        0    11261 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/loaders.py
+-rw-r--r--   0        0        0        0 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/py.typed
+-rw-r--r--   0        0        0     1918 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/response_handler.py
+-rw-r--r--   0        0        0      856 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/response_handler_factory.py
+-rw-r--r--   0        0        0    26872 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/schema_tester.py
+-rw-r--r--   0        0        0     2326 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/utils.py
+-rw-r--r--   0        0        0     9307 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/openapi_tester/validators.py
+-rw-r--r--   0        0        0     4045 2024-05-07 18:03:44.211497 django_contract_tester-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10900 1970-01-01 00:00:00.000000 django_contract_tester-1.3.2/PKG-INFO
```

### Comparing `django_contract_tester-1.3.1/CHANGELOG.md` & `django_contract_tester-1.3.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/LICENSE` & `django_contract_tester-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/README.md` & `django_contract_tester-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/__init__.py` & `django_contract_tester-1.3.2/openapi_tester/__init__.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/case_testers.py` & `django_contract_tester-1.3.2/openapi_tester/case_testers.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/clients.py` & `django_contract_tester-1.3.2/openapi_tester/clients.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/constants.py` & `django_contract_tester-1.3.2/openapi_tester/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,21 @@
     "file": str.__name__,
     "array": list.__name__,
     "object": dict.__name__,
     "integer": int.__name__,
     "number": f"{int.__name__} or {float.__name__}",
 }
 
+NUMERIC_FORMATS = ["number", "float", "double"]
+
+INTERNET_PROTOCOLS = ["ipv4", "ipv6", "email"]
+
 # Validation errors
 VALIDATE_FORMAT_ERROR = (
-    'Expected: {article} "{format}" formatted value\n\nReceived: {received}'
+    'Expected: {article} "{format}" formatted "{type}" value\n\nReceived: {received}'
 )
 VALIDATE_PATTERN_ERROR = (
     'The string "{data}" does not match the specified pattern: {pattern}'
 )
 INVALID_PATTERN_ERROR = "String pattern is not valid regex: {pattern}"
 VALIDATE_ENUM_ERROR = "Expected: a member of the enum {enum}\n\nReceived: {received}"
 VALIDATE_TYPE_ERROR = 'Expected: {article} "{type}" type value\n\nReceived: {received}'
```

### Comparing `django_contract_tester-1.3.1/openapi_tester/exceptions.py` & `django_contract_tester-1.3.2/openapi_tester/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/loaders.py` & `django_contract_tester-1.3.2/openapi_tester/loaders.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/response_handler.py` & `django_contract_tester-1.3.2/openapi_tester/response_handler.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/response_handler_factory.py` & `django_contract_tester-1.3.2/openapi_tester/response_handler_factory.py`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.1/openapi_tester/schema_tester.py` & `django_contract_tester-1.3.2/openapi_tester/schema_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 from openapi_tester.loaders import (
     DrfSpectacularSchemaLoader,
     DrfYasgSchemaLoader,
     StaticSchemaLoader,
     UrlStaticSchemaLoader,
 )
 from openapi_tester.response_handler_factory import ResponseHandlerFactory
-from openapi_tester.utils import lazy_combinations, normalize_schema_section
+from openapi_tester.utils import (
+    lazy_combinations,
+    normalize_schema_section,
+    serialize_schema_section_data,
+)
 from openapi_tester.validators import (
     validate_enum,
     validate_format,
     validate_max_items,
     validate_max_length,
     validate_max_properties,
     validate_maximum,
@@ -550,37 +554,37 @@
         for key in properties.keys():
             self.test_key_casing(key, test_config.case_tester, test_config.ignore_case)
             if key in required_keys and key not in request_response_keys:
                 raise DocumentationError(
                     f"{VALIDATE_MISSING_KEY_ERROR.format(missing_key=key, http_message=test_config.http_message)}"
                     "\n\nReference:"
                     f"\n\n{test_config.reference} > {key}"
-                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
-                    f"\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {serialize_schema_section_data(data=data)}"
+                    f"\nSchema section:\n  {serialize_schema_section_data(data=properties)}"
                     "\n\nHint: Remove the key from your OpenAPI docs, or"
                     f" include it in your API {test_config.http_message}"
                 )
         for key in request_response_keys:
             self.test_key_casing(key, test_config.case_tester, test_config.ignore_case)
             if key not in properties and not additional_properties_allowed:
                 raise DocumentationError(
                     f"{VALIDATE_EXCESS_KEY_ERROR.format(excess_key=key, http_message=test_config.http_message)}"
                     "\n\nReference:"
                     f"\n\n{test_config.reference} > {key}"
-                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
-                    f"\n\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {serialize_schema_section_data(data=data)}"
+                    f"\n\nSchema section:\n  {serialize_schema_section_data(data=properties)}"
                     "\n\nHint: Remove the key from your API"
                     f" {test_config.http_message}, or include it in your OpenAPI docs"
                 )
             if key in write_only_properties:
                 raise DocumentationError(
                     f"{VALIDATE_WRITE_ONLY_RESPONSE_KEY_ERROR.format(write_only_key=key)}\n\nReference:"
                     f"\n\n{test_config.reference} > {key}"
-                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
-                    f"\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {serialize_schema_section_data(data=data)}"
+                    f"\nSchema section:\n  {serialize_schema_section_data(data=properties)}"
                     f"\n\nHint: Remove the key from your API {test_config.http_message}, or"
                     ' remove the "WriteOnly" restriction'
                 )
         for key, value in data.items():
             if key in properties:
                 drill_down_test_config = copy(test_config)
                 drill_down_test_config.reference = f"{test_config.reference} > {key}"
```

### Comparing `django_contract_tester-1.3.1/openapi_tester/utils.py` & `django_contract_tester-1.3.2/openapi_tester/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utils Module - this file contains utility functions used in multiple places.
 """
 
 from __future__ import annotations
 
+import json
 from copy import deepcopy
 from itertools import chain, combinations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any, Iterator, Sequence
 
@@ -51,14 +52,18 @@
             output[key] = [
                 normalize_schema_section(entry) if isinstance(entry, dict) else entry
                 for entry in value
             ]
     return output
 
 
+def serialize_schema_section_data(data: dict[str, Any]) -> str:
+    return json.dumps(data, indent=4, default=str)
+
+
 def lazy_combinations(options_list: Sequence[dict[str, Any]]) -> Iterator[dict]:
     """
     Lazily evaluate possible combinations.
     """
     for i in range(2, len(options_list) + 1):
         for combination in combinations(options_list, i):
             yield merge_objects(combination)
```

### Comparing `django_contract_tester-1.3.1/openapi_tester/validators.py` & `django_contract_tester-1.3.2/openapi_tester/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     URLValidator,
     validate_ipv4_address,
     validate_ipv6_address,
 )
 from django.utils.dateparse import parse_date, parse_datetime, parse_time
 
 from openapi_tester.constants import (
+    INTERNET_PROTOCOLS,
     INVALID_PATTERN_ERROR,
+    NUMERIC_FORMATS,
     VALIDATE_ENUM_ERROR,
     VALIDATE_FORMAT_ERROR,
     VALIDATE_MAX_ARRAY_LENGTH_ERROR,
     VALIDATE_MAX_LENGTH_ERROR,
     VALIDATE_MAXIMUM_ERROR,
     VALIDATE_MAXIMUM_NUMBER_OF_PROPERTIES_ERROR,
     VALIDATE_MIN_ARRAY_LENGTH_ERROR,
@@ -110,21 +112,38 @@
             type=schema_types,
             received=f'"{data}"' if isinstance(data, str) else data,
         )
     return None
 
 
 def validate_format(schema_section: dict[str, Any], data: Any) -> str | None:
+    value = data
     schema_format: str = schema_section.get("format", "")
-    if schema_format in VALIDATOR_MAP and not VALIDATOR_MAP[schema_format](data):
-        return VALIDATE_FORMAT_ERROR.format(
-            article="an" if format in ["ipv4", "ipv6", "email"] else "a",
-            format=schema_format,
-            received=f'"{data}"',
-        )
+    schema_type: str = schema_section.get("type", "object")
+    if schema_format in VALIDATOR_MAP:
+        if not isinstance(schema_type, list) and schema_type == "string":
+            try:
+                if schema_format == "integer":
+                    value = int(data)
+                if schema_format in NUMERIC_FORMATS:
+                    value = float(data)
+            except ValueError:
+                return VALIDATE_FORMAT_ERROR.format(
+                    article="an" if format in INTERNET_PROTOCOLS else "a",
+                    format=schema_format,
+                    type=schema_type,
+                    received=f'"{value}"',
+                )
+        if not VALIDATOR_MAP[schema_format](value):
+            return VALIDATE_FORMAT_ERROR.format(
+                article="an" if format in INTERNET_PROTOCOLS else "a",
+                format=schema_format,
+                type=schema_type,
+                received=f'"{value}"',
+            )
     return None
 
 
 def validate_enum(schema_section: dict[str, Any], data: Any) -> str | None:
     enum = schema_section.get("enum")
     if enum and data not in enum:
         return VALIDATE_ENUM_ERROR.format(
```

### Comparing `django_contract_tester-1.3.1/pyproject.toml` & `django_contract_tester-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-contract-tester"
-version = "1.3.1"
+version = "1.3.2"
 description = "Test utility for validating OpenAPI response documentation"
 authors =["Matías Cárdenas <cardenasmatias.1990@gmail.com>", "Sondre Lillebø Gundersen <sondrelg@live.no>", "Na'aman Hirschfeld <nhirschfeld@gmail.com>"]
 license = "BSD-4-Clause"
 readme = "README.md"
 homepage = "https://github.com/maticardenas/django-contract-tester"
 repository = "https://github.com/maticardenas/django-contract-tester"
 documentation = "https://github.com/maticardenas/django-contract-tester"
```

### Comparing `django_contract_tester-1.3.1/PKG-INFO` & `django_contract_tester-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-contract-tester
-Version: 1.3.1
+Version: 1.3.2
 Summary: Test utility for validating OpenAPI response documentation
 Home-page: https://github.com/maticardenas/django-contract-tester
 License: BSD-4-Clause
 Keywords: openapi,swagger,api,testing,schema,django,drf
 Author: Matías Cárdenas
 Author-email: cardenasmatias.1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

