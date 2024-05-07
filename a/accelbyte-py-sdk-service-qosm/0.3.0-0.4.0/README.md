# Comparing `tmp/accelbyte-py-sdk-service-qosm-0.3.0.tar.gz` & `tmp/accelbyte_py_sdk_service_qosm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-qosm-0.3.0.tar", last modified: Tue Jan 30 06:03:42 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_qosm-0.4.0.tar", last modified: Tue May  7 06:29:39 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-qosm-0.3.0.tar` & `accelbyte_py_sdk_service_qosm-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.512666 accelbyte-py-sdk-service-qosm-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1127 2024-01-30 06:03:42.512666 accelbyte-py-sdk-service-qosm-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      874 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.504665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.504665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/
--rw-rw-r--   0 root         (0) root         (0)      999 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/
--rw-rw-r--   0 root         (0) root         (0)      806 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4876 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_heartbeat_request.py
--rw-rw-r--   0 root         (0) root         (0)     4115 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_list_server_response.py
--rw-rw-r--   0 root         (0) root         (0)     6628 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     3740 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_set_alias_request.py
--rw-rw-r--   0 root         (0) root         (0)     3804 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_update_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     4215 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/
--rw-rw-r--   0 root         (0) root         (0)      440 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/
--rw-rw-r--   0 root         (0) root         (0)      611 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5684 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/delete_server.py
--rw-rw-r--   0 root         (0) root         (0)     7252 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/set_server_alias.py
--rw-rw-r--   0 root         (0) root         (0)     8195 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/update_server_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/
--rw-rw-r--   0 root         (0) root         (0)      571 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5517 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/list_server.py
--rw-rw-r--   0 root         (0) root         (0)     7500 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/list_server_per_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/server/
--rw-rw-r--   0 root         (0) root         (0)      506 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6125 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/server/heartbeat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/
--rw-rw-r--   0 root         (0) root         (0)      955 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9298 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_admin.py
--rw-rw-r--   0 root         (0) root         (0)     8062 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_public.py
--rw-rw-r--   0 root         (0) root         (0)     3442 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 06:03:42.508665 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1127 2024-01-30 06:03:42.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1502 2024-01-30 06:03:42.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 06:03:42.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-30 06:03:42.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-30 06:03:42.000000 accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      360 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-qosm-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-30 06:03:42.512666 accelbyte-py-sdk-service-qosm-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      874 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.390993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.390993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/
+-rw-rw-r--   0 root         (0) root         (0)      999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/
+-rw-rw-r--   0 root         (0) root         (0)      806 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_heartbeat_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4115 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_list_server_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6628 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     3740 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_set_alias_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3804 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_update_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4215 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/
+-rw-rw-r--   0 root         (0) root         (0)      611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5945 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/delete_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7519 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/set_server_alias.py
+-rw-rw-r--   0 root         (0) root         (0)     8479 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/update_server_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/
+-rw-rw-r--   0 root         (0) root         (0)      571 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5766 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/list_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7772 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/list_server_per_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/server/
+-rw-rw-r--   0 root         (0) root         (0)      506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6381 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/server/heartbeat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)      955 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9298 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_admin.py
+-rw-rw-r--   0 root         (0) root         (0)     8062 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_public.py
+-rw-rw-r--   0 root         (0) root         (0)     3442 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-07 06:29:39.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-07 06:29:39.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:29:39.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:29:39.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:29:39.000000 accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      360 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_qosm-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:29:39.394993 accelbyte_py_sdk_service_qosm-0.4.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/PKG-INFO` & `accelbyte_py_sdk_service_qosm-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-qosm
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Qos Manager Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/README.md` & `accelbyte_py_sdk_service_qosm-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/__init__.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/__init__.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_heartbeat_request.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_heartbeat_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_list_server_response.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_list_server_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_server.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_set_alias_request.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_set_alias_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/models_update_server_request.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/models_update_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/models/response_error.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/__init__.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/delete_server.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/delete_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,31 +68,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/admin/servers/{region}"
+    _path: str = "/qosm/admin/servers/{region}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
+
     region: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/set_server_alias.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/set_server_alias.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,32 +75,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/admin/servers/{region}/alias"
+    _path: str = "/qosm/admin/servers/{region}/alias"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
+
     body: ModelsSetAliasRequest  # REQUIRED in [body]
     region: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/admin/update_server_config.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/admin/update_server_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,33 +77,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/admin/namespaces/{namespace}/servers/{region}"
+    _path: str = "/qosm/admin/namespaces/{namespace}/servers/{region}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
+
     body: ModelsUpdateServerRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     region: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/__init__.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/list_server.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/list_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,29 +72,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/public/qos"
+    _path: str = "/qosm/public/qos"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/public/list_server_per_namespace.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/public/list_server_per_namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,32 +76,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/public/namespaces/{namespace}/qos"
+    _path: str = "/qosm/public/namespaces/{namespace}/qos"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
+
     namespace: str  # REQUIRED in [path]
     status: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/operations/server/heartbeat.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/operations/server/heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/qosm/servers/heartbeat"
+    _path: str = "/qosm/servers/heartbeat"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "qosm"
+
     body: ModelsHeartbeatRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/__init__.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_admin.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_admin.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_public.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_public.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk/api/qosm/wrappers/_server.py` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk/api/qosm/wrappers/_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-qosm
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Qos Manager Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-qosm-0.3.0/accelbyte_py_sdk_service_qosm.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_qosm-0.4.0/accelbyte_py_sdk_service_qosm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

