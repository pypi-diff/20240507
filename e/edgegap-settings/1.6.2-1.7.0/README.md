# Comparing `tmp/edgegap_settings-1.6.2.tar.gz` & `tmp/edgegap_settings-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.6.2.tar", max compression
+gzip compressed data, was "edgegap_settings-1.7.0.tar", max compression
```

## Comparing `edgegap_settings-1.6.2.tar` & `edgegap_settings-1.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1993 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/LICENSE
--rw-r--r--   0        0        0     2182 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/README.md
--rw-r--r--   0        0        0       17 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/BUILD
--rw-r--r--   0        0        0      472 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_apm.py
--rw-r--r--   0        0        0     1169 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     2998 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      917 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-05-04 01:34:08.346442 edgegap_settings-1.6.2/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      741 2024-05-04 01:35:40.887658 edgegap_settings-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/LICENSE
+-rw-r--r--   0        0        0     2182 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/BUILD
+-rw-r--r--   0        0        0      472 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0     1169 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     3147 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      581 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      798 2024-05-07 13:29:33.612393 edgegap_settings-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 edgegap_settings-1.7.0/PKG-INFO
```

### Comparing `edgegap_settings-1.6.2/LICENSE` & `edgegap_settings-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.6.2/README.md` & `edgegap_settings-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.6.2/edgegap_settings/_apm.py` & `edgegap_settings-1.7.0/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.6.2/edgegap_settings/_base.py` & `edgegap_settings-1.7.0/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.6.2/edgegap_settings/_factory.py` & `edgegap_settings-1.7.0/edgegap_settings/_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import logging
 import os
 import sys
-from typing import Any
+from typing import Any, TypeVar
 
 from dotenv import load_dotenv
 from edgegap_consul import ConsulReader, ConsulReaderFactory
 from edgegap_logging import DefaultFormatter
 from pydantic import ValidationError
+from pydantic_core import PydanticUndefined
 from pydantic_settings import BaseSettings
 
 load_dotenv()
 
 logger = logging.getLogger('settings.Factory')
 
 # Small Temporary formatting since this is most likely be called before any Logger Initialization
 fmt = DefaultFormatter()
 handler = logging.StreamHandler(sys.stdout)
 handler.setFormatter(fmt)
 logger.addHandler(handler)
 
+T = TypeVar('T', bound=BaseSettings)
+
 
 class SettingsFactory:
     __mapping__: dict[str, type(BaseSettings)] = {}
     __consul_reader: ConsulReader = ConsulReaderFactory().from_env()
 
     @classmethod
-    def from_settings(cls, settings: type(BaseSettings)) -> type(BaseSettings):
+    def from_settings(cls, settings: type[T]) -> T:
         name = settings.__name__
 
         if name not in cls.__mapping__.keys():
             consul_prefix = settings.model_config.get('prefix')
             data = {}
 
             for field_name, field in settings.model_fields.items():
@@ -49,22 +52,22 @@
 
                     if value is not None:
                         data[field_name] = value
 
             try:
                 cls.__mapping__[name] = settings(**data)
             except ValidationError as e:
-                raise Exception('There was some errors during the Validation of your Settings, please adjust') from e
+                raise ValueError('There was some errors during the Validation of your Settings, please adjust') from e
 
         return cls.__mapping__.get(name)
 
     @classmethod
-    def __from_consul(cls, consul_full_key: str, default: Any = None) -> Any:
+    def __from_consul(cls, consul_full_key: str, default: Any) -> Any:
         exists, value = cls.__consul_reader.get(key=consul_full_key)
-        has_default = default is not None
+        has_default = default not in (None, PydanticUndefined)
         has_value = value is not None
 
         if has_value:
             return value
         elif not has_value and has_default:
             if exists:
                 logger.warning(
@@ -72,8 +75,12 @@
                     f" will fallback to default value '{default}'",
                 )
             else:
                 logger.warning(
                     f'Key [{consul_full_key}] does not exists in Consul but ' f"default is defined to: '{default}'",
                 )
         else:
-            raise Exception(f'Consul key [{consul_full_key}] is not defined and no default value')
+            raise ValueError(f'Consul key [{consul_full_key}] is not defined and no default value')
+
+    @classmethod
+    def clear(cls):
+        cls.__mapping__.clear()
```

### Comparing `edgegap_settings-1.6.2/pyproject.toml` & `edgegap_settings-1.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "1.6.2"
+version = "1.7.0"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
 pydantic = "^2.7.1"
 python-dotenv = "^1.0.1"
 edgegap-logging = "^1.0.0"
 edgegap-consul = "^1.0.0"
+python-logstash-async = "^3.0.0"
+elastic-apm = "^6.22.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
 ruff = "^0.4.2"
```

### Comparing `edgegap_settings-1.6.2/PKG-INFO` & `edgegap_settings-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.6.2
+Version: 1.7.0
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
+Requires-Dist: elastic-apm (>=6.22.0,<7.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: python-logstash-async (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Settings Library
 
 This is the README for the Edgegap Settings Helper, which is part of the Edgegap suite of helpers.
 This library provides utilities for interacting with Explicit Settings Models.
```

