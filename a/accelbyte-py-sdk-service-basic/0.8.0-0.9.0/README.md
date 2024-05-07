# Comparing `tmp/accelbyte-py-sdk-service-basic-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-basic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-basic-0.8.0.tar", last modified: Wed Mar 13 06:09:55 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-basic-0.9.0.tar", last modified: Tue Mar 26 05:40:11 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-basic-0.8.0.tar` & `accelbyte-py-sdk-service-basic-0.9.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.117845 accelbyte-py-sdk-service-basic-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-13 06:09:55.113845 accelbyte-py-sdk-service-basic-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      869 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.101845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.101845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.105845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/
--rw-rw-r--   0 root         (0) root         (0)     7235 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.105845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/
--rw-rw-r--   0 root         (0) root         (0)     3110 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4567 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_for_unban_user_api_call.py
--rw-rw-r--   0 root         (0) root         (0)     3944 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_for_update_equ8_config_api_call.py
--rw-rw-r--   0 root         (0) root         (0)     4632 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_ban_status.py
--rw-rw-r--   0 root         (0) root         (0)     6809 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_status.py
--rw-rw-r--   0 root         (0) root         (0)     7565 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/action.py
--rw-rw-r--   0 root         (0) root         (0)     6028 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/add_country_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     6041 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/add_country_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     4124 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_create.py
--rw-rw-r--   0 root         (0) root         (0)     6424 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_info.py
--rw-rw-r--   0 root         (0) root         (0)     3587 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_update.py
--rw-rw-r--   0 root         (0) root         (0)     5958 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/country_group_object.py
--rw-rw-r--   0 root         (0) root         (0)     4266 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/country_object.py
--rw-rw-r--   0 root         (0) root         (0)     4376 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/equ8_config.py
--rw-rw-r--   0 root         (0) root         (0)     6319 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/error_entity.py
--rw-rw-r--   0 root         (0) root         (0)     7297 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/field_validation_error.py
--rw-rw-r--   0 root         (0) root         (0)     5896 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/file_upload_url_info.py
--rw-rw-r--   0 root         (0) root         (0)     6627 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_context.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_create.py
--rw-rw-r--   0 root         (0) root         (0)     8559 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_info.py
--rw-rw-r--   0 root         (0) root         (0)     4855 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_publisher_info.py
--rw-rw-r--   0 root         (0) root         (0)     4160 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_status_update.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_update.py
--rw-rw-r--   0 root         (0) root         (0)     6120 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/retrieve_country_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     3926 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/retrieve_time_response.py
--rw-rw-r--   0 root         (0) root         (0)     5160 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/update_country_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     5136 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_ban_request.py
--rw-rw-r--   0 root         (0) root         (0)    13637 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_admin.py
--rw-rw-r--   0 root         (0) root         (0)     3919 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_bulk_request.py
--rw-rw-r--   0 root         (0) root         (0)    10685 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_create.py
--rw-rw-r--   0 root         (0) root         (0)    14320 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_info.py
--rw-rw-r--   0 root         (0) root         (0)    12097 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_private_create.py
--rw-rw-r--   0 root         (0) root         (0)    15787 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_private_info.py
--rw-rw-r--   0 root         (0) root         (0)     9545 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_public_info.py
--rw-rw-r--   0 root         (0) root         (0)     4197 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_status_update.py
--rw-rw-r--   0 root         (0) root         (0)    12644 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_update.py
--rw-rw-r--   0 root         (0) root         (0)     6778 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_report_request.py
--rw-rw-r--   0 root         (0) root         (0)     3684 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_zip_code.py
--rw-rw-r--   0 root         (0) root         (0)     3724 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_zip_code_update.py
--rw-rw-r--   0 root         (0) root         (0)     5625 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/validation_error_entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.105845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/
--rw-rw-r--   0 root         (0) root         (0)      434 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.105845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      524 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7291 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/anonymization/anonymize_user_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/
--rw-rw-r--   0 root         (0) root         (0)      683 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7871 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/create_config.py
--rw-rw-r--   0 root         (0) root         (0)     7519 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/delete_config_1.py
--rw-rw-r--   0 root         (0) root         (0)     7464 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/get_config_1.py
--rw-rw-r--   0 root         (0) root         (0)     7645 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/get_publisher_config.py
--rw-rw-r--   0 root         (0) root         (0)     8731 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/update_config_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/
--rw-rw-r--   0 root         (0) root         (0)      581 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/delete_config.py
--rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/get_config.py
--rw-rw-r--   0 root         (0) root         (0)     7333 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/update_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/
--rw-rw-r--   0 root         (0) root         (0)      740 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8591 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_upload_url.py
--rw-rw-r--   0 root         (0) root         (0)    10223 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_user_upload_c_8f862a.py
--rw-rw-r--   0 root         (0) root         (0)     8623 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_upload_url.py
--rw-rw-r--   0 root         (0) root         (0)    10448 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_user_u_2061db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/
--rw-rw-r--   0 root         (0) root         (0)      993 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8279 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/add_country_group.py
--rw-rw-r--   0 root         (0) root         (0)     7881 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/delete_country_group.py
--rw-rw-r--   0 root         (0) root         (0)     6994 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_countries.py
--rw-rw-r--   0 root         (0) root         (0)     8065 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_country_groups.py
--rw-rw-r--   0 root         (0) root         (0)     6024 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_languages.py
--rw-rw-r--   0 root         (0) root         (0)     5993 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_time_zones.py
--rw-rw-r--   0 root         (0) root         (0)     6716 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_countries.py
--rw-rw-r--   0 root         (0) root         (0)     5731 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_languages.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time.py
--rw-rw-r--   0 root         (0) root         (0)     5700 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time_zones.py
--rw-rw-r--   0 root         (0) root         (0)     9718 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/update_country_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/
--rw-rw-r--   0 root         (0) root         (0)     1091 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/change_namespace_status.py
--rw-rw-r--   0 root         (0) root         (0)     7814 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/create_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     6958 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/delete_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     7414 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_child_namespaces.py
--rw-rw-r--   0 root         (0) root         (0)     7355 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_game_namespaces.py
--rw-rw-r--   0 root         (0) root         (0)     7790 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     6174 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_context.py
--rw-rw-r--   0 root         (0) root         (0)     6949 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_publisher.py
--rw-rw-r--   0 root         (0) root         (0)     6219 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespaces.py
--rw-rw-r--   0 root         (0) root         (0)     6969 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespace_publisher.py
--rw-rw-r--   0 root         (0) root         (0)     5905 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespaces.py
--rw-rw-r--   0 root         (0) root         (0)     8192 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/update_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.109845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/
--rw-rw-r--   0 root         (0) root         (0)      745 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7887 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/ban_users.py
--rw-rw-r--   0 root         (0) root         (0)     6414 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_actions.py
--rw-rw-r--   0 root         (0) root         (0)     8185 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_banned_users.py
--rw-rw-r--   0 root         (0) root         (0)     7918 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_user_status.py
--rw-rw-r--   0 root         (0) root         (0)     8190 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/public_report_user.py
--rw-rw-r--   0 root         (0) root         (0)     7059 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/report_user.py
--rw-rw-r--   0 root         (0) root         (0)     7885 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/un_ban_users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.113845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/
--rw-rw-r--   0 root         (0) root         (0)     2192 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7443 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/admin_get_user_profile__eda78b.py
--rw-rw-r--   0 root         (0) root         (0)     8805 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/create_my_profile.py
--rw-rw-r--   0 root         (0) root         (0)     7706 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/delete_user_profile.py
--rw-rw-r--   0 root         (0) root         (0)     7325 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_custom_attributes_info.py
--rw-rw-r--   0 root         (0) root         (0)     6610 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_private_custom_a_61114d.py
--rw-rw-r--   0 root         (0) root         (0)     7319 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_profile_info.py
--rw-rw-r--   0 root         (0) root         (0)     6164 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_zip_code.py
--rw-rw-r--   0 root         (0) root         (0)     7411 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_private_custom_attr_322032.py
--rw-rw-r--   0 root         (0) root         (0)     7653 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info.py
--rw-rw-r--   0 root         (0) root         (0)     7856 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info_b_5dfc7f.py
--rw-rw-r--   0 root         (0) root         (0)     8986 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_create_user_profile.py
--rw-rw-r--   0 root         (0) root         (0)     6700 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_custom_attri_5323c2.py
--rw-rw-r--   0 root         (0) root         (0)     7300 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_0d683e.py
--rw-rw-r--   0 root         (0) root         (0)     7099 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_64cc50.py
--rw-rw-r--   0 root         (0) root         (0)     6927 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_cdd77a.py
--rw-rw-r--   0 root         (0) root         (0)     7644 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_info.py
--rw-rw-r--   0 root         (0) root         (0)     8971 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_custom_at_7dcf23.py
--rw-rw-r--   0 root         (0) root         (0)     9047 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_prof_c93172.py
--rw-rw-r--   0 root         (0) root         (0)     9020 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_profile.py
--rw-rw-r--   0 root         (0) root         (0)     8947 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_custom_attribute_105f42.py
--rw-rw-r--   0 root         (0) root         (0)     8200 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_private_custo_49ebda.py
--rw-rw-r--   0 root         (0) root         (0)     8776 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_profile.py
--rw-rw-r--   0 root         (0) root         (0)     8107 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_zip_code.py
--rw-rw-r--   0 root         (0) root         (0)     9040 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_private_custom_a_62b74f.py
--rw-rw-r--   0 root         (0) root         (0)     8914 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile.py
--rw-rw-r--   0 root         (0) root         (0)     9036 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.113845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     7490 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4409 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    17778 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_config.py
--rw-rw-r--   0 root         (0) root         (0)     8549 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_equ8_config.py
--rw-rw-r--   0 root         (0) root         (0)    18348 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_file_upload.py
--rw-rw-r--   0 root         (0) root         (0)    31986 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_misc.py
--rw-rw-r--   0 root         (0) root         (0)    39193 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_namespace.py
--rw-rw-r--   0 root         (0) root         (0)    23847 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_user_action.py
--rw-rw-r--   0 root         (0) root         (0)    94690 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_user_profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:55.113845 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-13 06:09:55.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8709 2024-03-13 06:09:55.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:09:55.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:09:55.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:09:55.000000 accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      355 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-basic-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:09:55.117845 accelbyte-py-sdk-service-basic-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.758378 accelbyte-py-sdk-service-basic-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:40:11.758378 accelbyte-py-sdk-service-basic-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.742379 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.742379 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.746379 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/
+-rw-rw-r--   0 root         (0) root         (0)     7235 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/
+-rw-rw-r--   0 root         (0) root         (0)     3110 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4567 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_for_unban_user_api_call.py
+-rw-rw-r--   0 root         (0) root         (0)     3944 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_for_update_equ8_config_api_call.py
+-rw-rw-r--   0 root         (0) root         (0)     4632 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_ban_status.py
+-rw-rw-r--   0 root         (0) root         (0)     6809 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_status.py
+-rw-rw-r--   0 root         (0) root         (0)     7565 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/action.py
+-rw-rw-r--   0 root         (0) root         (0)     6028 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/add_country_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6041 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/add_country_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4124 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_create.py
+-rw-rw-r--   0 root         (0) root         (0)     6424 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3587 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5958 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/country_group_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4266 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/country_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4376 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/equ8_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6319 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/error_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     7297 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/field_validation_error.py
+-rw-rw-r--   0 root         (0) root         (0)     5896 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/file_upload_url_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6627 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_context.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_create.py
+-rw-rw-r--   0 root         (0) root         (0)     8559 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4855 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_publisher_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4160 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_status_update.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6120 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/retrieve_country_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3926 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/retrieve_time_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5160 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/update_country_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5136 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_ban_request.py
+-rw-rw-r--   0 root         (0) root         (0)    13637 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_admin.py
+-rw-rw-r--   0 root         (0) root         (0)     3919 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_bulk_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10685 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_create.py
+-rw-rw-r--   0 root         (0) root         (0)    14320 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_info.py
+-rw-rw-r--   0 root         (0) root         (0)    12097 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_private_create.py
+-rw-rw-r--   0 root         (0) root         (0)    15787 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_private_info.py
+-rw-rw-r--   0 root         (0) root         (0)     9545 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_public_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4197 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_status_update.py
+-rw-rw-r--   0 root         (0) root         (0)    12644 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_update.py
+-rw-rw-r--   0 root         (0) root         (0)     6778 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_report_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3684 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_zip_code.py
+-rw-rw-r--   0 root         (0) root         (0)     3724 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_zip_code_update.py
+-rw-rw-r--   0 root         (0) root         (0)     5625 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/validation_error_entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/
+-rw-rw-r--   0 root         (0) root         (0)      434 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      524 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7291 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/anonymization/anonymize_user_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      683 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7871 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/create_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7519 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/delete_config_1.py
+-rw-rw-r--   0 root         (0) root         (0)     7464 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/get_config_1.py
+-rw-rw-r--   0 root         (0) root         (0)     7645 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/get_publisher_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8731 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/update_config_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/
+-rw-rw-r--   0 root         (0) root         (0)      581 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/delete_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6000 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/get_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7333 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/update_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/
+-rw-rw-r--   0 root         (0) root         (0)      740 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8591 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_upload_url.py
+-rw-rw-r--   0 root         (0) root         (0)    10223 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_user_upload_c_8f862a.py
+-rw-rw-r--   0 root         (0) root         (0)     8623 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_upload_url.py
+-rw-rw-r--   0 root         (0) root         (0)    10448 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_user_u_2061db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/
+-rw-rw-r--   0 root         (0) root         (0)      993 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8279 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/add_country_group.py
+-rw-rw-r--   0 root         (0) root         (0)     7881 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/delete_country_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6994 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_countries.py
+-rw-rw-r--   0 root         (0) root         (0)     8065 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_country_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     6024 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_languages.py
+-rw-rw-r--   0 root         (0) root         (0)     5993 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_time_zones.py
+-rw-rw-r--   0 root         (0) root         (0)     6716 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_countries.py
+-rw-rw-r--   0 root         (0) root         (0)     5731 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_languages.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time.py
+-rw-rw-r--   0 root         (0) root         (0)     5700 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time_zones.py
+-rw-rw-r--   0 root         (0) root         (0)     9718 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/update_country_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.750378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/
+-rw-rw-r--   0 root         (0) root         (0)     1091 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8271 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/change_namespace_status.py
+-rw-rw-r--   0 root         (0) root         (0)     7814 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/create_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     6958 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/delete_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     7414 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_child_namespaces.py
+-rw-rw-r--   0 root         (0) root         (0)     7355 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_game_namespaces.py
+-rw-rw-r--   0 root         (0) root         (0)     7790 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     6174 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_context.py
+-rw-rw-r--   0 root         (0) root         (0)     6949 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_publisher.py
+-rw-rw-r--   0 root         (0) root         (0)     6219 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespaces.py
+-rw-rw-r--   0 root         (0) root         (0)     6969 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespace_publisher.py
+-rw-rw-r--   0 root         (0) root         (0)     5905 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespaces.py
+-rw-rw-r--   0 root         (0) root         (0)     8192 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/update_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.754378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/
+-rw-rw-r--   0 root         (0) root         (0)      745 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7887 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/ban_users.py
+-rw-rw-r--   0 root         (0) root         (0)     6414 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_actions.py
+-rw-rw-r--   0 root         (0) root         (0)     8185 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_banned_users.py
+-rw-rw-r--   0 root         (0) root         (0)     7918 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_user_status.py
+-rw-rw-r--   0 root         (0) root         (0)     8190 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/public_report_user.py
+-rw-rw-r--   0 root         (0) root         (0)     7059 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/report_user.py
+-rw-rw-r--   0 root         (0) root         (0)     7885 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/un_ban_users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.754378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/
+-rw-rw-r--   0 root         (0) root         (0)     2192 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7443 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/admin_get_user_profile__eda78b.py
+-rw-rw-r--   0 root         (0) root         (0)     8805 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/create_my_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     7706 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/delete_user_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     7325 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_custom_attributes_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6610 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_private_custom_a_61114d.py
+-rw-rw-r--   0 root         (0) root         (0)     7319 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_profile_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6164 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_zip_code.py
+-rw-rw-r--   0 root         (0) root         (0)     7411 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_private_custom_attr_322032.py
+-rw-rw-r--   0 root         (0) root         (0)     7653 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info.py
+-rw-rw-r--   0 root         (0) root         (0)     7856 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info_b_5dfc7f.py
+-rw-rw-r--   0 root         (0) root         (0)     8986 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_create_user_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     6700 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_custom_attri_5323c2.py
+-rw-rw-r--   0 root         (0) root         (0)     7300 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_0d683e.py
+-rw-rw-r--   0 root         (0) root         (0)     7099 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_64cc50.py
+-rw-rw-r--   0 root         (0) root         (0)     6927 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_cdd77a.py
+-rw-rw-r--   0 root         (0) root         (0)     7644 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8971 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_custom_at_7dcf23.py
+-rw-rw-r--   0 root         (0) root         (0)     9047 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_prof_c93172.py
+-rw-rw-r--   0 root         (0) root         (0)     9020 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     8947 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_custom_attribute_105f42.py
+-rw-rw-r--   0 root         (0) root         (0)     8200 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_private_custo_49ebda.py
+-rw-rw-r--   0 root         (0) root         (0)     8776 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     8107 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_zip_code.py
+-rw-rw-r--   0 root         (0) root         (0)     9040 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_private_custom_a_62b74f.py
+-rw-rw-r--   0 root         (0) root         (0)     8914 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile.py
+-rw-rw-r--   0 root         (0) root         (0)     9036 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.754378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     7490 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4409 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    17778 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8549 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_equ8_config.py
+-rw-rw-r--   0 root         (0) root         (0)    18348 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_file_upload.py
+-rw-rw-r--   0 root         (0) root         (0)    31986 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_misc.py
+-rw-rw-r--   0 root         (0) root         (0)    39193 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)    23847 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_user_action.py
+-rw-rw-r--   0 root         (0) root         (0)    94690 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_user_profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:11.758378 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-26 05:40:11.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8709 2024-03-26 05:40:11.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:40:11.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:40:11.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:40:11.000000 accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-basic-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:40:11.758378 accelbyte-py-sdk-service-basic-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-basic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-basic
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Basic Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Basic Service
-* Version: 2.19.0
+* Version: 2.19.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/README.md` & `accelbyte-py-sdk-service-basic-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Basic Service
-* Version: 2.19.0
+* Version: 2.19.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # anonymization
 from .wrappers import anonymize_user_profile
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .a_dto_for_unban_user_api_call import ADTOForUnbanUserAPICall
 from .a_dto_for_update_equ8_config_api_call import ADTOForUpdateEqu8ConfigAPICall
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_for_unban_user_api_call.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_for_unban_user_api_call.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_for_update_equ8_config_api_call.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_for_update_equ8_config_api_call.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_ban_status.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_ban_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_status.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/a_dto_object_for_equ8_user_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/action.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/action.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/add_country_group_request.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/add_country_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/add_country_group_response.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/add_country_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_create.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/config_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/config_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/country_group_object.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/country_group_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/country_object.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/country_object.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/equ8_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/equ8_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/error_entity.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/field_validation_error.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/field_validation_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/file_upload_url_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/file_upload_url_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_context.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_context.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_create.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_publisher_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_publisher_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_status_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_status_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/namespace_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/namespace_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/retrieve_country_group_response.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/retrieve_country_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/retrieve_time_response.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/retrieve_time_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/update_country_group_request.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/update_country_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_ban_request.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_ban_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_admin.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_admin.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_bulk_request.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_bulk_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_create.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_private_create.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_private_create.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_private_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_private_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_public_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_public_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_status_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_status_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_profile_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_profile_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_report_request.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_report_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_zip_code.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_zip_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/user_zip_code_update.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/user_zip_code_update.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/models/validation_error_entity.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/models/validation_error_entity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/anonymization/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/anonymization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .anonymize_user_profile import AnonymizeUserProfile
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/anonymization/anonymize_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/anonymization/anonymize_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_config import CreateConfig
 from .delete_config_1 import DeleteConfig1
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/create_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/create_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/delete_config_1.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/delete_config_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/get_config_1.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/get_config_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/get_publisher_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/get_publisher_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/config/update_config_1.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/config/update_config_1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_config import DeleteConfig
 from .get_config import GetConfig
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/delete_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/delete_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/get_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/get_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/equ8_config/update_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/equ8_config/update_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .generated_upload_url import GeneratedUploadUrl
 from .generated_user_upload_c_8f862a import GeneratedUserUploadContentUrl
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_upload_url.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_upload_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_user_upload_c_8f862a.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/generated_user_upload_c_8f862a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_upload_url.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_upload_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_user_u_2061db.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/file_upload/public_generated_user_u_2061db.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .add_country_group import AddCountryGroup
 from .delete_country_group import DeleteCountryGroup
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/add_country_group.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/add_country_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/delete_country_group.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/delete_country_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_countries.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_countries.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_country_groups.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_country_groups.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_languages.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_languages.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/get_time_zones.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/get_time_zones.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_countries.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_countries.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_languages.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_languages.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time_zones.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/public_get_time_zones.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/misc/update_country_group.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/misc/update_country_group.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .change_namespace_status import ChangeNamespaceStatus
 from .create_namespace import CreateNamespace
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/change_namespace_status.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/change_namespace_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/create_namespace.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/create_namespace.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/delete_namespace.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/delete_namespace.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_child_namespaces.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_child_namespaces.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_game_namespaces.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_game_namespaces.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_context.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_context.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_publisher.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespace_publisher.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespaces.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespace_publisher.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespace_publisher.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespaces.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/public_get_namespaces.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/namespace/update_namespace.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/namespace/update_namespace.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .ban_users import BanUsers
 from .get_actions import GetActions
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/ban_users.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/ban_users.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_actions.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_actions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_banned_users.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_banned_users.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/get_user_status.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/get_user_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/public_report_user.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/public_report_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/report_user.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/report_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_action/un_ban_users.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_action/un_ban_users.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_user_profile__eda78b import AdminGetUserProfilePublicInfoByIds
 from .create_my_profile import CreateMyProfile
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/admin_get_user_profile__eda78b.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/admin_get_user_profile__eda78b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/create_my_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/create_my_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/delete_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/delete_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_custom_attributes_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_custom_attributes_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_private_custom_a_61114d.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_private_custom_a_61114d.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_profile_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_profile_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_zip_code.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_my_zip_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_private_custom_attr_322032.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_private_custom_attr_322032.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info_b_5dfc7f.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/get_user_profile_info_b_5dfc7f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_create_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_create_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_custom_attri_5323c2.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_custom_attri_5323c2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_0d683e.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_0d683e.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_64cc50.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_64cc50.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_cdd77a.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_cdd77a.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_info.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_get_user_profile_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_custom_at_7dcf23.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_custom_at_7dcf23.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_prof_c93172.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_prof_c93172.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/public_update_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_custom_attribute_105f42.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_custom_attribute_105f42.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_private_custo_49ebda.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_private_custo_49ebda.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_zip_code.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_my_zip_code.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_private_custom_a_62b74f.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_private_custom_a_62b74f.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile_status.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/operations/user_profile/update_user_profile_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/__init__.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Basic Service."""
 
-__version__ = "2.19.0"
+__version__ = "2.19.1"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._anonymization import anonymize_user_profile
 from ._anonymization import anonymize_user_profile_async
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_anonymization.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_anonymization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_equ8_config.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_equ8_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_file_upload.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_file_upload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_misc.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_misc.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_namespace.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_namespace.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_user_action.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_user_action.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk/api/basic/wrappers/_user_profile.py` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk/api/basic/wrappers/_user_profile.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-basic
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Basic Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Basic Service
-* Version: 2.19.0
+* Version: 2.19.1
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-basic-0.8.0/accelbyte_py_sdk_service_basic.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-basic-0.9.0/accelbyte_py_sdk_service_basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

