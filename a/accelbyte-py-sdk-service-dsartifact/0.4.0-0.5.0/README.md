# Comparing `tmp/accelbyte-py-sdk-service-dsartifact-0.4.0.tar.gz` & `tmp/accelbyte_py_sdk_service_dsartifact-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-dsartifact-0.4.0.tar", last modified: Tue Mar 26 05:41:01 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_dsartifact-0.5.0.tar", last modified: Tue May  7 06:26:45 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0.tar` & `accelbyte_py_sdk_service_dsartifact-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1139 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      880 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.161130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.161130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/
--rw-rw-r--   0 root         (0) root         (0)     1957 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/
--rw-rw-r--   0 root         (0) root         (0)     1579 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7055 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     7962 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py
--rw-rw-r--   0 root         (0) root         (0)     4910 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py
--rw-rw-r--   0 root         (0) root         (0)     5055 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py
--rw-rw-r--   0 root         (0) root         (0)     4872 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py
--rw-rw-r--   0 root         (0) root         (0)     4982 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py
--rw-rw-r--   0 root         (0) root         (0)     5363 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py
--rw-rw-r--   0 root         (0) root         (0)     6386 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py
--rw-rw-r--   0 root         (0) root         (0)     5674 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py
--rw-rw-r--   0 root         (0) root         (0)     5483 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)     8386 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py
--rw-rw-r--   0 root         (0) root         (0)     5176 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py
--rw-rw-r--   0 root         (0) root         (0)     3813 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py
--rw-rw-r--   0 root         (0) root         (0)     6031 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py
--rw-rw-r--   0 root         (0) root         (0)     4451 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)    17809 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     4404 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py
--rw-rw-r--   0 root         (0) root         (0)     4439 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/
--rw-rw-r--   0 root         (0) root         (0)      440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      532 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14709 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/
--rw-rw-r--   0 root         (0) root         (0)      934 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6176 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)     6794 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     7709 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py
--rw-rw-r--   0 root         (0) root         (0)     6420 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)    10719 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py
--rw-rw-r--   0 root         (0) root         (0)    12416 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py
--rw-rw-r--   0 root         (0) root         (0)     8720 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py
--rw-rw-r--   0 root         (0) root         (0)     8760 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py
--rw-rw-r--   0 root         (0) root         (0)     6918 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py
--rw-rw-r--   0 root         (0) root         (0)     6951 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/
--rw-rw-r--   0 root         (0) root         (0)      591 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7258 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py
--rw-rw-r--   0 root         (0) root         (0)     7038 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.165130 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      524 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4727 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/
--rw-rw-r--   0 root         (0) root         (0)      552 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15925 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     2405 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5983 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py
--rw-rw-r--   0 root         (0) root         (0)    32309 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py
--rw-rw-r--   0 root         (0) root         (0)     7686 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py
--rw-rw-r--   0 root         (0) root         (0)     2614 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)     6684 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1139 2024-03-26 05:41:01.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3843 2024-03-26 05:41:01.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:41:01.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:41:01.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:41:01.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      366 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-dsartifact-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:41:01.169129 accelbyte-py-sdk-service-dsartifact-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      880 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/
+-rw-rw-r--   0 root         (0) root         (0)     1957 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.223721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/
+-rw-rw-r--   0 root         (0) root         (0)     1579 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     7962 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4872 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py
+-rw-rw-r--   0 root         (0) root         (0)     4982 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5674 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py
+-rw-rw-r--   0 root         (0) root         (0)     5483 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     5176 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py
+-rw-rw-r--   0 root         (0) root         (0)     3813 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py
+-rw-rw-r--   0 root         (0) root         (0)     6031 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4451 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)    17809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     4404 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py
+-rw-rw-r--   0 root         (0) root         (0)     4439 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      532 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14974 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/
+-rw-rw-r--   0 root         (0) root         (0)      934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6450 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7072 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     6694 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)    11020 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py
+-rw-rw-r--   0 root         (0) root         (0)    12710 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     8998 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py
+-rw-rw-r--   0 root         (0) root         (0)     9027 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7192 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py
+-rw-rw-r--   0 root         (0) root         (0)     7225 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/
+-rw-rw-r--   0 root         (0) root         (0)      591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py
+-rw-rw-r--   0 root         (0) root         (0)     7364 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      524 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4989 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/
+-rw-rw-r--   0 root         (0) root         (0)      552 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16213 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     2405 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5983 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py
+-rw-rw-r--   0 root         (0) root         (0)    32309 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     7686 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py
+-rw-rw-r--   0 root         (0) root         (0)     2614 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)     6684 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3843 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:26:45.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsartifact-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:26:45.227721 accelbyte_py_sdk_service_dsartifact-0.5.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/PKG-INFO` & `accelbyte_py_sdk_service_dsartifact-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsartifact
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Artifact Manager
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.1
+* Version: 1.11.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/README.md` & `accelbyte_py_sdk_service_dsartifact-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.1
+* Version: 1.11.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # all_terminated_servers
 from .wrappers import list_terminated_servers
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .log_app_message_declaration import LogAppMessageDeclaration
 from .models_all_queue_result import ModelsAllQueueResult
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_all_queue_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_artifact_file_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_all_queue_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_nodes_ip_address.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_queue_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_list_terminated_servers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_match_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_notif_payload_server_status_change.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_queue_result.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_match_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_request_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/models_status_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .list_terminated_servers import ListTerminatedServers
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/all_terminated_servers/list_terminated_servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/servers/search"
+    _path: str = "/dsartifact/servers/search"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     deployment: str  # OPTIONAL in [query]
     game_mode: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     party_id: str  # OPTIONAL in [query]
     pod_name: str  # OPTIONAL in [query]
     previous: str  # OPTIONAL in [query]
@@ -116,14 +120,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_active_queue import DeleteActiveQueue
 from .delete_node_by_id import DeleteNodeByID
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_active_queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,31 +68,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/artifacts/queues/active"
+    _path: str = "/dsartifact/artifacts/queues/active"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     node_ip: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_node_by_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/artifacts/nodes/ipaddresses"
+    _path: str = "/dsartifact/artifacts/nodes/ipaddresses"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     node_ip: str  # REQUIRED in [query]
     pod_name: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/delete_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,33 +73,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/namespaces/{namespace}/artifacts/queues"
+    _path: str = "/dsartifact/namespaces/{namespace}/artifacts/queues"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     namespace: str  # REQUIRED in [path]
     node_ip: str  # REQUIRED in [query]
     pod_name: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/get_active_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,31 +71,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/artifacts/queues/active"
+    _path: str = "/dsartifact/artifacts/queues/active"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     node_ip: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_active_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/namespaces/{namespace}/artifacts/queues/active/all"
+    _path: str = "/dsartifact/namespaces/{namespace}/artifacts/queues/active/all"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     node_ip: str  # OPTIONAL in [query]
     pod_name: str  # OPTIONAL in [query]
     previous: str  # OPTIONAL in [query]
 
@@ -104,14 +108,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_all_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,20 +86,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/namespaces/{namespace}/artifacts/queues/all"
+    _path: str = "/dsartifact/namespaces/{namespace}/artifacts/queues/all"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     namespace: str  # REQUIRED in [path]
     exclude_uploading: bool  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     node_ip: str  # OPTIONAL in [query]
     order: str  # OPTIONAL in [query]
     pod_name: str  # OPTIONAL in [query]
@@ -110,14 +114,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_nodes_ip_address.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,34 +76,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/artifacts/nodes/ipaddresses"
+    _path: str = "/dsartifact/artifacts/nodes/ipaddresses"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     node_ip: str  # OPTIONAL in [query]
     previous: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/list_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,34 +77,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/artifacts/queues"
+    _path: str = "/dsartifact/artifacts/queues"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     previous: str  # OPTIONAL in [query]
     node_ip: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,29 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class ReportFailedUpload(Operation):
-    """Report failed artifact upload (reportFailedUpload)
+class SetActiveQueue(Operation):
+    """Set a queue as active queue (setActiveQueue)
 
     ```
     Required permission: ADMIN:DSAM:ARTIFACT:QUEUE [UPDATE]
 
-    This endpoint is used to report a failed artifact upload
+    This endpoint is used to set a queue entry as the current active queue
+    for artifact uploading process on a node
     ```
 
     Required Permission(s):
         - ADMIN:DSAM:ARTIFACT:QUEUE [UPDATE]
 
     Properties:
-        url: /dsartifact/artifacts/queues/failed
+        url: /dsartifact/artifacts/queues/active
 
         method: PUT
 
         tags: ["Artifact Upload Process Queue"]
 
         consumes: ["application/json"]
 
@@ -69,33 +70,45 @@
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsartifact/artifacts/queues/failed"
+    _url: str = "/dsartifact/artifacts/queues/active"
+    _path: str = "/dsartifact/artifacts/queues/active"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     node_ip: str  # REQUIRED in [query]
     pod_name: str  # REQUIRED in [query]
 
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
 
@@ -136,19 +149,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_node_ip(self, value: str) -> ReportFailedUpload:
+    def with_node_ip(self, value: str) -> SetActiveQueue:
         self.node_ip = value
         return self
 
-    def with_pod_name(self, value: str) -> ReportFailedUpload:
+    def with_pod_name(self, value: str) -> SetActiveQueue:
         self.pod_name = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -209,26 +222,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, node_ip: str, pod_name: str, **kwargs) -> ReportFailedUpload:
+    def create(cls, node_ip: str, pod_name: str, **kwargs) -> SetActiveQueue:
         instance = cls()
         instance.node_ip = node_ip
         instance.pod_name = pod_name
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ReportFailedUpload:
+    ) -> SetActiveQueue:
         instance = cls()
         if "nodeIP" in dict_ and dict_["nodeIP"] is not None:
             instance.node_ip = str(dict_["nodeIP"])
         elif include_empty:
             instance.node_ip = ""
         if "podName" in dict_ and dict_["podName"] is not None:
             instance.pod_name = str(dict_["podName"])
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/set_active_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/artifact_upload_process_queue/report_failed_upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,29 +28,28 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class SetActiveQueue(Operation):
-    """Set a queue as active queue (setActiveQueue)
+class ReportFailedUpload(Operation):
+    """Report failed artifact upload (reportFailedUpload)
 
     ```
     Required permission: ADMIN:DSAM:ARTIFACT:QUEUE [UPDATE]
 
-    This endpoint is used to set a queue entry as the current active queue
-    for artifact uploading process on a node
+    This endpoint is used to report a failed artifact upload
     ```
 
     Required Permission(s):
         - ADMIN:DSAM:ARTIFACT:QUEUE [UPDATE]
 
     Properties:
-        url: /dsartifact/artifacts/queues/active
+        url: /dsartifact/artifacts/queues/failed
 
         method: PUT
 
         tags: ["Artifact Upload Process Queue"]
 
         consumes: ["application/json"]
 
@@ -70,33 +69,45 @@
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsartifact/artifacts/queues/active"
+    _url: str = "/dsartifact/artifacts/queues/failed"
+    _path: str = "/dsartifact/artifacts/queues/failed"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     node_ip: str  # REQUIRED in [query]
     pod_name: str  # REQUIRED in [query]
 
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
 
@@ -137,19 +148,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_node_ip(self, value: str) -> SetActiveQueue:
+    def with_node_ip(self, value: str) -> ReportFailedUpload:
         self.node_ip = value
         return self
 
-    def with_pod_name(self, value: str) -> SetActiveQueue:
+    def with_pod_name(self, value: str) -> ReportFailedUpload:
         self.pod_name = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -210,26 +221,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, node_ip: str, pod_name: str, **kwargs) -> SetActiveQueue:
+    def create(cls, node_ip: str, pod_name: str, **kwargs) -> ReportFailedUpload:
         instance = cls()
         instance.node_ip = node_ip
         instance.pod_name = pod_name
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> SetActiveQueue:
+    ) -> ReportFailedUpload:
         instance = cls()
         if "nodeIP" in dict_ and dict_["nodeIP"] is not None:
             instance.node_ip = str(dict_["nodeIP"])
         elif include_empty:
             instance.node_ip = ""
         if "podName" in dict_ and dict_["podName"] is not None:
             instance.pod_name = str(dict_["podName"])
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .check_server_artifact import CheckServerArtifact
 from .download_server_artifacts import DownloadServerArtifacts
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/check_server_artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,32 +76,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/namespaces/{namespace}/servers/{podName}/artifacts/exists"
+    _path: str = "/dsartifact/namespaces/{namespace}/servers/{podName}/artifacts/exists"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/download_server_artifact/download_server_artifacts.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,32 +73,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsartifact/namespaces/{namespace}/servers/{podName}/artifacts/download"
     )
+    _path: str = (
+        "/dsartifact/namespaces/{namespace}/servers/{podName}/artifacts/download"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_get_messages import PublicGetMessages
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/operations/public_get_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,29 +56,41 @@
 
         500: Internal Server Error - ResponseError
     """
 
     # region fields
 
     _url: str = "/dsartifact/v1/messages"
+    _path: str = "/dsartifact/v1/messages"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .list_terminated_servers_e10383 import ListTerminatedServersWithNamespace
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/operations/terminated_servers/list_terminated_servers_e10383.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,20 +91,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsartifact/namespaces/{namespace}/servers/search"
+    _path: str = "/dsartifact/namespaces/{namespace}/servers/search"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json", "text/x-log"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsartifact"
+
     namespace: str  # REQUIRED in [path]
     deployment: str  # OPTIONAL in [query]
     game_mode: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     next_: str  # OPTIONAL in [query]
     party_id: str  # OPTIONAL in [query]
     pod_name: str  # OPTIONAL in [query]
@@ -119,14 +123,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Ds Artifact Manager."""
 
-__version__ = "1.11.1"
+__version__ = "1.11.3"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._all_terminated_servers import list_terminated_servers
 from ._all_terminated_servers import list_terminated_servers_async
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_all_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_artifact_upload_process_queue.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_download_server_artifact.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk/api/dsartifact/wrappers/_terminated_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsartifact
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Ds Artifact Manager
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Ds Artifact Manager
-* Version: 1.11.1
+* Version: 1.11.3
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-dsartifact-0.4.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_dsartifact-0.5.0/accelbyte_py_sdk_service_dsartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

