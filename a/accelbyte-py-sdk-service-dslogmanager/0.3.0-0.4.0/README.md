# Comparing `tmp/accelbyte-py-sdk-service-dslogmanager-0.3.0.tar.gz` & `tmp/accelbyte_py_sdk_service_dslogmanager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-dslogmanager-0.3.0.tar", last modified: Tue Jan 30 05:58:45 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_dslogmanager-0.4.0.tar", last modified: Tue May  7 06:26:56 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0.tar` & `accelbyte_py_sdk_service_dslogmanager-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1148 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      884 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/
--rw-rw-r--   0 root         (0) root         (0)     1214 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/
--rw-rw-r--   0 root         (0) root         (0)     1477 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7058 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     5139 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_allocation_event.py
--rw-rw-r--   0 root         (0) root         (0)     4384 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_batch_download_logs_request.py
--rw-rw-r--   0 root         (0) root         (0)     5181 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_download_logs_request.py
--rw-rw-r--   0 root         (0) root         (0)     5366 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_list_terminated_servers_response.py
--rw-rw-r--   0 root         (0) root         (0)     3876 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_log_file_status.py
--rw-rw-r--   0 root         (0) root         (0)     6451 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_match_result.py
--rw-rw-r--   0 root         (0) root         (0)     5056 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_notif_payload_server_status_change.py
--rw-rw-r--   0 root         (0) root         (0)     5486 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)     3816 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_member.py
--rw-rw-r--   0 root         (0) root         (0)     6034 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_party.py
--rw-rw-r--   0 root         (0) root         (0)     4454 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)    22193 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     4517 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_server_logs.py
--rw-rw-r--   0 root         (0) root         (0)     4407 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_status_history.py
--rw-rw-r--   0 root         (0) root         (0)     4442 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/
--rw-rw-r--   0 root         (0) root         (0)      442 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.597344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/
--rw-rw-r--   0 root         (0) root         (0)      518 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9902 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/get_server_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      605 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6392 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/batch_download_server_logs.py
--rw-rw-r--   0 root         (0) root         (0)    18126 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/list_all_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/
--rw-rw-r--   0 root         (0) root         (0)      526 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4759 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      634 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7035 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/check_server_logs.py
--rw-rw-r--   0 root         (0) root         (0)     6930 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/download_server_logs.py
--rw-rw-r--   0 root         (0) root         (0)    19058 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/list_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     1288 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4951 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_admin.py
--rw-rw-r--   0 root         (0) root         (0)     9564 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_all_terminated_servers.py
--rw-rw-r--   0 root         (0) root         (0)     2681 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_dslogmanager_operations.py
--rw-rw-r--   0 root         (0) root         (0)    13617 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1148 2024-01-30 05:58:45.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2842 2024-01-30 05:58:45.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 05:58:45.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-30 05:58:45.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-30 05:58:45.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      371 2024-01-30 05:56:16.000000 accelbyte-py-sdk-service-dslogmanager-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-30 05:58:45.601344 accelbyte-py-sdk-service-dslogmanager-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      884 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/
+-rw-rw-r--   0 root         (0) root         (0)     1214 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/
+-rw-rw-r--   0 root         (0) root         (0)     1477 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7058 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     5139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_allocation_event.py
+-rw-rw-r--   0 root         (0) root         (0)     4384 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_batch_download_logs_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5181 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_download_logs_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_list_terminated_servers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_log_file_status.py
+-rw-rw-r--   0 root         (0) root         (0)     6451 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_match_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5056 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_notif_payload_server_status_change.py
+-rw-rw-r--   0 root         (0) root         (0)     5486 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     3816 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_member.py
+-rw-rw-r--   0 root         (0) root         (0)     6034 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4454 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)    22193 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     4517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_server_logs.py
+-rw-rw-r--   0 root         (0) root         (0)     4407 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_status_history.py
+-rw-rw-r--   0 root         (0) root         (0)     4442 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/
+-rw-rw-r--   0 root         (0) root         (0)      518 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10208 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/get_server_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.635413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      605 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6668 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/batch_download_server_logs.py
+-rw-rw-r--   0 root         (0) root         (0)    18395 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/list_all_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/
+-rw-rw-r--   0 root         (0) root         (0)      526 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5025 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      634 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7342 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/check_server_logs.py
+-rw-rw-r--   0 root         (0) root         (0)     7239 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/download_server_logs.py
+-rw-rw-r--   0 root         (0) root         (0)    19350 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/list_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     1288 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4951 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_admin.py
+-rw-rw-r--   0 root         (0) root         (0)     9564 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_all_terminated_servers.py
+-rw-rw-r--   0 root         (0) root         (0)     2681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_dslogmanager_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    13617 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-07 06:26:56.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-07 06:26:56.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:26:56.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:26:56.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:26:56.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      371 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dslogmanager-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:26:56.639413 accelbyte_py_sdk_service_dslogmanager-0.4.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/PKG-INFO` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dslogmanager
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Log Manager Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/README.md` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/log_app_message_declaration.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_allocation_event.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_allocation_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_batch_download_logs_request.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_batch_download_logs_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_download_logs_request.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_download_logs_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_list_terminated_servers_response.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_list_terminated_servers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_log_file_status.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_log_file_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_match_result.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_match_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_notif_payload_server_status_change.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_notif_payload_server_status_change.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_paging_cursor.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_member.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_party.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_match_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_matching_ally.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_request_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_server.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_server_logs.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_server_logs.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/models_status_history.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/models_status_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/models/response_error.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/get_server_logs.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/admin/get_server_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/admin/namespaces/{namespace}/servers/{podName}/logs"
+    _path: str = "/dslogmanager/admin/namespaces/{namespace}/servers/{podName}/logs"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     namespace: str  # REQUIRED in [path]
     pod_name: str  # REQUIRED in [path]
     log_type: str  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     origin: str  # OPTIONAL in [query]
 
     # endregion fields
@@ -103,14 +107,22 @@
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/batch_download_server_logs.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/batch_download_server_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,31 +70,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/servers/logs/download"
+    _path: str = "/dslogmanager/servers/logs/download"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     body: ModelsBatchDownloadLogsRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/list_all_terminated_servers.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/all_terminated_servers/list_all_terminated_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/servers/search"
+    _path: str = "/dslogmanager/servers/search"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     deployment: str  # OPTIONAL in [query]
     end_date: str  # OPTIONAL in [query]
     game_mode: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     namespace: str  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     party_id: str  # OPTIONAL in [query]
@@ -128,14 +132,22 @@
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/public_get_messages.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/dslogmanager_operations/public_get_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,29 +56,41 @@
 
         500: Internal Server Error - ResponseError
     """
 
     # region fields
 
     _url: str = "/dslogmanager/v1/messages"
+    _path: str = "/dslogmanager/v1/messages"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/check_server_logs.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/check_server_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/namespaces/{namespace}/servers/{podName}/logs/exists"
+    _path: str = "/dslogmanager/namespaces/{namespace}/servers/{podName}/logs/exists"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     namespace: str  # REQUIRED in [path]
     pod_name: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/download_server_logs.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/download_server_logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/namespaces/{namespace}/servers/{podName}/logs/download"
+    _path: str = "/dslogmanager/namespaces/{namespace}/servers/{podName}/logs/download"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     namespace: str  # REQUIRED in [path]
     pod_name: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/list_terminated_servers.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/operations/terminated_servers/list_terminated_servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dslogmanager/namespaces/{namespace}/servers/search"
+    _path: str = "/dslogmanager/namespaces/{namespace}/servers/search"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dslogmanager"
+
     namespace: str  # REQUIRED in [path]
     deployment: str  # OPTIONAL in [query]
     end_date: str  # OPTIONAL in [query]
     game_mode: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     party_id: str  # OPTIONAL in [query]
@@ -133,14 +137,22 @@
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

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/__init__.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_admin.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_admin.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_all_terminated_servers.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_all_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_dslogmanager_operations.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_dslogmanager_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_terminated_servers.py` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk/api/dslogmanager/wrappers/_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dslogmanager
-Version: 0.3.0
+Version: 0.4.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Log Manager Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-dslogmanager-0.3.0/accelbyte_py_sdk_service_dslogmanager.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_dslogmanager-0.4.0/accelbyte_py_sdk_service_dslogmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

