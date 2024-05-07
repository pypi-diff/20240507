# Comparing `tmp/accelbyte-py-sdk-service-gdpr-0.7.0.tar.gz` & `tmp/accelbyte_py_sdk_service_gdpr-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-gdpr-0.7.0.tar", last modified: Tue Mar 26 05:42:02 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_gdpr-0.8.0.tar", last modified: Tue May  7 06:27:42 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-gdpr-0.7.0.tar` & `accelbyte_py_sdk_service_gdpr-0.8.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      866 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/
--rw-rw-r--   0 root         (0) root         (0)     3744 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/
--rw-rw-r--   0 root         (0) root         (0)     1754 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py
--rw-rw-r--   0 root         (0) root         (0)     4663 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py
--rw-rw-r--   0 root         (0) root         (0)     7023 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py
--rw-rw-r--   0 root         (0) root         (0)     4427 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     4382 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py
--rw-rw-r--   0 root         (0) root         (0)     5241 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py
--rw-rw-r--   0 root         (0) root         (0)     6657 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py
--rw-rw-r--   0 root         (0) root         (0)     7490 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py
--rw-rw-r--   0 root         (0) root         (0)     5062 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     5062 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     5433 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     8595 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py
--rw-rw-r--   0 root         (0) root         (0)     4517 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py
--rw-rw-r--   0 root         (0) root         (0)     3632 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py
--rw-rw-r--   0 root         (0) root         (0)     5368 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py
--rw-rw-r--   0 root         (0) root         (0)     5091 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py
--rw-rw-r--   0 root         (0) root         (0)     4432 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/
--rw-rw-r--   0 root         (0) root         (0)      432 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.779636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/
--rw-rw-r--   0 root         (0) root         (0)      982 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6538 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py
--rw-rw-r--   0 root         (0) root         (0)     6232 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py
--rw-rw-r--   0 root         (0) root         (0)     7774 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py
--rw-rw-r--   0 root         (0) root         (0)     7865 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py
--rw-rw-r--   0 root         (0) root         (0)     6158 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     7231 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     7184 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/
--rw-rw-r--   0 root         (0) root         (0)     1268 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7511 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py
--rw-rw-r--   0 root         (0) root         (0)    10996 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py
--rw-rw-r--   0 root         (0) root         (0)     7320 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py
--rw-rw-r--   0 root         (0) root         (0)     7672 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py
--rw-rw-r--   0 root         (0) root         (0)     5305 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py
--rw-rw-r--   0 root         (0) root         (0)     7102 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py
--rw-rw-r--   0 root         (0) root         (0)     5243 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py
--rw-rw-r--   0 root         (0) root         (0)     7041 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py
--rw-rw-r--   0 root         (0) root         (0)     7912 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py
--rw-rw-r--   0 root         (0) root         (0)     8484 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/
--rw-rw-r--   0 root         (0) root         (0)     1140 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8196 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py
--rw-rw-r--   0 root         (0) root         (0)     9241 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py
--rw-rw-r--   0 root         (0) root         (0)     9496 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py
--rw-rw-r--   0 root         (0) root         (0)     8987 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py
--rw-rw-r--   0 root         (0) root         (0)     8339 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py
--rw-rw-r--   0 root         (0) root         (0)     7989 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py
--rw-rw-r--   0 root         (0) root         (0)     9039 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py
--rw-rw-r--   0 root         (0) root         (0)     8785 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py
--rw-rw-r--   0 root         (0) root         (0)     7999 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4025 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    23047 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    31048 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py
--rw-rw-r--   0 root         (0) root         (0)    31574 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-03-26 05:42:02.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4108 2024-03-26 05:42:02.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:42:02.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:42:02.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:42:02.000000 accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      353 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-gdpr-0.7.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:42:02.783636 accelbyte-py-sdk-service-gdpr-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      866 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.302171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/
+-rw-rw-r--   0 root         (0) root         (0)     3744 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/
+-rw-rw-r--   0 root         (0) root         (0)     1754 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     4663 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     7023 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py
+-rw-rw-r--   0 root         (0) root         (0)     4427 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4382 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5241 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6657 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7490 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5062 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5433 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     8595 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3632 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py
+-rw-rw-r--   0 root         (0) root         (0)     5368 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5091 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/
+-rw-rw-r--   0 root         (0) root         (0)      432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      982 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py
+-rw-rw-r--   0 root         (0) root         (0)     6353 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py
+-rw-rw-r--   0 root         (0) root         (0)     7885 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py
+-rw-rw-r--   0 root         (0) root         (0)     7972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py
+-rw-rw-r--   0 root         (0) root         (0)     6269 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     7338 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     7354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/
+-rw-rw-r--   0 root         (0) root         (0)     1268 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py
+-rw-rw-r--   0 root         (0) root         (0)    11263 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py
+-rw-rw-r--   0 root         (0) root         (0)     7579 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py
+-rw-rw-r--   0 root         (0) root         (0)     5608 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py
+-rw-rw-r--   0 root         (0) root         (0)     7499 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py
+-rw-rw-r--   0 root         (0) root         (0)     7455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py
+-rw-rw-r--   0 root         (0) root         (0)     8284 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py
+-rw-rw-r--   0 root         (0) root         (0)     8882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.306171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/
+-rw-rw-r--   0 root         (0) root         (0)     1140 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py
+-rw-rw-r--   0 root         (0) root         (0)     9407 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py
+-rw-rw-r--   0 root         (0) root         (0)     9638 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py
+-rw-rw-r--   0 root         (0) root         (0)     9128 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py
+-rw-rw-r--   0 root         (0) root         (0)     8482 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py
+-rw-rw-r--   0 root         (0) root         (0)     8413 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py
+-rw-rw-r--   0 root         (0) root         (0)     9455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py
+-rw-rw-r--   0 root         (0) root         (0)     8359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4025 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    20661 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    31388 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py
+-rw-rw-r--   0 root         (0) root         (0)    30852 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:27:42.000000 accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      353 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_gdpr-0.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:27:42.310171 accelbyte_py_sdk_service_gdpr-0.8.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/PKG-INFO` & `accelbyte_py_sdk_service_gdpr-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gdpr
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Gdpr Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.8.0
+* Version: 2.9.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/README.md` & `accelbyte_py_sdk_service_gdpr-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.8.0
+* Version: 2.9.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # configuration
 from .wrappers import admin_get_services_configuration
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .dto_extend_config_dto import DtoExtendConfigDTO
 from .dto_service_config_dto import DtoServiceConfigDTO
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_extend_config_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_config_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_service_configuration_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/dto_services_configuration_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_data_retrieval_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_deletion_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_deletion_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_list_personal_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_personal_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_request_delete_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_data_url.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/models_user_personal_data_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/models/response_error.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_services_conf_be46ef import AdminGetServicesConfiguration
 from .admin_reset_services_co_abf06c import AdminResetServicesConfiguration
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_get_services_conf_be46ef.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,15 @@
 from ...models import ResponseError
 
 
 class AdminGetServicesConfiguration(Operation):
     """Get Registered Services Configuration (AdminGetServicesConfiguration)
 
     Get Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -71,31 +66,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/services/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/services/configurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_reset_services_co_abf06c.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,17 @@
 
 from ...models import ResponseError
 
 
 class AdminResetServicesConfiguration(Operation):
     """Reset Registered Services Configuration (AdminResetServicesConfiguration)
 
-    [TEST FACILITY ONLY]
+    **[TEST FACILITY ONLY]**
     Reset Registered Services Configuration to use the default configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations/reset
 
@@ -69,31 +64,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/services/configurations/reset"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/services/configurations/reset"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/admin_update_services_c_ea010e.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,15 @@
 from ...models import ResponseError
 
 
 class AdminUpdateServicesConfiguration(Operation):
     """Update Registered Services Configuration (AdminUpdateServicesConfiguration)
 
     Update Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -73,32 +68,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/services/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/services/configurations"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     body: DtoServiceConfigurationUpdateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/delete_admin_email_conf_009cca.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,15 @@
 from ...models import ResponseError
 
 
 class DeleteAdminEmailConfiguration(Operation):
     """Delete admin emails configurations (DeleteAdminEmailConfiguration)
 
     Delete a list of admin email addresses to stop receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -76,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     emails: List[str]  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/get_admin_email_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,15 @@
 from ...models import ResponseError
 
 
 class GetAdminEmailConfiguration(Operation):
     """Get admin email addresses configuration (GetAdminEmailConfiguration)
 
     Get list of admin email address configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -68,31 +63,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/save_admin_email_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,15 @@
 from ...models import ResponseError
 
 
 class SaveAdminEmailConfiguration(Operation):
     """Add admin email address configuration (SaveAdminEmailConfiguration)
 
     Add admin email address for receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -72,32 +67,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     body: List[str]  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/configuration/update_admin_email_conf_71e966.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,19 +32,18 @@
 from ...models import ResponseError
 
 
 class UpdateAdminEmailConfiguration(Operation):
     """Update admin email address configuration (UpdateAdminEmailConfiguration)
 
     Update admin email address for receiving personal data request notification.
+    Scope: account
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
         method: PUT
 
         tags: ["Configuration"]
@@ -68,32 +67,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/emails/configurations"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     body: List[str]  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_cancel_user_accou_de1ba5 import AdminCancelUserAccountDeletionRequest
 from .admin_get_list_deletion_227d7d import AdminGetListDeletionDataRequest
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_cancel_user_accou_de1ba5.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 
 from ...models import ResponseError
 
 
 class AdminCancelUserAccountDeletionRequest(Operation):
     """Cancel user's account deletion request (AdminCancelUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -73,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_list_deletion_227d7d.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 from ...models import ModelsListDeletionDataResponse
 from ...models import ResponseError
 
 
 class AdminGetListDeletionDataRequest(Operation):
     """Retrieve all user's account deletion requests in specified date (AdminGetListDeletionDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER[READ]` and scope `account`
+    Retrieve all user's account deletion requests in specified date
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/deletions
 
@@ -79,20 +80,24 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/deletions"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/deletions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     after: str  # OPTIONAL in [query]
     before: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     request_date: str  # OPTIONAL in [query]
 
@@ -101,14 +106,22 @@
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_get_user_account__84ef5a.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 from ...models import ModelsDeletionData
 from ...models import ResponseError
 
 
 class AdminGetUserAccountDeletionRequest(Operation):
     """Retrieve specific user's account deletion request (AdminGetUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId}[READ]` and scope `account`
+    Retrieve specific user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -69,32 +70,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/admin_submit_user_accou_b7780f.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 from ...models import ModelsRequestDeleteResponse
 from ...models import ResponseError
 
 
 class AdminSubmitUserAccountDeletionRequest(Operation):
     """Submit user's account deletion requests (AdminSubmitUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Submit user's account deletion requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -74,32 +72,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/deletions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["*/*"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_my_accoun_107811.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from ...models import ResponseError
 
 
 class PublicCancelMyAccountDeletionRequest(Operation):
     """Cancel my account deletion request (PublicCancelMyAccountDeletionRequest)
 
+    Cancel my account deletion request
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: DELETE
 
@@ -61,29 +62,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/users/me/deletions"
+    _path: str = "/gdpr/public/users/me/deletions"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_cancel_user_acco_16b962.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 
 from ...models import ResponseError
 
 
 class PublicCancelUserAccountDeletionRequest(Operation):
     """Cancel user's account deletion request (PublicCancelUserAccountDeletionRequest)
 
+    Cancel user's account deletion request
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: DELETE
 
         tags: ["Data Deletion"]
@@ -65,32 +70,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_my_account_d_8595d0.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from ...models import ModelsDeletionStatus
 from ...models import ResponseError
 
 
 class PublicGetMyAccountDeletionStatus(Operation):
     """Retrieve my account deletion status (PublicGetMyAccountDeletionStatus)
 
+    Retrieve my account deletion status
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions/status
 
         method: GET
 
@@ -60,29 +61,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/users/me/deletions/status"
+    _path: str = "/gdpr/public/users/me/deletions/status"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_get_user_account_09e4f2.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,20 @@
 from ...models import ModelsDeletionStatus
 from ...models import ResponseError
 
 
 class PublicGetUserAccountDeletionStatus(Operation):
     """Retrieve specific user's account deletion status (PublicGetUserAccountDeletionStatus)
 
+    Retrieve specific user's account deletion status
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions/status
 
         method: GET
 
         tags: ["Data Deletion"]
@@ -64,32 +69,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions/status"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions/status"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_my_accoun_f5ded3.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 from ...models import ModelsRequestDeleteResponse
 from ...models import ResponseError
 
 
 class PublicSubmitMyAccountDeletionRequest(Operation):
     """Submit my account deletion requests. (PublicSubmitMyAccountDeletionRequest)
 
+    Submit my account deletion requests.
     Requires valid user access token
-
-    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
+    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use [/gdpr/public/namespaces/{namespace}/users/{userId}/deletions](#operations-Data_Deletion-PublicSubmitUserAccountDeletionRequest)
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/users/me/deletions"
+    _path: str = "/gdpr/public/users/me/deletions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     platform_id: str  # REQUIRED in [form_data]
     platform_token: str  # REQUIRED in [form_data]
 
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_deletion/public_submit_user_acco_a6db4f.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,20 @@
 from ...models import ModelsRequestDeleteResponse
 from ...models import ResponseError
 
 
 class PublicSubmitUserAccountDeletionRequest(Operation):
     """Submit user's account deletion requests (PublicSubmitUserAccountDeletionRequest)
 
+    Submit user's account deletion requests
     Requires valid user access token and password
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
@@ -70,33 +75,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/deletions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     password: str  # REQUIRED in [form_data]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_cancel_user_perso_78952d import AdminCancelUserPersonalDataRequest
 from .admin_generate_personal_48c32b import AdminGeneratePersonalDataURL
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,26 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminCancelUserPersonalDataRequest(Operation):
-    """Cancel user's personal data requests (AdminCancelUserPersonalDataRequest)
+class PublicCancelUserPersonalDataRequest(Operation):
+    """Cancel user's personal data requests (PublicCancelUserPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's personal data requests
+    Requires valid user access token
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
-        url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}
+        url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
         method: DELETE
 
         tags: ["Data Retrieval"]
 
         consumes: ["application/json"]
 
@@ -73,35 +72,49 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = (
-        "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
+        "/gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
+    )
+    _path: str = (
+        "/gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
     )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     request_date: str  # REQUIRED in [path]
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
 
@@ -144,23 +157,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> AdminCancelUserPersonalDataRequest:
+    def with_namespace(self, value: str) -> PublicCancelUserPersonalDataRequest:
         self.namespace = value
         return self
 
-    def with_request_date(self, value: str) -> AdminCancelUserPersonalDataRequest:
+    def with_request_date(self, value: str) -> PublicCancelUserPersonalDataRequest:
         self.request_date = value
         return self
 
-    def with_user_id(self, value: str) -> AdminCancelUserPersonalDataRequest:
+    def with_user_id(self, value: str) -> PublicCancelUserPersonalDataRequest:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -231,27 +244,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, request_date: str, user_id: str, **kwargs
-    ) -> AdminCancelUserPersonalDataRequest:
+    ) -> PublicCancelUserPersonalDataRequest:
         instance = cls()
         instance.namespace = namespace
         instance.request_date = request_date
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminCancelUserPersonalDataRequest:
+    ) -> PublicCancelUserPersonalDataRequest:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "requestDate" in dict_ and dict_["requestDate"] is not None:
             instance.request_date = str(dict_["requestDate"])
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_generate_personal_48c32b.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 from ...models import ModelsUserDataURL
 from ...models import ResponseError
 
 
 class AdminGeneratePersonalDataURL(Operation):
     """Generate personal data download url (AdminGeneratePersonalDataURL)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Generate personal data download url
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
@@ -76,34 +74,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     password: str  # REQUIRED in [form_data]
     namespace: str  # REQUIRED in [path]
     request_date: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_list_personal_424fda.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 from ...models import ModelsListPersonalDataResponse
 from ...models import ResponseError
 
 
 class AdminGetListPersonalDataRequest(Operation):
     """Get list personal data requests (AdminGetListPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]
+    Get list personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/requests
 
@@ -78,34 +76,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/requests"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/requests"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     request_date: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_get_user_personal_a892c0.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,16 @@
 from ...models import ModelsUserPersonalDataResponse
 from ...models import ResponseError
 
 
 class AdminGetUserPersonalDataRequests(Operation):
     """Get user's personal data requests (AdminGetUserPersonalDataRequests)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Get user's personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -74,34 +72,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_request_data_retrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,17 @@
 from ...models import ModelsDataRetrievalResponse
 from ...models import ResponseError
 
 
 class AdminRequestDataRetrieval(Operation):
     """Submit user personal data retrieval request (AdminRequestDataRetrieval)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-
-
-
+    Submit user personal data retrieval request
     If admin request data for themselves, password is need to be set
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -77,33 +71,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests"
+    _path: str = "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     password: str  # OPTIONAL in [form_data]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_cancel_user_pers_19dafa.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/admin_cancel_user_perso_78952d.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,25 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class PublicCancelUserPersonalDataRequest(Operation):
-    """Cancel user's personal data requests (PublicCancelUserPersonalDataRequest)
+class AdminCancelUserPersonalDataRequest(Operation):
+    """Cancel user's personal data requests (AdminCancelUserPersonalDataRequest)
 
-    Requires valid user access token
+    Cancel user's personal data requests
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
-        url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}
+        url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
         method: DELETE
 
         tags: ["Data Retrieval"]
 
         consumes: ["application/json"]
 
@@ -67,35 +71,49 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = (
-        "/gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
+        "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
+    )
+    _path: str = (
+        "/gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}"
     )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     request_date: str  # REQUIRED in [path]
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
 
@@ -138,23 +156,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublicCancelUserPersonalDataRequest:
+    def with_namespace(self, value: str) -> AdminCancelUserPersonalDataRequest:
         self.namespace = value
         return self
 
-    def with_request_date(self, value: str) -> PublicCancelUserPersonalDataRequest:
+    def with_request_date(self, value: str) -> AdminCancelUserPersonalDataRequest:
         self.request_date = value
         return self
 
-    def with_user_id(self, value: str) -> PublicCancelUserPersonalDataRequest:
+    def with_user_id(self, value: str) -> AdminCancelUserPersonalDataRequest:
         self.user_id = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -225,27 +243,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, request_date: str, user_id: str, **kwargs
-    ) -> PublicCancelUserPersonalDataRequest:
+    ) -> AdminCancelUserPersonalDataRequest:
         instance = cls()
         instance.namespace = namespace
         instance.request_date = request_date
         instance.user_id = user_id
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicCancelUserPersonalDataRequest:
+    ) -> AdminCancelUserPersonalDataRequest:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "requestDate" in dict_ and dict_["requestDate"] is not None:
             instance.request_date = str(dict_["requestDate"])
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_generate_persona_6b68a4.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,20 @@
 from ...models import ModelsUserDataURL
 from ...models import ResponseError
 
 
 class PublicGeneratePersonalDataURL(Operation):
     """Generate personal data download url (PublicGeneratePersonalDataURL)
 
+    Generate personal data download url
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
         method: POST
 
         tags: ["Data Retrieval"]
@@ -70,34 +75,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     password: str  # REQUIRED in [form_data]
     namespace: str  # REQUIRED in [path]
     request_date: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_get_user_persona_7e40c3.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,20 @@
 from ...models import ModelsUserPersonalDataResponse
 from ...models import ResponseError
 
 
 class PublicGetUserPersonalDataRequests(Operation):
     """Get user's personal data requests (PublicGetUserPersonalDataRequests)
 
+    Get user's personal data requests
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: GET
 
         tags: ["Data Retrieval"]
@@ -68,34 +73,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/operations/data_retrieval/public_request_data_retrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 from ...models import ModelsDataRetrievalResponse
 from ...models import ResponseError
 
 
 class PublicRequestDataRetrieval(Operation):
     """Submit personal data retrieval request (PublicRequestDataRetrieval)
 
-    Requires valid user access token
+    Submit personal data retrieval request.
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: POST
 
         tags: ["Data Retrieval"]
@@ -66,33 +70,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests"
+    _path: str = "/gdpr/public/namespaces/{namespace}/users/{userId}/requests"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/x-www-form-urlencoded"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "gdpr"
+
     password: str  # REQUIRED in [form_data]
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

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Gdpr Service."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._configuration import admin_get_services_configuration
 from ._configuration import admin_get_services_configuration_async
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get Registered Services Configuration (AdminGetServicesConfiguration)
 
     Get Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -100,20 +95,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get Registered Services Configuration (AdminGetServicesConfiguration)
 
     Get Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -154,22 +144,17 @@
 def admin_reset_services_configuration(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Reset Registered Services Configuration (AdminResetServicesConfiguration)
 
-    [TEST FACILITY ONLY]
+    **[TEST FACILITY ONLY]**
     Reset Registered Services Configuration to use the default configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations/reset
 
@@ -206,22 +191,17 @@
 async def admin_reset_services_configuration_async(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Reset Registered Services Configuration (AdminResetServicesConfiguration)
 
-    [TEST FACILITY ONLY]
+    **[TEST FACILITY ONLY]**
     Reset Registered Services Configuration to use the default configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations/reset
 
@@ -262,20 +242,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Registered Services Configuration (AdminUpdateServicesConfiguration)
 
     Update Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -319,20 +294,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Registered Services Configuration (AdminUpdateServicesConfiguration)
 
     Update Registered Services Configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:GDPR:CONFIGURATION [UPDATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/services/configurations
 
@@ -378,20 +348,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete admin emails configurations (DeleteAdminEmailConfiguration)
 
     Delete a list of admin email addresses to stop receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -439,20 +404,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Delete admin emails configurations (DeleteAdminEmailConfiguration)
 
     Delete a list of admin email addresses to stop receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [DELETE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -501,20 +461,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get admin email addresses configuration (GetAdminEmailConfiguration)
 
     Get list of admin email address configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -552,20 +507,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get admin email addresses configuration (GetAdminEmailConfiguration)
 
     Get list of admin email address configuration.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [READ]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -606,20 +556,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add admin email address configuration (SaveAdminEmailConfiguration)
 
     Add admin email address for receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -663,20 +608,15 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Add admin email address configuration (SaveAdminEmailConfiguration)
 
     Add admin email address for receiving personal data request notification.
-
-
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
@@ -722,19 +662,18 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update admin email address configuration (UpdateAdminEmailConfiguration)
 
     Update admin email address for receiving personal data request notification.
+    Scope: account
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
         method: PUT
 
         tags: ["Configuration"]
@@ -775,19 +714,18 @@
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update admin email address configuration (UpdateAdminEmailConfiguration)
 
     Update admin email address for receiving personal data request notification.
+    Scope: account
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:EMAIL:CONFIGURATION [UPDATE]
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/emails/configurations
 
         method: PUT
 
         tags: ["Configuration"]
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_deletion.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,18 +52,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's account deletion request (AdminCancelUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -110,18 +108,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's account deletion request (AdminCancelUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -174,15 +170,16 @@
     request_date: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve all user's account deletion requests in specified date (AdminGetListDeletionDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER[READ]` and scope `account`
+    Retrieve all user's account deletion requests in specified date
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/deletions
 
@@ -245,15 +242,16 @@
     request_date: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve all user's account deletion requests in specified date (AdminGetListDeletionDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER[READ]` and scope `account`
+    Retrieve all user's account deletion requests in specified date
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/deletions
 
@@ -314,15 +312,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve specific user's account deletion request (AdminGetUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId}[READ]` and scope `account`
+    Retrieve specific user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -367,15 +366,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve specific user's account deletion request (AdminGetUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId}[READ]` and scope `account`
+    Retrieve specific user's account deletion request
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -422,18 +422,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user's account deletion requests (AdminSubmitUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Submit user's account deletion requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -480,18 +478,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user's account deletion requests (AdminSubmitUserAccountDeletionRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Submit user's account deletion requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/deletions
 
@@ -537,14 +533,15 @@
 
 @same_doc_as(PublicCancelMyAccountDeletionRequest)
 def public_cancel_my_account_deletion_request(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Cancel my account deletion request (PublicCancelMyAccountDeletionRequest)
 
+    Cancel my account deletion request
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: DELETE
 
@@ -573,14 +570,15 @@
 
 @same_doc_as(PublicCancelMyAccountDeletionRequest)
 async def public_cancel_my_account_deletion_request_async(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Cancel my account deletion request (PublicCancelMyAccountDeletionRequest)
 
+    Cancel my account deletion request
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: DELETE
 
@@ -614,15 +612,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's account deletion request (PublicCancelUserAccountDeletionRequest)
 
+    Cancel user's account deletion request
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: DELETE
 
         tags: ["Data Deletion"]
@@ -664,15 +667,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's account deletion request (PublicCancelUserAccountDeletionRequest)
 
+    Cancel user's account deletion request
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: DELETE
 
         tags: ["Data Deletion"]
@@ -713,14 +721,15 @@
 
 @same_doc_as(PublicGetMyAccountDeletionStatus)
 def public_get_my_account_deletion_status(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve my account deletion status (PublicGetMyAccountDeletionStatus)
 
+    Retrieve my account deletion status
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions/status
 
         method: GET
 
@@ -747,14 +756,15 @@
 
 @same_doc_as(PublicGetMyAccountDeletionStatus)
 async def public_get_my_account_deletion_status_async(
     x_additional_headers: Optional[Dict[str, str]] = None, **kwargs
 ):
     """Retrieve my account deletion status (PublicGetMyAccountDeletionStatus)
 
+    Retrieve my account deletion status
     Requires valid user access token
 
     Properties:
         url: /gdpr/public/users/me/deletions/status
 
         method: GET
 
@@ -786,15 +796,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve specific user's account deletion status (PublicGetUserAccountDeletionStatus)
 
+    Retrieve specific user's account deletion status
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions/status
 
         method: GET
 
         tags: ["Data Deletion"]
@@ -834,15 +849,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Retrieve specific user's account deletion status (PublicGetUserAccountDeletionStatus)
 
+    Retrieve specific user's account deletion status
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions/status
 
         method: GET
 
         tags: ["Data Deletion"]
@@ -884,17 +904,17 @@
     platform_id: str,
     platform_token: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit my account deletion requests. (PublicSubmitMyAccountDeletionRequest)
 
+    Submit my account deletion requests.
     Requires valid user access token
-
-    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
+    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use [/gdpr/public/namespaces/{namespace}/users/{userId}/deletions](#operations-Data_Deletion-PublicSubmitUserAccountDeletionRequest)
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
@@ -934,17 +954,17 @@
     platform_id: str,
     platform_token: str,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit my account deletion requests. (PublicSubmitMyAccountDeletionRequest)
 
+    Submit my account deletion requests.
     Requires valid user access token
-
-    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
+    This is for in-game only and require a valid platformId and platform token. If a full account is not logged by 3rd platform, then please use [/gdpr/public/namespaces/{namespace}/users/{userId}/deletions](#operations-Data_Deletion-PublicSubmitUserAccountDeletionRequest)
 
     Properties:
         url: /gdpr/public/users/me/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
@@ -987,15 +1007,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user's account deletion requests (PublicSubmitUserAccountDeletionRequest)
 
+    Submit user's account deletion requests
     Requires valid user access token and password
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
@@ -1043,15 +1068,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user's account deletion requests (PublicSubmitUserAccountDeletionRequest)
 
+    Submit user's account deletion requests
     Requires valid user access token and password
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/deletions
 
         method: POST
 
         tags: ["Data Deletion"]
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk/api/gdpr/wrappers/_data_retrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,18 +52,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's personal data requests (AdminCancelUserPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
@@ -112,18 +110,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's personal data requests (AdminCancelUserPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [DELETE]
+    Cancel user's personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
@@ -175,18 +171,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate personal data download url (AdminGeneratePersonalDataURL)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Generate personal data download url
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
@@ -239,18 +233,16 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate personal data download url (AdminGeneratePersonalDataURL)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Generate personal data download url
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
@@ -305,18 +297,16 @@
     request_date: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get list personal data requests (AdminGetListPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]
+    Get list personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/requests
 
@@ -371,18 +361,16 @@
     request_date: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get list personal data requests (AdminGetListPersonalDataRequest)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER [READ]
+    Get list personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/requests
 
@@ -439,18 +427,16 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's personal data requests (AdminGetUserPersonalDataRequests)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Get user's personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -501,18 +487,16 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's personal data requests (AdminGetUserPersonalDataRequests)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]` and scope `account`
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [READ]
+    Get user's personal data requests
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -564,23 +548,17 @@
     password: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user personal data retrieval request (AdminRequestDataRetrieval)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-
-
-
+    Submit user personal data retrieval request
     If admin request data for themselves, password is need to be set
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -627,23 +605,17 @@
     password: Optional[str] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit user personal data retrieval request (AdminRequestDataRetrieval)
 
-    Required permission `ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]` and scope `account`
-
-
-
-
+    Submit user personal data retrieval request
     If admin request data for themselves, password is need to be set
-
-    Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:INFORMATION:USER:{userId} [CREATE]
+    Scope: account
 
     Required Scope(s):
         - account
 
     Properties:
         url: /gdpr/admin/namespaces/{namespace}/users/{userId}/requests
 
@@ -692,15 +664,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's personal data requests (PublicCancelUserPersonalDataRequest)
 
+    Cancel user's personal data requests
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
         method: DELETE
 
         tags: ["Data Retrieval"]
@@ -746,15 +723,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Cancel user's personal data requests (PublicCancelUserPersonalDataRequest)
 
+    Cancel user's personal data requests
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}
 
         method: DELETE
 
         tags: ["Data Retrieval"]
@@ -803,15 +785,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate personal data download url (PublicGeneratePersonalDataURL)
 
+    Generate personal data download url
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
         method: POST
 
         tags: ["Data Retrieval"]
@@ -861,15 +848,20 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Generate personal data download url (PublicGeneratePersonalDataURL)
 
+    Generate personal data download url
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests/{requestDate}/generate
 
         method: POST
 
         tags: ["Data Retrieval"]
@@ -921,15 +913,20 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's personal data requests (PublicGetUserPersonalDataRequests)
 
+    Get user's personal data requests
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: GET
 
         tags: ["Data Retrieval"]
@@ -977,15 +974,20 @@
     offset: Optional[int] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Get user's personal data requests (PublicGetUserPersonalDataRequests)
 
+    Get user's personal data requests
     Requires valid user access token
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: GET
 
         tags: ["Data Retrieval"]
@@ -1034,15 +1036,19 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit personal data retrieval request (PublicRequestDataRetrieval)
 
-    Requires valid user access token
+    Submit personal data retrieval request.
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: POST
 
         tags: ["Data Retrieval"]
@@ -1086,15 +1092,19 @@
     user_id: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Submit personal data retrieval request (PublicRequestDataRetrieval)
 
-    Requires valid user access token
+    Submit personal data retrieval request.
+    Scope: account
+
+    Required Scope(s):
+        - account
 
     Properties:
         url: /gdpr/public/namespaces/{namespace}/users/{userId}/requests
 
         method: POST
 
         tags: ["Data Retrieval"]
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-gdpr
-Version: 0.7.0
+Version: 0.8.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Gdpr Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Gdpr Service
-* Version: 2.8.0
+* Version: 2.9.0
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-gdpr-0.7.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_gdpr-0.8.0/accelbyte_py_sdk_service_gdpr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

