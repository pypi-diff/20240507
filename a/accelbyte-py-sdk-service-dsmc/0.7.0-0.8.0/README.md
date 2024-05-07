# Comparing `tmp/accelbyte-py-sdk-service-dsmc-0.7.0.tar.gz` & `tmp/accelbyte_py_sdk_service_dsmc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-dsmc-0.7.0.tar", last modified: Tue Feb 27 05:36:47 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_dsmc-0.8.0.tar", last modified: Tue May  7 06:27:08 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-dsmc-0.7.0.tar` & `accelbyte_py_sdk_service_dsmc-0.8.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.444120 accelbyte-py-sdk-service-dsmc-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-27 05:36:47.444120 accelbyte-py-sdk-service-dsmc-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      876 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.424120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.424120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.428120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/
--rw-rw-r--   0 root         (0) root         (0)     7642 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.432120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/
--rw-rw-r--   0 root         (0) root         (0)     4922 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7058 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     5139 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_allocation_event.py
--rw-rw-r--   0 root         (0) root         (0)     3887 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_claim_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     3785 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_count_server_response.py
--rw-rw-r--   0 root         (0) root         (0)     3796 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_count_session_response.py
--rw-rw-r--   0 root         (0) root         (0)    14432 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_override_request.py
--rw-rw-r--   0 root         (0) root         (0)    16506 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_request.py
--rw-rw-r--   0 root         (0) root         (0)    10000 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_dsm_config_request.py
--rw-rw-r--   0 root         (0) root         (0)    11398 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_patch_request.py
--rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_request.py
--rw-rw-r--   0 root         (0) root         (0)     5197 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_pod_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     3743 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_port_request.py
--rw-rw-r--   0 root         (0) root         (0)     7773 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_region_override_request.py
--rw-rw-r--   0 root         (0) root         (0)     4619 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_repository_request.py
--rw-rw-r--   0 root         (0) root         (0)    11587 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_session_request.py
--rw-rw-r--   0 root         (0) root         (0)     3902 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_default_provider.py
--rw-rw-r--   0 root         (0) root         (0)    14825 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_config_override.py
--rw-rw-r--   0 root         (0) root         (0)    19828 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_with_override.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deregister_local_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     6357 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_detailed_count_server_response.py
--rw-rw-r--   0 root         (0) root         (0)     3828 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_ds_heartbeat_request.py
--rw-rw-r--   0 root         (0) root         (0)    12670 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_dsm_config_record.py
--rw-rw-r--   0 root         (0) root         (0)     4073 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_detail_response.py
--rw-rw-r--   0 root         (0) root         (0)     4228 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response.py
--rw-rw-r--   0 root         (0) root         (0)     7434 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response_data.py
--rw-rw-r--   0 root         (0) root         (0)     4203 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_patch_detail_response.py
--rw-rw-r--   0 root         (0) root         (0)    14471 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_record.py
--rw-rw-r--   0 root         (0) root         (0)     9796 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_record_update.py
--rw-rw-r--   0 root         (0) root         (0)     5668 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_replication.py
--rw-rw-r--   0 root         (0) root         (0)     4571 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_import_response.py
--rw-rw-r--   0 root         (0) root         (0)     4191 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_instance_spec.py
--rw-rw-r--   0 root         (0) root         (0)     4211 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     5340 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_deployment_response.py
--rw-rw-r--   0 root         (0) root         (0)     4265 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_patches_response.py
--rw-rw-r--   0 root         (0) root         (0)     5025 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_response.py
--rw-rw-r--   0 root         (0) root         (0)     5242 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_pod_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     5100 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_server_response.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     3994 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_match_result_notification_payload.py
--rw-rw-r--   0 root         (0) root         (0)     4326 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_paging_cursor.py
--rw-rw-r--   0 root         (0) root         (0)    16103 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_patch_image_record.py
--rw-rw-r--   0 root         (0) root         (0)     8464 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_pod_config_record.py
--rw-rw-r--   0 root         (0) root         (0)     8274 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_pod_count_config_override.py
--rw-rw-r--   0 root         (0) root         (0)     5788 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_register_local_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     4695 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_register_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     6640 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_repository_record.py
--rw-rw-r--   0 root         (0) root         (0)     3816 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_member.py
--rw-rw-r--   0 root         (0) root         (0)     6034 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_party.py
--rw-rw-r--   0 root         (0) root         (0)     4454 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_matching_ally.py
--rw-rw-r--   0 root         (0) root         (0)    24972 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server_deployment_config_session_timeout_response.py
--rw-rw-r--   0 root         (0) root         (0)     3909 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     6354 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_session.py
--rw-rw-r--   0 root         (0) root         (0)     4017 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_session_response.py
--rw-rw-r--   0 root         (0) root         (0)     4527 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_shutdown_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     4407 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_status_history.py
--rw-rw-r--   0 root         (0) root         (0)    11915 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_override_request.py
--rw-rw-r--   0 root         (0) root         (0)    13661 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_request.py
--rw-rw-r--   0 root         (0) root         (0)     9283 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_dsm_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     5770 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_pod_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     4311 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_port_request.py
--rw-rw-r--   0 root         (0) root         (0)     7773 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_region_override_request.py
--rw-rw-r--   0 root         (0) root         (0)     4442 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.432120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/
--rw-rw-r--   0 root         (0) root         (0)      442 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.432120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/
--rw-rw-r--   0 root         (0) root         (0)      896 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6245 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server.py
--rw-rw-r--   0 root         (0) root         (0)     7302 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server_detailed.py
--rw-rw-r--   0 root         (0) root         (0)     7161 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_session.py
--rw-rw-r--   0 root         (0) root         (0)     6832 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_local_server.py
--rw-rw-r--   0 root         (0) root         (0)     7047 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_server.py
--rw-rw-r--   0 root         (0) root         (0)     6919 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_session.py
--rw-rw-r--   0 root         (0) root         (0)     7092 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/get_server.py
--rw-rw-r--   0 root         (0) root         (0)     6284 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_local_server.py
--rw-rw-r--   0 root         (0) root         (0)     8616 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_server.py
--rw-rw-r--   0 root         (0) root         (0)     9527 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.436120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/
--rw-rw-r--   0 root         (0) root         (0)      929 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/add_port.py
--rw-rw-r--   0 root         (0) root         (0)     6004 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/clear_cache.py
--rw-rw-r--   0 root         (0) root         (0)     8726 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/create_config.py
--rw-rw-r--   0 root         (0) root         (0)     6502 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_config.py
--rw-rw-r--   0 root         (0) root         (0)     7285 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_port.py
--rw-rw-r--   0 root         (0) root         (0)     6545 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/export_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6391 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/get_config.py
--rw-rw-r--   0 root         (0) root         (0)     7872 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/import_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5203 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/list_config.py
--rw-rw-r--   0 root         (0) root         (0)     8391 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/save_config.py
--rw-rw-r--   0 root         (0) root         (0)     8856 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/update_config.py
--rw-rw-r--   0 root         (0) root         (0)     8419 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/update_port.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.436120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/
--rw-rw-r--   0 root         (0) root         (0)     1506 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8807 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     8820 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_client.py
--rw-rw-r--   0 root         (0) root         (0)    10004 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_override.py
--rw-rw-r--   0 root         (0) root         (0)    10832 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_override_region__89178f.py
--rw-rw-r--   0 root         (0) root         (0)     9975 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_root_region_override.py
--rw-rw-r--   0 root         (0) root         (0)     7367 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     7388 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_client.py
--rw-rw-r--   0 root         (0) root         (0)     8488 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_override.py
--rw-rw-r--   0 root         (0) root         (0)     9349 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_override_region__2e7e2d.py
--rw-rw-r--   0 root         (0) root         (0)     8502 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_root_region_override.py
--rw-rw-r--   0 root         (0) root         (0)     8831 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     8866 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment_client.py
--rw-rw-r--   0 root         (0) root         (0)     7536 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     9020 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment.py
--rw-rw-r--   0 root         (0) root         (0)     9757 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment_override.py
--rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_override_region__fb90bf.py
--rw-rw-r--   0 root         (0) root         (0)     9739 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_root_region_override.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.436120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/
--rw-rw-r--   0 root         (0) root         (0)      526 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4841 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.436120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/
--rw-rw-r--   0 root         (0) root         (0)     1498 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6794 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image.py
--rw-rw-r--   0 root         (0) root         (0)     7013 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image_patch.py
--rw-rw-r--   0 root         (0) root         (0)     6583 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_repository.py
--rw-rw-r--   0 root         (0) root         (0)     8448 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image.py
--rw-rw-r--   0 root         (0) root         (0)     9309 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image_patch.py
--rw-rw-r--   0 root         (0) root         (0)     6675 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/export_images.py
--rw-rw-r--   0 root         (0) root         (0)     7230 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_detail.py
--rw-rw-r--   0 root         (0) root         (0)     6441 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_limit.py
--rw-rw-r--   0 root         (0) root         (0)     8240 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patch_detail.py
--rw-rw-r--   0 root         (0) root         (0)     7084 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patches.py
--rw-rw-r--   0 root         (0) root         (0)     6471 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_repository.py
--rw-rw-r--   0 root         (0) root         (0)     7231 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_detail_client.py
--rw-rw-r--   0 root         (0) root         (0)     6525 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_limit_client.py
--rw-rw-r--   0 root         (0) root         (0)     6870 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/import_images.py
--rw-rw-r--   0 root         (0) root         (0)    11117 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images.py
--rw-rw-r--   0 root         (0) root         (0)    11339 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images_client.py
--rw-rw-r--   0 root         (0) root         (0)     6568 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/update_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/
--rw-rw-r--   0 root         (0) root         (0)      946 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8522 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config.py
--rw-rw-r--   0 root         (0) root         (0)     8551 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config_client.py
--rw-rw-r--   0 root         (0) root         (0)     7407 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config.py
--rw-rw-r--   0 root         (0) root         (0)     7430 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config_client.py
--rw-rw-r--   0 root         (0) root         (0)     8038 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config.py
--rw-rw-r--   0 root         (0) root         (0)     8067 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config_client.py
--rw-rw-r--   0 root         (0) root         (0)     5296 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_lowest_instance_spec.py
--rw-rw-r--   0 root         (0) root         (0)     7275 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_pod_config.py
--rw-rw-r--   0 root         (0) root         (0)     8757 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/update_pod_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/
--rw-rw-r--   0 root         (0) root         (0)      630 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4524 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/get_default_provider.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers.py
--rw-rw-r--   0 root         (0) root         (0)     5334 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers_by_region.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/
--rw-rw-r--   0 root         (0) root         (0)      885 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7650 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/deregister_local_server.py
--rw-rw-r--   0 root         (0) root         (0)     7582 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session.py
--rw-rw-r--   0 root         (0) root         (0)     8014 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session_timeout.py
--rw-rw-r--   0 root         (0) root         (0)     8666 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/list_server_client.py
--rw-rw-r--   0 root         (0) root         (0)     8325 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/register_local_server.py
--rw-rw-r--   0 root         (0) root         (0)     8226 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/register_server.py
--rw-rw-r--   0 root         (0) root         (0)     8026 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/server_heartbeat.py
--rw-rw-r--   0 root         (0) root         (0)     7792 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/shutdown_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/
--rw-rw-r--   0 root         (0) root         (0)      633 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7522 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/cancel_session.py
--rw-rw-r--   0 root         (0) root         (0)     8177 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/claim_server.py
--rw-rw-r--   0 root         (0) root         (0)     8788 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/create_session.py
--rw-rw-r--   0 root         (0) root         (0)     7488 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/get_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     8025 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31852 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_admin.py
--rw-rw-r--   0 root         (0) root         (0)    45080 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_config.py
--rw-rw-r--   0 root         (0) root         (0)    65317 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_deployment_config.py
--rw-rw-r--   0 root         (0) root         (0)     2747 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_dsmc_operations.py
--rw-rw-r--   0 root         (0) root         (0)    56682 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_image_config.py
--rw-rw-r--   0 root         (0) root         (0)    30179 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_pod_config.py
--rw-rw-r--   0 root         (0) root         (0)     5673 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_public.py
--rw-rw-r--   0 root         (0) root         (0)    30981 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_server.py
--rw-rw-r--   0 root         (0) root         (0)    16585 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:36:47.440120 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-27 05:36:47.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11242 2024-02-27 05:36:47.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:36:47.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:36:47.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:36:47.000000 accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-dsmc-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:36:47.444120 accelbyte-py-sdk-service-dsmc-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.007104 accelbyte_py_sdk_service_dsmc-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:27:08.007104 accelbyte_py_sdk_service_dsmc-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.991105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.991105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.991105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/
+-rw-rw-r--   0 root         (0) root         (0)     7642 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.995105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/
+-rw-rw-r--   0 root         (0) root         (0)     4922 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7058 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     5139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_allocation_event.py
+-rw-rw-r--   0 root         (0) root         (0)     3887 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_claim_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3785 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_count_server_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3796 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_count_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_override_request.py
+-rw-rw-r--   0 root         (0) root         (0)    16506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10000 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_dsm_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11398 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_patch_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9794 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5197 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_pod_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3743 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_port_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7773 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_region_override_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4619 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_repository_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11587 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_session_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3902 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_default_provider.py
+-rw-rw-r--   0 root         (0) root         (0)    14825 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_config_override.py
+-rw-rw-r--   0 root         (0) root         (0)    19828 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_with_override.py
+-rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deregister_local_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6357 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_detailed_count_server_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3828 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_ds_heartbeat_request.py
+-rw-rw-r--   0 root         (0) root         (0)    12670 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_dsm_config_record.py
+-rw-rw-r--   0 root         (0) root         (0)     4073 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_detail_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4228 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7434 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4203 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_patch_detail_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14471 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_record.py
+-rw-rw-r--   0 root         (0) root         (0)     9796 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_record_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5668 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_replication.py
+-rw-rw-r--   0 root         (0) root         (0)     4571 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_import_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4191 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_instance_spec.py
+-rw-rw-r--   0 root         (0) root         (0)     4211 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5340 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_deployment_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4265 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_patches_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5025 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5242 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_pod_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5100 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_server_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3994 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_match_result_notification_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     4326 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_paging_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)    16103 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_patch_image_record.py
+-rw-rw-r--   0 root         (0) root         (0)     8464 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_pod_config_record.py
+-rw-rw-r--   0 root         (0) root         (0)     8274 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_pod_count_config_override.py
+-rw-rw-r--   0 root         (0) root         (0)     5788 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_register_local_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4695 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_register_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6640 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_repository_record.py
+-rw-rw-r--   0 root         (0) root         (0)     3816 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_member.py
+-rw-rw-r--   0 root         (0) root         (0)     6034 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4454 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_matching_ally.py
+-rw-rw-r--   0 root         (0) root         (0)    24972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server_deployment_config_session_timeout_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3909 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_session.py
+-rw-rw-r--   0 root         (0) root         (0)     4017 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_session_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4527 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_shutdown_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4407 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_status_history.py
+-rw-rw-r--   0 root         (0) root         (0)    11915 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_override_request.py
+-rw-rw-r--   0 root         (0) root         (0)    13661 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9283 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_dsm_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5770 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_pod_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4311 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_port_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7773 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_region_override_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4442 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.995105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.999105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/
+-rw-rw-r--   0 root         (0) root         (0)      896 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6535 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7601 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server_detailed.py
+-rw-rw-r--   0 root         (0) root         (0)     7452 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7129 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_local_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7216 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/get_server.py
+-rw-rw-r--   0 root         (0) root         (0)     6574 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_local_server.py
+-rw-rw-r--   0 root         (0) root         (0)     8900 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_server.py
+-rw-rw-r--   0 root         (0) root         (0)     9812 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.999105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      929 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/add_port.py
+-rw-rw-r--   0 root         (0) root         (0)     6294 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/clear_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     9010 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/create_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6786 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7582 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_port.py
+-rw-rw-r--   0 root         (0) root         (0)     6839 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/export_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6675 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/get_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8166 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/import_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5464 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/list_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8665 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/save_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9140 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/update_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8716 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/update_port.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.999105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/
+-rw-rw-r--   0 root         (0) root         (0)     1506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9132 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     9139 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_client.py
+-rw-rw-r--   0 root         (0) root         (0)    10341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_override.py
+-rw-rw-r--   0 root         (0) root         (0)    11187 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_override_region__89178f.py
+-rw-rw-r--   0 root         (0) root         (0)    10311 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_root_region_override.py
+-rw-rw-r--   0 root         (0) root         (0)     7692 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     7707 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_client.py
+-rw-rw-r--   0 root         (0) root         (0)     8826 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_override.py
+-rw-rw-r--   0 root         (0) root         (0)     9704 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_override_region__2e7e2d.py
+-rw-rw-r--   0 root         (0) root         (0)     8838 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_root_region_override.py
+-rw-rw-r--   0 root         (0) root         (0)     9127 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     9156 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment_client.py
+-rw-rw-r--   0 root         (0) root         (0)     7861 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     9345 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)    10095 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment_override.py
+-rw-rw-r--   0 root         (0) root         (0)    10951 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_override_region__fb90bf.py
+-rw-rw-r--   0 root         (0) root         (0)    10075 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_root_region_override.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:07.999105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/
+-rw-rw-r--   0 root         (0) root         (0)      526 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5100 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.003105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/
+-rw-rw-r--   0 root         (0) root         (0)     1498 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7054 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image.py
+-rw-rw-r--   0 root         (0) root         (0)     7281 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image_patch.py
+-rw-rw-r--   0 root         (0) root         (0)     6847 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_repository.py
+-rw-rw-r--   0 root         (0) root         (0)     8731 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image.py
+-rw-rw-r--   0 root         (0) root         (0)     9600 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image_patch.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/export_images.py
+-rw-rw-r--   0 root         (0) root         (0)     7532 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     6730 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     8565 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patch_detail.py
+-rw-rw-r--   0 root         (0) root         (0)     7410 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patches.py
+-rw-rw-r--   0 root         (0) root         (0)     6758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_repository.py
+-rw-rw-r--   0 root         (0) root         (0)     7527 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_detail_client.py
+-rw-rw-r--   0 root         (0) root         (0)     6808 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_limit_client.py
+-rw-rw-r--   0 root         (0) root         (0)     7137 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/import_images.py
+-rw-rw-r--   0 root         (0) root         (0)    11400 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images.py
+-rw-rw-r--   0 root         (0) root         (0)    11616 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images_client.py
+-rw-rw-r--   0 root         (0) root         (0)     6828 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/update_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.003105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/
+-rw-rw-r--   0 root         (0) root         (0)      946 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8818 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8841 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config_client.py
+-rw-rw-r--   0 root         (0) root         (0)     7703 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7720 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config_client.py
+-rw-rw-r--   0 root         (0) root         (0)     8327 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8350 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config_client.py
+-rw-rw-r--   0 root         (0) root         (0)     5571 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_lowest_instance_spec.py
+-rw-rw-r--   0 root         (0) root         (0)     7571 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_pod_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9053 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/update_pod_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.003105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/
+-rw-rw-r--   0 root         (0) root         (0)      630 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4795 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/get_default_provider.py
+-rw-rw-r--   0 root         (0) root         (0)     4690 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers.py
+-rw-rw-r--   0 root         (0) root         (0)     5615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers_by_region.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.003105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/
+-rw-rw-r--   0 root         (0) root         (0)      885 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7945 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/deregister_local_server.py
+-rw-rw-r--   0 root         (0) root         (0)     7878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8340 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session_timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     8944 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/list_server_client.py
+-rw-rw-r--   0 root         (0) root         (0)     8618 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/register_local_server.py
+-rw-rw-r--   0 root         (0) root         (0)     8513 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/register_server.py
+-rw-rw-r--   0 root         (0) root         (0)     8314 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/server_heartbeat.py
+-rw-rw-r--   0 root         (0) root         (0)     8079 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/shutdown_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.003105 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/
+-rw-rw-r--   0 root         (0) root         (0)      633 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7820 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/cancel_session.py
+-rw-rw-r--   0 root         (0) root         (0)     8462 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/claim_server.py
+-rw-rw-r--   0 root         (0) root         (0)     9067 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/create_session.py
+-rw-rw-r--   0 root         (0) root         (0)     7779 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/get_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.007104 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     8025 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31852 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_admin.py
+-rw-rw-r--   0 root         (0) root         (0)    45080 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)    65317 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_deployment_config.py
+-rw-rw-r--   0 root         (0) root         (0)     2747 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_dsmc_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    56682 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_image_config.py
+-rw-rw-r--   0 root         (0) root         (0)    30179 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_pod_config.py
+-rw-rw-r--   0 root         (0) root         (0)     5673 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_public.py
+-rw-rw-r--   0 root         (0) root         (0)    30981 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_server.py
+-rw-rw-r--   0 root         (0) root         (0)    16585 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:08.007104 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:27:07.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11242 2024-05-07 06:27:07.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:07.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:07.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:07.000000 accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_dsmc-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:08.007104 accelbyte_py_sdk_service_dsmc-0.8.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/PKG-INFO` & `accelbyte_py_sdk_service_dsmc-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsmc
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Dsm Controller Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/README.md` & `accelbyte_py_sdk_service_dsmc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/log_app_message_declaration.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_allocation_event.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_allocation_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_claim_session_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_claim_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_count_server_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_count_server_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_count_session_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_count_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_override_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_override_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_deployment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_dsm_config_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_dsm_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_patch_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_patch_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_image_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_pod_config_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_pod_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_port_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_port_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_region_override_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_region_override_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_repository_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_repository_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_create_session_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_create_session_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_default_provider.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_default_provider.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_config_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_config_override.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_with_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deployment_with_override.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_deregister_local_server_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_deregister_local_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_detailed_count_server_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_detailed_count_server_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_ds_heartbeat_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_ds_heartbeat_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_dsm_config_record.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_dsm_config_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_detail_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_detail_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response_data.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_limit_response_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_patch_detail_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_get_image_patch_detail_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_record.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_record_update.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_record_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_image_replication.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_image_replication.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_import_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_import_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_instance_spec.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_instance_spec.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_config_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_deployment_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_deployment_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_patches_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_patches_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_image_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_pod_config_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_pod_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_server_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_server_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_list_session_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_list_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_match_result_notification_payload.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_match_result_notification_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_paging_cursor.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_paging_cursor.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_patch_image_record.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_patch_image_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_pod_config_record.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_pod_config_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_pod_count_config_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_pod_count_config_override.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_register_local_server_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_register_local_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_register_server_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_register_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_repository_record.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_repository_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_member.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_member.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_party.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_match_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_request_matching_ally.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_request_matching_ally.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server_deployment_config_session_timeout_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server_deployment_config_session_timeout_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_server_session_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_server_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_session_response.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_session_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_shutdown_server_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_shutdown_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_status_history.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_status_history.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_override_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_override_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_deployment_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_dsm_config_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_dsm_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_pod_config_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_pod_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_port_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_port_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/models_update_region_override_request.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/models_update_region_override_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/models/response_error.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,31 +70,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/count"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/count"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server_detailed.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_server_detailed.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/count/detailed"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/count/detailed"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     region: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/count_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions/count"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions/count"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     region: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_local_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_local_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/local/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/local/{name}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,32 +73,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/{podName}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/{podName}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/delete_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions/{sessionID}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions/{sessionID}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     session_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/get_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/get_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/{podName}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/{podName}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_local_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_local_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,31 +70,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/local"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers/local"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,34 +78,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/servers"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/servers"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     region: str  # OPTIONAL in [query]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/admin/list_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/sessions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     region: str  # OPTIONAL in [query]
     with_server: bool  # OPTIONAL in [query]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/add_port.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/add_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,33 +81,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreatePortRequest  # REQUIRED in [body]
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/clear_cache.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/get_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,75 +25,90 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelsDSMConfigRecord
 from ...models import ResponseError
 
 
-class ClearCache(Operation):
-    """Clear config cache (ClearCache)
+class GetConfig(Operation):
+    """Get config for a namespace (GetConfig)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required scope: social
 
-    This endpoint clears config cache in a namespace
+    This endpoint get a dedicated servers config in a namespace.
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs/cache
+        url: /dsmcontroller/admin/namespaces/{namespace}/configs
 
-        method: DELETE
+        method: GET
 
         tags: ["Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (ok)
+        200: OK - ModelsDSMConfigRecord (config retrieved)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
+        404: Not Found - ResponseError (config not found)
+
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/cache"
-    _method: str = "DELETE"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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
 
@@ -132,15 +147,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ClearCache:
+    def with_namespace(self, value: str) -> GetConfig:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -155,21 +170,25 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[
+        Union[None, ModelsDSMConfigRecord], Union[None, HttpResponse, ResponseError]
+    ]:
         """Parse the given response.
 
-        204: No Content - (ok)
+        200: OK - ModelsDSMConfigRecord (config retrieved)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
+        404: Not Found - ResponseError (config not found)
+
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -177,39 +196,41 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ModelsDSMConfigRecord.create_from_dict(content), None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> ClearCache:
+    def create(cls, namespace: str, **kwargs) -> GetConfig:
         instance = cls()
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ClearCache:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetConfig:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/create_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/create_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,32 +105,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateDSMConfigRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,31 +75,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_port.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/delete_port.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,32 +76,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/export_config_v1.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/export_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,79 +25,92 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelsImageRecord
 from ...models import ResponseError
 
 
-class ExportConfigV1(Operation):
-    """export DSM Controller configuration for a namespace (exportConfigV1)
+class ExportImages(Operation):
+    """export DSM Controller images for a namespace (ExportImages)
 
     Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required scope: social
 
-    This endpoint export a dedicated servers config in a namespace.
+    This endpoint export a dedicated servers images in a namespace.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/v1/namespaces/{namespace}/configs/export
+        url: /dsmcontroller/admin/namespaces/{namespace}/images/export
 
         method: GET
 
-        tags: ["Config"]
+        tags: ["Image Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - Any (config exported)
+        200: OK - List[ModelsImageRecord] (images exported)
 
         401: Unauthorized - ResponseError (unauthorized access)
 
         403: Forbidden - ResponseError (forbidden access)
 
-        404: Not Found - ResponseError (config not found)
+        404: Not Found - ResponseError (images not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/v1/namespaces/{namespace}/configs/export"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/export"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images/export"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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
 
@@ -136,15 +149,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ExportConfigV1:
+    def with_namespace(self, value: str) -> ExportImages:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -159,24 +172,26 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, Any], Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[
+        Union[None, List[ModelsImageRecord]], Union[None, HttpResponse, ResponseError]
+    ]:
         """Parse the given response.
 
-        200: OK - Any (config exported)
+        200: OK - List[ModelsImageRecord] (images exported)
 
         401: Unauthorized - ResponseError (unauthorized access)
 
         403: Forbidden - ResponseError (forbidden access)
 
-        404: Not Found - ResponseError (config not found)
+        404: Not Found - ResponseError (images not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -186,15 +201,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return content, None
+            return [ModelsImageRecord.create_from_dict(i) for i in content], None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 403:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
@@ -205,25 +220,23 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> ExportConfigV1:
+    def create(cls, namespace: str, **kwargs) -> ExportImages:
         instance = cls()
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> ExportConfigV1:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ExportImages:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/get_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/export_config_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,78 +25,91 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsDSMConfigRecord
 from ...models import ResponseError
 
 
-class GetConfig(Operation):
-    """Get config for a namespace (GetConfig)
+class ExportConfigV1(Operation):
+    """export DSM Controller configuration for a namespace (exportConfigV1)
 
     Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required scope: social
 
-    This endpoint get a dedicated servers config in a namespace.
+    This endpoint export a dedicated servers config in a namespace.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs
+        url: /dsmcontroller/admin/v1/namespaces/{namespace}/configs/export
 
         method: GET
 
         tags: ["Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsDSMConfigRecord (config retrieved)
+        200: OK - Any (config exported)
 
-        401: Unauthorized - ResponseError (Unauthorized)
+        401: Unauthorized - ResponseError (unauthorized access)
+
+        403: Forbidden - ResponseError (forbidden access)
 
         404: Not Found - ResponseError (config not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _url: str = "/dsmcontroller/admin/v1/namespaces/{namespace}/configs/export"
+    _path: str = "/dsmcontroller/admin/v1/namespaces/{namespace}/configs/export"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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
 
@@ -135,15 +148,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetConfig:
+    def with_namespace(self, value: str) -> ExportConfigV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -158,22 +171,22 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsDSMConfigRecord], Union[None, HttpResponse, ResponseError]
-    ]:
+    ) -> Tuple[Union[None, Any], Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsDSMConfigRecord (config retrieved)
+        200: OK - Any (config exported)
 
-        401: Unauthorized - ResponseError (Unauthorized)
+        401: Unauthorized - ResponseError (unauthorized access)
+
+        403: Forbidden - ResponseError (forbidden access)
 
         404: Not Found - ResponseError (config not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
@@ -185,40 +198,44 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsDSMConfigRecord.create_from_dict(content), None
+            return content, None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 403:
+            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> GetConfig:
+    def create(cls, namespace: str, **kwargs) -> ExportConfigV1:
         instance = cls()
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetConfig:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> ExportConfigV1:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/import_config_v1.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/import_config_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,32 +80,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/v1/namespaces/{namespace}/configs/import"
+    _path: str = "/dsmcontroller/admin/v1/namespaces/{namespace}/configs/import"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["multipart/form-data"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     file: Any  # OPTIONAL in [form_data]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/list_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/list_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,29 +68,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/configs"
+    _path: str = "/dsmcontroller/admin/configs"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/save_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/save_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from accelbyte_py_sdk.core import deprecated
 
 from ...models import ModelsDSMConfigRecord
 from ...models import ResponseError
 
 
 class SaveConfig(Operation):
-    """Save config (SaveConfig)
+    """[DEPRECATED] Save config (SaveConfig)
 
     ```
     Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
     Required scope: social
 
     This endpoint adds/modifies config. When there are ready servers and
     the server version is updated, those servers will be replaced with newer version.
@@ -142,31 +142,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/configs"
+    _path: str = "/dsmcontroller/admin/configs"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsDSMConfigRecord  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/update_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/update_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,32 +106,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdateDSMConfigRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/config/update_port.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/update_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,33 +79,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/ports/{name}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdatePortRequest  # REQUIRED in [body]
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,33 +81,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
     )
+    _path: str = (
+        "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateDeploymentRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,33 +79,47 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/configs/deployments/{deployment}"
+    _path: str = (
+        "/dsmcontroller/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateDeploymentRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_deployment_override.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,34 +83,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/version/{version}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/version/{version}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateDeploymentOverrideRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_override_region__89178f.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_root_region_override.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreateRegionOverrideRequest
 from ...models import ModelsDeploymentWithOverride
 from ...models import ResponseError
 
 
-class CreateOverrideRegionOverride(Operation):
-    """Create region override for deployment override (CreateOverrideRegionOverride)
+class CreateRootRegionOverride(Operation):
+    """Create region override (CreateRootRegionOverride)
 
     Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required scope: social
 
-    This endpoint creates a dedicated servers deployment override in a namespace in a region for deployment overrides.
+    This endpoint creates a dedicated servers deployment override in a namespace in a region for root deployment.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}
+        url: /dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}
 
         method: POST
 
         tags: ["Deployment Config"]
 
         consumes: ["application/json"]
 
@@ -66,16 +66,14 @@
 
         deployment: (deployment) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         region: (region) REQUIRED str in path
 
-        version: (version) REQUIRED str in path
-
     Responses:
         201: Created - ModelsDeploymentWithOverride (region override created)
 
         400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
@@ -84,36 +82,47 @@
         409: Conflict - ResponseError (deployment already has region override)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateRegionOverrideRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     region: str  # REQUIRED in [path]
-    version: str  # REQUIRED in [path]
 
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
 
@@ -152,48 +161,42 @@
         result = {}
         if hasattr(self, "deployment"):
             result["deployment"] = self.deployment
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         if hasattr(self, "region"):
             result["region"] = self.region
-        if hasattr(self, "version"):
-            result["version"] = self.version
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
         self, value: ModelsCreateRegionOverrideRequest
-    ) -> CreateOverrideRegionOverride:
+    ) -> CreateRootRegionOverride:
         self.body = value
         return self
 
-    def with_deployment(self, value: str) -> CreateOverrideRegionOverride:
+    def with_deployment(self, value: str) -> CreateRootRegionOverride:
         self.deployment = value
         return self
 
-    def with_namespace(self, value: str) -> CreateOverrideRegionOverride:
+    def with_namespace(self, value: str) -> CreateRootRegionOverride:
         self.namespace = value
         return self
 
-    def with_region(self, value: str) -> CreateOverrideRegionOverride:
+    def with_region(self, value: str) -> CreateRootRegionOverride:
         self.region = value
         return self
 
-    def with_version(self, value: str) -> CreateOverrideRegionOverride:
-        self.version = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
@@ -208,18 +211,14 @@
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "region") and self.region:
             result["region"] = str(self.region)
         elif include_empty:
             result["region"] = ""
-        if hasattr(self, "version") and self.version:
-            result["version"] = str(self.version)
-        elif include_empty:
-            result["version"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
@@ -280,31 +279,29 @@
     @classmethod
     def create(
         cls,
         body: ModelsCreateRegionOverrideRequest,
         deployment: str,
         namespace: str,
         region: str,
-        version: str,
         **kwargs,
-    ) -> CreateOverrideRegionOverride:
+    ) -> CreateRootRegionOverride:
         instance = cls()
         instance.body = body
         instance.deployment = deployment
         instance.namespace = namespace
         instance.region = region
-        instance.version = version
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreateOverrideRegionOverride:
+    ) -> CreateRootRegionOverride:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsCreateRegionOverrideRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsCreateRegionOverrideRequest()
@@ -316,34 +313,28 @@
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "region" in dict_ and dict_["region"] is not None:
             instance.region = str(dict_["region"])
         elif include_empty:
             instance.region = ""
-        if "version" in dict_ and dict_["version"] is not None:
-            instance.version = str(dict_["version"])
-        elif include_empty:
-            instance.version = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
             "deployment": "deployment",
             "namespace": "namespace",
             "region": "region",
-            "version": "version",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
             "deployment": True,
             "namespace": True,
             "region": True,
-            "version": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/create_root_region_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_root_region_override.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,92 +25,102 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsCreateRegionOverrideRequest
 from ...models import ModelsDeploymentWithOverride
+from ...models import ModelsUpdateRegionOverrideRequest
 from ...models import ResponseError
 
 
-class CreateRootRegionOverride(Operation):
-    """Create region override (CreateRootRegionOverride)
+class UpdateRootRegionOverride(Operation):
+    """Update region override (UpdateRootRegionOverride)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
 
     Required scope: social
 
-    This endpoint creates a dedicated servers deployment override in a namespace in a region for root deployment.
+    This endpoint update a dedicated servers deployment override in a namespace in a region for root deployment.
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
 
     Required Scope(s):
         - social
 
     Properties:
         url: /dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}
 
-        method: POST
+        method: PATCH
 
         tags: ["Deployment Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsCreateRegionOverrideRequest in body
+        body: (body) REQUIRED ModelsUpdateRegionOverrideRequest in body
 
         deployment: (deployment) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
         region: (region) REQUIRED str in path
 
     Responses:
-        201: Created - ModelsDeploymentWithOverride (region override created)
+        200: OK - ModelsDeploymentWithOverride (deployment region override updated)
 
         400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         404: Not Found - ResponseError (deployment not found)
 
-        409: Conflict - ResponseError (deployment already has region override)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
-    _method: str = "POST"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
+    _base_path: str = ""
+    _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsCreateRegionOverrideRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "dsmc"
+
+    body: ModelsUpdateRegionOverrideRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
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
 
@@ -160,41 +170,41 @@
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
-        self, value: ModelsCreateRegionOverrideRequest
-    ) -> CreateRootRegionOverride:
+        self, value: ModelsUpdateRegionOverrideRequest
+    ) -> UpdateRootRegionOverride:
         self.body = value
         return self
 
-    def with_deployment(self, value: str) -> CreateRootRegionOverride:
+    def with_deployment(self, value: str) -> UpdateRootRegionOverride:
         self.deployment = value
         return self
 
-    def with_namespace(self, value: str) -> CreateRootRegionOverride:
+    def with_namespace(self, value: str) -> UpdateRootRegionOverride:
         self.namespace = value
         return self
 
-    def with_region(self, value: str) -> CreateRootRegionOverride:
+    def with_region(self, value: str) -> UpdateRootRegionOverride:
         self.region = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsCreateRegionOverrideRequest()
+            result["body"] = ModelsUpdateRegionOverrideRequest()
         if hasattr(self, "deployment") and self.deployment:
             result["deployment"] = str(self.deployment)
         elif include_empty:
             result["deployment"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
@@ -214,24 +224,22 @@
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
         Union[None, ModelsDeploymentWithOverride],
         Union[None, HttpResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        201: Created - ModelsDeploymentWithOverride (region override created)
+        200: OK - ModelsDeploymentWithOverride (deployment region override updated)
 
         400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         404: Not Found - ResponseError (deployment not found)
 
-        409: Conflict - ResponseError (deployment already has region override)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -239,64 +247,62 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
+        if code == 200:
             return ModelsDeploymentWithOverride.create_from_dict(content), None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
-        if code == 409:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsCreateRegionOverrideRequest,
+        body: ModelsUpdateRegionOverrideRequest,
         deployment: str,
         namespace: str,
         region: str,
         **kwargs,
-    ) -> CreateRootRegionOverride:
+    ) -> UpdateRootRegionOverride:
         instance = cls()
         instance.body = body
         instance.deployment = deployment
         instance.namespace = namespace
         instance.region = region
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreateRootRegionOverride:
+    ) -> UpdateRootRegionOverride:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsCreateRegionOverrideRequest.create_from_dict(
+            instance.body = ModelsUpdateRegionOverrideRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsCreateRegionOverrideRequest()
+            instance.body = ModelsUpdateRegionOverrideRequest()
         if "deployment" in dict_ and dict_["deployment"] is not None:
             instance.deployment = str(dict_["deployment"])
         elif include_empty:
             instance.deployment = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,32 +77,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
     )
+    _path: str = (
+        "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,32 +75,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/configs/deployments/{deployment}"
+    _path: str = (
+        "/dsmcontroller/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_deployment_override.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,33 +78,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_override_region__2e7e2d.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_override_region__2e7e2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,34 +80,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     region: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_root_region_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/delete_root_region_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,33 +78,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,34 +80,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     name: str  # OPTIONAL in [query]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_all_deployment_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,34 +80,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/configs/deployments"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/configs/deployments"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     name: str  # OPTIONAL in [query]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_deployment.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/get_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,32 +78,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
     )
+    _path: str = (
+        "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,33 +83,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
     )
+    _path: str = (
+        "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}"
+    )
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdateDeploymentRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_deployment_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,34 +81,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdateDeploymentOverrideRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_override_region__fb90bf.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_override_region__fb90bf.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,20 +83,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/versions/{version}/regions/{region}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdateRegionOverrideRequest  # REQUIRED in [body]
     deployment: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     region: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
     # endregion fields
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/deployment_config/update_root_region_override.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/list_server_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,90 +25,99 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsDeploymentWithOverride
-from ...models import ModelsUpdateRegionOverrideRequest
+from ...models import ModelsListServerResponse
 from ...models import ResponseError
 
 
-class UpdateRootRegionOverride(Operation):
-    """Update region override (UpdateRootRegionOverride)
+class ListServerClient(Operation):
+    """List all managed servers in a region for client (ListServerClient)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
+    Required permission: NAMESPACE:{namespace}:DSM:SERVER [READ]
 
     Required scope: social
 
-    This endpoint update a dedicated servers deployment override in a namespace in a region for root deployment.
+    This endpoint lists all of dedicated servers in a namespace managed by this service.
+
+    Parameter Offset and Count is Required
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
+        - NAMESPACE:{namespace}:DSM:SERVER [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}
+        url: /dsmcontroller/namespaces/{namespace}/servers
 
-        method: PATCH
+        method: GET
 
-        tags: ["Deployment Config"]
+        tags: ["Server"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUpdateRegionOverrideRequest in body
+        namespace: (namespace) REQUIRED str in path
 
-        deployment: (deployment) REQUIRED str in path
+        region: (region) OPTIONAL str in query
 
-        namespace: (namespace) REQUIRED str in path
+        count: (count) REQUIRED int in query
 
-        region: (region) REQUIRED str in path
+        offset: (offset) REQUIRED int in query
 
     Responses:
-        200: OK - ModelsDeploymentWithOverride (deployment region override updated)
-
-        400: Bad Request - ResponseError (malformed request)
+        200: OK - ModelsListServerResponse (servers listed)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (deployment not found)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/deployments/{deployment}/overrides/regions/{region}"
-    _method: str = "PATCH"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/servers"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsUpdateRegionOverrideRequest  # REQUIRED in [body]
-    deployment: str  # REQUIRED in [path]
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
-    region: str  # REQUIRED in [path]
+    region: str  # OPTIONAL in [query]
+    count: int  # REQUIRED in [query]
+    offset: int  # REQUIRED in [query]
 
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
 
@@ -130,104 +139,98 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
+            "query": self.get_query_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "deployment"):
-            result["deployment"] = self.deployment
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        return result
+
+    def get_query_params(self) -> dict:
+        result = {}
         if hasattr(self, "region"):
             result["region"] = self.region
+        if hasattr(self, "count"):
+            result["count"] = self.count
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(
-        self, value: ModelsUpdateRegionOverrideRequest
-    ) -> UpdateRootRegionOverride:
-        self.body = value
+    def with_namespace(self, value: str) -> ListServerClient:
+        self.namespace = value
         return self
 
-    def with_deployment(self, value: str) -> UpdateRootRegionOverride:
-        self.deployment = value
+    def with_region(self, value: str) -> ListServerClient:
+        self.region = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateRootRegionOverride:
-        self.namespace = value
+    def with_count(self, value: int) -> ListServerClient:
+        self.count = value
         return self
 
-    def with_region(self, value: str) -> UpdateRootRegionOverride:
-        self.region = value
+    def with_offset(self, value: int) -> ListServerClient:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsUpdateRegionOverrideRequest()
-        if hasattr(self, "deployment") and self.deployment:
-            result["deployment"] = str(self.deployment)
-        elif include_empty:
-            result["deployment"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         if hasattr(self, "region") and self.region:
             result["region"] = str(self.region)
         elif include_empty:
             result["region"] = ""
+        if hasattr(self, "count") and self.count:
+            result["count"] = int(self.count)
+        elif include_empty:
+            result["count"] = 0
+        if hasattr(self, "offset") and self.offset:
+            result["offset"] = int(self.offset)
+        elif include_empty:
+            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelsDeploymentWithOverride],
-        Union[None, HttpResponse, ResponseError],
+        Union[None, ModelsListServerResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsDeploymentWithOverride (deployment region override updated)
-
-        400: Bad Request - ResponseError (malformed request)
+        200: OK - ModelsListServerResponse (servers listed)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (deployment not found)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -236,87 +239,82 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsDeploymentWithOverride.create_from_dict(content), None
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
+            return ModelsListServerResponse.create_from_dict(content), None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
-        body: ModelsUpdateRegionOverrideRequest,
-        deployment: str,
         namespace: str,
-        region: str,
+        count: int,
+        offset: int,
+        region: Optional[str] = None,
         **kwargs,
-    ) -> UpdateRootRegionOverride:
+    ) -> ListServerClient:
         instance = cls()
-        instance.body = body
-        instance.deployment = deployment
         instance.namespace = namespace
-        instance.region = region
+        instance.count = count
+        instance.offset = offset
+        if region is not None:
+            instance.region = region
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateRootRegionOverride:
+    ) -> ListServerClient:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsUpdateRegionOverrideRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsUpdateRegionOverrideRequest()
-        if "deployment" in dict_ and dict_["deployment"] is not None:
-            instance.deployment = str(dict_["deployment"])
-        elif include_empty:
-            instance.deployment = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "region" in dict_ and dict_["region"] is not None:
             instance.region = str(dict_["region"])
         elif include_empty:
             instance.region = ""
+        if "count" in dict_ and dict_["count"] is not None:
+            instance.count = int(dict_["count"])
+        elif include_empty:
+            instance.count = 0
+        if "offset" in dict_ and dict_["offset"] is not None:
+            instance.offset = int(dict_["offset"])
+        elif include_empty:
+            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
-            "deployment": "deployment",
             "namespace": "namespace",
             "region": "region",
+            "count": "count",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
-            "deployment": True,
             "namespace": True,
-            "region": True,
+            "region": False,
+            "count": True,
+            "offset": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/public_get_messages.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/dsmc_operations/public_get_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,29 +56,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/v1/messages"
+    _path: str = "/dsmcontroller/v1/messages"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,31 +83,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/images"
+    _path: str = "/dsmcontroller/admin/images"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateImageRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image_patch.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_image_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,31 +84,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/images/patches"
+    _path: str = "/dsmcontroller/admin/images/patches"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateImagePatchRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_repository.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/create_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,31 +79,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/repository"
+    _path: str = "/dsmcontroller/admin/repository"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateRepositoryRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,33 +81,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     image_uri: str  # REQUIRED in [query]
     version: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image_patch.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/delete_image_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,34 +81,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/patches"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images/patches"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     image_uri: str  # REQUIRED in [query]
     version: str  # REQUIRED in [query]
     version_patch: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/export_images.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,80 +25,90 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsImageRecord
+from ...models import ModelsRepositoryRecord
 from ...models import ResponseError
 
 
-class ExportImages(Operation):
-    """export DSM Controller images for a namespace (ExportImages)
+class GetRepository(Operation):
+    """Get repository for a namespace (GetRepository)
 
     Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required scope: social
 
-    This endpoint export a dedicated servers images in a namespace.
+    This endpoint get a dedicated servers repository name in a namespace.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/images/export
+        url: /dsmcontroller/admin/namespaces/{namespace}/repository
 
         method: GET
 
         tags: ["Image Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - List[ModelsImageRecord] (images exported)
+        200: OK - ModelsRepositoryRecord (repository retrieved)
 
-        401: Unauthorized - ResponseError (unauthorized access)
+        401: Unauthorized - ResponseError (Unauthorized)
 
-        403: Forbidden - ResponseError (forbidden access)
-
-        404: Not Found - ResponseError (images not found)
+        404: Not Found - ResponseError (repository not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/export"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/repository"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/repository"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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
 
@@ -137,15 +147,15 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ExportImages:
+    def with_namespace(self, value: str) -> GetRepository:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -161,25 +171,23 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, List[ModelsImageRecord]], Union[None, HttpResponse, ResponseError]
+        Union[None, ModelsRepositoryRecord], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - List[ModelsImageRecord] (images exported)
+        200: OK - ModelsRepositoryRecord (repository retrieved)
 
-        401: Unauthorized - ResponseError (unauthorized access)
+        401: Unauthorized - ResponseError (Unauthorized)
 
-        403: Forbidden - ResponseError (forbidden access)
-
-        404: Not Found - ResponseError (images not found)
+        404: Not Found - ResponseError (repository not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -189,42 +197,42 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [ModelsImageRecord.create_from_dict(i) for i in content], None
+            return ModelsRepositoryRecord.create_from_dict(content), None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
-        if code == 403:
-            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> ExportImages:
+    def create(cls, namespace: str, **kwargs) -> GetRepository:
         instance = cls()
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ExportImages:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> GetRepository:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_detail.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_limit.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,31 +72,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/limit"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images/limit"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patch_detail.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patch_detail.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,33 +76,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}/patches/{versionPatch}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}/patches/{versionPatch}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
     version_patch: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patches.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_image_patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,32 +76,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}/patches"
     )
+    _path: str = (
+        "/dsmcontroller/admin/namespaces/{namespace}/images/versions/{version}/patches"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/get_repository.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/update_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,78 +25,99 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsRepositoryRecord
+from ...models import ModelsImageRecordUpdate
 from ...models import ResponseError
 
 
-class GetRepository(Operation):
-    """Get repository for a namespace (GetRepository)
-
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
+class UpdateImage(Operation):
+    """Update image (UpdateImage)
 
+    ```
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
     Required scope: social
 
-    This endpoint get a dedicated servers repository name in a namespace.
+    This endpoint will update an image name and/or image persistent flag.
+
+    Sample image:
+    {
+    "namespace":"dewa",
+    "version":"1.0.0",
+    "image":"144436415367.dkr.ecr.us-west-2.amazonaws.com/dewa:1.0.0",
+    "persistent":false
+    }
+    ```
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [READ]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/repository
+        url: /dsmcontroller/admin/images
 
-        method: GET
+        method: PUT
 
         tags: ["Image Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        body: (body) REQUIRED ModelsImageRecordUpdate in body
 
     Responses:
-        200: OK - ModelsRepositoryRecord (repository retrieved)
+        204: No Content - (image updated)
 
-        401: Unauthorized - ResponseError (Unauthorized)
+        400: Bad Request - ResponseError (malformed request)
 
-        404: Not Found - ResponseError (repository not found)
+        401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/repository"
-    _method: str = "GET"
+    _url: str = "/dsmcontroller/admin/images"
+    _path: str = "/dsmcontroller/admin/images"
+    _base_path: str = ""
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    namespace: str  # REQUIRED in [path]
+    service_name: Optional[str] = "dsmc"
+
+    body: ModelsImageRecordUpdate  # REQUIRED in [body]
 
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
 
@@ -118,64 +139,61 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "path": self.get_path_params(),
+            "body": self.get_body_params(),
         }
 
-    def get_path_params(self) -> dict:
-        result = {}
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
-        return result
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetRepository:
-        self.namespace = value
+    def with_body(self, value: ModelsImageRecordUpdate) -> UpdateImage:
+        self.body = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["namespace"] = ""
+            result["body"] = ModelsImageRecordUpdate()
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsRepositoryRecord], Union[None, HttpResponse, ResponseError]
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsRepositoryRecord (repository retrieved)
+        204: No Content - (image updated)
 
-        401: Unauthorized - ResponseError (Unauthorized)
+        400: Bad Request - ResponseError (malformed request)
 
-        404: Not Found - ResponseError (repository not found)
+        401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -184,56 +202,56 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsRepositoryRecord.create_from_dict(content), None
-        if code == 401:
+        if code == 204:
+            return None, None
+        if code == 400:
             return None, ResponseError.create_from_dict(content)
-        if code == 404:
+        if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> GetRepository:
+    def create(cls, body: ModelsImageRecordUpdate, **kwargs) -> UpdateImage:
         instance = cls()
-        instance.namespace = namespace
+        instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> GetRepository:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UpdateImage:
         instance = cls()
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsImageRecordUpdate.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.namespace = ""
+            instance.body = ModelsImageRecordUpdate()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "namespace": "namespace",
+            "body": "body",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "namespace": True,
+            "body": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_detail_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_detail_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/images/versions/{version}"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/images/versions/{version}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     version: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_limit_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/image_limit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,31 +72,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/images/limit"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/images/limit"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/import_images.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/import_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,31 +86,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/images/import"
+    _path: str = "/dsmcontroller/admin/images/import"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["multipart/form-data"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     file: Any  # REQUIRED in [form_data]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/images"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/images"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     q: str  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
     sort_direction: Union[str, SortDirectionEnum]  # OPTIONAL in [query]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
@@ -118,14 +122,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/image_config/list_images_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/images"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/images"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     count: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     q: str  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
     sort_direction: Union[str, SortDirectionEnum]  # OPTIONAL in [query]
 
@@ -118,14 +122,22 @@
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/image_config/update_image.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_lowest_instance_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,87 +25,84 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsImageRecordUpdate
+from ...models import ModelsInstanceSpec
 from ...models import ResponseError
 
 
-class UpdateImage(Operation):
-    """Update image (UpdateImage)
+class GetLowestInstanceSpec(Operation):
+    """Get lowest instance spec. (GetLowestInstanceSpec)
 
-    ```
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
-    Required scope: social
+    Required permission: ADMIN:NAMESPACE:*:DSM:CONFIG [READ]
 
-    This endpoint will update an image name and/or image persistent flag.
+    Required scope: social
 
-    Sample image:
-    {
-    "namespace":"dewa",
-    "version":"1.0.0",
-    "image":"144436415367.dkr.ecr.us-west-2.amazonaws.com/dewa:1.0.0",
-    "persistent":false
-    }
-    ```
+    This endpoint returns the lowest instance spec, both cpu (in Mhz) and memory (in Mb).
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [UPDATE]
+        - ADMIN:NAMESPACE:*:DSM:CONFIG [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/images
+        url: /dsmcontroller/admin/instances/spec/lowest
 
-        method: PUT
+        method: GET
 
-        tags: ["Image Config"]
+        tags: ["Pod Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsImageRecordUpdate in body
-
     Responses:
-        204: No Content - (image updated)
-
-        400: Bad Request - ResponseError (malformed request)
+        200: OK - ModelsInstanceSpec (Lowest Instance Spec)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/images"
-    _method: str = "PUT"
+    _url: str = "/dsmcontroller/admin/instances/spec/lowest"
+    _path: str = "/dsmcontroller/admin/instances/spec/lowest"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsImageRecordUpdate  # REQUIRED in [body]
+    service_name: Optional[str] = "dsmc"
 
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
 
@@ -126,60 +123,45 @@
     # region get methods
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
-        return {
-            "body": self.get_body_params(),
-        }
-
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
+        return {}
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsImageRecordUpdate) -> UpdateImage:
-        self.body = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsImageRecordUpdate()
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[
+        Union[None, ModelsInstanceSpec], Union[None, HttpResponse, ResponseError]
+    ]:
         """Parse the given response.
 
-        204: No Content - (image updated)
-
-        400: Bad Request - ResponseError (malformed request)
+        200: OK - ModelsInstanceSpec (Lowest Instance Spec)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
@@ -190,56 +172,45 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
+        if code == 200:
+            return ModelsInstanceSpec.create_from_dict(content), None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, body: ModelsImageRecordUpdate, **kwargs) -> UpdateImage:
+    def create(cls, **kwargs) -> GetLowestInstanceSpec:
         instance = cls()
-        instance.body = body
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UpdateImage:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> GetLowestInstanceSpec:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsImageRecordUpdate.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsImageRecordUpdate()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
-        return {
-            "body": "body",
-        }
+        return {}
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
-        return {
-            "body": True,
-        }
+        return {}
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreatePodConfigRequest
 from ...models import ModelsPodConfigRecord
 from ...models import ResponseError
 
 
-class CreatePodConfig(Operation):
-    """Create pod config (CreatePodConfig)
+class CreatePodConfigClient(Operation):
+    """Create pod config for client (CreatePodConfigClient)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+    Required permission: NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required scope: social
 
     This endpoint create a dedicated servers pod config in a namespace.
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+        - NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}
+        url: /dsmcontroller/namespaces/{namespace}/configs/pods/{name}
 
         method: POST
 
         tags: ["Pod Config"]
 
         consumes: ["application/json"]
 
@@ -78,34 +78,46 @@
         409: Conflict - ResponseError (pod config already exists)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreatePodConfigRequest  # REQUIRED in [body]
     name: str  # REQUIRED in [path]
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
 
@@ -152,23 +164,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreatePodConfigRequest) -> CreatePodConfig:
+    def with_body(self, value: ModelsCreatePodConfigRequest) -> CreatePodConfigClient:
         self.body = value
         return self
 
-    def with_name(self, value: str) -> CreatePodConfig:
+    def with_name(self, value: str) -> CreatePodConfigClient:
         self.name = value
         return self
 
-    def with_namespace(self, value: str) -> CreatePodConfig:
+    def with_namespace(self, value: str) -> CreatePodConfigClient:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -241,27 +253,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, body: ModelsCreatePodConfigRequest, name: str, namespace: str, **kwargs
-    ) -> CreatePodConfig:
+    ) -> CreatePodConfigClient:
         instance = cls()
         instance.body = body
         instance.name = name
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreatePodConfig:
+    ) -> CreatePodConfigClient:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsCreatePodConfigRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsCreatePodConfigRequest()
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/create_pod_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelsCreatePodConfigRequest
 from ...models import ModelsPodConfigRecord
 from ...models import ResponseError
 
 
-class CreatePodConfigClient(Operation):
-    """Create pod config for client (CreatePodConfigClient)
+class CreatePodConfig(Operation):
+    """Create pod config (CreatePodConfig)
 
-    Required permission: NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required scope: social
 
     This endpoint create a dedicated servers pod config in a namespace.
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [CREATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/configs/pods/{name}
+        url: /dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}
 
         method: POST
 
         tags: ["Pod Config"]
 
         consumes: ["application/json"]
 
@@ -78,34 +78,46 @@
         409: Conflict - ResponseError (pod config already exists)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreatePodConfigRequest  # REQUIRED in [body]
     name: str  # REQUIRED in [path]
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
 
@@ -152,23 +164,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsCreatePodConfigRequest) -> CreatePodConfigClient:
+    def with_body(self, value: ModelsCreatePodConfigRequest) -> CreatePodConfig:
         self.body = value
         return self
 
-    def with_name(self, value: str) -> CreatePodConfigClient:
+    def with_name(self, value: str) -> CreatePodConfig:
         self.name = value
         return self
 
-    def with_namespace(self, value: str) -> CreatePodConfigClient:
+    def with_namespace(self, value: str) -> CreatePodConfig:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -241,27 +253,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, body: ModelsCreatePodConfigRequest, name: str, namespace: str, **kwargs
-    ) -> CreatePodConfigClient:
+    ) -> CreatePodConfig:
         instance = cls()
         instance.body = body
         instance.name = name
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> CreatePodConfigClient:
+    ) -> CreatePodConfig:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelsCreatePodConfigRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelsCreatePodConfigRequest()
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,31 +28,31 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class DeletePodConfig(Operation):
-    """Delete pod config (DeletePodConfig)
+class DeletePodConfigClient(Operation):
+    """Delete pod config for client (DeletePodConfigClient)
 
-    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+    Required permission: NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required scope: social
 
     This endpoint delete a dedicated server pod config in a namespace
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+        - NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}
+        url: /dsmcontroller/namespaces/{namespace}/configs/pods/{name}
 
         method: DELETE
 
         tags: ["Pod Config"]
 
         consumes: ["application/json"]
 
@@ -76,33 +76,45 @@
         409: Conflict - ResponseError (pod config in use)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     name: str  # REQUIRED in [path]
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
 
@@ -143,19 +155,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_name(self, value: str) -> DeletePodConfig:
+    def with_name(self, value: str) -> DeletePodConfigClient:
         self.name = value
         return self
 
-    def with_namespace(self, value: str) -> DeletePodConfig:
+    def with_namespace(self, value: str) -> DeletePodConfigClient:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -224,26 +236,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, name: str, namespace: str, **kwargs) -> DeletePodConfig:
+    def create(cls, name: str, namespace: str, **kwargs) -> DeletePodConfigClient:
         instance = cls()
         instance.name = name
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeletePodConfig:
+    ) -> DeletePodConfigClient:
         instance = cls()
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/delete_pod_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,31 +28,31 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class DeletePodConfigClient(Operation):
-    """Delete pod config for client (DeletePodConfigClient)
+class DeletePodConfig(Operation):
+    """Delete pod config (DeletePodConfig)
 
-    Required permission: NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required scope: social
 
     This endpoint delete a dedicated server pod config in a namespace
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/configs/pods/{name}
+        url: /dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}
 
         method: DELETE
 
         tags: ["Pod Config"]
 
         consumes: ["application/json"]
 
@@ -76,33 +76,45 @@
         409: Conflict - ResponseError (pod config in use)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/configs/pods/{name}"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     name: str  # REQUIRED in [path]
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
 
@@ -143,19 +155,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_name(self, value: str) -> DeletePodConfigClient:
+    def with_name(self, value: str) -> DeletePodConfig:
         self.name = value
         return self
 
-    def with_namespace(self, value: str) -> DeletePodConfigClient:
+    def with_namespace(self, value: str) -> DeletePodConfig:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -224,26 +236,26 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, name: str, namespace: str, **kwargs) -> DeletePodConfigClient:
+    def create(cls, name: str, namespace: str, **kwargs) -> DeletePodConfig:
         instance = cls()
         instance.name = name
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeletePodConfigClient:
+    ) -> DeletePodConfig:
         instance = cls()
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,33 +78,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_all_pod_config_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,33 +78,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/configs/pods"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/configs/pods"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     count: int  # REQUIRED in [query]
     offset: int  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_lowest_instance_spec.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/config/clear_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,72 +25,87 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsInstanceSpec
 from ...models import ResponseError
 
 
-class GetLowestInstanceSpec(Operation):
-    """Get lowest instance spec. (GetLowestInstanceSpec)
+class ClearCache(Operation):
+    """Clear config cache (ClearCache)
 
-    Required permission: ADMIN:NAMESPACE:*:DSM:CONFIG [READ]
+    Required permission: ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required scope: social
 
-    This endpoint returns the lowest instance spec, both cpu (in Mhz) and memory (in Mb).
+    This endpoint clears config cache in a namespace
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:*:DSM:CONFIG [READ]
+        - ADMIN:NAMESPACE:{namespace}:DSM:CONFIG [DELETE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/admin/instances/spec/lowest
+        url: /dsmcontroller/admin/namespaces/{namespace}/configs/cache
 
-        method: GET
+        method: DELETE
 
-        tags: ["Pod Config"]
+        tags: ["Config"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        namespace: (namespace) REQUIRED str in path
+
     Responses:
-        200: OK - ModelsInstanceSpec (Lowest Instance Spec)
+        204: No Content - (ok)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/admin/instances/spec/lowest"
-    _method: str = "GET"
+    _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/cache"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/cache"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
+    namespace: str  # REQUIRED in [path]
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
 
@@ -111,45 +126,59 @@
     # region get methods
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
-        return {}
+        return {
+            "path": self.get_path_params(),
+        }
+
+    def get_path_params(self) -> dict:
+        result = {}
+        if hasattr(self, "namespace"):
+            result["namespace"] = self.namespace
+        return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
+    def with_namespace(self, value: str) -> ClearCache:
+        self.namespace = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "namespace") and self.namespace:
+            result["namespace"] = str(self.namespace)
+        elif include_empty:
+            result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsInstanceSpec], Union[None, HttpResponse, ResponseError]
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsInstanceSpec (Lowest Instance Spec)
+        204: No Content - (ok)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
@@ -160,45 +189,52 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsInstanceSpec.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> GetLowestInstanceSpec:
+    def create(cls, namespace: str, **kwargs) -> ClearCache:
         instance = cls()
+        instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> GetLowestInstanceSpec:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ClearCache:
         instance = cls()
+        if "namespace" in dict_ and dict_["namespace"] is not None:
+            instance.namespace = str(dict_["namespace"])
+        elif include_empty:
+            instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
-        return {}
+        return {
+            "namespace": "namespace",
+        }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
-        return {}
+        return {
+            "namespace": True,
+        }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/get_pod_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,32 +76,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/update_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/pod_config/update_pod_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,33 +81,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _path: str = "/dsmcontroller/admin/namespaces/{namespace}/configs/pods/{name}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsUpdatePodConfigRequest  # REQUIRED in [body]
     name: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/get_default_provider.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/get_default_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,29 +53,41 @@
     Responses:
         200: OK - ModelsDefaultProvider (Default provider got)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/public/provider/default"
+    _path: str = "/dsmcontroller/public/provider/default"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,29 +51,41 @@
     Responses:
         200: OK - List[str] (Providers listed)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/public/providers"
+    _path: str = "/dsmcontroller/public/providers"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers_by_region.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/public/list_providers_by_region.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,31 +53,43 @@
     Responses:
         200: OK - List[str] (Default providers got)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/public/providers/regions/{region}"
+    _path: str = "/dsmcontroller/public/providers/regions/{region}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/deregister_local_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/deregister_local_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,32 +77,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/servers/local/deregister"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/local/deregister"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsDeregisterLocalServerRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,32 +79,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/servers/{podName}/session"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/{podName}/session"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session_timeout.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/get_server_session_timeout.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,32 +81,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/dsmcontroller/namespaces/{namespace}/servers/{podName}/config/sessiontimeout"
     )
+    _path: str = (
+        "/dsmcontroller/namespaces/{namespace}/servers/{podName}/config/sessiontimeout"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/list_server_client.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/register_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,87 +25,102 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsListServerResponse
+from ...models import ModelsRegisterServerRequest
+from ...models import ModelsServer
 from ...models import ResponseError
 
 
-class ListServerClient(Operation):
-    """List all managed servers in a region for client (ListServerClient)
-
-    Required permission: NAMESPACE:{namespace}:DSM:SERVER [READ]
+class RegisterServer(Operation):
+    """Register a DS (RegisterServer)
 
+    ```
+    Required permission: NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
     Required scope: social
 
-    This endpoint lists all of dedicated servers in a namespace managed by this service.
+    This endpoint is intended to be called by dedicated server to let DSM know that it is ready for use.
+    This MUST be called by DS after it is ready to accept match data and incoming client connections.
 
-    Parameter Offset and Count is Required
+    Upon successfully calling this endpoint, the dedicated
+    server is listed under READY servers.```
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:DSM:SERVER [READ]
+        - NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/servers
+        url: /dsmcontroller/namespaces/{namespace}/servers/register
 
-        method: GET
+        method: POST
 
         tags: ["Server"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsRegisterServerRequest in body
+
         namespace: (namespace) REQUIRED str in path
 
-        region: (region) OPTIONAL str in query
+    Responses:
+        200: OK - ModelsServer (server registered)
 
-        count: (count) REQUIRED int in query
+        400: Bad Request - ResponseError (malformed request)
 
-        offset: (offset) REQUIRED int in query
+        401: Unauthorized - ResponseError (Unauthorized)
 
-    Responses:
-        200: OK - ModelsListServerResponse (servers listed)
+        404: Not Found - ResponseError (allocation not found)
 
-        401: Unauthorized - ResponseError (Unauthorized)
+        409: Conflict - ResponseError (server with same name already registered)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/servers"
-    _method: str = "GET"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/servers/register"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/register"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
+    body: ModelsRegisterServerRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
-    region: str  # OPTIONAL in [query]
-    count: int  # REQUIRED in [query]
-    offset: int  # REQUIRED in [query]
 
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
 
@@ -127,98 +142,81 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
+    def get_body_params(self) -> Any:
+        if not hasattr(self, "body") or self.body is None:
+            return None
+        return self.body.to_dict()
+
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "region"):
-            result["region"] = self.region
-        if hasattr(self, "count"):
-            result["count"] = self.count
-        if hasattr(self, "offset"):
-            result["offset"] = self.offset
-        return result
-
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ListServerClient:
-        self.namespace = value
-        return self
-
-    def with_region(self, value: str) -> ListServerClient:
-        self.region = value
+    def with_body(self, value: ModelsRegisterServerRequest) -> RegisterServer:
+        self.body = value
         return self
 
-    def with_count(self, value: int) -> ListServerClient:
-        self.count = value
-        return self
-
-    def with_offset(self, value: int) -> ListServerClient:
-        self.offset = value
+    def with_namespace(self, value: str) -> RegisterServer:
+        self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ModelsRegisterServerRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "region") and self.region:
-            result["region"] = str(self.region)
-        elif include_empty:
-            result["region"] = ""
-        if hasattr(self, "count") and self.count:
-            result["count"] = int(self.count)
-        elif include_empty:
-            result["count"] = 0
-        if hasattr(self, "offset") and self.offset:
-            result["offset"] = int(self.offset)
-        elif include_empty:
-            result["offset"] = 0
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelsListServerResponse], Union[None, HttpResponse, ResponseError]
-    ]:
+    ) -> Tuple[Union[None, ModelsServer], Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsListServerResponse (servers listed)
+        200: OK - ModelsServer (server registered)
+
+        400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
+        404: Not Found - ResponseError (allocation not found)
+
+        409: Conflict - ResponseError (server with same name already registered)
+
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -227,82 +225,70 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelsListServerResponse.create_from_dict(content), None
+            return ModelsServer.create_from_dict(content), None
+        if code == 400:
+            return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
+        if code == 404:
+            return None, ResponseError.create_from_dict(content)
+        if code == 409:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls,
-        namespace: str,
-        count: int,
-        offset: int,
-        region: Optional[str] = None,
-        **kwargs,
-    ) -> ListServerClient:
+        cls, body: ModelsRegisterServerRequest, namespace: str, **kwargs
+    ) -> RegisterServer:
         instance = cls()
+        instance.body = body
         instance.namespace = namespace
-        instance.count = count
-        instance.offset = offset
-        if region is not None:
-            instance.region = region
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> ListServerClient:
+    ) -> RegisterServer:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsRegisterServerRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ModelsRegisterServerRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "region" in dict_ and dict_["region"] is not None:
-            instance.region = str(dict_["region"])
-        elif include_empty:
-            instance.region = ""
-        if "count" in dict_ and dict_["count"] is not None:
-            instance.count = int(dict_["count"])
-        elif include_empty:
-            instance.count = 0
-        if "offset" in dict_ and dict_["offset"] is not None:
-            instance.offset = int(dict_["offset"])
-        elif include_empty:
-            instance.offset = 0
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "namespace": "namespace",
-            "region": "region",
-            "count": "count",
-            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "namespace": True,
-            "region": False,
-            "count": True,
-            "offset": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/register_local_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/register_local_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,32 +84,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/servers/local/register"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/local/register"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsRegisterLocalServerRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/register_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/shutdown_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,90 +25,95 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsRegisterServerRequest
-from ...models import ModelsServer
+from ...models import ModelsShutdownServerRequest
 from ...models import ResponseError
 
 
-class RegisterServer(Operation):
-    """Register a DS (RegisterServer)
+class ShutdownServer(Operation):
+    """Mark a DS is shutting down (ShutdownServer)
 
-    ```
     Required permission: NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
-    Required scope: social
 
-    This endpoint is intended to be called by dedicated server to let DSM know that it is ready for use.
-    This MUST be called by DS after it is ready to accept match data and incoming client connections.
+    Required scope: social
 
-    Upon successfully calling this endpoint, the dedicated
-    server is listed under READY servers.```
+    This endpoint is intended to be called by dedicated server to let DSM know that it is shutting down. Calling this will remove the server and session records from DB.Set 'kill_me' in request to 'true' if the DS cannot shut itself down.
 
     Required Permission(s):
         - NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/servers/register
+        url: /dsmcontroller/namespaces/{namespace}/servers/shutdown
 
         method: POST
 
         tags: ["Server"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsRegisterServerRequest in body
+        body: (body) REQUIRED ModelsShutdownServerRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsServer (server registered)
+        204: No Content - (server removed)
 
         400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (allocation not found)
-
-        409: Conflict - ResponseError (server with same name already registered)
+        404: Not Found - ResponseError (server not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/servers/register"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/servers/shutdown"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/shutdown"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsRegisterServerRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "dsmc"
+
+    body: ModelsShutdownServerRequest  # REQUIRED in [body]
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
 
@@ -153,57 +158,55 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsRegisterServerRequest) -> RegisterServer:
+    def with_body(self, value: ModelsShutdownServerRequest) -> ShutdownServer:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> RegisterServer:
+    def with_namespace(self, value: str) -> ShutdownServer:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsRegisterServerRequest()
+            result["body"] = ModelsShutdownServerRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[Union[None, ModelsServer], Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        200: OK - ModelsServer (server registered)
+        204: No Content - (server removed)
 
         400: Bad Request - ResponseError (malformed request)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (allocation not found)
-
-        409: Conflict - ResponseError (server with same name already registered)
+        404: Not Found - ResponseError (server not found)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -212,57 +215,55 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelsServer.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
-        if code == 409:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsRegisterServerRequest, namespace: str, **kwargs
-    ) -> RegisterServer:
+        cls, body: ModelsShutdownServerRequest, namespace: str, **kwargs
+    ) -> ShutdownServer:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> RegisterServer:
+    ) -> ShutdownServer:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsRegisterServerRequest.create_from_dict(
+            instance.body = ModelsShutdownServerRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsRegisterServerRequest()
+            instance.body = ModelsShutdownServerRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/server_heartbeat.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/server/server_heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,32 +82,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/servers/heartbeat"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/servers/heartbeat"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsDSHeartbeatRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/server/shutdown_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/claim_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,83 +25,99 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsShutdownServerRequest
+from ...models import ModelsClaimSessionRequest
 from ...models import ResponseError
 
 
-class ShutdownServer(Operation):
-    """Mark a DS is shutting down (ShutdownServer)
+class ClaimServer(Operation):
+    """Claim a DS for a game session (ClaimServer)
 
-    Required permission: NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
+    Required permission: NAMESPACE:{namespace}:DSM:SESSION [UPDATE]
 
     Required scope: social
 
-    This endpoint is intended to be called by dedicated server to let DSM know that it is shutting down. Calling this will remove the server and session records from DB.Set 'kill_me' in request to 'true' if the DS cannot shut itself down.
+    This endpoint is intended to be called by game session manager (matchmaker, lobby, etc.) to claim a dedicated server. The dedicated server cannot be claimed unless the status is READY
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:DSM:SERVER [UPDATE]
+        - NAMESPACE:{namespace}:DSM:SESSION [UPDATE]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/servers/shutdown
+        url: /dsmcontroller/namespaces/{namespace}/sessions/claim
 
         method: POST
 
-        tags: ["Server"]
+        tags: ["Session"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsShutdownServerRequest in body
+        body: (body) REQUIRED ModelsClaimSessionRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (server removed)
-
-        400: Bad Request - ResponseError (malformed request)
+        204: No Content - (DS claimed for session)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (server not found)
+        404: Not Found - ResponseError (session not found)
+
+        409: Conflict - ResponseError (DS is already claimed)
+
+        425: Too Early - ResponseError (DS is not ready to be claimed)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
+
+        503: Service Unavailable - ResponseError (DS is unreachable)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/servers/shutdown"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/sessions/claim"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/sessions/claim"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsShutdownServerRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "dsmc"
+
+    body: ModelsClaimSessionRequest  # REQUIRED in [body]
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
 
@@ -146,32 +162,32 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsShutdownServerRequest) -> ShutdownServer:
+    def with_body(self, value: ModelsClaimSessionRequest) -> ClaimServer:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> ShutdownServer:
+    def with_namespace(self, value: str) -> ClaimServer:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsShutdownServerRequest()
+            result["body"] = ModelsClaimSessionRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
@@ -180,24 +196,28 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
-        204: No Content - (server removed)
-
-        400: Bad Request - ResponseError (malformed request)
+        204: No Content - (DS claimed for session)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
-        404: Not Found - ResponseError (server not found)
+        404: Not Found - ResponseError (session not found)
+
+        409: Conflict - ResponseError (DS is already claimed)
+
+        425: Too Early - ResponseError (DS is not ready to be claimed)
 
         500: Internal Server Error - ResponseError (Internal Server Error)
 
+        503: Service Unavailable - ResponseError (DS is unreachable)
+
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
@@ -205,53 +225,55 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 204:
             return None, None
-        if code == 400:
-            return None, ResponseError.create_from_dict(content)
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
+        if code == 409:
+            return None, ResponseError.create_from_dict(content)
+        if code == 425:
+            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
+        if code == 503:
+            return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsShutdownServerRequest, namespace: str, **kwargs
-    ) -> ShutdownServer:
+        cls, body: ModelsClaimSessionRequest, namespace: str, **kwargs
+    ) -> ClaimServer:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> ShutdownServer:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ClaimServer:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsShutdownServerRequest.create_from_dict(
+            instance.body = ModelsClaimSessionRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsShutdownServerRequest()
+            instance.body = ModelsClaimSessionRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/cancel_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/cancel_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,32 +75,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/sessions/{sessionID}/cancel"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/sessions/{sessionID}/cancel"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
     session_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/claim_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/get_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,87 +25,95 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsClaimSessionRequest
+from ...models import ModelsSessionResponse
 from ...models import ResponseError
 
 
-class ClaimServer(Operation):
-    """Claim a DS for a game session (ClaimServer)
+class GetSession(Operation):
+    """Query specified session (GetSession)
 
-    Required permission: NAMESPACE:{namespace}:DSM:SESSION [UPDATE]
+    Required permission: NAMESPACE:{namespace}:DSM:SESSION [READ]
 
     Required scope: social
 
-    This endpoint is intended to be called by game session manager (matchmaker, lobby, etc.) to claim a dedicated server. The dedicated server cannot be claimed unless the status is READY
+    This endpoint is intended to be called by game session manager (matchmaker, lobby, etc.) to query the status of dedicated server that is created for the session.
+
+    The server is ready to use when the status is READY. At which point, the game session manager can claim the server using the GET /namespaces/{namespace}/sessions/{sessionID}/claim endpoint
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:DSM:SESSION [UPDATE]
+        - NAMESPACE:{namespace}:DSM:SESSION [READ]
 
     Required Scope(s):
         - social
 
     Properties:
-        url: /dsmcontroller/namespaces/{namespace}/sessions/claim
+        url: /dsmcontroller/namespaces/{namespace}/sessions/{sessionID}
 
-        method: POST
+        method: GET
 
         tags: ["Session"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsClaimSessionRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
+        session_id: (sessionID) REQUIRED str in path
+
     Responses:
-        204: No Content - (DS claimed for session)
+        200: OK - ModelsSessionResponse (session queried)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         404: Not Found - ResponseError (session not found)
 
-        409: Conflict - ResponseError (DS is already claimed)
-
-        425: Too Early - ResponseError (DS is not ready to be claimed)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
-
-        503: Service Unavailable - ResponseError (DS is unreachable)
     """
 
     # region fields
 
-    _url: str = "/dsmcontroller/namespaces/{namespace}/sessions/claim"
-    _method: str = "POST"
+    _url: str = "/dsmcontroller/namespaces/{namespace}/sessions/{sessionID}"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/sessions/{sessionID}"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsClaimSessionRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "dsmc"
+
     namespace: str  # REQUIRED in [path]
+    session_id: str  # REQUIRED in [path]
 
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
 
@@ -127,155 +135,137 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
-            "body": self.get_body_params(),
             "path": self.get_path_params(),
         }
 
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "session_id"):
+            result["sessionID"] = self.session_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsClaimSessionRequest) -> ClaimServer:
-        self.body = value
+    def with_namespace(self, value: str) -> GetSession:
+        self.namespace = value
         return self
 
-    def with_namespace(self, value: str) -> ClaimServer:
-        self.namespace = value
+    def with_session_id(self, value: str) -> GetSession:
+        self.session_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsClaimSessionRequest()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "session_id") and self.session_id:
+            result["sessionID"] = str(self.session_id)
+        elif include_empty:
+            result["sessionID"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
+    ) -> Tuple[
+        Union[None, ModelsSessionResponse], Union[None, HttpResponse, ResponseError]
+    ]:
         """Parse the given response.
 
-        204: No Content - (DS claimed for session)
+        200: OK - ModelsSessionResponse (session queried)
 
         401: Unauthorized - ResponseError (Unauthorized)
 
         404: Not Found - ResponseError (session not found)
 
-        409: Conflict - ResponseError (DS is already claimed)
-
-        425: Too Early - ResponseError (DS is not ready to be claimed)
-
         500: Internal Server Error - ResponseError (Internal Server Error)
 
-        503: Service Unavailable - ResponseError (DS is unreachable)
-
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ModelsSessionResponse.create_from_dict(content), None
         if code == 401:
             return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
-        if code == 409:
-            return None, ResponseError.create_from_dict(content)
-        if code == 425:
-            return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
-        if code == 503:
-            return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, body: ModelsClaimSessionRequest, namespace: str, **kwargs
-    ) -> ClaimServer:
+    def create(cls, namespace: str, session_id: str, **kwargs) -> GetSession:
         instance = cls()
-        instance.body = body
         instance.namespace = namespace
+        instance.session_id = session_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ClaimServer:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> GetSession:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsClaimSessionRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsClaimSessionRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "sessionID" in dict_ and dict_["sessionID"] is not None:
+            instance.session_id = str(dict_["sessionID"])
+        elif include_empty:
+            instance.session_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
             "namespace": "namespace",
+            "sessionID": "session_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
             "namespace": True,
+            "sessionID": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/operations/session/create_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/operations/session/create_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,32 +87,44 @@
 
         503: Service Unavailable - ResponseError (server count is at max)
     """
 
     # region fields
 
     _url: str = "/dsmcontroller/namespaces/{namespace}/sessions"
+    _path: str = "/dsmcontroller/namespaces/{namespace}/sessions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "dsmc"
+
     body: ModelsCreateSessionRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/__init__.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_admin.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_admin.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_deployment_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_deployment_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_dsmc_operations.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_dsmc_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_image_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_image_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_pod_config.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_pod_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_public.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_public.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_server.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk/api/dsmc/wrappers/_session.py` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk/api/dsmc/wrappers/_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-dsmc
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Dsm Controller Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-dsmc-0.7.0/accelbyte_py_sdk_service_dsmc.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_dsmc-0.8.0/accelbyte_py_sdk_service_dsmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

