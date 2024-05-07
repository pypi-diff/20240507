# Comparing `tmp/accelbyte-py-sdk-service-gametelemetry-0.6.0.tar.gz` & `tmp/accelbyte_py_sdk_service_gametelemetry-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-gametelemetry-0.6.0.tar", last modified: Wed Mar 13 06:11:36 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_gametelemetry-0.7.0.tar", last modified: Tue May  7 06:27:31 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0.tar` & `accelbyte_py_sdk_service_gametelemetry-0.7.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      862 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.839937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.839937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.839937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/
--rw-rw-r--   0 root         (0) root         (0)     1516 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/
--rw-rw-r--   0 root         (0) root         (0)      920 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4480 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     8995 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4088 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     3715 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py
--rw-rw-r--   0 root         (0) root         (0)     4971 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     3825 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py
--rw-rw-r--   0 root         (0) root         (0)     7624 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/
--rw-rw-r--   0 root         (0) root         (0)      419 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/
--rw-rw-r--   0 root         (0) root         (0)      818 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8136 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py
--rw-rw-r--   0 root         (0) root         (0)     8855 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py
--rw-rw-r--   0 root         (0) root         (0)     8988 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/
--rw-rw-r--   0 root         (0) root         (0)      663 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14611 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py
--rw-rw-r--   0 root         (0) root         (0)     4984 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     1605 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13207 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py
--rw-rw-r--   0 root         (0) root         (0)     8148 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-03-13 06:11:36.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1874 2024-03-13 06:11:36.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:11:36.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:11:36.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:11:36.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      348 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-gametelemetry-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:11:36.843937 accelbyte-py-sdk-service-gametelemetry-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      862 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.022477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/
+-rw-rw-r--   0 root         (0) root         (0)     1516 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/
+-rw-rw-r--   0 root         (0) root         (0)      947 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4480 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9154 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4088 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     3715 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py
+-rw-rw-r--   0 root         (0) root         (0)     5143 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paging.py
+-rw-rw-r--   0 root         (0) root         (0)     3825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/
+-rw-rw-r--   0 root         (0) root         (0)      419 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/
+-rw-rw-r--   0 root         (0) root         (0)      818 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8434 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py
+-rw-rw-r--   0 root         (0) root         (0)     9132 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py
+-rw-rw-r--   0 root         (0) root         (0)     9297 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14907 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py
+-rw-rw-r--   0 root         (0) root         (0)     5261 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     1605 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13207 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py
+-rw-rw-r--   0 root         (0) root         (0)     8148 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:31.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      348 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gametelemetry-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:31.026477 accelbyte_py_sdk_service_gametelemetry-0.7.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/PKG-INFO` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gametelemetry
-Version: 0.6.0
+Version: 0.7.0
 Summary: AccelByte Python SDK - Analytics Game Telemetry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.1
+* Version: 1.24.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/README.md` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.1
+* Version: 1.24.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.1"
+__version__ = "1.24.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # gametelemetry_operations
 from .wrappers import (
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.1"
+__version__ = "1.24.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .base_error_response import BaseErrorResponse
 from .get_namespace_event_response import GetNamespaceEventResponse
 from .http_validation_error import HTTPValidationError
 from .list_base_response_str import ListBaseResponseStr
 from .paged_response_get_namespace_event_response import (
     PagedResponseGetNamespaceEventResponse,
 )
+from .paging import Paging
 from .play_time_response import PlayTimeResponse
 from .telemetry_body import TelemetryBody
 from .validation_error import ValidationError
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,35 +34,35 @@
     Properties:
         event_id: (EventId) REQUIRED str
 
         event_name: (EventName) REQUIRED str
 
         event_namespace: (EventNamespace) REQUIRED str
 
-        event_time_stamp: (EventTimeStamp) REQUIRED str
+        event_timestamp: (EventTimestamp) REQUIRED str
 
-        flight_id: (FlightId) REQUIRED str
+        flight_id: (FlightId) OPTIONAL str
 
-        user_id: (UserId) REQUIRED str
+        payload: (Payload) OPTIONAL Dict[str, Any]
 
-        user_namespace: (UserNamespace) REQUIRED str
+        user_id: (UserId) OPTIONAL str
 
-        payload: (Payload) OPTIONAL Dict[str, Any]
+        user_namespace: (UserNamespace) OPTIONAL str
     """
 
     # region fields
 
     event_id: str  # REQUIRED
     event_name: str  # REQUIRED
     event_namespace: str  # REQUIRED
-    event_time_stamp: str  # REQUIRED
-    flight_id: str  # REQUIRED
-    user_id: str  # REQUIRED
-    user_namespace: str  # REQUIRED
+    event_timestamp: str  # REQUIRED
+    flight_id: str  # OPTIONAL
     payload: Dict[str, Any]  # OPTIONAL
+    user_id: str  # OPTIONAL
+    user_namespace: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_event_id(self, value: str) -> GetNamespaceEventResponse:
         self.event_id = value
@@ -72,34 +72,34 @@
         self.event_name = value
         return self
 
     def with_event_namespace(self, value: str) -> GetNamespaceEventResponse:
         self.event_namespace = value
         return self
 
-    def with_event_time_stamp(self, value: str) -> GetNamespaceEventResponse:
-        self.event_time_stamp = value
+    def with_event_timestamp(self, value: str) -> GetNamespaceEventResponse:
+        self.event_timestamp = value
         return self
 
     def with_flight_id(self, value: str) -> GetNamespaceEventResponse:
         self.flight_id = value
         return self
 
+    def with_payload(self, value: Dict[str, Any]) -> GetNamespaceEventResponse:
+        self.payload = value
+        return self
+
     def with_user_id(self, value: str) -> GetNamespaceEventResponse:
         self.user_id = value
         return self
 
     def with_user_namespace(self, value: str) -> GetNamespaceEventResponse:
         self.user_namespace = value
         return self
 
-    def with_payload(self, value: Dict[str, Any]) -> GetNamespaceEventResponse:
-        self.payload = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "event_id"):
@@ -110,63 +110,66 @@
             result["EventName"] = str(self.event_name)
         elif include_empty:
             result["EventName"] = ""
         if hasattr(self, "event_namespace"):
             result["EventNamespace"] = str(self.event_namespace)
         elif include_empty:
             result["EventNamespace"] = ""
-        if hasattr(self, "event_time_stamp"):
-            result["EventTimeStamp"] = str(self.event_time_stamp)
+        if hasattr(self, "event_timestamp"):
+            result["EventTimestamp"] = str(self.event_timestamp)
         elif include_empty:
-            result["EventTimeStamp"] = ""
+            result["EventTimestamp"] = ""
         if hasattr(self, "flight_id"):
             result["FlightId"] = str(self.flight_id)
         elif include_empty:
             result["FlightId"] = ""
+        if hasattr(self, "payload"):
+            result["Payload"] = {str(k0): v0 for k0, v0 in self.payload.items()}
+        elif include_empty:
+            result["Payload"] = {}
         if hasattr(self, "user_id"):
             result["UserId"] = str(self.user_id)
         elif include_empty:
             result["UserId"] = ""
         if hasattr(self, "user_namespace"):
             result["UserNamespace"] = str(self.user_namespace)
         elif include_empty:
             result["UserNamespace"] = ""
-        if hasattr(self, "payload"):
-            result["Payload"] = {str(k0): v0 for k0, v0 in self.payload.items()}
-        elif include_empty:
-            result["Payload"] = {}
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         event_id: str,
         event_name: str,
         event_namespace: str,
-        event_time_stamp: str,
-        flight_id: str,
-        user_id: str,
-        user_namespace: str,
+        event_timestamp: str,
+        flight_id: Optional[str] = None,
         payload: Optional[Dict[str, Any]] = None,
+        user_id: Optional[str] = None,
+        user_namespace: Optional[str] = None,
         **kwargs,
     ) -> GetNamespaceEventResponse:
         instance = cls()
         instance.event_id = event_id
         instance.event_name = event_name
         instance.event_namespace = event_namespace
-        instance.event_time_stamp = event_time_stamp
-        instance.flight_id = flight_id
-        instance.user_id = user_id
-        instance.user_namespace = user_namespace
+        instance.event_timestamp = event_timestamp
+        if flight_id is not None:
+            instance.flight_id = flight_id
         if payload is not None:
             instance.payload = payload
+        if user_id is not None:
+            instance.user_id = user_id
+        if user_namespace is not None:
+            instance.user_namespace = user_namespace
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> GetNamespaceEventResponse:
         instance = cls()
@@ -180,34 +183,34 @@
             instance.event_name = str(dict_["EventName"])
         elif include_empty:
             instance.event_name = ""
         if "EventNamespace" in dict_ and dict_["EventNamespace"] is not None:
             instance.event_namespace = str(dict_["EventNamespace"])
         elif include_empty:
             instance.event_namespace = ""
-        if "EventTimeStamp" in dict_ and dict_["EventTimeStamp"] is not None:
-            instance.event_time_stamp = str(dict_["EventTimeStamp"])
+        if "EventTimestamp" in dict_ and dict_["EventTimestamp"] is not None:
+            instance.event_timestamp = str(dict_["EventTimestamp"])
         elif include_empty:
-            instance.event_time_stamp = ""
+            instance.event_timestamp = ""
         if "FlightId" in dict_ and dict_["FlightId"] is not None:
             instance.flight_id = str(dict_["FlightId"])
         elif include_empty:
             instance.flight_id = ""
+        if "Payload" in dict_ and dict_["Payload"] is not None:
+            instance.payload = {str(k0): v0 for k0, v0 in dict_["Payload"].items()}
+        elif include_empty:
+            instance.payload = {}
         if "UserId" in dict_ and dict_["UserId"] is not None:
             instance.user_id = str(dict_["UserId"])
         elif include_empty:
             instance.user_id = ""
         if "UserNamespace" in dict_ and dict_["UserNamespace"] is not None:
             instance.user_namespace = str(dict_["UserNamespace"])
         elif include_empty:
             instance.user_namespace = ""
-        if "Payload" in dict_ and dict_["Payload"] is not None:
-            instance.payload = {str(k0): v0 for k0, v0 in dict_["Payload"].items()}
-        elif include_empty:
-            instance.payload = {}
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, GetNamespaceEventResponse]:
         return (
@@ -246,28 +249,28 @@
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "EventId": "event_id",
             "EventName": "event_name",
             "EventNamespace": "event_namespace",
-            "EventTimeStamp": "event_time_stamp",
+            "EventTimestamp": "event_timestamp",
             "FlightId": "flight_id",
+            "Payload": "payload",
             "UserId": "user_id",
             "UserNamespace": "user_namespace",
-            "Payload": "payload",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "EventId": True,
             "EventName": True,
             "EventNamespace": True,
-            "EventTimeStamp": True,
-            "FlightId": True,
-            "UserId": True,
-            "UserNamespace": True,
+            "EventTimestamp": True,
+            "FlightId": False,
             "Payload": False,
+            "UserId": False,
+            "UserNamespace": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,41 +24,42 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 from ..models.get_namespace_event_response import GetNamespaceEventResponse
+from ..models.paging import Paging
 
 
 class PagedResponseGetNamespaceEventResponse(Model):
     """Paged response get namespace event response (PagedResponse_GetNamespaceEventResponse_)
 
     Properties:
         data: (data) REQUIRED List[GetNamespaceEventResponse]
 
-        paging: (paging) REQUIRED int
+        paging: (paging) REQUIRED Paging
     """
 
     # region fields
 
     data: List[GetNamespaceEventResponse]  # REQUIRED
-    paging: int  # REQUIRED
+    paging: Paging  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_data(
         self, value: List[GetNamespaceEventResponse]
     ) -> PagedResponseGetNamespaceEventResponse:
         self.data = value
         return self
 
-    def with_paging(self, value: int) -> PagedResponseGetNamespaceEventResponse:
+    def with_paging(self, value: Paging) -> PagedResponseGetNamespaceEventResponse:
         self.paging = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -67,26 +68,26 @@
         if hasattr(self, "data"):
             result["data"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.data
             ]
         elif include_empty:
             result["data"] = []
         if hasattr(self, "paging"):
-            result["paging"] = int(self.paging)
+            result["paging"] = self.paging.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["paging"] = 0
+            result["paging"] = Paging()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, data: List[GetNamespaceEventResponse], paging: int, **kwargs
+        cls, data: List[GetNamespaceEventResponse], paging: Paging, **kwargs
     ) -> PagedResponseGetNamespaceEventResponse:
         instance = cls()
         instance.data = data
         instance.paging = paging
         return instance
 
     @classmethod
@@ -102,17 +103,19 @@
                     i0, include_empty=include_empty
                 )
                 for i0 in dict_["data"]
             ]
         elif include_empty:
             instance.data = []
         if "paging" in dict_ and dict_["paging"] is not None:
-            instance.paging = int(dict_["paging"])
+            instance.paging = Paging.create_from_dict(
+                dict_["paging"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.paging = 0
+            instance.paging = Paging()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, PagedResponseGetNamespaceEventResponse]:
         return (
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.1"
+__version__ = "1.24.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .protected_get_playtime__9a0e17 import (
     ProtectedGetPlaytimeGameTelemetryV1ProtectedSteamIdsSteamIdPlaytimeGet,
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - BaseErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/game-telemetry/v1/protected/steamIds/{steamId}/playtime"
+    _path: str = "/game-telemetry/v1/protected/steamIds/{steamId}/playtime"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["COOKIE_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gametelemetry"
+
     cookie: Union[str, HeaderStr]  # OPTIONAL in [header]
     steam_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,32 +113,44 @@
 
         507: Insufficient Storage - BaseErrorResponse (Insufficient space)
     """
 
     # region fields
 
     _url: str = "/game-telemetry/v1/protected/events"
+    _path: str = "/game-telemetry/v1/protected/events"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["COOKIE_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gametelemetry"
+
     body: List[TelemetryBody]  # REQUIRED in [body]
     cookie: Union[str, HeaderStr]  # OPTIONAL in [header]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_update_playti_4b5b85.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,33 +71,45 @@
 
         500: Internal Server Error - BaseErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/game-telemetry/v1/protected/steamIds/{steamId}/playtime/{playtime}"
+    _path: str = "/game-telemetry/v1/protected/steamIds/{steamId}/playtime/{playtime}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["COOKIE_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gametelemetry"
+
     cookie: Union[str, HeaderStr]  # OPTIONAL in [header]
     playtime: str  # REQUIRED in [path]
     steam_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.1"
+__version__ = "1.24.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_events_game_telemet_b2983d import (
     GetEventsGameTelemetryV1AdminNamespacesNamespaceEventsGet,
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_events_game_telemet_b2983d.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,24 @@
 
         422: Unprocessable Entity - HTTPValidationError (Validation Error)
     """
 
     # region fields
 
     _url: str = "/game-telemetry/v1/admin/namespaces/{namespace}/events"
+    _path: str = "/game-telemetry/v1/admin/namespaces/{namespace}/events"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["COOKIE_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gametelemetry"
+
     namespace: str  # REQUIRED in [path]
     end_time: str  # OPTIONAL in [query]
     event_id: str  # OPTIONAL in [query]
     event_name: str  # OPTIONAL in [query]
     event_payload: str  # OPTIONAL in [query]
     flight_id: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
@@ -106,14 +110,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/operations/telemetry/get_namespaces_game_tel_1106fd.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,29 +57,41 @@
 
         500: Internal Server Error - BaseErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/game-telemetry/v1/admin/namespaces"
+    _path: str = "/game-telemetry/v1/admin/namespaces"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["COOKIE_AUTH"], ["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gametelemetry"
+
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the Analytics Game Telemetry."""
 
-__version__ = "1.24.1"
+__version__ = "1.24.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._gametelemetry_operations import (
     protected_get_playtime_game_telemetry_v1_protected_steam_ids_steam_id_playtime_get,
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_gametelemetry_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk/api/gametelemetry/wrappers/_telemetry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gametelemetry
-Version: 0.6.0
+Version: 0.7.0
 Summary: AccelByte Python SDK - Analytics Game Telemetry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Analytics Game Telemetry
-* Version: 1.24.1
+* Version: 1.24.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gametelemetry-0.6.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_gametelemetry-0.7.0/accelbyte_py_sdk_service_gametelemetry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 accelbyte_py_sdk/api/gametelemetry/__init__.py
 accelbyte_py_sdk/api/gametelemetry/models/__init__.py
 accelbyte_py_sdk/api/gametelemetry/models/base_error_response.py
 accelbyte_py_sdk/api/gametelemetry/models/get_namespace_event_response.py
 accelbyte_py_sdk/api/gametelemetry/models/http_validation_error.py
 accelbyte_py_sdk/api/gametelemetry/models/list_base_response_str.py
 accelbyte_py_sdk/api/gametelemetry/models/paged_response_get_namespace_event_response.py
+accelbyte_py_sdk/api/gametelemetry/models/paging.py
 accelbyte_py_sdk/api/gametelemetry/models/play_time_response.py
 accelbyte_py_sdk/api/gametelemetry/models/telemetry_body.py
 accelbyte_py_sdk/api/gametelemetry/models/validation_error.py
 accelbyte_py_sdk/api/gametelemetry/operations/__init__.py
 accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/__init__.py
 accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_get_playtime__9a0e17.py
 accelbyte_py_sdk/api/gametelemetry/operations/gametelemetry_operations/protected_save_events_g_832bbb.py
```

