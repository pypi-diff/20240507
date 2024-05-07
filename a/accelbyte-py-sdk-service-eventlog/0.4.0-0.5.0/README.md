# Comparing `tmp/accelbyte-py-sdk-service-eventlog-0.4.0.tar.gz` & `tmp/accelbyte_py_sdk_service_eventlog-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-eventlog-0.4.0.tar", last modified: Tue Feb 13 03:09:17 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_eventlog-0.5.0.tar", last modified: Tue May  7 06:27:19 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-eventlog-0.4.0.tar` & `accelbyte_py_sdk_service_eventlog-0.5.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1130 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      875 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.431722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.431722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.431722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/
--rw-rw-r--   0 root         (0) root         (0)     4256 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/
--rw-rw-r--   0 root         (0) root         (0)     1456 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4430 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_agent_type.py
--rw-rw-r--   0 root         (0) root         (0)    12244 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event.py
--rw-rw-r--   0 root         (0) root         (0)     4366 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_id.py
--rw-rw-r--   0 root         (0) root         (0)     4462 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_level.py
--rw-rw-r--   0 root         (0) root         (0)     5652 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_registry.py
--rw-rw-r--   0 root         (0) root         (0)     4932 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4873 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_response_v2.py
--rw-rw-r--   0 root         (0) root         (0)     4430 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_type.py
--rw-rw-r--   0 root         (0) root         (0)     9500 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_v2.py
--rw-rw-r--   0 root         (0) root         (0)     8097 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_generic_query_payload.py
--rw-rw-r--   0 root         (0) root         (0)     4210 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_agent_type.py
--rw-rw-r--   0 root         (0) root         (0)     4132 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_id.py
--rw-rw-r--   0 root         (0) root         (0)     4242 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_level.py
--rw-rw-r--   0 root         (0) root         (0)     4190 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_type.py
--rw-rw-r--   0 root         (0) root         (0)     3835 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_ux.py
--rw-rw-r--   0 root         (0) root         (0)     4403 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     5619 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_paging.py
--rw-rw-r--   0 root         (0) root         (0)     5293 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_user_last_activity.py
--rw-rw-r--   0 root         (0) root         (0)     4179 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_ux.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/
--rw-rw-r--   0 root         (0) root         (0)     1119 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10683 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_id_handler.py
--rw-rw-r--   0 root         (0) root         (0)    11703 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_8d579c.py
--rw-rw-r--   0 root         (0) root         (0)    10760 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_f075bc.py
--rw-rw-r--   0 root         (0) root         (0)     9860 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_namespace_handler.py
--rw-rw-r--   0 root         (0) root         (0)    12527 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_event_af55e0.py
--rw-rw-r--   0 root         (0) root         (0)    11546 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_30e3ad.py
--rw-rw-r--   0 root         (0) root         (0)    11624 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_c0de1a.py
--rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7208 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/post_event_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/
--rw-rw-r--   0 root         (0) root         (0)     1213 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4506 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/agent_type_description_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4481 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_id_description_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4518 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_level_description_9599c9.py
--rw-rw-r--   0 root         (0) root         (0)     4506 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_type_description_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6034 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_agent_type_des_abc470.py
--rw-rw-r--   0 root         (0) root         (0)     5950 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_id_descr_a3e19b.py
--rw-rw-r--   0 root         (0) root         (0)     6075 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_level_de_346d03.py
--rw-rw-r--   0 root         (0) root         (0)     6034 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_type_des_d1ea80.py
--rw-rw-r--   0 root         (0) root         (0)     5687 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_ux_description_86d7b4.py
--rw-rw-r--   0 root         (0) root         (0)     4442 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/ux_name_description_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/
--rw-rw-r--   0 root         (0) root         (0)      887 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6535 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_event_id_f55558.py
--rw-rw-r--   0 root         (0) root         (0)     6665 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_b_671cec.py
--rw-rw-r--   0 root         (0) root         (0)     5247 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6613 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/register_event_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6227 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/unregister_event_id_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7532 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/update_event_registry_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.435722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/
--rw-rw-r--   0 root         (0) root         (0)      727 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11742 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_event_specific_user_585e9a.py
--rw-rw-r--   0 root         (0) root         (0)    11615 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_public_edit_history.py
--rw-rw-r--   0 root         (0) root         (0)    11657 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_user_events_v2_public.py
--rw-rw-r--   0 root         (0) root         (0)    11445 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/query_event_stream_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/
--rw-rw-r--   0 root         (0) root         (0)      680 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7047 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/delete_user_activities_handler.py
--rw-rw-r--   0 root         (0) root         (0)     9044 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/get_user_activities_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7207 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/last_user_activity_time_4f2a6a.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4510 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    35991 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event.py
--rw-rw-r--   0 root         (0) root         (0)    18659 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_descriptions.py
--rw-rw-r--   0 root         (0) root         (0)    16139 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_registry.py
--rw-rw-r--   0 root         (0) root         (0)    17210 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_v2.py
--rw-rw-r--   0 root         (0) root         (0)    10502 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_user_information.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1130 2024-02-13 03:09:17.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5036 2024-02-13 03:09:17.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-13 03:09:17.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-13 03:09:17.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-13 03:09:17.000000 accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      362 2024-02-13 03:05:52.000000 accelbyte-py-sdk-service-eventlog-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-13 03:09:17.439722 accelbyte-py-sdk-service-eventlog-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.526789 accelbyte_py_sdk_service_eventlog-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-07 06:27:19.526789 accelbyte_py_sdk_service_eventlog-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      875 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.518789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.518789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.518789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/
+-rw-rw-r--   0 root         (0) root         (0)     4256 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/
+-rw-rw-r--   0 root         (0) root         (0)     1456 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4430 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_agent_type.py
+-rw-rw-r--   0 root         (0) root         (0)    12244 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event.py
+-rw-rw-r--   0 root         (0) root         (0)     4366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_id.py
+-rw-rw-r--   0 root         (0) root         (0)     4462 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_level.py
+-rw-rw-r--   0 root         (0) root         (0)     5652 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_registry.py
+-rw-rw-r--   0 root         (0) root         (0)     4932 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4873 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_response_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     4430 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_type.py
+-rw-rw-r--   0 root         (0) root         (0)     9500 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_v2.py
+-rw-rw-r--   0 root         (0) root         (0)     8097 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_generic_query_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     4210 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_agent_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4132 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_id.py
+-rw-rw-r--   0 root         (0) root         (0)     4242 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_level.py
+-rw-rw-r--   0 root         (0) root         (0)     4190 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3835 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_ux.py
+-rw-rw-r--   0 root         (0) root         (0)     4403 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     5619 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_paging.py
+-rw-rw-r--   0 root         (0) root         (0)     5293 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_user_last_activity.py
+-rw-rw-r--   0 root         (0) root         (0)     4179 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_ux.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/
+-rw-rw-r--   0 root         (0) root         (0)     1119 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_id_handler.py
+-rw-rw-r--   0 root         (0) root         (0)    12022 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_8d579c.py
+-rw-rw-r--   0 root         (0) root         (0)    11061 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_f075bc.py
+-rw-rw-r--   0 root         (0) root         (0)    10139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_namespace_handler.py
+-rw-rw-r--   0 root         (0) root         (0)    12861 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_event_af55e0.py
+-rw-rw-r--   0 root         (0) root         (0)    11858 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_30e3ad.py
+-rw-rw-r--   0 root         (0) root         (0)    11940 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_c0de1a.py
+-rw-rw-r--   0 root         (0) root         (0)    10890 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7487 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/post_event_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/
+-rw-rw-r--   0 root         (0) root         (0)     1213 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4785 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/agent_type_description_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_id_description_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4798 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_level_description_9599c9.py
+-rw-rw-r--   0 root         (0) root         (0)     4785 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_type_description_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     6330 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_agent_type_des_abc470.py
+-rw-rw-r--   0 root         (0) root         (0)     6242 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_id_descr_a3e19b.py
+-rw-rw-r--   0 root         (0) root         (0)     6373 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_level_de_346d03.py
+-rw-rw-r--   0 root         (0) root         (0)     6330 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_type_des_d1ea80.py
+-rw-rw-r--   0 root         (0) root         (0)     5968 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_ux_description_86d7b4.py
+-rw-rw-r--   0 root         (0) root         (0)     4714 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/ux_name_description_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/
+-rw-rw-r--   0 root         (0) root         (0)      887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6819 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_event_id_f55558.py
+-rw-rw-r--   0 root         (0) root         (0)     6953 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_b_671cec.py
+-rw-rw-r--   0 root         (0) root         (0)     5521 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     6887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/register_event_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     6511 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/unregister_event_id_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/update_event_registry_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/
+-rw-rw-r--   0 root         (0) root         (0)      727 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12038 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_event_specific_user_585e9a.py
+-rw-rw-r--   0 root         (0) root         (0)    11918 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_public_edit_history.py
+-rw-rw-r--   0 root         (0) root         (0)    11954 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_user_events_v2_public.py
+-rw-rw-r--   0 root         (0) root         (0)    11726 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/query_event_stream_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.522789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/
+-rw-rw-r--   0 root         (0) root         (0)      680 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7352 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/delete_user_activities_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     9349 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/get_user_activities_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7518 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/last_user_activity_time_4f2a6a.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.526789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4510 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    35991 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event.py
+-rw-rw-r--   0 root         (0) root         (0)    18659 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_descriptions.py
+-rw-rw-r--   0 root         (0) root         (0)    16139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_registry.py
+-rw-rw-r--   0 root         (0) root         (0)    17210 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_v2.py
+-rw-rw-r--   0 root         (0) root         (0)    10502 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_user_information.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:19.526789 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-07 06:27:19.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5036 2024-05-07 06:27:19.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:19.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:19.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:19.000000 accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      362 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_eventlog-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:19.526789 accelbyte_py_sdk_service_eventlog-0.5.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/PKG-INFO` & `accelbyte_py_sdk_service_eventlog-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-eventlog
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Event Log Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Event Log Service
-* Version: 2.2.3
+* Version: 2.2.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/README.md` & `accelbyte_py_sdk_service_eventlog-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Event Log Service
-* Version: 2.2.3
+* Version: 2.2.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # event
 from .wrappers import get_event_by_event_id_handler
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_agent_type import ModelsAgentType
 from .models_event import ModelsEvent
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_agent_type.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_agent_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_id.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_level.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_level.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_registry.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_registry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_response.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_response_v2.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_response_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_type.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_event_v2.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_event_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_generic_query_payload.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_generic_query_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_agent_type.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_agent_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_id.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_id.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_level.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_level.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_type.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_event_type.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_ux.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_multiple_ux.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_pagination.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_paging.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_paging.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_user_last_activity.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_user_last_activity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/models/models_ux.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/models/models_ux.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_event_by_event_id_handler import GetEventByEventIDHandler
 from .get_event_by_event_type_8d579c import GetEventByEventTypeAndEventIDHandler
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_id_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_id_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByEventIDHandler(Operation):
-    """Get events from all users in a namespace with specific eventID (GetEventByEventIDHandler)
+    """[DEPRECATED] Get events from all users in a namespace with specific eventID (GetEventByEventIDHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]` and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/eventId/{eventId}"
+    _path: str = "/event/namespaces/{namespace}/eventId/{eventId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_8d579c.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_8d579c.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByEventTypeAndEventIDHandler(Operation):
-    """Get events from all users in a namespace with specific eventID and eventType (GetEventByEventTypeAndEventIDHandler)
+    """[DEPRECATED] Get events from all users in a namespace with specific eventID and eventType (GetEventByEventTypeAndEventIDHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -84,20 +84,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/eventType/{eventType}/eventId/{eventId}"
+    _path: str = "/event/namespaces/{namespace}/eventType/{eventType}/eventId/{eventId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: float  # REQUIRED in [path]
     event_type: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
@@ -107,14 +111,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_f075bc.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_event_type_f075bc.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByEventTypeHandler(Operation):
-    """Get events from all users in a namespace with specific eventType (GetEventByEventTypeHandler)
+    """[DEPRECATED] Get events from all users in a namespace with specific eventType (GetEventByEventTypeHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/eventType/{eventType}"
+    _path: str = "/event/namespaces/{namespace}/eventType/{eventType}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_type: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_namespace_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_namespace_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByNamespaceHandler(Operation):
-    """Get events from all users in a namespace (GetEventByNamespaceHandler)
+    """[DEPRECATED] Get events from all users in a namespace (GetEventByNamespaceHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]` and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -80,20 +80,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}"
+    _path: str = "/event/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
 
     # endregion fields
@@ -101,14 +105,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_event_af55e0.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_event_af55e0.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByUserEventIDAndEventTypeHandler(Operation):
-    """Get events from specific user with specific eventID and eventType (GetEventByUserEventIDAndEventTypeHandler)
+    """[DEPRECATED] Get events from specific user with specific eventID and eventType (GetEventByUserEventIDAndEventTypeHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -86,20 +86,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/eventType/{eventType}/eventId/{eventId}"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/eventType/{eventType}/eventId/{eventId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: float  # REQUIRED in [path]
     event_type: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_30e3ad.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_30e3ad.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByUserIDAndEventIDHandler(Operation):
-    """Get events from specific user with specific eventID (GetEventByUserIDAndEventIDHandler)
+    """[DEPRECATED] Get events from specific user with specific eventID (GetEventByUserIDAndEventIDHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]` and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -84,20 +84,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/eventId/{eventId}"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/eventId/{eventId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
@@ -107,14 +111,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_c0de1a.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_an_c0de1a.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByUserIDAndEventTypeHandler(Operation):
-    """Get events from specific user with specific eventType (GetEventByUserIDAndEventTypeHandler)
+    """[DEPRECATED] Get events from specific user with specific eventType (GetEventByUserIDAndEventTypeHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -84,20 +84,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/eventType/{eventType}"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/eventType/{eventType}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_type: float  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
@@ -107,14 +111,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/get_event_by_user_id_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetEventByUserIDHandler(Operation):
-    """Get events from specific user (GetEventByUserIDHandler)
+    """[DEPRECATED] Get events from specific user (GetEventByUserIDHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]` and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     end_date: str  # REQUIRED in [query]
     page_size: int  # REQUIRED in [query]
     start_date: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event/post_event_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event/post_event_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEvent
 
 
 class PostEventHandler(Operation):
-    """Post an activity log (PostEventHandler)
+    """[DEPRECATED] Post an activity log (PostEventHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [CREATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [CREATE]
 
     Required Scope(s):
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}"
+    _path: str = "/event/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     body: ModelsEvent  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .agent_type_description_handler import AgentTypeDescriptionHandler
 from .event_id_description_handler import EventIDDescriptionHandler
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/agent_type_description_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/agent_type_description_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleAgentType
 
 
 class AgentTypeDescriptionHandler(Operation):
-    """Get list of agent type and the descriptions (AgentTypeDescriptionHandler)
+    """[DEPRECATED] Get list of agent type and the descriptions (AgentTypeDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/agentType
 
         method: GET
 
@@ -53,29 +53,41 @@
     Responses:
         200: OK - ModelsMultipleAgentType (OK)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/agentType"
+    _path: str = "/event/descriptions/agentType"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_id_description_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_id_description_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleEventID
 
 
 class EventIDDescriptionHandler(Operation):
-    """Get list of eventID and the descriptions (EventIDDescriptionHandler)
+    """[DEPRECATED] Get list of eventID and the descriptions (EventIDDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/eventId
 
         method: GET
 
@@ -53,29 +53,41 @@
     Responses:
         200: OK - ModelsMultipleEventID (OK)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/eventId"
+    _path: str = "/event/descriptions/eventId"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_level_description_9599c9.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_level_description_9599c9.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleEventLevel
 
 
 class EventLevelDescriptionHandler(Operation):
-    """Get list of event level and the descriptions (EventLevelDescriptionHandler)
+    """[DEPRECATED] Get list of event level and the descriptions (EventLevelDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/eventLevel
 
         method: GET
 
@@ -53,29 +53,41 @@
     Responses:
         200: OK - ModelsMultipleEventLevel (OK)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/eventLevel"
+    _path: str = "/event/descriptions/eventLevel"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_type_description_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/ux_name_description_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,56 +26,68 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
-from ...models import ModelsMultipleEventType
+from ...models import ModelsMultipleUX
 
 
-class EventTypeDescriptionHandler(Operation):
-    """Get list of event type and the descriptions (EventTypeDescriptionHandler)
+class UXNameDescriptionHandler(Operation):
+    """[DEPRECATED] Get list of ux name and the descriptions (UXNameDescriptionHandler)
 
 
     Properties:
-        url: /event/descriptions/eventType
+        url: /event/descriptions/ux
 
         method: GET
 
         tags: ["Event Descriptions"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - ModelsMultipleEventType (OK)
+        200: OK - ModelsMultipleUX (OK)
     """
 
     # region fields
 
-    _url: str = "/event/descriptions/eventType"
+    _url: str = "/event/descriptions/ux"
+    _path: str = "/event/descriptions/ux"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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
 
@@ -121,18 +133,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, ModelsMultipleEventType], Union[None, HttpResponse]]:
+    ) -> Tuple[Union[None, ModelsMultipleUX], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - ModelsMultipleEventType (OK)
+        200: OK - ModelsMultipleUX (OK)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -140,35 +152,35 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsMultipleEventType.create_from_dict(content), None
+            return ModelsMultipleUX.create_from_dict(content), None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> EventTypeDescriptionHandler:
+    def create(cls, **kwargs) -> UXNameDescriptionHandler:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> EventTypeDescriptionHandler:
+    ) -> UXNameDescriptionHandler:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_agent_type_des_abc470.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_agent_type_des_abc470.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleAgentType
 
 
 class SpecificAgentTypeDescriptionHandler(Operation):
-    """Get specific list of agent type and the descriptions by comma separated value of agent types (SpecificAgentTypeDescriptionHandler)
+    """[DEPRECATED] Get specific list of agent type and the descriptions by comma separated value of agent types (SpecificAgentTypeDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/agentType/listByAgentTypes
 
         method: GET
 
@@ -59,31 +59,43 @@
 
         404: Not Found - (Not Found)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/agentType/listByAgentTypes"
+    _path: str = "/event/descriptions/agentType/listByAgentTypes"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     agent_types: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_id_descr_a3e19b.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_id_descr_a3e19b.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleEventID
 
 
 class SpecificEventIDDescriptionHandler(Operation):
-    """Get specific list of eventID and the descriptions by comma separated value of eventIDs (SpecificEventIDDescriptionHandler)
+    """[DEPRECATED] Get specific list of eventID and the descriptions by comma separated value of eventIDs (SpecificEventIDDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/eventId/listByEventIds
 
         method: GET
 
@@ -59,31 +59,43 @@
 
         404: Not Found - (Not Found)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/eventId/listByEventIds"
+    _path: str = "/event/descriptions/eventId/listByEventIds"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_ids: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_level_de_346d03.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_level_de_346d03.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleEventLevel
 
 
 class SpecificEventLevelDescriptionHandler(Operation):
-    """Get specific list of event level and the descriptions by comma separated value of event levels (SpecificEventLevelDescriptionHandler)
+    """[DEPRECATED] Get specific list of event level and the descriptions by comma separated value of event levels (SpecificEventLevelDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/eventLevel/listByEventLevels
 
         method: GET
 
@@ -59,31 +59,43 @@
 
         404: Not Found - (Not Found)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/eventLevel/listByEventLevels"
+    _path: str = "/event/descriptions/eventLevel/listByEventLevels"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_levels: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_type_des_d1ea80.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_event_type_des_d1ea80.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleEventType
 
 
 class SpecificEventTypeDescriptionHandler(Operation):
-    """Get specific list of event type and the descriptions by comma separated value of event types (SpecificEventTypeDescriptionHandler)
+    """[DEPRECATED] Get specific list of event type and the descriptions by comma separated value of event types (SpecificEventTypeDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/eventType/listByEventTypes
 
         method: GET
 
@@ -59,31 +59,43 @@
 
         404: Not Found - (Not Found)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/eventType/listByEventTypes"
+    _path: str = "/event/descriptions/eventType/listByEventTypes"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_types: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_ux_description_86d7b4.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/specific_ux_description_86d7b4.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsMultipleUX
 
 
 class SpecificUXDescriptionHandler(Operation):
-    """Get specific list of UX and the descriptions by comma separated value of UX (SpecificUXDescriptionHandler)
+    """[DEPRECATED] Get specific list of UX and the descriptions by comma separated value of UX (SpecificUXDescriptionHandler)
 
 
     Properties:
         url: /event/descriptions/ux/listByUx
 
         method: GET
 
@@ -59,31 +59,43 @@
 
         404: Not Found - (Not Found)
     """
 
     # region fields
 
     _url: str = "/event/descriptions/ux/listByUx"
+    _path: str = "/event/descriptions/ux/listByUx"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     ux: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/ux_name_description_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_descriptions/event_type_description_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,56 +26,68 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
-from ...models import ModelsMultipleUX
+from ...models import ModelsMultipleEventType
 
 
-class UXNameDescriptionHandler(Operation):
-    """Get list of ux name and the descriptions (UXNameDescriptionHandler)
+class EventTypeDescriptionHandler(Operation):
+    """[DEPRECATED] Get list of event type and the descriptions (EventTypeDescriptionHandler)
 
 
     Properties:
-        url: /event/descriptions/ux
+        url: /event/descriptions/eventType
 
         method: GET
 
         tags: ["Event Descriptions"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - ModelsMultipleUX (OK)
+        200: OK - ModelsMultipleEventType (OK)
     """
 
     # region fields
 
-    _url: str = "/event/descriptions/ux"
+    _url: str = "/event/descriptions/eventType"
+    _path: str = "/event/descriptions/eventType"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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
 
@@ -121,18 +133,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, ModelsMultipleUX], Union[None, HttpResponse]]:
+    ) -> Tuple[Union[None, ModelsMultipleEventType], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - ModelsMultipleUX (OK)
+        200: OK - ModelsMultipleEventType (OK)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -140,35 +152,35 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsMultipleUX.create_from_dict(content), None
+            return ModelsMultipleEventType.create_from_dict(content), None
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> UXNameDescriptionHandler:
+    def create(cls, **kwargs) -> EventTypeDescriptionHandler:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UXNameDescriptionHandler:
+    ) -> EventTypeDescriptionHandler:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_registered_event_id_f55558 import GetRegisteredEventIDHandler
 from .get_registered_events_b_671cec import GetRegisteredEventsByEventTypeHandler
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_event_id_f55558.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/unregister_event_id_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,77 +26,85 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
-from ...models import ModelsEventRegistry
 
+class UnregisterEventIDHandler(Operation):
+    """[DEPRECATED] Unregister eventID from the Event Registry (UnregisterEventIDHandler)
 
-class GetRegisteredEventIDHandler(Operation):
-    """Get registered eventID data from the Event Registry (GetRegisteredEventIDHandler)
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [READ]`and scope `analytics`
+    Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [DELETE]`and scope `analytics`
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EVENT [READ]
+        - ADMIN:NAMESPACE:{namespace}:EVENT [DELETE]
 
     Required Scope(s):
         - analytics
 
     Properties:
         url: /event/registry/eventIds/{eventId}
 
-        method: GET
+        method: DELETE
 
         tags: ["Event Registry"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         event_id: (eventId) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsEventRegistry (OK)
-
-        400: Bad Request - (Bad Request)
+        204: No Content - (No Content)
 
         401: Unauthorized - (Unauthorized)
 
         403: Forbidden - (Forbidden)
 
         404: Not Found - (Not Found)
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventIds/{eventId}"
-    _method: str = "GET"
+    _path: str = "/event/registry/eventIds/{eventId}"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: str  # REQUIRED in [path]
 
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
 
@@ -135,15 +143,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_event_id(self, value: str) -> GetRegisteredEventIDHandler:
+    def with_event_id(self, value: str) -> UnregisterEventIDHandler:
         self.event_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -158,20 +166,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, ModelsEventRegistry], Union[None, HttpResponse]]:
+    ) -> Tuple[None, Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - ModelsEventRegistry (OK)
-
-        400: Bad Request - (Bad Request)
+        204: No Content - (No Content)
 
         401: Unauthorized - (Unauthorized)
 
         403: Forbidden - (Forbidden)
 
         404: Not Found - (Not Found)
 
@@ -186,18 +192,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsEventRegistry.create_from_dict(content), None
-        if code == 400:
-            return None, HttpResponse.create(code, "Bad Request")
+        if code == 204:
+            return None, None
         if code == 401:
             return None, HttpResponse.create(code, "Unauthorized")
         if code == 403:
             return None, HttpResponse.create(code, "Forbidden")
         if code == 404:
             return None, HttpResponse.create(code, "Not Found")
         if code == 500:
@@ -208,25 +212,25 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, event_id: str, **kwargs) -> GetRegisteredEventIDHandler:
+    def create(cls, event_id: str, **kwargs) -> UnregisterEventIDHandler:
         instance = cls()
         instance.event_id = event_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> GetRegisteredEventIDHandler:
+    ) -> UnregisterEventIDHandler:
         instance = cls()
         if "eventId" in dict_ and dict_["eventId"] is not None:
             instance.event_id = str(dict_["eventId"])
         elif include_empty:
             instance.event_id = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_b_671cec.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_b_671cec.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventRegistry
 
 
 class GetRegisteredEventsByEventTypeHandler(Operation):
-    """Get registered eventID data from the Event Registry based on the event type (GetRegisteredEventsByEventTypeHandler)
+    """[DEPRECATED] Get registered eventID data from the Event Registry based on the event type (GetRegisteredEventsByEventTypeHandler)
 
     Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [READ]`and scope `analytics`
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:EVENT [READ]
 
     Required Scope(s):
@@ -72,31 +72,43 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventTypes/{eventType}"
+    _path: str = "/event/registry/eventTypes/{eventType}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_type: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_events_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventRegistry
 
 
 class GetRegisteredEventsHandler(Operation):
-    """Get registered events in the Event Registry (GetRegisteredEventsHandler)
+    """[DEPRECATED] Get registered events in the Event Registry (GetRegisteredEventsHandler)
 
     Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [READ]`and scope `analytics`
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:EVENT [READ]
 
     Required Scope(s):
@@ -66,29 +66,41 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventIds"
+    _path: str = "/event/registry/eventIds"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/register_event_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/register_event_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventRegistry
 
 
 class RegisterEventHandler(Operation):
-    """Register an eventID to the Event Registry (RegisterEventHandler)
+    """[DEPRECATED] Register an eventID to the Event Registry (RegisterEventHandler)
 
     Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [CREATE]`and scope `analytics`
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:EVENT [CREATE]
 
     Required Scope(s):
@@ -72,31 +72,43 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventIds"
+    _path: str = "/event/registry/eventIds"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     body: ModelsEventRegistry  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/unregister_event_id_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/get_registered_event_id_f55558.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,73 +26,89 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
+from ...models import ModelsEventRegistry
 
-class UnregisterEventIDHandler(Operation):
-    """Unregister eventID from the Event Registry (UnregisterEventIDHandler)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [DELETE]`and scope `analytics`
+class GetRegisteredEventIDHandler(Operation):
+    """[DEPRECATED] Get registered eventID data from the Event Registry (GetRegisteredEventIDHandler)
+
+    Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [READ]`and scope `analytics`
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EVENT [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:EVENT [READ]
 
     Required Scope(s):
         - analytics
 
     Properties:
         url: /event/registry/eventIds/{eventId}
 
-        method: DELETE
+        method: GET
 
         tags: ["Event Registry"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         event_id: (eventId) REQUIRED str in path
 
     Responses:
-        204: No Content - (No Content)
+        200: OK - ModelsEventRegistry (OK)
+
+        400: Bad Request - (Bad Request)
 
         401: Unauthorized - (Unauthorized)
 
         403: Forbidden - (Forbidden)
 
         404: Not Found - (Not Found)
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventIds/{eventId}"
-    _method: str = "DELETE"
+    _path: str = "/event/registry/eventIds/{eventId}"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     event_id: str  # REQUIRED in [path]
 
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
 
@@ -131,15 +147,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_event_id(self, value: str) -> UnregisterEventIDHandler:
+    def with_event_id(self, value: str) -> GetRegisteredEventIDHandler:
         self.event_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -154,18 +170,20 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse]]:
+    ) -> Tuple[Union[None, ModelsEventRegistry], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        204: No Content - (No Content)
+        200: OK - ModelsEventRegistry (OK)
+
+        400: Bad Request - (Bad Request)
 
         401: Unauthorized - (Unauthorized)
 
         403: Forbidden - (Forbidden)
 
         404: Not Found - (Not Found)
 
@@ -180,16 +198,18 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ModelsEventRegistry.create_from_dict(content), None
+        if code == 400:
+            return None, HttpResponse.create(code, "Bad Request")
         if code == 401:
             return None, HttpResponse.create(code, "Unauthorized")
         if code == 403:
             return None, HttpResponse.create(code, "Forbidden")
         if code == 404:
             return None, HttpResponse.create(code, "Not Found")
         if code == 500:
@@ -200,25 +220,25 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, event_id: str, **kwargs) -> UnregisterEventIDHandler:
+    def create(cls, event_id: str, **kwargs) -> GetRegisteredEventIDHandler:
         instance = cls()
         instance.event_id = event_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UnregisterEventIDHandler:
+    ) -> GetRegisteredEventIDHandler:
         instance = cls()
         if "eventId" in dict_ and dict_["eventId"] is not None:
             instance.event_id = str(dict_["eventId"])
         elif include_empty:
             instance.event_id = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/update_event_registry_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_registry/update_event_registry_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventRegistry
 
 
 class UpdateEventRegistryHandler(Operation):
-    """Update an eventID data in the Event Registry (UpdateEventRegistryHandler)
+    """[DEPRECATED] Update an eventID data in the Event Registry (UpdateEventRegistryHandler)
 
     Required permission `ADMIN:NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/registry/eventIds/{eventId}"
+    _path: str = "/event/registry/eventIds/{eventId}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     body: ModelsEventRegistry  # REQUIRED in [body]
     event_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get_event_specific_user_585e9a import GetEventSpecificUserV2Handler
 from .get_public_edit_history import GetPublicEditHistory
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_event_specific_user_585e9a.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_event_specific_user_585e9a.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,24 @@
 
         501: Not Implemented - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/v2/admin/namespaces/{namespace}/users/{userId}/event"
+    _path: str = "/event/v2/admin/namespaces/{namespace}/users/{userId}/event"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     end_date: str  # OPTIONAL in [query]
     event_name: str  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     page_size: int  # OPTIONAL in [query]
     start_date: str  # OPTIONAL in [query]
@@ -102,14 +106,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_public_edit_history.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_public_edit_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,24 @@
 
         501: Not Implemented - (Not Implemented)
     """
 
     # region fields
 
     _url: str = "/event/v2/public/namespaces/{namespace}/users/{userId}/edithistory"
+    _path: str = "/event/v2/public/namespaces/{namespace}/users/{userId}/edithistory"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     end_date: str  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     page_size: int  # OPTIONAL in [query]
     start_date: str  # OPTIONAL in [query]
     type_: str  # OPTIONAL in [query]
@@ -108,14 +112,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_user_events_v2_public.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/get_user_events_v2_public.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,24 @@
 
         501: Not Implemented - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/v2/public/namespaces/{namespace}/users/{userId}/event"
+    _path: str = "/event/v2/public/namespaces/{namespace}/users/{userId}/event"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     end_date: str  # OPTIONAL in [query]
     event_name: str  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     page_size: int  # OPTIONAL in [query]
     start_date: str  # OPTIONAL in [query]
@@ -102,14 +106,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/query_event_stream_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/event_v2/query_event_stream_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,24 @@
 
         501: Not Implemented - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/v2/admin/namespaces/{namespace}/query"
+    _path: str = "/event/v2/admin/namespaces/{namespace}/query"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     body: ModelsGenericQueryPayload  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     end_date: str  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     page_size: int  # OPTIONAL in [query]
     start_date: str  # OPTIONAL in [query]
 
@@ -102,14 +106,22 @@
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_user_activities_handler import DeleteUserActivitiesHandler
 from .get_user_activities_handler import GetUserActivitiesHandler
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/delete_user_activities_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/delete_user_activities_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 
 class DeleteUserActivitiesHandler(Operation):
-    """Delete all user's activities (DeleteUserActivitiesHandler)
+    """[DEPRECATED] Delete all user's activities (DeleteUserActivitiesHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/activities"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/activities"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/get_user_activities_handler.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/get_user_activities_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsEventResponse
 
 
 class GetUserActivitiesHandler(Operation):
-    """Get all user's activities (GetUserActivitiesHandler)
+    """[DEPRECATED] Get all user's activities (GetUserActivitiesHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -78,34 +78,46 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/activities"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/activities"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     offset: int  # OPTIONAL in [query]
     page_size: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/operations/user_information/last_user_activity_time_4f2a6a.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/operations/user_information/last_user_activity_time_4f2a6a.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from accelbyte_py_sdk.core import HttpResponse
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsUserLastActivity
 
 
 class LastUserActivityTimeHandler(Operation):
-    """Get last activity time of a user in a namespace (LastUserActivityTimeHandler)
+    """[DEPRECATED] Get last activity time of a user in a namespace (LastUserActivityTimeHandler)
 
     Required permission `NAMESPACE:{namespace}:EVENT [UPDATE]`and scope `analytics`
 
     Required Permission(s):
         - NAMESPACE:{namespace}:EVENT [UPDATE]
 
     Required Scope(s):
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/event/namespaces/{namespace}/users/{userId}/lastActivityTime"
+    _path: str = "/event/namespaces/{namespace}/users/{userId}/lastActivityTime"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "eventlog"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/__init__.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Event Log Service."""
 
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._event import get_event_by_event_id_handler
 from ._event import get_event_by_event_id_handler_async
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_descriptions.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_descriptions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_registry.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_registry.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_v2.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_event_v2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk/api/eventlog/wrappers/_user_information.py` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk/api/eventlog/wrappers/_user_information.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-eventlog
-Version: 0.4.0
+Version: 0.5.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Event Log Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Event Log Service
-* Version: 2.2.3
+* Version: 2.2.4
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-eventlog-0.4.0/accelbyte_py_sdk_service_eventlog.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_eventlog-0.5.0/accelbyte_py_sdk_service_eventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

