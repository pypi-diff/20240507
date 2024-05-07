# Comparing `tmp/accelbyte-py-sdk-service-ams-0.7.0.tar.gz` & `tmp/accelbyte_py_sdk_service_ams-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-ams-0.7.0.tar", last modified: Tue Mar 26 05:39:59 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_ams-0.8.0.tar", last modified: Tue May  7 06:25:47 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-ams-0.7.0.tar` & `accelbyte_py_sdk_service_ams-0.8.0.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.570694 accelbyte-py-sdk-service-ams-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-03-26 05:39:59.570694 accelbyte-py-sdk-service-ams-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      843 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.558694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.558694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.558694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/
--rw-rw-r--   0 root         (0) root         (0)     4248 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.562694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/
--rw-rw-r--   0 root         (0) root         (0)     3890 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3712 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     5933 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     7626 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py
--rw-rw-r--   0 root         (0) root         (0)     3710 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py
--rw-rw-r--   0 root         (0) root         (0)     5905 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py
--rw-rw-r--   0 root         (0) root         (0)     3777 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py
--rw-rw-r--   0 root         (0) root         (0)     5831 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_response.py
--rw-rw-r--   0 root         (0) root         (0)     3872 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    10866 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py
--rw-rw-r--   0 root         (0) root         (0)     4484 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5109 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py
--rw-rw-r--   0 root         (0) root         (0)     3681 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py
--rw-rw-r--   0 root         (0) root         (0)     5325 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py
--rw-rw-r--   0 root         (0) root         (0)     4810 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py
--rw-rw-r--   0 root         (0) root         (0)     5415 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     3992 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py
--rw-rw-r--   0 root         (0) root         (0)     7606 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py
--rw-rw-r--   0 root         (0) root         (0)     4833 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py
--rw-rw-r--   0 root         (0) root         (0)     5335 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     5170 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py
--rw-rw-r--   0 root         (0) root         (0)     5243 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py
--rw-rw-r--   0 root         (0) root         (0)     4317 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py
--rw-rw-r--   0 root         (0) root         (0)     5630 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py
--rw-rw-r--   0 root         (0) root         (0)     3672 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     9876 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py
--rw-rw-r--   0 root         (0) root         (0)     7967 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py
--rw-rw-r--   0 root         (0) root         (0)     4174 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     9957 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py
--rw-rw-r--   0 root         (0) root         (0)     7934 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py
--rw-rw-r--   0 root         (0) root         (0)     6137 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     7978 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py
--rw-rw-r--   0 root         (0) root         (0)     4354 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py
--rw-rw-r--   0 root         (0) root         (0)    12550 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     5362 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py
--rw-rw-r--   0 root         (0) root         (0)     6671 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py
--rw-rw-r--   0 root         (0) root         (0)    10824 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_details.py
--rw-rw-r--   0 root         (0) root         (0)     3917 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_list.py
--rw-rw-r--   0 root         (0) root         (0)    10462 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py
--rw-rw-r--   0 root         (0) root         (0)     5849 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_update.py
--rw-rw-r--   0 root         (0) root         (0)     7271 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py
--rw-rw-r--   0 root         (0) root         (0)     8240 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py
--rw-rw-r--   0 root         (0) root         (0)     4323 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4066 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py
--rw-rw-r--   0 root         (0) root         (0)     6600 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py
--rw-rw-r--   0 root         (0) root         (0)     5104 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py
--rw-rw-r--   0 root         (0) root         (0)     5941 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_region_config.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_time.py
--rw-rw-r--   0 root         (0) root         (0)     5513 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_timeout.py
--rw-rw-r--   0 root         (0) root         (0)     3741 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py
--rw-rw-r--   0 root         (0) root         (0)     5191 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/response_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     7999 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_location.py
--rw-rw-r--   0 root         (0) root         (0)     4688 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_zone.py
--rw-rw-r--   0 root         (0) root         (0)     5338 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.562694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/
--rw-rw-r--   0 root         (0) root         (0)      410 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.562694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/
--rw-rw-r--   0 root         (0) root         (0)      715 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6553 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py
--rw-rw-r--   0 root         (0) root         (0)     6622 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py
--rw-rw-r--   0 root         (0) root         (0)     6907 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py
--rw-rw-r--   0 root         (0) root         (0)     7762 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.562694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/
--rw-rw-r--   0 root         (0) root         (0)      583 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6347 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py
--rw-rw-r--   0 root         (0) root         (0)     6502 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py
--rw-rw-r--   0 root         (0) root         (0)     4203 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.562694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/
--rw-rw-r--   0 root         (0) root         (0)      537 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py
--rw-rw-r--   0 root         (0) root         (0)     8653 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/
--rw-rw-r--   0 root         (0) root         (0)      767 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7648 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py
--rw-rw-r--   0 root         (0) root         (0)    16707 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py
--rw-rw-r--   0 root         (0) root         (0)     7776 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py
--rw-rw-r--   0 root         (0) root         (0)     6440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py
--rw-rw-r--   0 root         (0) root         (0)     7878 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py
--rw-rw-r--   0 root         (0) root         (0)     8932 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/auth/
--rw-rw-r--   0 root         (0) root         (0)      477 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/
--rw-rw-r--   0 root         (0) root         (0)      762 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8187 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py
--rw-rw-r--   0 root         (0) root         (0)     8472 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py
--rw-rw-r--   0 root         (0) root         (0)     6811 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py
--rw-rw-r--   0 root         (0) root         (0)     8494 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/
--rw-rw-r--   0 root         (0) root         (0)      568 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4189 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py
--rw-rw-r--   0 root         (0) root         (0)     4139 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py
--rw-rw-r--   0 root         (0) root         (0)     4201 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/
--rw-rw-r--   0 root         (0) root         (0)      759 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8657 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py
--rw-rw-r--   0 root         (0) root         (0)     8020 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py
--rw-rw-r--   0 root         (0) root         (0)     7673 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py
--rw-rw-r--   0 root         (0) root         (0)     7400 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py
--rw-rw-r--   0 root         (0) root         (0)     7521 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py
--rw-rw-r--   0 root         (0) root         (0)     5829 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py
--rw-rw-r--   0 root         (0) root         (0)     7609 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py
--rw-rw-r--   0 root         (0) root         (0)     8551 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/
--rw-rw-r--   0 root         (0) root         (0)      545 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7284 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py
--rw-rw-r--   0 root         (0) root         (0)     6651 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py
--rw-rw-r--   0 root         (0) root         (0)     8426 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/
--rw-rw-r--   0 root         (0) root         (0)      653 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7621 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py
--rw-rw-r--   0 root         (0) root         (0)    13265 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py
--rw-rw-r--   0 root         (0) root         (0)     7467 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py
--rw-rw-r--   0 root         (0) root         (0)     7461 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.566694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/
--rw-rw-r--   0 root         (0) root         (0)      546 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6287 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py
--rw-rw-r--   0 root         (0) root         (0)     6212 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.570694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4219 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16497 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_account.py
--rw-rw-r--   0 root         (0) root         (0)     7740 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py
--rw-rw-r--   0 root         (0) root         (0)     9299 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py
--rw-rw-r--   0 root         (0) root         (0)    23216 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py
--rw-rw-r--   0 root         (0) root         (0)     2878 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py
--rw-rw-r--   0 root         (0) root         (0)    15202 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_development.py
--rw-rw-r--   0 root         (0) root         (0)     4481 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py
--rw-rw-r--   0 root         (0) root         (0)    25867 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py
--rw-rw-r--   0 root         (0) root         (0)    10383 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_images.py
--rw-rw-r--   0 root         (0) root         (0)    15196 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py
--rw-rw-r--   0 root         (0) root         (0)     5840 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:39:59.570694 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-03-26 05:39:59.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7713 2024-03-26 05:39:59.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:39:59.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:39:59.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:39:59.000000 accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      329 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-ams-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:39:59.570694 accelbyte-py-sdk-service-ams-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      843 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.709260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/
+-rw-rw-r--   0 root         (0) root         (0)     4248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/
+-rw-rw-r--   0 root         (0) root         (0)     4009 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3712 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5933 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7626 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py
+-rw-rw-r--   0 root         (0) root         (0)     3710 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5905 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3777 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5831 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3872 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4484 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5109 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     3681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4810 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5643 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3992 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5300 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7606 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py
+-rw-rw-r--   0 root         (0) root         (0)     4833 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py
+-rw-rw-r--   0 root         (0) root         (0)     5335 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     5170 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     5243 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py
+-rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py
+-rw-rw-r--   0 root         (0) root         (0)     5630 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3672 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10552 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4174 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    10632 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py
+-rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py
+-rw-rw-r--   0 root         (0) root         (0)     6137 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7978 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13441 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5362 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py
+-rw-rw-r--   0 root         (0) root         (0)    10824 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3917 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list.py
+-rw-rw-r--   0 root         (0) root         (0)    10462 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py
+-rw-rw-r--   0 root         (0) root         (0)     5849 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_update.py
+-rw-rw-r--   0 root         (0) root         (0)     7271 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8240 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4323 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4066 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6600 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py
+-rw-rw-r--   0 root         (0) root         (0)     5104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py
+-rw-rw-r--   0 root         (0) root         (0)     5941 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_region_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_time.py
+-rw-rw-r--   0 root         (0) root         (0)     5513 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     3741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5191 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/response_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_location.py
+-rw-rw-r--   0 root         (0) root         (0)     4688 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone.py
+-rw-rw-r--   0 root         (0) root         (0)     5338 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/
+-rw-rw-r--   0 root         (0) root         (0)      410 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.713260 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6823 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py
+-rw-rw-r--   0 root         (0) root         (0)     7829 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6898 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py
+-rw-rw-r--   0 root         (0) root         (0)     7188 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/
+-rw-rw-r--   0 root         (0) root         (0)      583 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py
+-rw-rw-r--   0 root         (0) root         (0)     6790 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/
+-rw-rw-r--   0 root         (0) root         (0)      537 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/
+-rw-rw-r--   0 root         (0) root         (0)      767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py
+-rw-rw-r--   0 root         (0) root         (0)    16985 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8071 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py
+-rw-rw-r--   0 root         (0) root         (0)     6724 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py
+-rw-rw-r--   0 root         (0) root         (0)     8204 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py
+-rw-rw-r--   0 root         (0) root         (0)     9258 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/
+-rw-rw-r--   0 root         (0) root         (0)      477 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5321 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/
+-rw-rw-r--   0 root         (0) root         (0)      762 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py
+-rw-rw-r--   0 root         (0) root         (0)     8782 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py
+-rw-rw-r--   0 root         (0) root         (0)     8819 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py
+-rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/
+-rw-rw-r--   0 root         (0) root         (0)      568 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4429 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py
+-rw-rw-r--   0 root         (0) root         (0)     4383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py
+-rw-rw-r--   0 root         (0) root         (0)     4445 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8942 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py
+-rw-rw-r--   0 root         (0) root         (0)     8296 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py
+-rw-rw-r--   0 root         (0) root         (0)     7948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py
+-rw-rw-r--   0 root         (0) root         (0)     7685 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py
+-rw-rw-r--   0 root         (0) root         (0)     7806 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py
+-rw-rw-r--   0 root         (0) root         (0)     6104 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py
+-rw-rw-r--   0 root         (0) root         (0)     7902 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py
+-rw-rw-r--   0 root         (0) root         (0)     8836 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/
+-rw-rw-r--   0 root         (0) root         (0)      545 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7569 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py
+-rw-rw-r--   0 root         (0) root         (0)     6926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8711 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py
+-rw-rw-r--   0 root         (0) root         (0)    13566 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py
+-rw-rw-r--   0 root         (0) root         (0)     7754 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7756 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.717259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/
+-rw-rw-r--   0 root         (0) root         (0)      546 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6576 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py
+-rw-rw-r--   0 root         (0) root         (0)     6505 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4219 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_account.py
+-rw-rw-r--   0 root         (0) root         (0)     7740 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9299 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py
+-rw-rw-r--   0 root         (0) root         (0)    23216 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py
+-rw-rw-r--   0 root         (0) root         (0)     2878 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py
+-rw-rw-r--   0 root         (0) root         (0)    15713 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_development.py
+-rw-rw-r--   0 root         (0) root         (0)     4481 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py
+-rw-rw-r--   0 root         (0) root         (0)    25867 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py
+-rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_images.py
+-rw-rw-r--   0 root         (0) root         (0)    15196 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py
+-rw-rw-r--   0 root         (0) root         (0)     5840 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7799 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:25:47.000000 accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      329 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_ams-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:25:47.721259 accelbyte_py_sdk_service_ams-0.8.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/PKG-INFO` & `accelbyte_py_sdk_service_ams-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ams
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - Fleet Commander
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.13.0
+* Version: 1.17.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/README.md` & `accelbyte_py_sdk_service_ams-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.13.0
+* Version: 1.17.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # account
 from .wrappers import account_get
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .api_account_create_request import ApiAccountCreateRequest
 from .api_account_create_response import ApiAccountCreateResponse
@@ -34,14 +34,17 @@
 )
 from .api_development_server_configuration_create_response import (
     ApiDevelopmentServerConfigurationCreateResponse,
 )
 from .api_development_server_configuration_get_response import (
     ApiDevelopmentServerConfigurationGetResponse,
 )
+from .api_development_server_configuration_list_response import (
+    ApiDevelopmentServerConfigurationListResponse,
+)
 from .api_ds_history_event import ApiDSHistoryEvent
 from .api_ds_history_list import ApiDSHistoryList
 from .api_ds_host_configuration import ApiDSHostConfiguration
 from .api_fleet_artifacts_sample_rules import ApiFleetArtifactsSampleRules
 from .api_fleet_claim_by_keys_req import ApiFleetClaimByKeysReq
 from .api_fleet_claim_req import ApiFleetClaimReq
 from .api_fleet_claim_response import ApiFleetClaimResponse
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_limits.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_link_token_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_account_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_account_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ams_regions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_sampling_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 from accelbyte_py_sdk.core import Model
 
 
 class ApiDevelopmentServerConfigurationCreateRequest(Model):
     """Api development server configuration create request (api.DevelopmentServerConfigurationCreateRequest)
 
     Properties:
-        command_line: (commandLine) REQUIRED str
+        command_line_arguments: (commandLineArguments) REQUIRED str
 
         image_id: (imageId) REQUIRED str
 
         name: (name) REQUIRED str
     """
 
     # region fields
 
-    command_line: str  # REQUIRED
+    command_line_arguments: str  # REQUIRED
     image_id: str  # REQUIRED
     name: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_command_line(
+    def with_command_line_arguments(
         self, value: str
     ) -> ApiDevelopmentServerConfigurationCreateRequest:
-        self.command_line = value
+        self.command_line_arguments = value
         return self
 
     def with_image_id(
         self, value: str
     ) -> ApiDevelopmentServerConfigurationCreateRequest:
         self.image_id = value
         return self
@@ -67,18 +67,18 @@
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "command_line"):
-            result["commandLine"] = str(self.command_line)
+        if hasattr(self, "command_line_arguments"):
+            result["commandLineArguments"] = str(self.command_line_arguments)
         elif include_empty:
-            result["commandLine"] = ""
+            result["commandLineArguments"] = ""
         if hasattr(self, "image_id"):
             result["imageId"] = str(self.image_id)
         elif include_empty:
             result["imageId"] = ""
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
@@ -87,33 +87,36 @@
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, command_line: str, image_id: str, name: str, **kwargs
+        cls, command_line_arguments: str, image_id: str, name: str, **kwargs
     ) -> ApiDevelopmentServerConfigurationCreateRequest:
         instance = cls()
-        instance.command_line = command_line
+        instance.command_line_arguments = command_line_arguments
         instance.image_id = image_id
         instance.name = name
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApiDevelopmentServerConfigurationCreateRequest:
         instance = cls()
         if not dict_:
             return instance
-        if "commandLine" in dict_ and dict_["commandLine"] is not None:
-            instance.command_line = str(dict_["commandLine"])
+        if (
+            "commandLineArguments" in dict_
+            and dict_["commandLineArguments"] is not None
+        ):
+            instance.command_line_arguments = str(dict_["commandLineArguments"])
         elif include_empty:
-            instance.command_line = ""
+            instance.command_line_arguments = ""
         if "imageId" in dict_ and dict_["imageId"] is not None:
             instance.image_id = str(dict_["imageId"])
         elif include_empty:
             instance.image_id = ""
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
@@ -157,21 +160,21 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "commandLine": "command_line",
+            "commandLineArguments": "command_line_arguments",
             "imageId": "image_id",
             "name": "name",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "commandLine": True,
+            "commandLineArguments": True,
             "imageId": True,
             "name": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 from accelbyte_py_sdk.core import Model
 
 
 class ApiDevelopmentServerConfigurationGetResponse(Model):
     """Api development server configuration get response (api.DevelopmentServerConfigurationGetResponse)
 
     Properties:
-        command_line: (commandLine) REQUIRED str
+        command_line_arguments: (commandLineArguments) REQUIRED str
 
         image_id: (imageId) REQUIRED str
 
         name: (name) REQUIRED str
     """
 
     # region fields
 
-    command_line: str  # REQUIRED
+    command_line_arguments: str  # REQUIRED
     image_id: str  # REQUIRED
     name: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
-    def with_command_line(
+    def with_command_line_arguments(
         self, value: str
     ) -> ApiDevelopmentServerConfigurationGetResponse:
-        self.command_line = value
+        self.command_line_arguments = value
         return self
 
     def with_image_id(self, value: str) -> ApiDevelopmentServerConfigurationGetResponse:
         self.image_id = value
         return self
 
     def with_name(self, value: str) -> ApiDevelopmentServerConfigurationGetResponse:
@@ -65,18 +65,18 @@
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "command_line"):
-            result["commandLine"] = str(self.command_line)
+        if hasattr(self, "command_line_arguments"):
+            result["commandLineArguments"] = str(self.command_line_arguments)
         elif include_empty:
-            result["commandLine"] = ""
+            result["commandLineArguments"] = ""
         if hasattr(self, "image_id"):
             result["imageId"] = str(self.image_id)
         elif include_empty:
             result["imageId"] = ""
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
@@ -85,33 +85,36 @@
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, command_line: str, image_id: str, name: str, **kwargs
+        cls, command_line_arguments: str, image_id: str, name: str, **kwargs
     ) -> ApiDevelopmentServerConfigurationGetResponse:
         instance = cls()
-        instance.command_line = command_line
+        instance.command_line_arguments = command_line_arguments
         instance.image_id = image_id
         instance.name = name
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApiDevelopmentServerConfigurationGetResponse:
         instance = cls()
         if not dict_:
             return instance
-        if "commandLine" in dict_ and dict_["commandLine"] is not None:
-            instance.command_line = str(dict_["commandLine"])
+        if (
+            "commandLineArguments" in dict_
+            and dict_["commandLineArguments"] is not None
+        ):
+            instance.command_line_arguments = str(dict_["commandLineArguments"])
         elif include_empty:
-            instance.command_line = ""
+            instance.command_line_arguments = ""
         if "imageId" in dict_ and dict_["imageId"] is not None:
             instance.image_id = str(dict_["imageId"])
         elif include_empty:
             instance.image_id = ""
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
@@ -155,21 +158,21 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "commandLine": "command_line",
+            "commandLineArguments": "command_line_arguments",
             "imageId": "image_id",
             "name": "name",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "commandLine": True,
+            "commandLineArguments": True,
             "imageId": True,
             "name": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_event.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_history_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_get_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,26 +46,29 @@
 
         image_deployment_profile: (imageDeploymentProfile) REQUIRED ApiImageDeploymentProfile
 
         is_local: (isLocal) REQUIRED bool
 
         name: (name) REQUIRED str
 
+        on_demand: (onDemand) REQUIRED bool
+
         regions: (regions) REQUIRED List[ApiRegionConfig]
     """
 
     # region fields
 
     active: bool  # REQUIRED
     claim_keys: List[str]  # REQUIRED
     ds_host_configuration: ApiDSHostConfiguration  # REQUIRED
     id_: str  # REQUIRED
     image_deployment_profile: ApiImageDeploymentProfile  # REQUIRED
     is_local: bool  # REQUIRED
     name: str  # REQUIRED
+    on_demand: bool  # REQUIRED
     regions: List[ApiRegionConfig]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_active(self, value: bool) -> ApiFleetGetResponse:
@@ -96,14 +99,18 @@
         self.is_local = value
         return self
 
     def with_name(self, value: str) -> ApiFleetGetResponse:
         self.name = value
         return self
 
+    def with_on_demand(self, value: bool) -> ApiFleetGetResponse:
+        self.on_demand = value
+        return self
+
     def with_regions(self, value: List[ApiRegionConfig]) -> ApiFleetGetResponse:
         self.regions = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -138,14 +145,18 @@
             result["isLocal"] = bool(self.is_local)
         elif include_empty:
             result["isLocal"] = False
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
+        if hasattr(self, "on_demand"):
+            result["onDemand"] = bool(self.on_demand)
+        elif include_empty:
+            result["onDemand"] = False
         if hasattr(self, "regions"):
             result["regions"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.regions
             ]
         elif include_empty:
             result["regions"] = []
         return result
@@ -160,25 +171,27 @@
         active: bool,
         claim_keys: List[str],
         ds_host_configuration: ApiDSHostConfiguration,
         id_: str,
         image_deployment_profile: ApiImageDeploymentProfile,
         is_local: bool,
         name: str,
+        on_demand: bool,
         regions: List[ApiRegionConfig],
         **kwargs,
     ) -> ApiFleetGetResponse:
         instance = cls()
         instance.active = active
         instance.claim_keys = claim_keys
         instance.ds_host_configuration = ds_host_configuration
         instance.id_ = id_
         instance.image_deployment_profile = image_deployment_profile
         instance.is_local = is_local
         instance.name = name
+        instance.on_demand = on_demand
         instance.regions = regions
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApiFleetGetResponse:
@@ -218,14 +231,18 @@
             instance.is_local = bool(dict_["isLocal"])
         elif include_empty:
             instance.is_local = False
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
+        if "onDemand" in dict_ and dict_["onDemand"] is not None:
+            instance.on_demand = bool(dict_["onDemand"])
+        elif include_empty:
+            instance.on_demand = False
         if "regions" in dict_ and dict_["regions"] is not None:
             instance.regions = [
                 ApiRegionConfig.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["regions"]
             ]
         elif include_empty:
             instance.regions = []
@@ -273,24 +290,26 @@
             "active": "active",
             "claimKeys": "claim_keys",
             "dsHostConfiguration": "ds_host_configuration",
             "id": "id_",
             "imageDeploymentProfile": "image_deployment_profile",
             "isLocal": "is_local",
             "name": "name",
+            "onDemand": "on_demand",
             "regions": "regions",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "active": True,
             "claimKeys": True,
             "dsHostConfiguration": True,
             "id": True,
             "imageDeploymentProfile": True,
             "isLocal": True,
             "name": True,
+            "onDemand": True,
             "regions": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_item_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 
         image: (image) REQUIRED str
 
         is_local: (isLocal) REQUIRED bool
 
         name: (name) REQUIRED str
 
+        on_demand: (onDemand) REQUIRED bool
+
         regions: (regions) REQUIRED List[str]
     """
 
     # region fields
 
     active: bool  # REQUIRED
     counts: List[ApiFleetRegionalServerCounts]  # REQUIRED
     id_: str  # REQUIRED
     image: str  # REQUIRED
     is_local: bool  # REQUIRED
     name: str  # REQUIRED
+    on_demand: bool  # REQUIRED
     regions: List[str]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_active(self, value: bool) -> ApiFleetListItemResponse:
@@ -85,14 +88,18 @@
         self.is_local = value
         return self
 
     def with_name(self, value: str) -> ApiFleetListItemResponse:
         self.name = value
         return self
 
+    def with_on_demand(self, value: bool) -> ApiFleetListItemResponse:
+        self.on_demand = value
+        return self
+
     def with_regions(self, value: List[str]) -> ApiFleetListItemResponse:
         self.regions = value
         return self
 
     # endregion with_x methods
 
     # region to methods
@@ -121,14 +128,18 @@
             result["isLocal"] = bool(self.is_local)
         elif include_empty:
             result["isLocal"] = False
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
+        if hasattr(self, "on_demand"):
+            result["onDemand"] = bool(self.on_demand)
+        elif include_empty:
+            result["onDemand"] = False
         if hasattr(self, "regions"):
             result["regions"] = [str(i0) for i0 in self.regions]
         elif include_empty:
             result["regions"] = []
         return result
 
     # endregion to methods
@@ -140,24 +151,26 @@
         cls,
         active: bool,
         counts: List[ApiFleetRegionalServerCounts],
         id_: str,
         image: str,
         is_local: bool,
         name: str,
+        on_demand: bool,
         regions: List[str],
         **kwargs,
     ) -> ApiFleetListItemResponse:
         instance = cls()
         instance.active = active
         instance.counts = counts
         instance.id_ = id_
         instance.image = image
         instance.is_local = is_local
         instance.name = name
+        instance.on_demand = on_demand
         instance.regions = regions
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApiFleetListItemResponse:
@@ -189,14 +202,18 @@
             instance.is_local = bool(dict_["isLocal"])
         elif include_empty:
             instance.is_local = False
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
+        if "onDemand" in dict_ and dict_["onDemand"] is not None:
+            instance.on_demand = bool(dict_["onDemand"])
+        elif include_empty:
+            instance.on_demand = False
         if "regions" in dict_ and dict_["regions"] is not None:
             instance.regions = [str(i0) for i0 in dict_["regions"]]
         elif include_empty:
             instance.regions = []
         return instance
 
     @classmethod
@@ -242,23 +259,25 @@
         return {
             "active": "active",
             "counts": "counts",
             "id": "id_",
             "image": "image",
             "isLocal": "is_local",
             "name": "name",
+            "onDemand": "on_demand",
             "regions": "regions",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "active": True,
             "counts": True,
             "id": True,
             "image": True,
             "isLocal": True,
             "name": True,
+            "onDemand": True,
             "regions": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,30 @@
 
         ds_host_configuration: (dsHostConfiguration) REQUIRED ApiDSHostConfiguration
 
         image_deployment_profile: (imageDeploymentProfile) REQUIRED ApiImageDeploymentProfile
 
         name: (name) REQUIRED str
 
+        on_demand: (onDemand) REQUIRED bool
+
         regions: (regions) REQUIRED List[ApiRegionConfig]
 
         claim_keys: (claimKeys) OPTIONAL List[str]
 
         sampling_rules: (samplingRules) OPTIONAL ApiFleetArtifactsSampleRules
     """
 
     # region fields
 
     active: bool  # REQUIRED
     ds_host_configuration: ApiDSHostConfiguration  # REQUIRED
     image_deployment_profile: ApiImageDeploymentProfile  # REQUIRED
     name: str  # REQUIRED
+    on_demand: bool  # REQUIRED
     regions: List[ApiRegionConfig]  # REQUIRED
     claim_keys: List[str]  # OPTIONAL
     sampling_rules: ApiFleetArtifactsSampleRules  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
@@ -82,14 +85,18 @@
         self.image_deployment_profile = value
         return self
 
     def with_name(self, value: str) -> ApiFleetParameters:
         self.name = value
         return self
 
+    def with_on_demand(self, value: bool) -> ApiFleetParameters:
+        self.on_demand = value
+        return self
+
     def with_regions(self, value: List[ApiRegionConfig]) -> ApiFleetParameters:
         self.regions = value
         return self
 
     def with_claim_keys(self, value: List[str]) -> ApiFleetParameters:
         self.claim_keys = value
         return self
@@ -122,14 +129,18 @@
             )
         elif include_empty:
             result["imageDeploymentProfile"] = ApiImageDeploymentProfile()
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
+        if hasattr(self, "on_demand"):
+            result["onDemand"] = bool(self.on_demand)
+        elif include_empty:
+            result["onDemand"] = False
         if hasattr(self, "regions"):
             result["regions"] = [
                 i0.to_dict(include_empty=include_empty) for i0 in self.regions
             ]
         elif include_empty:
             result["regions"] = []
         if hasattr(self, "claim_keys"):
@@ -151,24 +162,26 @@
     @classmethod
     def create(
         cls,
         active: bool,
         ds_host_configuration: ApiDSHostConfiguration,
         image_deployment_profile: ApiImageDeploymentProfile,
         name: str,
+        on_demand: bool,
         regions: List[ApiRegionConfig],
         claim_keys: Optional[List[str]] = None,
         sampling_rules: Optional[ApiFleetArtifactsSampleRules] = None,
         **kwargs,
     ) -> ApiFleetParameters:
         instance = cls()
         instance.active = active
         instance.ds_host_configuration = ds_host_configuration
         instance.image_deployment_profile = image_deployment_profile
         instance.name = name
+        instance.on_demand = on_demand
         instance.regions = regions
         if claim_keys is not None:
             instance.claim_keys = claim_keys
         if sampling_rules is not None:
             instance.sampling_rules = sampling_rules
         return instance
 
@@ -200,14 +213,18 @@
             )
         elif include_empty:
             instance.image_deployment_profile = ApiImageDeploymentProfile()
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
+        if "onDemand" in dict_ and dict_["onDemand"] is not None:
+            instance.on_demand = bool(dict_["onDemand"])
+        elif include_empty:
+            instance.on_demand = False
         if "regions" in dict_ and dict_["regions"] is not None:
             instance.regions = [
                 ApiRegionConfig.create_from_dict(i0, include_empty=include_empty)
                 for i0 in dict_["regions"]
             ]
         elif include_empty:
             instance.regions = []
@@ -262,25 +279,27 @@
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "active": "active",
             "dsHostConfiguration": "ds_host_configuration",
             "imageDeploymentProfile": "image_deployment_profile",
             "name": "name",
+            "onDemand": "on_demand",
             "regions": "regions",
             "claimKeys": "claim_keys",
             "samplingRules": "sampling_rules",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "active": True,
             "dsHostConfiguration": True,
             "imageDeploymentProfile": True,
             "name": True,
+            "onDemand": True,
             "regions": True,
             "claimKeys": False,
             "samplingRules": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_regional_server_counts.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_connection_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_event_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_history_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_server_info_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
         port_configuration: (portConfiguration) REQUIRED List[ApiPortConfiguration]
 
         ports: (ports) REQUIRED Dict[str, int]
 
         region: (region) REQUIRED str
 
+        server_configuration: (serverConfiguration) REQUIRED str
+
         server_id: (serverId) REQUIRED str
 
         session_id: (sessionId) REQUIRED str
 
         status: (status) REQUIRED str
     """
 
@@ -69,14 +71,15 @@
     image_cmd: str  # REQUIRED
     image_id: str  # REQUIRED
     instance_type: str  # REQUIRED
     ip_address: str  # REQUIRED
     port_configuration: List[ApiPortConfiguration]  # REQUIRED
     ports: Dict[str, int]  # REQUIRED
     region: str  # REQUIRED
+    server_configuration: str  # REQUIRED
     server_id: str  # REQUIRED
     session_id: str  # REQUIRED
     status: str  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
@@ -119,14 +122,18 @@
         self.ports = value
         return self
 
     def with_region(self, value: str) -> ApiFleetServerInfoResponse:
         self.region = value
         return self
 
+    def with_server_configuration(self, value: str) -> ApiFleetServerInfoResponse:
+        self.server_configuration = value
+        return self
+
     def with_server_id(self, value: str) -> ApiFleetServerInfoResponse:
         self.server_id = value
         return self
 
     def with_session_id(self, value: str) -> ApiFleetServerInfoResponse:
         self.session_id = value
         return self
@@ -180,14 +187,18 @@
             result["ports"] = {str(k0): int(v0) for k0, v0 in self.ports.items()}
         elif include_empty:
             result["ports"] = {}
         if hasattr(self, "region"):
             result["region"] = str(self.region)
         elif include_empty:
             result["region"] = ""
+        if hasattr(self, "server_configuration"):
+            result["serverConfiguration"] = str(self.server_configuration)
+        elif include_empty:
+            result["serverConfiguration"] = ""
         if hasattr(self, "server_id"):
             result["serverId"] = str(self.server_id)
         elif include_empty:
             result["serverId"] = ""
         if hasattr(self, "session_id"):
             result["sessionId"] = str(self.session_id)
         elif include_empty:
@@ -211,14 +222,15 @@
         image_cmd: str,
         image_id: str,
         instance_type: str,
         ip_address: str,
         port_configuration: List[ApiPortConfiguration],
         ports: Dict[str, int],
         region: str,
+        server_configuration: str,
         server_id: str,
         session_id: str,
         status: str,
         **kwargs,
     ) -> ApiFleetServerInfoResponse:
         instance = cls()
         instance.created_at = created_at
@@ -227,14 +239,15 @@
         instance.image_cmd = image_cmd
         instance.image_id = image_id
         instance.instance_type = instance_type
         instance.ip_address = ip_address
         instance.port_configuration = port_configuration
         instance.ports = ports
         instance.region = region
+        instance.server_configuration = server_configuration
         instance.server_id = server_id
         instance.session_id = session_id
         instance.status = status
         return instance
 
     @classmethod
     def create_from_dict(
@@ -282,14 +295,18 @@
             instance.ports = {str(k0): int(v0) for k0, v0 in dict_["ports"].items()}
         elif include_empty:
             instance.ports = {}
         if "region" in dict_ and dict_["region"] is not None:
             instance.region = str(dict_["region"])
         elif include_empty:
             instance.region = ""
+        if "serverConfiguration" in dict_ and dict_["serverConfiguration"] is not None:
+            instance.server_configuration = str(dict_["serverConfiguration"])
+        elif include_empty:
+            instance.server_configuration = ""
         if "serverId" in dict_ and dict_["serverId"] is not None:
             instance.server_id = str(dict_["serverId"])
         elif include_empty:
             instance.server_id = ""
         if "sessionId" in dict_ and dict_["sessionId"] is not None:
             instance.session_id = str(dict_["sessionId"])
         elif include_empty:
@@ -347,14 +364,15 @@
             "imageCmd": "image_cmd",
             "imageId": "image_id",
             "instanceType": "instance_type",
             "ipAddress": "ip_address",
             "portConfiguration": "port_configuration",
             "ports": "ports",
             "region": "region",
+            "serverConfiguration": "server_configuration",
             "serverId": "server_id",
             "sessionId": "session_id",
             "status": "status",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
@@ -365,13 +383,14 @@
             "imageCmd": True,
             "imageId": True,
             "instanceType": True,
             "ipAddress": True,
             "portConfiguration": True,
             "ports": True,
             "region": True,
+            "serverConfiguration": True,
             "serverId": True,
             "sessionId": True,
             "status": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_fleet_servers_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_deployment_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_details.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_details.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_list.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_list_item.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_image_update.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_image_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_instance_type_description_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_paging_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_port_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_qo_s_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_referencing_fleet.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_region_config.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_region_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_time.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_time.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_timeout.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_timeout.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/api_update_server_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/response_error_response.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/response_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_location.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_location.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_zone.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/models/time_zone_trans.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .account_get import AccountGet
 from .admin_account_create import AdminAccountCreate
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/account_get.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,31 +67,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/namespaces/{namespace}/account"
+    _path: str = "/ams/v1/namespaces/{namespace}/account"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/account"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/account"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiAccountCreateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,31 +67,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/account"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/account"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,31 +69,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/account/link"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/account/link"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/account/admin_account_link_token_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/account/link"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/account/link"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiAccountLinkRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .info_regions import InfoRegions
 from .info_supported_instances import InfoSupportedInstances
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,31 +65,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/regions"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/regions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/info_supported_instances.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,31 +65,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/supported-instances"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/supported-instances"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,53 +26,65 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 
-class UploadURLGet(Operation):
-    """get an URL for uploading an image (UploadURLGet)
+class PortalHealthCheck(Operation):
+    """Health check (PortalHealthCheck)
 
 
     Properties:
-        url: /ams/v1/upload-url
+        url: /ams/healthz
 
         method: GET
 
-        tags: ["AMS Info"]
+        tags: ["Fleet Commander"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - (success)
+        200: OK - (OK)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/upload-url"
+    _url: str = "/ams/healthz"
+    _path: str = "/ams/healthz"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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
 
@@ -121,15 +133,15 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[Union[None, HttpResponse], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - (success)
+        200: OK - (OK)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -148,22 +160,24 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> UploadURLGet:
+    def create(cls, **kwargs) -> PortalHealthCheck:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UploadURLGet:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> PortalHealthCheck:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .qo_s_regions_get import QoSRegionsGet
 from .qo_s_regions_update import QoSRegionsUpdate
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,32 +86,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/qos"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/qos"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_qo_s/qo_s_regions_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,33 +76,45 @@
 
         500: Internal Server Error - ResponseErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/qos/{region}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/qos/{region}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiUpdateServerRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .artifact_delete import ArtifactDelete
 from .artifact_get import ArtifactGet
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/{artifactID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/{artifactID}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     artifact_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,24 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/artifacts"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/artifacts"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
     artifact_type: str  # OPTIONAL in [query]
     count: int  # OPTIONAL in [query]
     end_date: str  # OPTIONAL in [query]
     fleet_id: str  # OPTIONAL in [query]
     image_id: str  # OPTIONAL in [query]
     max_size: int  # OPTIONAL in [query]
@@ -122,14 +126,22 @@
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_get_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/{artifactID}/url"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/{artifactID}/url"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     artifact_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/artifact_usage_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,31 +65,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/usage"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/artifacts/usage"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_739743.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,32 +73,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/artifacts-sampling-rules"
     )
+    _path: str = (
+        "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/artifacts-sampling-rules"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     fleet_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/artifacts/fleet_artifact_sampling_a22d2b.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,33 +75,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/artifacts-sampling-rules"
     )
+    _path: str = (
+        "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/artifacts-sampling-rules"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiFleetArtifactsSampleRules  # REQUIRED in [body]
     fleet_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/auth/auth_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,29 +59,41 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/auth"
+    _path: str = "/ams/auth"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .development_server_conf_a8e4dd import DevelopmentServerConfigurationCreate
 from .development_server_conf_2194f5 import DevelopmentServerConfigurationDelete
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_2194f5.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: DELETE
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     development_server_config_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_282185.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     development_server_config_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,71 +25,88 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiDevelopmentServerConfigurationGetResponse
+from ...models import ApiImageDetails
 from ...models import ResponseErrorResponse
 
 
-class DevelopmentServerConfigurationList(Operation):
-    """lists all development server configurations (DevelopmentServerConfigurationList)
+class ImageGet(Operation):
+    """get image details. (ImageGet)
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
+        url: /ams/v1/admin/namespaces/{namespace}/images/{imageID}
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Images"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        image_id: (imageID) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - List[ApiDevelopmentServerConfigurationGetResponse] (development server configurations)
+        200: OK - ApiImageDetails (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
+        404: Not Found - ResponseErrorResponse (account not linked)
+
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
+    image_id: str  # REQUIRED in [path]
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
 
@@ -116,61 +133,72 @@
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "image_id"):
+            result["imageID"] = self.image_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DevelopmentServerConfigurationList:
+    def with_image_id(self, value: str) -> ImageGet:
+        self.image_id = value
+        return self
+
+    def with_namespace(self, value: str) -> ImageGet:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "image_id") and self.image_id:
+            result["imageID"] = str(self.image_id)
+        elif include_empty:
+            result["imageID"] = ""
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
     ) -> Tuple[
-        Union[None, List[ApiDevelopmentServerConfigurationGetResponse]],
-        Union[None, HttpResponse, ResponseErrorResponse],
+        Union[None, ApiImageDetails], Union[None, HttpResponse, ResponseErrorResponse]
     ]:
         """Parse the given response.
 
-        200: OK - List[ApiDevelopmentServerConfigurationGetResponse] (development server configurations)
+        200: OK - ApiImageDetails (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
+        404: Not Found - ResponseErrorResponse (account not linked)
+
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -179,58 +207,62 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [
-                ApiDevelopmentServerConfigurationGetResponse.create_from_dict(i)
-                for i in content
-            ], None
+            return ApiImageDetails.create_from_dict(content), None
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
+        if code == 404:
+            return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ResponseErrorResponse.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> DevelopmentServerConfigurationList:
+    def create(cls, image_id: str, namespace: str, **kwargs) -> ImageGet:
         instance = cls()
+        instance.image_id = image_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> DevelopmentServerConfigurationList:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImageGet:
         instance = cls()
+        if "imageID" in dict_ and dict_["imageID"] is not None:
+            instance.image_id = str(dict_["imageID"])
+        elif include_empty:
+            instance.image_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "imageID": "image_id",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "imageID": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_a8e4dd.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,25 +33,27 @@
 from ...models import ApiDevelopmentServerConfigurationCreateResponse
 from ...models import ResponseErrorResponse
 
 
 class DevelopmentServerConfigurationCreate(Operation):
     """create a new development server configuration (DevelopmentServerConfigurationCreate)
 
+    Configuration name can be up to 128 characters and must conform to ^[.a-zA-Z0-9_-]+$
+
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
         method: POST
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -70,32 +72,46 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations"
+    _path: str = (
+        "/ams/v1/admin/namespaces/{namespace}/development/server-configurations"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiDevelopmentServerConfigurationCreateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .basic_health_check import BasicHealthCheck
 from .func1 import Func1
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/basic_health_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,29 +50,41 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/healthz"
+    _path: str = "/healthz"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/func1.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,29 +50,41 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/ams/version"
+    _path: str = "/ams/version"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleet_commander/portal_health_check.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/ams_info/upload_url_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,53 +26,65 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 
-class PortalHealthCheck(Operation):
-    """Health check (PortalHealthCheck)
+class UploadURLGet(Operation):
+    """get an URL for uploading an image (UploadURLGet)
 
 
     Properties:
-        url: /ams/healthz
+        url: /ams/v1/upload-url
 
         method: GET
 
-        tags: ["Fleet Commander"]
+        tags: ["AMS Info"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - (OK)
+        200: OK - (success)
     """
 
     # region fields
 
-    _url: str = "/ams/healthz"
+    _url: str = "/ams/v1/upload-url"
+    _path: str = "/ams/v1/upload-url"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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
 
@@ -121,15 +133,15 @@
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[Union[None, HttpResponse], Union[None, HttpResponse]]:
         """Parse the given response.
 
-        200: OK - (OK)
+        200: OK - (success)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -148,24 +160,22 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> PortalHealthCheck:
+    def create(cls, **kwargs) -> UploadURLGet:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> PortalHealthCheck:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> UploadURLGet:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .fleet_claim_by_id import FleetClaimByID
 from .fleet_claim_by_keys import FleetClaimByKeys
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,33 +74,45 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/namespaces/{namespace}/fleets/{fleetID}/claim"
+    _path: str = "/ams/v1/namespaces/{namespace}/fleets/{fleetID}/claim"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiFleetClaimReq  # REQUIRED in [body]
     fleet_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_claim_by_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/namespaces/{namespace}/servers/claim"
+    _path: str = "/ams/v1/namespaces/{namespace}/servers/claim"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiFleetClaimByKeysReq  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,79 +25,95 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiFleetCreateResponse
 from ...models import ApiFleetParameters
 from ...models import ResponseErrorResponse
 
 
-class FleetCreate(Operation):
-    """create a fleet (FleetCreate)
+class FleetUpdate(Operation):
+    """update a fleet -– overrides current data (FleetUpdate)
 
-    Optionally, sampling rules for the fleet can also be specified
+    Optionally, sampling rules for the fleet can also be updated
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [UPDATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [UPDATE]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/fleets
+        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}
 
-        method: POST
+        method: PUT
 
         tags: ["Fleets"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         body: (body) REQUIRED ApiFleetParameters in body
 
+        fleet_id: (fleetID) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        201: Created - ApiFleetCreateResponse (success)
+        204: No Content - (no content)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
-        403: Forbidden - ResponseErrorResponse (exceeded quota)
+        403: Forbidden - ResponseErrorResponse (insufficient permissions)
+
+        404: Not Found - ResponseErrorResponse (fleet not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets"
-    _method: str = "POST"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _base_path: str = ""
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     body: ApiFleetParameters  # REQUIRED in [body]
+    fleet_id: str  # REQUIRED in [path]
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
 
@@ -130,70 +146,79 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "fleet_id"):
+            result["fleetID"] = self.fleet_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApiFleetParameters) -> FleetCreate:
+    def with_body(self, value: ApiFleetParameters) -> FleetUpdate:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> FleetCreate:
+    def with_fleet_id(self, value: str) -> FleetUpdate:
+        self.fleet_id = value
+        return self
+
+    def with_namespace(self, value: str) -> FleetUpdate:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
             result["body"] = ApiFleetParameters()
+        if hasattr(self, "fleet_id") and self.fleet_id:
+            result["fleetID"] = str(self.fleet_id)
+        elif include_empty:
+            result["fleetID"] = ""
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
-    ) -> Tuple[
-        Union[None, ApiFleetCreateResponse],
-        Union[None, HttpResponse, ResponseErrorResponse],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
         """Parse the given response.
 
-        201: Created - ApiFleetCreateResponse (success)
+        204: No Content - (no content)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
-        403: Forbidden - ResponseErrorResponse (exceeded quota)
+        403: Forbidden - ResponseErrorResponse (insufficient permissions)
+
+        404: Not Found - ResponseErrorResponse (fleet not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -202,65 +227,76 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
-            return ApiFleetCreateResponse.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
+        if code == 404:
+            return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ResponseErrorResponse.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, body: ApiFleetParameters, namespace: str, **kwargs) -> FleetCreate:
+    def create(
+        cls, body: ApiFleetParameters, fleet_id: str, namespace: str, **kwargs
+    ) -> FleetUpdate:
         instance = cls()
         instance.body = body
+        instance.fleet_id = fleet_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetCreate:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetUpdate:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ApiFleetParameters.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ApiFleetParameters()
+        if "fleetID" in dict_ and dict_["fleetID"] is not None:
+            instance.fleet_id = str(dict_["fleetID"])
+        elif include_empty:
+            instance.fleet_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
+            "fleetID": "fleet_id",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
+            "fleetID": True,
             "namespace": True,
         }
 
     # endregion static methods
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,77 +25,90 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ApiFleetServersResponse
 from ...models import ResponseErrorResponse
 
 
-class FleetDelete(Operation):
-    """delete a fleet (FleetDelete)
+class FleetServers(Operation):
+    """get server details & counts for a fleet (FleetServers)
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}
+        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers
 
-        method: DELETE
+        method: GET
 
         tags: ["Fleets"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         fleet_id: (fleetID) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (no content)
+        200: OK - ApiFleetServersResponse (success)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (fleet not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
-    _method: str = "DELETE"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     fleet_id: str  # REQUIRED in [path]
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
 
@@ -136,19 +149,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_fleet_id(self, value: str) -> FleetDelete:
+    def with_fleet_id(self, value: str) -> FleetServers:
         self.fleet_id = value
         return self
 
-    def with_namespace(self, value: str) -> FleetDelete:
+    def with_namespace(self, value: str) -> FleetServers:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -167,18 +180,21 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
+    ) -> Tuple[
+        Union[None, ApiFleetServersResponse],
+        Union[None, HttpResponse, ResponseErrorResponse],
+    ]:
         """Parse the given response.
 
-        204: No Content - (no content)
+        200: OK - ApiFleetServersResponse (success)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
@@ -195,16 +211,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ApiFleetServersResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
@@ -217,24 +233,24 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, fleet_id: str, namespace: str, **kwargs) -> FleetDelete:
+    def create(cls, fleet_id: str, namespace: str, **kwargs) -> FleetServers:
         instance = cls()
         instance.fleet_id = fleet_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetDelete:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetServers:
         instance = cls()
         if "fleetID" in dict_ and dict_["fleetID"] is not None:
             instance.fleet_id = str(dict_["fleetID"])
         elif include_empty:
             instance.fleet_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_get.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     fleet_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,31 +61,43 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_servers.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,78 +25,89 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiFleetServersResponse
 from ...models import ResponseErrorResponse
 
 
-class FleetServers(Operation):
-    """get server details & counts for a fleet (FleetServers)
+class FleetDelete(Operation):
+    """delete a fleet (FleetDelete)
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers
+        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}
 
-        method: GET
+        method: DELETE
 
         tags: ["Fleets"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         fleet_id: (fleetID) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ApiFleetServersResponse (success)
+        204: No Content - (no content)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (fleet not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers"
-    _method: str = "GET"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     fleet_id: str  # REQUIRED in [path]
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
 
@@ -137,19 +148,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_fleet_id(self, value: str) -> FleetServers:
+    def with_fleet_id(self, value: str) -> FleetDelete:
         self.fleet_id = value
         return self
 
-    def with_namespace(self, value: str) -> FleetServers:
+    def with_namespace(self, value: str) -> FleetDelete:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -168,21 +179,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ApiFleetServersResponse],
-        Union[None, HttpResponse, ResponseErrorResponse],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
         """Parse the given response.
 
-        200: OK - ApiFleetServersResponse (success)
+        204: No Content - (no content)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
@@ -199,16 +207,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ApiFleetServersResponse.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
@@ -221,24 +229,24 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, fleet_id: str, namespace: str, **kwargs) -> FleetServers:
+    def create(cls, fleet_id: str, namespace: str, **kwargs) -> FleetDelete:
         instance = cls()
         instance.fleet_id = fleet_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetServers:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetDelete:
         instance = cls()
         if "fleetID" in dict_ and dict_["fleetID"] is not None:
             instance.fleet_id = str(dict_["fleetID"])
         elif include_empty:
             instance.fleet_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_update.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,83 +25,94 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiFleetParameters
+from ...models import ApiImageDetails
+from ...models import ApiImageUpdate
 from ...models import ResponseErrorResponse
 
 
-class FleetUpdate(Operation):
-    """update a fleet -– overrides current data (FleetUpdate)
+class ImagePatch(Operation):
+    """edit the image (ImagePatch)
 
-    Optionally, sampling rules for the fleet can also be updated
+    This allows editing of the image name, toggling `IsProtected`, or adding & removal of tags
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [UPDATE]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [UPDATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [UPDATE]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}
+        url: /ams/v1/admin/namespaces/{namespace}/images/{imageID}
 
-        method: PUT
+        method: PATCH
 
-        tags: ["Fleets"]
+        tags: ["Images"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ApiFleetParameters in body
+        body: (body) REQUIRED ApiImageUpdate in body
 
-        fleet_id: (fleetID) REQUIRED str in path
+        image_id: (imageID) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (no content)
-
-        400: Bad Request - ResponseErrorResponse (bad request)
+        200: OK - ApiImageDetails (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (fleet not found)
+        404: Not Found - ResponseErrorResponse (account not linked)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}"
-    _method: str = "PUT"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
+    _base_path: str = ""
+    _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ApiFleetParameters  # REQUIRED in [body]
-    fleet_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "ams"
+
+    body: ApiImageUpdate  # REQUIRED in [body]
+    image_id: str  # REQUIRED in [path]
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
 
@@ -134,79 +145,79 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "fleet_id"):
-            result["fleetID"] = self.fleet_id
+        if hasattr(self, "image_id"):
+            result["imageID"] = self.image_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApiFleetParameters) -> FleetUpdate:
+    def with_body(self, value: ApiImageUpdate) -> ImagePatch:
         self.body = value
         return self
 
-    def with_fleet_id(self, value: str) -> FleetUpdate:
-        self.fleet_id = value
+    def with_image_id(self, value: str) -> ImagePatch:
+        self.image_id = value
         return self
 
-    def with_namespace(self, value: str) -> FleetUpdate:
+    def with_namespace(self, value: str) -> ImagePatch:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ApiFleetParameters()
-        if hasattr(self, "fleet_id") and self.fleet_id:
-            result["fleetID"] = str(self.fleet_id)
+            result["body"] = ApiImageUpdate()
+        if hasattr(self, "image_id") and self.image_id:
+            result["imageID"] = str(self.image_id)
         elif include_empty:
-            result["fleetID"] = ""
+            result["imageID"] = ""
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
-    ) -> Tuple[None, Union[None, HttpResponse, ResponseErrorResponse]]:
+    ) -> Tuple[
+        Union[None, ApiImageDetails], Union[None, HttpResponse, ResponseErrorResponse]
+    ]:
         """Parse the given response.
 
-        204: No Content - (no content)
-
-        400: Bad Request - ResponseErrorResponse (bad request)
+        200: OK - ApiImageDetails (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (fleet not found)
+        404: Not Found - ResponseErrorResponse (account not linked)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -215,18 +226,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
-        if code == 400:
-            return None, ResponseErrorResponse.create_from_dict(content)
+        if code == 200:
+            return ApiImageDetails.create_from_dict(content), None
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
@@ -238,53 +247,53 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ApiFleetParameters, fleet_id: str, namespace: str, **kwargs
-    ) -> FleetUpdate:
+        cls, body: ApiImageUpdate, image_id: str, namespace: str, **kwargs
+    ) -> ImagePatch:
         instance = cls()
         instance.body = body
-        instance.fleet_id = fleet_id
+        instance.image_id = image_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetUpdate:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImagePatch:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ApiFleetParameters.create_from_dict(
+            instance.body = ApiImageUpdate.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ApiFleetParameters()
-        if "fleetID" in dict_ and dict_["fleetID"] is not None:
-            instance.fleet_id = str(dict_["fleetID"])
+            instance.body = ApiImageUpdate()
+        if "imageID" in dict_ and dict_["imageID"] is not None:
+            instance.image_id = str(dict_["imageID"])
         elif include_empty:
-            instance.fleet_id = ""
+            instance.image_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
-            "fleetID": "fleet_id",
+            "imageID": "image_id",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
-            "fleetID": True,
+            "imageID": True,
             "namespace": True,
         }
 
     # endregion static methods
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .image_get import ImageGet
 from .image_list import ImageList
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_get.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,76 +25,87 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiImageDetails
+from ...models import ApiImageList
 from ...models import ResponseErrorResponse
 
 
-class ImageGet(Operation):
-    """get image details. (ImageGet)
+class ImageList(Operation):
+    """get a list of existing images (ImageList)
+
+    Returns images which exist (uploaded, uploading, or building) in the linked account. This route fails if no account is linked
 
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/images/{imageID}
+        url: /ams/v1/admin/namespaces/{namespace}/images
 
         method: GET
 
         tags: ["Images"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        image_id: (imageID) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ApiImageDetails (success)
+        200: OK - ApiImageList (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (account not linked)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/images"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/images"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    image_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "ams"
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
 
@@ -121,65 +132,55 @@
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
-        if hasattr(self, "image_id"):
-            result["imageID"] = self.image_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_image_id(self, value: str) -> ImageGet:
-        self.image_id = value
-        return self
-
-    def with_namespace(self, value: str) -> ImageGet:
+    def with_namespace(self, value: str) -> ImageList:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "image_id") and self.image_id:
-            result["imageID"] = str(self.image_id)
-        elif include_empty:
-            result["imageID"] = ""
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
     ) -> Tuple[
-        Union[None, ApiImageDetails], Union[None, HttpResponse, ResponseErrorResponse]
+        Union[None, ApiImageList], Union[None, HttpResponse, ResponseErrorResponse]
     ]:
         """Parse the given response.
 
-        200: OK - ApiImageDetails (success)
+        200: OK - ApiImageList (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         404: Not Found - ResponseErrorResponse (account not linked)
 
@@ -195,15 +196,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ApiImageDetails.create_from_dict(content), None
+            return ApiImageList.create_from_dict(content), None
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
@@ -214,43 +215,36 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, image_id: str, namespace: str, **kwargs) -> ImageGet:
+    def create(cls, namespace: str, **kwargs) -> ImageList:
         instance = cls()
-        instance.image_id = image_id
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImageGet:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImageList:
         instance = cls()
-        if "imageID" in dict_ and dict_["imageID"] is not None:
-            instance.image_id = str(dict_["imageID"])
-        elif include_empty:
-            instance.image_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "imageID": "image_id",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "imageID": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_list.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,75 +25,90 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiImageList
+from ...models import ApiFleetServerConnectionInfoResponse
 from ...models import ResponseErrorResponse
 
 
-class ImageList(Operation):
-    """get a list of existing images (ImageList)
+class FleetServerConnectionInfo(Operation):
+    """get connection info for a dedicated server (FleetServerConnectionInfo)
 
-    Returns images which exist (uploaded, uploading, or building) in the linked account. This route fails if no account is linked
-
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:AMS:DS:LOGS [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [READ]
+        - ADMIN:NAMESPACE:{namespace}:AMS:DS:LOGS [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/images
+        url: /ams/v1/admin/namespaces/{namespace}/servers/{serverID}/connectioninfo
 
         method: GET
 
-        tags: ["Images"]
+        tags: ["Servers"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
+        server_id: (serverID) REQUIRED str in path
+
     Responses:
-        200: OK - ApiImageList (success)
+        200: OK - ApiFleetServerConnectionInfoResponse (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (account not linked)
+        404: Not Found - ResponseErrorResponse (dedicated server not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/images"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/connectioninfo"
+    _path: str = (
+        "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/connectioninfo"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
+    server_id: str  # REQUIRED in [path]
 
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
 
@@ -122,59 +137,70 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
+        if hasattr(self, "server_id"):
+            result["serverID"] = self.server_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ImageList:
+    def with_namespace(self, value: str) -> FleetServerConnectionInfo:
         self.namespace = value
         return self
 
+    def with_server_id(self, value: str) -> FleetServerConnectionInfo:
+        self.server_id = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
+        if hasattr(self, "server_id") and self.server_id:
+            result["serverID"] = str(self.server_id)
+        elif include_empty:
+            result["serverID"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ApiImageList], Union[None, HttpResponse, ResponseErrorResponse]
+        Union[None, ApiFleetServerConnectionInfoResponse],
+        Union[None, HttpResponse, ResponseErrorResponse],
     ]:
         """Parse the given response.
 
-        200: OK - ApiImageList (success)
+        200: OK - ApiFleetServerConnectionInfoResponse (success)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (account not linked)
+        404: Not Found - ResponseErrorResponse (dedicated server not found)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -184,15 +210,15 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ApiImageList.create_from_dict(content), None
+            return ApiFleetServerConnectionInfoResponse.create_from_dict(content), None
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
@@ -203,36 +229,47 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> ImageList:
+    def create(
+        cls, namespace: str, server_id: str, **kwargs
+    ) -> FleetServerConnectionInfo:
         instance = cls()
         instance.namespace = namespace
+        instance.server_id = server_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImageList:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> FleetServerConnectionInfo:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
+        if "serverID" in dict_ and dict_["serverID"] is not None:
+            instance.server_id = str(dict_["serverID"])
+        elif include_empty:
+            instance.server_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "namespace": "namespace",
+            "serverID": "server_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "namespace": True,
+            "serverID": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/images/image_patch.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/development/development_server_conf_7b687b.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,82 +25,91 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiImageDetails
-from ...models import ApiImageUpdate
+from ...models import ApiDevelopmentServerConfigurationListResponse
 from ...models import ResponseErrorResponse
 
 
-class ImagePatch(Operation):
-    """edit the image (ImagePatch)
+class DevelopmentServerConfigurationList(Operation):
+    """lists development server configurations with pagination (DevelopmentServerConfigurationList)
 
-    This allows editing of the image name, toggling `IsProtected`, or adding & removal of tags
-
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [UPDATE]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:ACCOUNT [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/images/{imageID}
+        url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
-        method: PATCH
+        method: GET
 
-        tags: ["Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ApiImageUpdate in body
+        namespace: (namespace) REQUIRED str in path
 
-        image_id: (imageID) REQUIRED str in path
+        count: (count) OPTIONAL int in query
 
-        namespace: (namespace) REQUIRED str in path
+        offset: (offset) OPTIONAL int in query
 
     Responses:
-        200: OK - ApiImageDetails (success)
+        200: OK - ApiDevelopmentServerConfigurationListResponse (development server configurations)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (account not linked)
-
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/images/{imageID}"
-    _method: str = "PATCH"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/development/server-configurations"
+    _path: str = (
+        "/ams/v1/admin/namespaces/{namespace}/development/server-configurations"
+    )
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ApiImageUpdate  # REQUIRED in [body]
-    image_id: str  # REQUIRED in [path]
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
+    count: int  # OPTIONAL in [query]
+    offset: int  # OPTIONAL in [query]
 
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
 
@@ -122,91 +131,91 @@
 
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
-        if hasattr(self, "image_id"):
-            result["imageID"] = self.image_id
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
+    def get_query_params(self) -> dict:
+        result = {}
+        if hasattr(self, "count"):
+            result["count"] = self.count
+        if hasattr(self, "offset"):
+            result["offset"] = self.offset
+        return result
+
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ApiImageUpdate) -> ImagePatch:
-        self.body = value
+    def with_namespace(self, value: str) -> DevelopmentServerConfigurationList:
+        self.namespace = value
         return self
 
-    def with_image_id(self, value: str) -> ImagePatch:
-        self.image_id = value
+    def with_count(self, value: int) -> DevelopmentServerConfigurationList:
+        self.count = value
         return self
 
-    def with_namespace(self, value: str) -> ImagePatch:
-        self.namespace = value
+    def with_offset(self, value: int) -> DevelopmentServerConfigurationList:
+        self.offset = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ApiImageUpdate()
-        if hasattr(self, "image_id") and self.image_id:
-            result["imageID"] = str(self.image_id)
-        elif include_empty:
-            result["imageID"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
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
-        Union[None, ApiImageDetails], Union[None, HttpResponse, ResponseErrorResponse]
+        Union[None, ApiDevelopmentServerConfigurationListResponse],
+        Union[None, HttpResponse, ResponseErrorResponse],
     ]:
         """Parse the given response.
 
-        200: OK - ApiImageDetails (success)
+        200: OK - ApiDevelopmentServerConfigurationListResponse (development server configurations)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (account not linked)
-
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -215,73 +224,80 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ApiImageDetails.create_from_dict(content), None
+            return (
+                ApiDevelopmentServerConfigurationListResponse.create_from_dict(content),
+                None,
+            )
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
-        if code == 404:
-            return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ResponseErrorResponse.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ApiImageUpdate, image_id: str, namespace: str, **kwargs
-    ) -> ImagePatch:
+        cls,
+        namespace: str,
+        count: Optional[int] = None,
+        offset: Optional[int] = None,
+        **kwargs,
+    ) -> DevelopmentServerConfigurationList:
         instance = cls()
-        instance.body = body
-        instance.image_id = image_id
         instance.namespace = namespace
+        if count is not None:
+            instance.count = count
+        if offset is not None:
+            instance.offset = offset
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ImagePatch:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> DevelopmentServerConfigurationList:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ApiImageUpdate.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ApiImageUpdate()
-        if "imageID" in dict_ and dict_["imageID"] is not None:
-            instance.image_id = str(dict_["imageID"])
-        elif include_empty:
-            instance.image_id = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
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
-            "imageID": "image_id",
             "namespace": "namespace",
+            "count": "count",
+            "offset": "offset",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
-            "imageID": True,
             "namespace": True,
+            "count": False,
+            "offset": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .fleet_server_connection_info import FleetServerConnectionInfo
 from .fleet_server_history import FleetServerHistory
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_connection_info.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiFleetServerConnectionInfoResponse
+from ...models import ApiFleetServerHistoryResponse
 from ...models import ResponseErrorResponse
 
 
-class FleetServerConnectionInfo(Operation):
-    """get connection info for a dedicated server (FleetServerConnectionInfo)
+class ServerHistory(Operation):
+    """get history records of a dedicated server (ServerHistory)
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:AMS:DS:LOGS [READ]
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:AMS:DS:LOGS [READ]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/servers/{serverID}/connectioninfo
+        url: /ams/v1/admin/namespaces/{namespace}/servers/{serverID}/history
 
         method: GET
 
         tags: ["Servers"]
 
         consumes: ["application/json"]
 
@@ -55,46 +55,58 @@
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
         server_id: (serverID) REQUIRED str in path
 
     Responses:
-        200: OK - ApiFleetServerConnectionInfoResponse (success)
+        200: OK - ApiFleetServerHistoryResponse (success)
+
+        400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (dedicated server not found)
-
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/connectioninfo"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/history"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/history"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
     server_id: str  # REQUIRED in [path]
 
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
 
@@ -135,19 +147,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> FleetServerConnectionInfo:
+    def with_namespace(self, value: str) -> ServerHistory:
         self.namespace = value
         return self
 
-    def with_server_id(self, value: str) -> FleetServerConnectionInfo:
+    def with_server_id(self, value: str) -> ServerHistory:
         self.server_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -167,27 +179,27 @@
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ApiFleetServerConnectionInfoResponse],
+        Union[None, ApiFleetServerHistoryResponse],
         Union[None, HttpResponse, ResponseErrorResponse],
     ]:
         """Parse the given response.
 
-        200: OK - ApiFleetServerConnectionInfoResponse (success)
+        200: OK - ApiFleetServerHistoryResponse (success)
+
+        400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
-        404: Not Found - ResponseErrorResponse (dedicated server not found)
-
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
@@ -196,47 +208,45 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ApiFleetServerConnectionInfoResponse.create_from_dict(content), None
+            return ApiFleetServerHistoryResponse.create_from_dict(content), None
+        if code == 400:
+            return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
-        if code == 404:
-            return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ResponseErrorResponse.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, namespace: str, server_id: str, **kwargs
-    ) -> FleetServerConnectionInfo:
+    def create(cls, namespace: str, server_id: str, **kwargs) -> ServerHistory:
         instance = cls()
         instance.namespace = namespace
         instance.server_id = server_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> FleetServerConnectionInfo:
+    ) -> ServerHistory:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "serverID" in dict_ and dict_["serverID"] is not None:
             instance.server_id = str(dict_["serverID"])
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,20 +83,24 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers/history"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets/{fleetID}/servers/history"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     fleet_id: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     count: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     reason: str  # OPTIONAL in [query]
     region: str  # OPTIONAL in [query]
     server_id: str  # OPTIONAL in [query]
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/servers/fleet_server_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
     _url: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
     server_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/servers/server_history.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/fleets/fleet_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,76 +25,91 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ApiFleetServerHistoryResponse
+from ...models import ApiFleetCreateResponse
+from ...models import ApiFleetParameters
 from ...models import ResponseErrorResponse
 
 
-class ServerHistory(Operation):
-    """get history records of a dedicated server (ServerHistory)
+class FleetCreate(Operation):
+    """create a fleet (FleetCreate)
 
-    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+    Optionally, sampling rules for the fleet can also be specified
+
+    Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
+        - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Properties:
-        url: /ams/v1/admin/namespaces/{namespace}/servers/{serverID}/history
+        url: /ams/v1/admin/namespaces/{namespace}/fleets
 
-        method: GET
+        method: POST
 
-        tags: ["Servers"]
+        tags: ["Fleets"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        namespace: (namespace) REQUIRED str in path
+        body: (body) REQUIRED ApiFleetParameters in body
 
-        server_id: (serverID) REQUIRED str in path
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ApiFleetServerHistoryResponse (success)
+        201: Created - ApiFleetCreateResponse (success)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
-        403: Forbidden - ResponseErrorResponse (insufficient permissions)
+        403: Forbidden - ResponseErrorResponse (exceeded quota)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
 
     # region fields
 
-    _url: str = "/ams/v1/admin/namespaces/{namespace}/servers/{serverID}/history"
-    _method: str = "GET"
+    _url: str = "/ams/v1/admin/namespaces/{namespace}/fleets"
+    _path: str = "/ams/v1/admin/namespaces/{namespace}/fleets"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
+    body: ApiFleetParameters  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
-    server_id: str  # REQUIRED in [path]
 
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
 
@@ -116,77 +131,81 @@
 
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
+            "body": self.get_body_params(),
             "path": self.get_path_params(),
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
-        if hasattr(self, "server_id"):
-            result["serverID"] = self.server_id
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> ServerHistory:
-        self.namespace = value
+    def with_body(self, value: ApiFleetParameters) -> FleetCreate:
+        self.body = value
         return self
 
-    def with_server_id(self, value: str) -> ServerHistory:
-        self.server_id = value
+    def with_namespace(self, value: str) -> FleetCreate:
+        self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ApiFleetParameters()
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "server_id") and self.server_id:
-            result["serverID"] = str(self.server_id)
-        elif include_empty:
-            result["serverID"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ApiFleetServerHistoryResponse],
+        Union[None, ApiFleetCreateResponse],
         Union[None, HttpResponse, ResponseErrorResponse],
     ]:
         """Parse the given response.
 
-        200: OK - ApiFleetServerHistoryResponse (success)
+        201: Created - ApiFleetCreateResponse (success)
 
         400: Bad Request - ResponseErrorResponse (bad request)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
-        403: Forbidden - ResponseErrorResponse (insufficient permissions)
+        403: Forbidden - ResponseErrorResponse (exceeded quota)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
@@ -195,16 +214,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ApiFleetServerHistoryResponse.create_from_dict(content), None
+        if code == 201:
+            return ApiFleetCreateResponse.create_from_dict(content), None
         if code == 400:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 401:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 403:
             return None, ResponseErrorResponse.create_from_dict(content)
         if code == 500:
@@ -215,45 +234,45 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, server_id: str, **kwargs) -> ServerHistory:
+    def create(cls, body: ApiFleetParameters, namespace: str, **kwargs) -> FleetCreate:
         instance = cls()
+        instance.body = body
         instance.namespace = namespace
-        instance.server_id = server_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> ServerHistory:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> FleetCreate:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ApiFleetParameters.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ApiFleetParameters()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "serverID" in dict_ and dict_["serverID"] is not None:
-            instance.server_id = str(dict_["serverID"])
-        elif include_empty:
-            instance.server_id = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "namespace": "namespace",
-            "serverID": "server_id",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "namespace": True,
-            "serverID": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .local_watchdog_connect import LocalWatchdogConnect
 from .watchdog_connect import WatchdogConnect
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/local_watchdog_connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,32 +60,44 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/ams/v1/namespaces/{namespace}/local/{watchdogID}/connect"
+    _path: str = "/ams/v1/namespaces/{namespace}/local/{watchdogID}/connect"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
     watchdog_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/operations/watchdogs/watchdog_connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,32 +58,44 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/ams/v1/namespaces/{namespace}/watchdogs/{watchdogID}/connect"
+    _path: str = "/ams/v1/namespaces/{namespace}/watchdogs/{watchdogID}/connect"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "ams"
+
     namespace: str  # REQUIRED in [path]
     watchdog_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the Fleet Commander."""
 
-__version__ = "1.13.0"
+__version__ = "1.17.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._account import account_get
 from ._account import account_get_async
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_account.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_account.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_ams_qo_s.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_artifacts.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_auth.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_development.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_development.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import ApiDevelopmentServerConfigurationCreateRequest
 from ..models import ApiDevelopmentServerConfigurationCreateResponse
 from ..models import ApiDevelopmentServerConfigurationGetResponse
+from ..models import ApiDevelopmentServerConfigurationListResponse
 from ..models import ResponseErrorResponse
 
 from ..operations.development import DevelopmentServerConfigurationCreate
 from ..operations.development import DevelopmentServerConfigurationDelete
 from ..operations.development import DevelopmentServerConfigurationGet
 from ..operations.development import DevelopmentServerConfigurationList
 
@@ -45,25 +46,27 @@
     body: ApiDevelopmentServerConfigurationCreateRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """create a new development server configuration (DevelopmentServerConfigurationCreate)
 
+    Configuration name can be up to 128 characters and must conform to ^[.a-zA-Z0-9_-]+$
+
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
         method: POST
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -98,25 +101,27 @@
     body: ApiDevelopmentServerConfigurationCreateRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """create a new development server configuration (DevelopmentServerConfigurationCreate)
 
+    Configuration name can be up to 128 characters and must conform to ^[.a-zA-Z0-9_-]+$
+
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [CREATE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
         method: POST
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -163,15 +168,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: DELETE
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -216,15 +221,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [DELETE]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: DELETE
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -271,15 +276,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -324,15 +329,15 @@
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations/{developmentServerConfigID}
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -362,99 +367,115 @@
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
 @same_doc_as(DevelopmentServerConfigurationList)
 def development_server_configuration_list(
+    count: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """lists all development server configurations (DevelopmentServerConfigurationList)
+    """lists development server configurations with pagination (DevelopmentServerConfigurationList)
 
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
+        count: (count) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        200: OK - List[ApiDevelopmentServerConfigurationGetResponse] (development server configurations)
+        200: OK - ApiDevelopmentServerConfigurationListResponse (development server configurations)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = DevelopmentServerConfigurationList.create(
+        count=count,
+        offset=offset,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
 @same_doc_as(DevelopmentServerConfigurationList)
 async def development_server_configuration_list_async(
+    count: Optional[int] = None,
+    offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """lists all development server configurations (DevelopmentServerConfigurationList)
+    """lists development server configurations with pagination (DevelopmentServerConfigurationList)
 
     Required Permission: ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:ARMADA:FLEET [READ]
 
     Properties:
         url: /ams/v1/admin/namespaces/{namespace}/development/server-configurations
 
         method: GET
 
-        tags: ["Development", "Fleets", "Images"]
+        tags: ["Development"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
+        count: (count) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
     Responses:
-        200: OK - List[ApiDevelopmentServerConfigurationGetResponse] (development server configurations)
+        200: OK - ApiDevelopmentServerConfigurationListResponse (development server configurations)
 
         401: Unauthorized - ResponseErrorResponse (no authorization provided)
 
         403: Forbidden - ResponseErrorResponse (insufficient permissions)
 
         500: Internal Server Error - ResponseErrorResponse (internal server error)
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
     request = DevelopmentServerConfigurationList.create(
+        count=count,
+        offset=offset,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleet_commander.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_fleets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_images.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_images.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_servers.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk/api/ams/wrappers/_watchdogs.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-ams
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - Fleet Commander
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 Fleet Commander
-* Version: 1.13.0
+* Version: 1.17.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-ams-0.7.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_ams-0.8.0/accelbyte_py_sdk_service_ams.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 accelbyte_py_sdk/api/ams/models/api_artifact_type_sampling_rules.py
 accelbyte_py_sdk/api/ams/models/api_artifact_url_response.py
 accelbyte_py_sdk/api/ams/models/api_artifact_usage_response.py
 accelbyte_py_sdk/api/ams/models/api_available_instance_types_response.py
 accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_request.py
 accelbyte_py_sdk/api/ams/models/api_development_server_configuration_create_response.py
 accelbyte_py_sdk/api/ams/models/api_development_server_configuration_get_response.py
+accelbyte_py_sdk/api/ams/models/api_development_server_configuration_list_response.py
 accelbyte_py_sdk/api/ams/models/api_ds_history_event.py
 accelbyte_py_sdk/api/ams/models/api_ds_history_list.py
 accelbyte_py_sdk/api/ams/models/api_ds_host_configuration.py
 accelbyte_py_sdk/api/ams/models/api_fleet_artifacts_sample_rules.py
 accelbyte_py_sdk/api/ams/models/api_fleet_claim_by_keys_req.py
 accelbyte_py_sdk/api/ams/models/api_fleet_claim_req.py
 accelbyte_py_sdk/api/ams/models/api_fleet_claim_response.py
```

