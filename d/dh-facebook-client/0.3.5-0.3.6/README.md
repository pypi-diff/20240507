# Comparing `tmp/dh-facebook-client-0.3.5.tar.gz` & `tmp/dh-facebook-client-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh-facebook-client-0.3.5.tar", max compression
+gzip compressed data, was "dh-facebook-client-0.3.6.tar", max compression
```

## Comparing `dh-facebook-client-0.3.5.tar` & `dh-facebook-client-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       21 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/PYPI_README.md
--rw-r--r--   0        0        0      927 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    12419 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/client.py
--rw-r--r--   0        0        0      296 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     3996 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4643 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2946 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0      435 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/dh_facebook_client/typings.py
--rw-r--r--   0        0        0      731 2024-05-06 16:30:42.057899 dh-facebook-client-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      709 2024-05-06 16:31:19.212638 dh-facebook-client-0.3.5/setup.py
--rw-r--r--   0        0        0      454 2024-05-06 16:31:19.212879 dh-facebook-client-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/PYPI_README.md
+-rw-r--r--   0        0        0      991 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    12419 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      296 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     3996 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4643 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2946 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0      435 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0      731 2024-05-06 17:01:56.609514 dh-facebook-client-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      709 2024-05-06 17:02:30.179206 dh-facebook-client-0.3.6/setup.py
+-rw-r--r--   0        0        0      454 2024-05-06 17:02:30.179427 dh-facebook-client-0.3.6/PKG-INFO
```

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/__init__.py` & `dh-facebook-client-0.3.6/dh_facebook_client/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .client import GraphAPIClient
-from .dataclasses import AppUsageDetails, GraphAPIResponse
+from .dataclasses import AppUsageDetails, BusinessUseCaseUsageDetails, GraphAPIResponse
 from .error_code import GraphAPICommonErrorCode
 from .exceptions import (
     GraphAPIApplicationError,
     GraphAPIError,
     GraphAPIServiceError,
     GraphAPITokenError,
     GraphAPIUsageError,
@@ -12,14 +12,15 @@
 )
 from .helpers import FieldConfig, build_field_config_list, format_fields_str
 from .typings import ErrorCodeExceptionMap, GraphAPIErrorClassType
 
 __all__ = [
     'GraphAPIClient',
     'AppUsageDetails',
+    'BusinessUseCaseUsageDetails',
     'GraphAPIResponse',
     'GraphAPICommonErrorCode',
     'GraphAPIApplicationError',
     'GraphAPIError',
     'GraphAPIServiceError',
     'GraphAPITokenError',
     'GraphAPIUsageError',
```

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/client.py` & `dh-facebook-client-0.3.6/dh_facebook_client/client.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/dataclasses.py` & `dh-facebook-client-0.3.6/dh_facebook_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/error_code.py` & `dh-facebook-client-0.3.6/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/exceptions.py` & `dh-facebook-client-0.3.6/dh_facebook_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.5/dh_facebook_client/helpers.py` & `dh-facebook-client-0.3.6/dh_facebook_client/helpers.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.5/pyproject.toml` & `dh-facebook-client-0.3.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.3.5"
+version = "0.3.6"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 readme = "PYPI_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
```

### Comparing `dh-facebook-client-0.3.5/setup.py` & `dh-facebook-client-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['backoff>=1.11.1,<2.0.0', 'requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'dh-facebook-client',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'Simple client for interacting with the Facebook Graph API',
     'long_description': '# dh-facebook-client\n',
     'author': 'pchisholm',
     'author_email': 'chisholm.p@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

