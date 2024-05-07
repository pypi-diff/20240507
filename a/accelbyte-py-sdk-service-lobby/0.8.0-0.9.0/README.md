# Comparing `tmp/accelbyte-py-sdk-service-lobby-0.8.0.tar.gz` & `tmp/accelbyte_py_sdk_service_lobby-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-lobby-0.8.0.tar", last modified: Wed Mar 13 06:13:06 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_lobby-0.9.0.tar", last modified: Tue May  7 06:28:52 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-lobby-0.8.0.tar` & `accelbyte_py_sdk_service_lobby-0.9.0.tar`

### file list

```diff
@@ -1,353 +1,361 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.426179 accelbyte-py-sdk-service-lobby-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-13 06:13:06.426179 accelbyte-py-sdk-service-lobby-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      868 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.394179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.394179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.394179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/
--rw-rw-r--   0 root         (0) root         (0)    11918 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.402179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/
--rw-rw-r--   0 root         (0) root         (0)     7977 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7354 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/handlers_get_users_presence_response.py
--rw-rw-r--   0 root         (0) root         (0)     7213 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/handlers_user_presence.py
--rw-rw-r--   0 root         (0) root         (0)     7048 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/log_app_message_declaration.py
--rw-rw-r--   0 root         (0) root         (0)     3901 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3916 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     5475 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_users_free_form_notification_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5580 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_template_request.py
--rw-rw-r--   0 root         (0) root         (0)     4463 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request.py
--rw-rw-r--   0 root         (0) root         (0)     4594 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4506 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request.py
--rw-rw-r--   0 root         (0) root         (0)     4623 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4501 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friend_with_platform.py
--rw-rw-r--   0 root         (0) root         (0)     4544 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection_response.py
--rw-rw-r--   0 root         (0) root         (0)     5169 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_template_slug_resp.py
--rw-rw-r--   0 root         (0) root         (0)     5324 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_topics_response.py
--rw-rw-r--   0 root         (0) root         (0)     6879 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     5988 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     4948 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_incoming_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     4948 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_outgoing_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     8767 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_global_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4671 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_incoming_friends_with_time_data.py
--rw-rw-r--   0 root         (0) root         (0)     4320 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_list_bulk_user_platforms_response.py
--rw-rw-r--   0 root         (0) root         (0)     5362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_load_incoming_friends_with_time_response.py
--rw-rw-r--   0 root         (0) root         (0)     5362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_load_outgoing_friends_with_time_response.py
--rw-rw-r--   0 root         (0) root         (0)     6612 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_localization.py
--rw-rw-r--   0 root         (0) root         (0)     6083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     5229 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_sync_response.py
--rw-rw-r--   0 root         (0) root         (0)     5389 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_template_response.py
--rw-rw-r--   0 root         (0) root         (0)     5921 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response.py
--rw-rw-r--   0 root         (0) root         (0)     6083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6557 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request.py
--rw-rw-r--   0 root         (0) root         (0)     6678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4671 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_outgoing_friends_with_time_data.py
--rw-rw-r--   0 root         (0) root         (0)     5419 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     8258 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_put_global_configuration_request.py
--rw-rw-r--   0 root         (0) root         (0)     4386 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_content.py
--rw-rw-r--   0 root         (0) root         (0)     7506 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_localization.py
--rw-rw-r--   0 root         (0) root         (0)     7161 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_localization_response.py
--rw-rw-r--   0 root         (0) root         (0)     4995 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_response.py
--rw-rw-r--   0 root         (0) root         (0)     6809 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_topic_by_namespaces_response.py
--rw-rw-r--   0 root         (0) root         (0)     4000 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_update_template_request.py
--rw-rw-r--   0 root         (0) root         (0)     3875 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_update_topic_request.py
--rw-rw-r--   0 root         (0) root         (0)     3883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_accept_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     3883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_cancel_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     4473 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_get_friendship_status_response.py
--rw-rw-r--   0 root         (0) root         (0)     5612 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_platform_info.py
--rw-rw-r--   0 root         (0) root         (0)     3883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_reject_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     4850 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_request_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     3838 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_unfriend_request.py
--rw-rw-r--   0 root         (0) root         (0)     7125 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_with_platform_info.py
--rw-rw-r--   0 root         (0) root         (0)     4624 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filter_into_list_request.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_filter_request.py
--rw-rw-r--   0 root         (0) root         (0)     4550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_request.py
--rw-rw-r--   0 root         (0) root         (0)     5357 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_create_profanity_list_request.py
--rw-rw-r--   0 root         (0) root         (0)     3964 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_delete_profanity_filter_request.py
--rw-rw-r--   0 root         (0) root         (0)     4424 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_list_filters_v1_response.py
--rw-rw-r--   0 root         (0) root         (0)     5411 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_lists_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     4006 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_set_profanity_rule_for_namespace_request.py
--rw-rw-r--   0 root         (0) root         (0)     5337 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_update_profanity_list.py
--rw-rw-r--   0 root         (0) root         (0)     4809 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_request.py
--rw-rw-r--   0 root         (0) root         (0)     4979 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_response.py
--rw-rw-r--   0 root         (0) root         (0)     3950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_block_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     4506 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_blocked_by_player_data.py
--rw-rw-r--   0 root         (0) root         (0)     4633 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_blocked_player_data.py
--rw-rw-r--   0 root         (0) root         (0)    25346 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config.py
--rw-rw-r--   0 root         (0) root         (0)     3988 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config_list.py
--rw-rw-r--   0 root         (0) root         (0)    24859 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config_req.py
--rw-rw-r--   0 root         (0) root         (0)     3809 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_create_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     4505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_create_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     3846 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_debug_profanity_filter_request.py
--rw-rw-r--   0 root         (0) root         (0)     4388 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_by_users_response.py
--rw-rw-r--   0 root         (0) root         (0)     4350 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_users_response.py
--rw-rw-r--   0 root         (0) root         (0)     4271 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_session_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_request.py
--rw-rw-r--   0 root         (0) root         (0)     4593 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_response.py
--rw-rw-r--   0 root         (0) root         (0)     4455 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     4040 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_lobby_ccu_response.py
--rw-rw-r--   0 root         (0) root         (0)     4511 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_player_session_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     6520 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_import_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     4221 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_list_blocked_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     8030 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_data.py
--rw-rw-r--   0 root         (0) root         (0)     5017 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_put_custom_attributes_request.py
--rw-rw-r--   0 root         (0) root         (0)     3832 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_put_limit_size_request.py
--rw-rw-r--   0 root         (0) root         (0)     5667 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_profanity_filter.py
--rw-rw-r--   0 root         (0) root         (0)     4337 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_profanity_rule.py
--rw-rw-r--   0 root         (0) root         (0)     4226 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_set_player_session_attribute_request.py
--rw-rw-r--   0 root         (0) root         (0)     3820 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_unblock_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     3809 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_update_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     4505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_update_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     4432 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/response_error.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_body.py
--rw-rw-r--   0 root         (0) root         (0)     4587 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.402179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/
--rw-rw-r--   0 root         (0) root         (0)      433 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.406179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/
--rw-rw-r--   0 root         (0) root         (0)     1212 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_delete_global_config.py
--rw-rw-r--   0 root         (0) root         (0)     5819 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_get_global_config.py
--rw-rw-r--   0 root         (0) root         (0)     6342 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_update_global_config.py
--rw-rw-r--   0 root         (0) root         (0)     7721 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/create_template.py
--rw-rw-r--   0 root         (0) root         (0)     8322 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_localization.py
--rw-rw-r--   0 root         (0) root         (0)     7222 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_slug.py
--rw-rw-r--   0 root         (0) root         (0)     7616 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/free_form_notification.py
--rw-rw-r--   0 root         (0) root         (0)     6499 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_game_template.py
--rw-rw-r--   0 root         (0) root         (0)     8464 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_localization_template.py
--rw-rw-r--   0 root         (0) root         (0)     9869 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_slug_template.py
--rw-rw-r--   0 root         (0) root         (0)     8019 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/notification_with_template.py
--rw-rw-r--   0 root         (0) root         (0)     8292 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/publish_template.py
--rw-rw-r--   0 root         (0) root         (0)     9484 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/update_localization_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.406179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/
--rw-rw-r--   0 root         (0) root         (0)      741 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14538 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_export_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     5763 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_all_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6724 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_import_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8075 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_update_config_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.406179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/
--rw-rw-r--   0 root         (0) root         (0)     1664 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8260 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/add_friends_without_con_a5cd59.py
--rw-rw-r--   0 root         (0) root         (0)    10919 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/admin_list_friends_of_friends.py
--rw-rw-r--   0 root         (0) root         (0)     8530 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/bulk_delete_friends.py
--rw-rw-r--   0 root         (0) root         (0)    10025 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_incoming_friend_requests.py
--rw-rw-r--   0 root         (0) root         (0)    10861 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_list_of_friends.py
--rw-rw-r--   0 root         (0) root         (0)     9196 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_outgoing_friend_requests.py
--rw-rw-r--   0 root         (0) root         (0)     8438 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_updated.py
--rw-rw-r--   0 root         (0) root         (0)     8505 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_with_platform.py
--rw-rw-r--   0 root         (0) root         (0)     8678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_frien_a30279.py
--rw-rw-r--   0 root         (0) root         (0)     8521 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_friends.py
--rw-rw-r--   0 root         (0) root         (0)     8678 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_frien_132c7c.py
--rw-rw-r--   0 root         (0) root         (0)     8521 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_friends.py
--rw-rw-r--   0 root         (0) root         (0)     8439 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/sync_native_friends.py
--rw-rw-r--   0 root         (0) root         (0)     7716 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_accept_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_cancel_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     7486 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_get_friendship_status.py
--rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_reject_friend_request.py
--rw-rw-r--   0 root         (0) root         (0)     8173 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_request_friend.py
--rw-rw-r--   0 root         (0) root         (0)     7656 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_unfriend_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.406179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/
--rw-rw-r--   0 root         (0) root         (0)      640 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8443 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_join_party_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9144 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_update_party_attr_920eb3.py
--rw-rw-r--   0 root         (0) root         (0)     4841 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/public_get_messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.410179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/
--rw-rw-r--   0 root         (0) root         (0)     2501 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8078 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_tem_590da9.py
--rw-rw-r--   0 root         (0) root         (0)     7483 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_top_701ddd.py
--rw-rw-r--   0 root         (0) root         (0)     7581 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_topic.py
--rw-rw-r--   0 root         (0) root         (0)     7417 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_tem_8c8a06.py
--rw-rw-r--   0 root         (0) root         (0)     7466 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_top_00eb0a.py
--rw-rw-r--   0 root         (0) root         (0)     8427 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_template_localiz_55eb81.py
--rw-rw-r--   0 root         (0) root         (0)     7269 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_topic_by_topic_name.py
--rw-rw-r--   0 root         (0) root         (0)     8381 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/free_form_notification__54ba50.py
--rw-rw-r--   0 root         (0) root         (0)     6969 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_te_0053f8.py
--rw-rw-r--   0 root         (0) root         (0)     9132 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_to_761be1.py
--rw-rw-r--   0 root         (0) root         (0)     7479 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_notification_topic__b8a441.py
--rw-rw-r--   0 root         (0) root         (0)     8586 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_single_template_loc_d01d4b.py
--rw-rw-r--   0 root         (0) root         (0)    10260 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_template_slug_local_385ba4.py
--rw-rw-r--   0 root         (0) root         (0)     8985 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_namespace.py
--rw-rw-r--   0 root         (0) root         (0)     7272 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_topic_name.py
--rw-rw-r--   0 root         (0) root         (0)     8788 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/notification_with_templ_f80964.py
--rw-rw-r--   0 root         (0) root         (0)     8495 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/publish_template_locali_b4f377.py
--rw-rw-r--   0 root         (0) root         (0)     7675 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_multiple_users_fre_78d5b0.py
--rw-rw-r--   0 root         (0) root         (0)     8491 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_freeform_not_1f36fa.py
--rw-rw-r--   0 root         (0) root         (0)     8858 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_templated_no_8a9ca4.py
--rw-rw-r--   0 root         (0) root         (0)     8531 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_free_3a173d.py
--rw-rw-r--   0 root         (0) root         (0)     8920 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_temp_0499f2.py
--rw-rw-r--   0 root         (0) root         (0)     7768 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_freeform_not_3d805f.py
--rw-rw-r--   0 root         (0) root         (0)     8153 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_templated_no_9d39cc.py
--rw-rw-r--   0 root         (0) root         (0)     8810 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_notification_top_0e4c05.py
--rw-rw-r--   0 root         (0) root         (0)     9839 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_template_localiz_cc6e6e.py
--rw-rw-r--   0 root         (0) root         (0)     8377 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_topic_by_topic_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.410179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/
--rw-rw-r--   0 root         (0) root         (0)      774 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7478 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_party_data_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7465 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_user_party_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7583 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_get_party_data_v1.py
--rw-rw-r--   0 root         (0) root         (0)     8677 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_set_party_limit_v1.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_update_party_att_aeeff0.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.410179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/
--rw-rw-r--   0 root         (0) root         (0)     1325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8426 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_bulk_block_players_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7362 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_all_player_se_b925d7.py
--rw-rw-r--   0 root         (0) root         (0)     8321 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_bulk_player_b_0addc5.py
--rw-rw-r--   0 root         (0) root         (0)     6815 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_lobby_ccu.py
--rw-rw-r--   0 root         (0) root         (0)     7748 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_7da3f3.py
--rw-rw-r--   0 root         (0) root         (0)     7823 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_8955db.py
--rw-rw-r--   0 root         (0) root         (0)     8598 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_sessio_625ce8.py
--rw-rw-r--   0 root         (0) root         (0)     8765 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_set_player_sessio_1bc722.py
--rw-rw-r--   0 root         (0) root         (0)     7107 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_0dc6b7.py
--rw-rw-r--   0 root         (0) root         (0)     7045 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_55d58a.py
--rw-rw-r--   0 root         (0) root         (0)     7882 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_player_block_players_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7812 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_unblock_player_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.414179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/presence/
--rw-rw-r--   0 root         (0) root         (0)      528 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/presence/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8181 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/presence/users_presence_handler_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.414179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/
--rw-rw-r--   0 root         (0) root         (0)     1381 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8798 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_fil_e31341.py
--rw-rw-r--   0 root         (0) root         (0)     8681 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_filters.py
--rw-rw-r--   0 root         (0) root         (0)     7871 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_create_profanity_list.py
--rw-rw-r--   0 root         (0) root         (0)     8090 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_debug_profanity_filters.py
--rw-rw-r--   0 root         (0) root         (0)     8862 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_filter.py
--rw-rw-r--   0 root         (0) root         (0)     7394 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_list.py
--rw-rw-r--   0 root         (0) root         (0)     7725 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lis_fd0d45.py
--rw-rw-r--   0 root         (0) root         (0)     6895 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lists.py
--rw-rw-r--   0 root         (0) root         (0)     6740 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_rule.py
--rw-rw-r--   0 root         (0) root         (0)     8337 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_import_profanity__286711.py
--rw-rw-r--   0 root         (0) root         (0)     8078 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_set_profanity_rul_e9d9e0.py
--rw-rw-r--   0 root         (0) root         (0)     8514 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_update_profanity_list.py
--rw-rw-r--   0 root         (0) root         (0)     8310 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_verify_message_pr_169572.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.414179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/
--rw-rw-r--   0 root         (0) root         (0)      749 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7977 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_create_third_part_225a9c.py
--rw-rw-r--   0 root         (0) root         (0)     6630 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_delete_third_part_c9d441.py
--rw-rw-r--   0 root         (0) root         (0)     6527 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_get_third_party_config.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_update_third_part_9b81f7.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.414179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/
--rw-rw-r--   0 root         (0) root         (0)    12107 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38576 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_admin.py
--rw-rw-r--   0 root         (0) root         (0)    25876 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_config.py
--rw-rw-r--   0 root         (0) root         (0)    63370 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_friends.py
--rw-rw-r--   0 root         (0) root         (0)     9467 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_lobby_operations.py
--rw-rw-r--   0 root         (0) root         (0)    91351 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_notification.py
--rw-rw-r--   0 root         (0) root         (0)    16671 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_party.py
--rw-rw-r--   0 root         (0) root         (0)    38641 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_player.py
--rw-rw-r--   0 root         (0) root         (0)     4148 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_presence.py
--rw-rw-r--   0 root         (0) root         (0)    41239 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_profanity.py
--rw-rw-r--   0 root         (0) root         (0)    12939 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_third_party.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.422179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/
--rw-rw-r--   0 root         (0) root         (0)    12726 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2946 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     3341 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3758 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     4083 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_response.py
--rw-rw-r--   0 root         (0) root         (0)     2926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     3793 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_request.py
--rw-rw-r--   0 root         (0) root         (0)     3347 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_response.py
--rw-rw-r--   0 root         (0) root         (0)     3993 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/channel_chat_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/client_reset_request.py
--rw-rw-r--   0 root         (0) root         (0)     2988 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/connect_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3345 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/disconnect_notif.py
--rw-rw-r--   0 root         (0) root         (0)    10171 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/ds_notif.py
--rw-rw-r--   0 root         (0) root         (0)     2898 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/error_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3281 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/exit_all_channel.py
--rw-rw-r--   0 root         (0) root         (0)     2520 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_request.py
--rw-rw-r--   0 root         (0) root         (0)     5533 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_response.py
--rw-rw-r--   0 root         (0) root         (0)     2570 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_request.py
--rw-rw-r--   0 root         (0) root         (0)     3783 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     3397 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_request.py
--rw-rw-r--   0 root         (0) root         (0)     3802 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_response.py
--rw-rw-r--   0 root         (0) root         (0)     3341 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_request.py
--rw-rw-r--   0 root         (0) root         (0)     3686 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     2016 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/heartbeat.py
--rw-rw-r--   0 root         (0) root         (0)     2554 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_request.py
--rw-rw-r--   0 root         (0) root         (0)     3748 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_response.py
--rw-rw-r--   0 root         (0) root         (0)     2558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3857 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     3359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3883 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     2550 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_online_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     2558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3907 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     5289 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/matchmaking_notif.py
--rw-rw-r--   0 root         (0) root         (0)     4587 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/message_notif.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/message_session_notif.py
--rw-rw-r--   0 root         (0) root         (0)     2558 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_request.py
--rw-rw-r--   0 root         (0) root         (0)     3355 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_response.py
--rw-rw-r--   0 root         (0) root         (0)     3935 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/online_friends.py
--rw-rw-r--   0 root         (0) root         (0)     4304 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_notif.py
--rw-rw-r--   0 root         (0) root         (0)     4312 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_request.py
--rw-rw-r--   0 root         (0) root         (0)     3301 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_response.py
--rw-rw-r--   0 root         (0) root         (0)     2512 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     5182 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     5517 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_data_update_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3708 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_get_invited_notif.py
--rw-rw-r--   0 root         (0) root         (0)     2504 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_request.py
--rw-rw-r--   0 root         (0) root         (0)     5656 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_response.py
--rw-rw-r--   0 root         (0) root         (0)     3325 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3351 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_request.py
--rw-rw-r--   0 root         (0) root         (0)     3309 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_response.py
--rw-rw-r--   0 root         (0) root         (0)     2910 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3770 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_request.py
--rw-rw-r--   0 root         (0) root         (0)     5174 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_response.py
--rw-rw-r--   0 root         (0) root         (0)     3634 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3343 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_request.py
--rw-rw-r--   0 root         (0) root         (0)     3301 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_response.py
--rw-rw-r--   0 root         (0) root         (0)     3281 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3454 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_request.py
--rw-rw-r--   0 root         (0) root         (0)     3305 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_response.py
--rw-rw-r--   0 root         (0) root         (0)     3475 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_request.py
--rw-rw-r--   0 root         (0) root         (0)     5224 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_response.py
--rw-rw-r--   0 root         (0) root         (0)     3642 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3778 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_request.py
--rw-rw-r--   0 root         (0) root         (0)     3666 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_response.py
--rw-rw-r--   0 root         (0) root         (0)     3397 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_request.py
--rw-rw-r--   0 root         (0) root         (0)     4043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_response.py
--rw-rw-r--   0 root         (0) root         (0)     4316 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_notif.py
--rw-rw-r--   0 root         (0) root         (0)     4324 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_request.py
--rw-rw-r--   0 root         (0) root         (0)     3313 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_response.py
--rw-rw-r--   0 root         (0) root         (0)     3319 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_request.py
--rw-rw-r--   0 root         (0) root         (0)     3313 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_response.py
--rw-rw-r--   0 root         (0) root         (0)     2926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3359 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     2976 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/rematchmaking_notif.py
--rw-rw-r--   0 root         (0) root         (0)     2950 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3377 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_request.py
--rw-rw-r--   0 root         (0) root         (0)     3335 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_response.py
--rw-rw-r--   0 root         (0) root         (0)     3762 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_request.py
--rw-rw-r--   0 root         (0) root         (0)     3339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_response.py
--rw-rw-r--   0 root         (0) root         (0)     3291 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3371 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_request.py
--rw-rw-r--   0 root         (0) root         (0)     3339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_response.py
--rw-rw-r--   0 root         (0) root         (0)     4043 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_request.py
--rw-rw-r--   0 root         (0) root         (0)     3355 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_response.py
--rw-rw-r--   0 root         (0) root         (0)     3754 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_request.py
--rw-rw-r--   0 root         (0) root         (0)     3331 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_response.py
--rw-rw-r--   0 root         (0) root         (0)     2910 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/shutdown_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3343 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/signaling_p2p_notif.py
--rw-rw-r--   0 root         (0) root         (0)     5032 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_request.py
--rw-rw-r--   0 root         (0) root         (0)     3343 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_response.py
--rw-rw-r--   0 root         (0) root         (0)     3369 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3806 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_request.py
--rw-rw-r--   0 root         (0) root         (0)     4145 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_response.py
--rw-rw-r--   0 root         (0) root         (0)     2926 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_notif.py
--rw-rw-r--   0 root         (0) root         (0)     3339 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_request.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_response.py
--rw-rw-r--   0 root         (0) root         (0)     2082 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_banned_notification.py
--rw-rw-r--   0 root         (0) root         (0)     2508 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_request.py
--rw-rw-r--   0 root         (0) root         (0)     3702 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_response.py
--rw-rw-r--   0 root         (0) root         (0)     4069 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_status_notif.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:13:06.426179 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-13 06:13:06.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22906 2024-03-13 06:13:06.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:13:06.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:13:06.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:13:06.000000 accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      354 2024-03-13 06:08:59.000000 accelbyte-py-sdk-service-lobby-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:13:06.426179 accelbyte-py-sdk-service-lobby-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.056278 accelbyte_py_sdk_service_lobby-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-07 06:28:52.056278 accelbyte_py_sdk_service_lobby-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      868 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.024279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.024279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.028279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/
+-rw-rw-r--   0 root         (0) root         (0)    12120 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.036279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/
+-rw-rw-r--   0 root         (0) root         (0)     8192 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/handlers_get_users_presence_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7213 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/handlers_user_presence.py
+-rw-rw-r--   0 root         (0) root         (0)     7048 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/log_app_message_declaration.py
+-rw-rw-r--   0 root         (0) root         (0)     3901 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3916 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5475 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_users_free_form_notification_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     5580 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_template_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4463 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4594 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4501 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friend_with_platform.py
+-rw-rw-r--   0 root         (0) root         (0)     4544 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5169 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_template_slug_resp.py
+-rw-rw-r--   0 root         (0) root         (0)     5324 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_topics_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6879 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5988 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_incoming_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_outgoing_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_global_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_incoming_friends_with_time_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4320 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_list_bulk_user_platforms_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5362 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_load_incoming_friends_with_time_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5362 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_load_outgoing_friends_with_time_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6612 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_localization.py
+-rw-rw-r--   0 root         (0) root         (0)     6083 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5229 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_sync_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4604 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_user_block_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5216 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_user_block_response.py
+-rw-rw-r--   0 root         (0) root         (0)    11685 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5389 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_template_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5921 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6083 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6557 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6678 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_outgoing_friends_with_time_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5419 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     8258 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_put_global_configuration_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_content.py
+-rw-rw-r--   0 root         (0) root         (0)     7506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_localization.py
+-rw-rw-r--   0 root         (0) root         (0)     7161 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_localization_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4995 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_topic_by_namespaces_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4000 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_update_template_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3875 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_update_topic_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3883 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_accept_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3883 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_cancel_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4473 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_get_friendship_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5612 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_platform_info.py
+-rw-rw-r--   0 root         (0) root         (0)     3883 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_reject_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4850 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_request_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3838 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_unfriend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7125 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_with_platform_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filter_into_list_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_filter_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4550 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5357 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_create_profanity_list_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3964 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_delete_profanity_filter_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_list_filters_v1_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5411 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_lists_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4006 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_set_profanity_rule_for_namespace_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5337 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_update_profanity_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4979 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3950 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_block_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4506 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_blocked_by_player_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4633 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_blocked_player_data.py
+-rw-rw-r--   0 root         (0) root         (0)    25346 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3988 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config_list.py
+-rw-rw-r--   0 root         (0) root         (0)    24859 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config_req.py
+-rw-rw-r--   0 root         (0) root         (0)     3809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_create_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4505 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_create_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3846 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_debug_profanity_filter_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4388 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_by_users_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4350 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_users_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4271 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_session_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4593 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4040 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_lobby_ccu_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4511 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_player_session_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6520 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_import_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4221 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_list_blocked_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8030 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5017 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_put_custom_attributes_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3832 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_put_limit_size_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5667 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_profanity_filter.py
+-rw-rw-r--   0 root         (0) root         (0)     4337 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_profanity_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     4226 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_set_player_session_attribute_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3820 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_unblock_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_update_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4505 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_update_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4432 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_body.py
+-rw-rw-r--   0 root         (0) root         (0)     4587 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.036279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/
+-rw-rw-r--   0 root         (0) root         (0)      433 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.036279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/
+-rw-rw-r--   0 root         (0) root         (0)     1212 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5221 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_delete_global_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6090 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_get_global_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6613 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_update_global_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8001 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/create_template.py
+-rw-rw-r--   0 root         (0) root         (0)     8646 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_localization.py
+-rw-rw-r--   0 root         (0) root         (0)     7517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_slug.py
+-rw-rw-r--   0 root         (0) root         (0)     7895 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/free_form_notification.py
+-rw-rw-r--   0 root         (0) root         (0)     6779 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_game_template.py
+-rw-rw-r--   0 root         (0) root         (0)     8788 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_localization_template.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_slug_template.py
+-rw-rw-r--   0 root         (0) root         (0)     8299 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/notification_with_template.py
+-rw-rw-r--   0 root         (0) root         (0)     8624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/publish_template.py
+-rw-rw-r--   0 root         (0) root         (0)     9808 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/update_localization_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.036279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/blocks/
+-rw-rw-r--   0 root         (0) root         (0)      526 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/blocks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8366 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/blocks/sync_native_blocked_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.036279 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14824 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_export_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6019 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_all_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7003 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_import_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_update_config_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.040278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/
+-rw-rw-r--   0 root         (0) root         (0)     1664 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8549 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/add_friends_without_con_a5cd59.py
+-rw-rw-r--   0 root         (0) root         (0)    11240 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/admin_list_friends_of_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     8822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/bulk_delete_friends.py
+-rw-rw-r--   0 root         (0) root         (0)    10328 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_incoming_friend_requests.py
+-rw-rw-r--   0 root         (0) root         (0)    11155 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_list_of_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     9499 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_outgoing_friend_requests.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_updated.py
+-rw-rw-r--   0 root         (0) root         (0)     8783 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_with_platform.py
+-rw-rw-r--   0 root         (0) root         (0)     8960 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_frien_a30279.py
+-rw-rw-r--   0 root         (0) root         (0)     8798 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     8960 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_frien_132c7c.py
+-rw-rw-r--   0 root         (0) root         (0)     8798 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     8803 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/sync_native_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     7999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_accept_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8019 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_cancel_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7772 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_get_friendship_status.py
+-rw-rw-r--   0 root         (0) root         (0)     8019 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_reject_friend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     8449 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_request_friend.py
+-rw-rw-r--   0 root         (0) root         (0)     7933 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_unfriend_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.040278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/
+-rw-rw-r--   0 root         (0) root         (0)      640 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8769 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_join_party_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9467 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_update_party_attr_920eb3.py
+-rw-rw-r--   0 root         (0) root         (0)     5093 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/public_get_messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.040278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/
+-rw-rw-r--   0 root         (0) root         (0)     2554 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8373 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_tem_590da9.py
+-rw-rw-r--   0 root         (0) root         (0)     7775 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_top_701ddd.py
+-rw-rw-r--   0 root         (0) root         (0)     7858 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_topic.py
+-rw-rw-r--   0 root         (0) root         (0)     7743 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_tem_8c8a06.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_top_00eb0a.py
+-rw-rw-r--   0 root         (0) root         (0)     8766 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_template_localiz_55eb81.py
+-rw-rw-r--   0 root         (0) root         (0)     7554 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_topic_by_topic_name.py
+-rw-rw-r--   0 root         (0) root         (0)     8675 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/free_form_notification__54ba50.py
+-rw-rw-r--   0 root         (0) root         (0)     7264 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_te_0053f8.py
+-rw-rw-r--   0 root         (0) root         (0)     9424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_to_761be1.py
+-rw-rw-r--   0 root         (0) root         (0)    10595 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_my_notifications.py
+-rw-rw-r--   0 root         (0) root         (0)     7799 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_notification_topic__b8a441.py
+-rw-rw-r--   0 root         (0) root         (0)     8925 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_single_template_loc_d01d4b.py
+-rw-rw-r--   0 root         (0) root         (0)    10586 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_template_slug_local_385ba4.py
+-rw-rw-r--   0 root         (0) root         (0)     9262 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_namespace.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_topic_name.py
+-rw-rw-r--   0 root         (0) root         (0)     9083 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/notification_with_templ_f80964.py
+-rw-rw-r--   0 root         (0) root         (0)     8842 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/publish_template_locali_b4f377.py
+-rw-rw-r--   0 root         (0) root         (0)     8002 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_multiple_users_fre_78d5b0.py
+-rw-rw-r--   0 root         (0) root         (0)     8810 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_freeform_not_1f36fa.py
+-rw-rw-r--   0 root         (0) root         (0)     9178 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_templated_no_8a9ca4.py
+-rw-rw-r--   0 root         (0) root         (0)     8847 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_free_3a173d.py
+-rw-rw-r--   0 root         (0) root         (0)     9237 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_temp_0499f2.py
+-rw-rw-r--   0 root         (0) root         (0)     8069 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_freeform_not_3d805f.py
+-rw-rw-r--   0 root         (0) root         (0)     8455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_templated_no_9d39cc.py
+-rw-rw-r--   0 root         (0) root         (0)     9130 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_notification_top_0e4c05.py
+-rw-rw-r--   0 root         (0) root         (0)    10178 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_template_localiz_cc6e6e.py
+-rw-rw-r--   0 root         (0) root         (0)     8662 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_topic_by_topic_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.044278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/
+-rw-rw-r--   0 root         (0) root         (0)      774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7774 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_party_data_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7764 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_user_party_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7880 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_get_party_data_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8980 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_set_party_limit_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     9500 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_update_party_att_aeeff0.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.044278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/
+-rw-rw-r--   0 root         (0) root         (0)     1325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8747 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_bulk_block_players_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7683 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_all_player_se_b925d7.py
+-rw-rw-r--   0 root         (0) root         (0)     8619 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_bulk_player_b_0addc5.py
+-rw-rw-r--   0 root         (0) root         (0)     7098 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_lobby_ccu.py
+-rw-rw-r--   0 root         (0) root         (0)     8050 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_7da3f3.py
+-rw-rw-r--   0 root         (0) root         (0)     8144 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_8955db.py
+-rw-rw-r--   0 root         (0) root         (0)     8915 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_sessio_625ce8.py
+-rw-rw-r--   0 root         (0) root         (0)     9086 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_set_player_sessio_1bc722.py
+-rw-rw-r--   0 root         (0) root         (0)     7407 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_0dc6b7.py
+-rw-rw-r--   0 root         (0) root         (0)     7342 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_55d58a.py
+-rw-rw-r--   0 root         (0) root         (0)     8177 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_player_block_players_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     8109 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_unblock_player_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.044278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/presence/
+-rw-rw-r--   0 root         (0) root         (0)      528 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/presence/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8478 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/presence/users_presence_handler_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.044278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/
+-rw-rw-r--   0 root         (0) root         (0)     1381 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9100 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_fil_e31341.py
+-rw-rw-r--   0 root         (0) root         (0)     9004 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_filters.py
+-rw-rw-r--   0 root         (0) root         (0)     8159 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_create_profanity_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_debug_profanity_filters.py
+-rw-rw-r--   0 root         (0) root         (0)     9187 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_filter.py
+-rw-rw-r--   0 root         (0) root         (0)     7689 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8027 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lis_fd0d45.py
+-rw-rw-r--   0 root         (0) root         (0)     7183 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lists.py
+-rw-rw-r--   0 root         (0) root         (0)     7027 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     8665 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_import_profanity__286711.py
+-rw-rw-r--   0 root         (0) root         (0)     8365 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_set_profanity_rul_e9d9e0.py
+-rw-rw-r--   0 root         (0) root         (0)     8809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_update_profanity_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8599 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_verify_message_pr_169572.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.044278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/
+-rw-rw-r--   0 root         (0) root         (0)      749 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8273 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_create_third_part_225a9c.py
+-rw-rw-r--   0 root         (0) root         (0)     6926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_delete_third_part_c9d441.py
+-rw-rw-r--   0 root         (0) root         (0)     6823 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_get_third_party_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8035 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_update_third_part_9b81f7.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.048278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)    12308 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38576 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_admin.py
+-rw-rw-r--   0 root         (0) root         (0)     4568 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_blocks.py
+-rw-rw-r--   0 root         (0) root         (0)    25876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)    63552 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     9467 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_lobby_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    95379 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_notification.py
+-rw-rw-r--   0 root         (0) root         (0)    16671 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_party.py
+-rw-rw-r--   0 root         (0) root         (0)    38641 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_player.py
+-rw-rw-r--   0 root         (0) root         (0)     4148 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_presence.py
+-rw-rw-r--   0 root         (0) root         (0)    41239 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_profanity.py
+-rw-rw-r--   0 root         (0) root         (0)    12939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_third_party.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.056278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/
+-rw-rw-r--   0 root         (0) root         (0)    12726 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2946 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4083 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3793 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3347 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3993 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/channel_chat_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3297 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/client_reset_request.py
+-rw-rw-r--   0 root         (0) root         (0)     2988 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/connect_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3345 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/disconnect_notif.py
+-rw-rw-r--   0 root         (0) root         (0)    10171 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/ds_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     2898 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/error_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3281 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/exit_all_channel.py
+-rw-rw-r--   0 root         (0) root         (0)     2520 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5533 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2570 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3783 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3397 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3802 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3686 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2016 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/heartbeat.py
+-rw-rw-r--   0 root         (0) root         (0)     2554 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3748 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2558 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3857 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3883 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2550 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_online_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     2558 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3907 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5289 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/matchmaking_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     4587 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/message_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/message_session_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     2558 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3355 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3935 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/online_friends.py
+-rw-rw-r--   0 root         (0) root         (0)     4304 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     4312 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3301 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2512 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5182 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5517 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_data_update_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3708 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_get_invited_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     2504 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5656 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3351 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3309 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3770 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5174 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3634 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3343 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3301 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3281 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3454 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3305 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3475 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5224 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3642 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3778 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3666 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3397 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4316 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     4324 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3313 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3319 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3313 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2976 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/rematchmaking_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     2950 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3377 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3335 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3762 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3339 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3291 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3371 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3339 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3355 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3754 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2910 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/shutdown_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3343 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/signaling_p2p_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     5032 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3343 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3369 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3806 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4145 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_notif.py
+-rw-rw-r--   0 root         (0) root         (0)     3339 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3297 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_response.py
+-rw-rw-r--   0 root         (0) root         (0)     2082 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_banned_notification.py
+-rw-rw-r--   0 root         (0) root         (0)     2508 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3702 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4069 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_status_notif.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:28:52.056278 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-07 06:28:52.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23362 2024-05-07 06:28:52.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:28:52.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:28:52.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:28:52.000000 accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      354 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_lobby-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:28:52.056278 accelbyte_py_sdk_service_lobby-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/PKG-INFO` & `accelbyte_py_sdk_service_lobby-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-lobby
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Lobby Server
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Lobby Server
-* Version: 3.35.0
+* Version: 3.35.5
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/README.md` & `accelbyte_py_sdk_service_lobby-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Lobby Server
-* Version: 3.35.0
+* Version: 3.35.5
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin
 from .wrappers import admin_delete_global_config
@@ -38,14 +38,18 @@
 from .wrappers import notification_with_template
 from .wrappers import notification_with_template_async
 from .wrappers import publish_template
 from .wrappers import publish_template_async
 from .wrappers import update_localization_template
 from .wrappers import update_localization_template_async
 
+# blocks
+from .wrappers import sync_native_blocked_user
+from .wrappers import sync_native_blocked_user_async
+
 # config
 from .wrappers import admin_export_config_v1
 from .wrappers import admin_export_config_v1_async
 from .wrappers import admin_get_all_config_v1
 from .wrappers import admin_get_all_config_v1_async
 from .wrappers import admin_get_config_v1
 from .wrappers import admin_get_config_v1_async
@@ -119,14 +123,16 @@
 from .wrappers import delete_topic_by_topic_name_async
 from .wrappers import free_form_notification_by_user_id
 from .wrappers import free_form_notification_by_user_id_async
 from .wrappers import get_all_notification_templates_v1_admin
 from .wrappers import get_all_notification_templates_v1_admin_async
 from .wrappers import get_all_notification_topics_v1_admin
 from .wrappers import get_all_notification_topics_v1_admin_async
+from .wrappers import get_my_notifications
+from .wrappers import get_my_notifications_async
 from .wrappers import get_notification_topic_v1_admin
 from .wrappers import get_notification_topic_v1_admin_async
 from .wrappers import get_single_template_localization_v1_admin
 from .wrappers import get_single_template_localization_v1_admin_async
 from .wrappers import get_template_slug_localizations_template_v1_admin
 from .wrappers import get_template_slug_localizations_template_v1_admin_async
 from .wrappers import get_topic_by_namespace
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .handlers_get_users_presence_response import HandlersGetUsersPresenceResponse
 from .handlers_user_presence import HandlersUserPresence
@@ -52,14 +52,17 @@
 )
 from .model_load_outgoing_friends_with_time_response import (
     ModelLoadOutgoingFriendsWithTimeResponse,
 )
 from .model_localization import ModelLocalization
 from .model_native_friend_request import ModelNativeFriendRequest
 from .model_native_friend_sync_response import ModelNativeFriendSyncResponse
+from .model_native_user_block_request import ModelNativeUserBlockRequest
+from .model_native_user_block_response import ModelNativeUserBlockResponse
+from .model_notification_response import ModelNotificationResponse
 from .model_notification_template_response import ModelNotificationTemplateResponse
 from .model_notification_topic_response import ModelNotificationTopicResponse
 from .model_notification_topic_response_v1 import ModelNotificationTopicResponseV1
 from .model_notification_with_template_request import (
     ModelNotificationWithTemplateRequest,
 )
 from .model_notification_with_template_request_v1 import (
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/handlers_get_users_presence_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/handlers_get_users_presence_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/handlers_user_presence.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/handlers_user_presence.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/log_app_message_declaration.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/log_app_message_declaration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_bulk_users_free_form_notification_request_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_bulk_users_free_form_notification_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_template_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_template_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_create_topic_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_free_form_notification_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friend_with_platform.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friend_with_platform.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_friendship_connection_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_template_slug_resp.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_template_slug_resp.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_topics_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_all_notification_topics_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_incoming_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_incoming_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_get_user_outgoing_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_get_user_outgoing_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_global_configuration.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_global_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_incoming_friends_with_time_data.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_incoming_friends_with_time_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_list_bulk_user_platforms_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_list_bulk_user_platforms_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_load_incoming_friends_with_time_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_load_incoming_friends_with_time_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_load_outgoing_friends_with_time_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_load_outgoing_friends_with_time_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_localization.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_localization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_sync_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_native_friend_sync_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_template_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_template_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_topic_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_outgoing_friends_with_time_data.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_outgoing_friends_with_time_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_pagination.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_put_global_configuration_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_put_global_configuration_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_content.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_content.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_localization.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_localization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_localization_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_localization_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_template_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_template_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_topic_by_namespaces_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_topic_by_namespaces_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_update_template_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_update_template_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_update_topic_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_update_topic_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_accept_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_accept_friend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_cancel_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_cancel_friend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_get_friendship_status_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_get_friendship_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_platform_info.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_platform_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_reject_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_reject_friend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_request_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_request_friend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_unfriend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_unfriend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/model_user_with_platform_info.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/model_user_with_platform_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filter_into_list_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filter_into_list_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_filter_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_filter_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_add_profanity_filters_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_create_profanity_list_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_create_profanity_list_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_delete_profanity_filter_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_delete_profanity_filter_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_list_filters_v1_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_list_filters_v1_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_lists_list_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_get_profanity_lists_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_set_profanity_rule_for_namespace_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_set_profanity_rule_for_namespace_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_update_profanity_list.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_update_profanity_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_admin_verify_message_profanity_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_block_player_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_block_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_blocked_by_player_data.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_blocked_by_player_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_blocked_player_data.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_blocked_player_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config_list.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_config_req.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_config_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_create_config_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_create_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_create_config_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_create_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_debug_profanity_filter_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_debug_profanity_filter_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_by_users_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_by_users_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_users_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_blocked_users_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_session_attribute_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_all_player_session_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_bulk_all_player_blocked_users_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_config_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_lobby_ccu_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_lobby_ccu_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_get_player_session_attribute_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_get_player_session_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_import_config_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_import_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_list_blocked_player_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_list_blocked_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_data.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_put_custom_attributes_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_put_custom_attributes_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_party_put_limit_size_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_party_put_limit_size_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_profanity_filter.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_profanity_filter.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_profanity_rule.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_profanity_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_set_player_session_attribute_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_set_player_session_attribute_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_unblock_player_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_unblock_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_update_config_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_update_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/models_update_config_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/models_update_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/response_error.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_body.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_body.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/models/restapi_error_response_v1.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_delete_global_config import AdminDeleteGlobalConfig
 from .admin_get_global_config import AdminGetGlobalConfig
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_delete_global_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/public_get_messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,61 +25,72 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import LogAppMessageDeclaration
 from ...models import RestapiErrorResponseBody
 
 
-class AdminDeleteGlobalConfig(Operation):
-    """Delete of global configuration data. (adminDeleteGlobalConfig)
+class PublicGetMessages(Operation):
+    """get service messages (publicGetMessages)
 
-    Delete of global configuration data.
+    get the list of messages.
 
     Properties:
-        url: /lobby/v1/admin/global-configurations
+        url: /lobby/v1/messages
 
-        method: DELETE
+        method: GET
 
-        tags: ["admin", "global-configurations"]
+        tags: ["Lobby Operations"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        204: No Content - str (No Content)
+        200: OK - List[LogAppMessageDeclaration] (OK)
 
-        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
-
-        403: Forbidden - RestapiErrorResponseBody (Forbidden)
+        500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/admin/global-configurations"
-    _method: str = "DELETE"
+    _url: str = "/lobby/v1/messages"
+    _path: str = "/lobby/v1/messages"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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
 
@@ -125,62 +136,61 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
+    ) -> Tuple[
+        Union[None, List[LogAppMessageDeclaration]],
+        Union[None, HttpResponse, RestapiErrorResponseBody],
+    ]:
         """Parse the given response.
 
-        204: No Content - str (No Content)
+        200: OK - List[LogAppMessageDeclaration] (OK)
 
-        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
-
-        403: Forbidden - RestapiErrorResponseBody (Forbidden)
+        500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
 
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
-        if code == 401:
-            return None, RestapiErrorResponseBody.create_from_dict(content)
-        if code == 403:
+        if code == 200:
+            return [LogAppMessageDeclaration.create_from_dict(i) for i in content], None
+        if code == 500:
             return None, RestapiErrorResponseBody.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> AdminDeleteGlobalConfig:
+    def create(cls, **kwargs) -> PublicGetMessages:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteGlobalConfig:
+    ) -> PublicGetMessages:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_get_global_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_get_global_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,29 +64,41 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/global-configurations"
+    _path: str = "/lobby/v1/admin/global-configurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_update_global_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_update_global_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,31 +61,43 @@
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/global-configurations"
+    _path: str = "/lobby/v1/admin/global-configurations"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelPutGlobalConfigurationRequest  # REQUIRED in [body]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/create_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/create_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,32 +70,44 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates"
+    _path: str = "/notification/namespaces/{namespace}/templates"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelCreateTemplateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_localization.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_slug.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/delete_template_slug.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/free_form_notification.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/free_form_notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,32 +66,44 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/freeform"
+    _path: str = "/notification/namespaces/{namespace}/freeform"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelFreeFormNotificationRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_game_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_game_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,31 +64,43 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates"
+    _path: str = "/notification/namespaces/{namespace}/templates"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_localization_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_localization_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,33 +68,45 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/get_slug_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/get_slug_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,24 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
     after: str  # OPTIONAL in [query]
     before: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
 
     # endregion fields
@@ -93,14 +97,22 @@
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/notification_with_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/notification_with_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templated"
+    _path: str = "/notification/namespaces/{namespace}/templated"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelNotificationWithTemplateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/publish_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/publish_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/admin/update_localization_template.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_template_localiz_cc6e6e.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,30 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelUpdateTemplateRequest
-from ...models import RestapiErrorResponseBody
+from ...models import RestapiErrorResponseV1
 
 
-class UpdateLocalizationTemplate(Operation):
-    """update template draft (updateLocalizationTemplate)
+class UpdateTemplateLocalizationV1Admin(Operation):
+    """update template localization (updateTemplateLocalizationV1Admin)
 
-    Modify draft template
+    Update template localization
+
+    Action Code: 50208
 
     Properties:
-        url: /notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
+        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
 
         method: PUT
 
-        tags: ["admin", "notification"]
+        tags: ["notification"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -58,46 +60,60 @@
         template_language: (templateLanguage) REQUIRED str in path
 
         template_slug: (templateSlug) REQUIRED str in path
 
     Responses:
         204: No Content - (No Content)
 
-        400: Bad Request - RestapiErrorResponseBody (Bad Request)
+        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
+
+        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
-        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
+        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
-        403: Forbidden - RestapiErrorResponseBody (Forbidden)
+        404: Not Found - RestapiErrorResponseV1 (Not Found)
 
-        404: Not Found - RestapiErrorResponseBody (Not Found)
+        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUpdateTemplateRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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
 
@@ -148,27 +164,27 @@
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
         self, value: ModelUpdateTemplateRequest
-    ) -> UpdateLocalizationTemplate:
+    ) -> UpdateTemplateLocalizationV1Admin:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateLocalizationTemplate:
+    def with_namespace(self, value: str) -> UpdateTemplateLocalizationV1Admin:
         self.namespace = value
         return self
 
-    def with_template_language(self, value: str) -> UpdateLocalizationTemplate:
+    def with_template_language(self, value: str) -> UpdateTemplateLocalizationV1Admin:
         self.template_language = value
         return self
 
-    def with_template_slug(self, value: str) -> UpdateLocalizationTemplate:
+    def with_template_slug(self, value: str) -> UpdateTemplateLocalizationV1Admin:
         self.template_slug = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -195,26 +211,28 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
+    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseV1]]:
         """Parse the given response.
 
         204: No Content - (No Content)
 
-        400: Bad Request - RestapiErrorResponseBody (Bad Request)
+        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
+
+        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
-        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
+        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
-        403: Forbidden - RestapiErrorResponseBody (Forbidden)
+        404: Not Found - RestapiErrorResponseV1 (Not Found)
 
-        404: Not Found - RestapiErrorResponseBody (Not Found)
+        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -224,21 +242,23 @@
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 204:
             return None, None
         if code == 400:
-            return None, RestapiErrorResponseBody.create_from_dict(content)
+            return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 401:
-            return None, RestapiErrorResponseBody.create_from_dict(content)
+            return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 403:
-            return None, RestapiErrorResponseBody.create_from_dict(content)
+            return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 404:
-            return None, RestapiErrorResponseBody.create_from_dict(content)
+            return None, RestapiErrorResponseV1.create_from_dict(content)
+        if code == 500:
+            return None, RestapiErrorResponseV1.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
@@ -248,28 +268,28 @@
     def create(
         cls,
         body: ModelUpdateTemplateRequest,
         namespace: str,
         template_language: str,
         template_slug: str,
         **kwargs,
-    ) -> UpdateLocalizationTemplate:
+    ) -> UpdateTemplateLocalizationV1Admin:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         instance.template_language = template_language
         instance.template_slug = template_slug
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateLocalizationTemplate:
+    ) -> UpdateTemplateLocalizationV1Admin:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelUpdateTemplateRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelUpdateTemplateRequest()
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_export_config_v1 import AdminExportConfigV1
 from .admin_get_all_config_v1 import AdminGetAllConfigV1
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_export_config_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_export_config_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -274,31 +274,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/config/namespaces/{namespace}/export"
+    _path: str = "/lobby/v1/admin/config/namespaces/{namespace}/export"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_all_config_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_all_config_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,29 +65,41 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/config"
+    _path: str = "/lobby/v1/admin/config"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_config_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_get_config_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,31 +67,43 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/config/namespaces/{namespace}"
+    _path: str = "/lobby/v1/admin/config/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_import_config_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_import_config_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/config/namespaces/{namespace}/import"
+    _path: str = "/lobby/v1/admin/config/namespaces/{namespace}/import"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["multipart/form-data"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/config/admin_update_config_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/config/admin_update_config_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/config/namespaces/{namespace}"
+    _path: str = "/lobby/v1/admin/config/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsConfigReq  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .add_friends_without_con_a5cd59 import AddFriendsWithoutConfirmation
 from .admin_list_friends_of_friends import AdminListFriendsOfFriends
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/add_friends_without_con_a5cd59.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/add_friends_without_con_a5cd59.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,33 +68,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/users/{userId}/add/bulk"
+    _path: str = "/friends/namespaces/{namespace}/users/{userId}/add/bulk"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelBulkFriendsRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/admin_list_friends_of_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/admin_list_friends_of_friends.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/of-friends"
     )
+    _path: str = (
+        "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/of-friends"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     friend_id: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     nopaging: bool  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
@@ -98,14 +104,22 @@
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/bulk_delete_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/bulk_delete_friends.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,33 +69,45 @@
 
         500: Internal Server Error - ModelBulkFriendsResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/users/{userId}/delete/bulk"
+    _path: str = "/friends/namespaces/{namespace}/users/{userId}/delete/bulk"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelBulkFriendsRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_incoming_friend_requests.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_incoming_friend_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,24 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/incoming"
+    _path: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/incoming"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     friend_id: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
     # endregion fields
@@ -93,14 +97,22 @@
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_list_of_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_list_of_friends.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,20 +74,24 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}"
+    _path: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     friend_id: str  # OPTIONAL in [query]
     friend_ids: List[str]  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
@@ -96,14 +100,22 @@
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_outgoing_friend_requests.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_outgoing_friend_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,34 +70,46 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/outgoing"
+    _path: str = "/lobby/v1/admin/friend/namespaces/{namespace}/users/{userId}/outgoing"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_updated.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_updated.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me"
+    _path: str = "/friends/namespaces/{namespace}/me"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_with_platform.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_friends_with_platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/platforms"
+    _path: str = "/friends/namespaces/{namespace}/me/platforms"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_frien_a30279.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_frien_a30279.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/incoming-time"
+    _path: str = "/friends/namespaces/{namespace}/me/incoming-time"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_incoming_friends.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/incoming"
+    _path: str = "/friends/namespaces/{namespace}/me/incoming"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_frien_132c7c.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_frien_132c7c.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/outgoing-time"
+    _path: str = "/friends/namespaces/{namespace}/me/outgoing-time"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/get_user_outgoing_friends.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/outgoing"
+    _path: str = "/friends/namespaces/{namespace}/me/outgoing"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/sync_native_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/sync_native_friends.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 from ...models import ModelNativeFriendSyncResponse
 from ...models import RestapiErrorResponseV1
 
 
 class SyncNativeFriends(Operation):
     """sync friends using server to server call to native first party server. (syncNativeFriends)
 
-    Sync friends using server to server call to native first party servere.
+    Sync friends using server to server call to native first party server.
     Supported platforms:
     steam: The platform_tokenâs value is the binary ticket returned by Steam.
     If this ticket was generated by Steam GetAuthTicketForWebApi with version >= 1.57, then platform token should use this style: {identity}:{ticket}
     the {identity} was the parameter to call GetAuthTicketForWebApi when the ticket was created. Note: Do not contain : in this {identity}
     ps4: The platform_tokenâs value is the authorization code returned by Sony OAuth.
     ps5: The platform_tokenâs value is the authorization code returned by Sony OAuth.
+    pspc: The platform_tokenâs value is the authorization code returned by Sony OAuth.
 
     Properties:
         url: /friends/sync/namespaces/{namespace}/me
 
         method: PATCH
 
         tags: ["friends", "public"]
@@ -73,32 +74,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/sync/namespaces/{namespace}/me"
+    _path: str = "/friends/sync/namespaces/{namespace}/me"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: List[ModelNativeFriendRequest]  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_accept_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_accept_friend_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/request/accept"
+    _path: str = "/friends/namespaces/{namespace}/me/request/accept"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUserAcceptFriendRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_cancel_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_cancel_friend_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/request/cancel"
+    _path: str = "/friends/namespaces/{namespace}/me/request/cancel"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUserCancelFriendRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_get_friendship_status.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_get_friendship_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/status/{friendId}"
+    _path: str = "/friends/namespaces/{namespace}/me/status/{friendId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     friend_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_reject_friend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_reject_friend_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/request/reject"
+    _path: str = "/friends/namespaces/{namespace}/me/request/reject"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUserRejectFriendRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_request_friend.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_request_friend.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/request"
+    _path: str = "/friends/namespaces/{namespace}/me/request"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUserRequestFriendRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/friends/user_unfriend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/friends/user_unfriend_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/friends/namespaces/{namespace}/me/unfriend"
+    _path: str = "/friends/namespaces/{namespace}/me/unfriend"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUserUnfriendRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_join_party_v1 import AdminJoinPartyV1
 from .admin_update_party_attr_920eb3 import AdminUpdatePartyAttributesV1
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_join_party_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_join_party_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,33 +73,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}/join/{userId}"
     )
+    _path: str = (
+        "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}/join/{userId}"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_update_party_attr_920eb3.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/admin_update_party_attr_920eb3.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,33 +75,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}/attributes"
     )
+    _path: str = (
+        "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}/attributes"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsPartyPUTCustomAttributesRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/lobby_operations/public_get_messages.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/admin_delete_global_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,60 +25,73 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import LogAppMessageDeclaration
 from ...models import RestapiErrorResponseBody
 
 
-class PublicGetMessages(Operation):
-    """get service messages (publicGetMessages)
+class AdminDeleteGlobalConfig(Operation):
+    """Delete of global configuration data. (adminDeleteGlobalConfig)
 
-    get the list of messages.
+    Delete of global configuration data.
 
     Properties:
-        url: /lobby/v1/messages
+        url: /lobby/v1/admin/global-configurations
 
-        method: GET
+        method: DELETE
 
-        tags: ["Lobby Operations"]
+        tags: ["admin", "global-configurations"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
     Responses:
-        200: OK - List[LogAppMessageDeclaration] (OK)
+        204: No Content - str (No Content)
 
-        500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
+        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
+
+        403: Forbidden - RestapiErrorResponseBody (Forbidden)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/messages"
-    _method: str = "GET"
+    _url: str = "/lobby/v1/admin/global-configurations"
+    _path: str = "/lobby/v1/admin/global-configurations"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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
 
@@ -124,61 +137,62 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, List[LogAppMessageDeclaration]],
-        Union[None, HttpResponse, RestapiErrorResponseBody],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
         """Parse the given response.
 
-        200: OK - List[LogAppMessageDeclaration] (OK)
+        204: No Content - str (No Content)
 
-        500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
+        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
+
+        403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
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
 
-        if code == 200:
-            return [LogAppMessageDeclaration.create_from_dict(i) for i in content], None
-        if code == 500:
+        if code == 204:
+            return None, None
+        if code == 401:
+            return None, RestapiErrorResponseBody.create_from_dict(content)
+        if code == 403:
             return None, RestapiErrorResponseBody.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, **kwargs) -> PublicGetMessages:
+    def create(cls, **kwargs) -> AdminDeleteGlobalConfig:
         instance = cls()
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicGetMessages:
+    ) -> AdminDeleteGlobalConfig:
         instance = cls()
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {}
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_notification_tem_590da9 import CreateNotificationTemplateV1Admin
 from .create_notification_top_701ddd import CreateNotificationTopicV1Admin
@@ -20,14 +20,15 @@
 from .delete_notification_tem_8c8a06 import DeleteNotificationTemplateSlugV1Admin
 from .delete_notification_top_00eb0a import DeleteNotificationTopicV1Admin
 from .delete_template_localiz_55eb81 import DeleteTemplateLocalizationV1Admin
 from .delete_topic_by_topic_name import DeleteTopicByTopicName
 from .free_form_notification__54ba50 import FreeFormNotificationByUserID
 from .get_all_notification_te_0053f8 import GetAllNotificationTemplatesV1Admin
 from .get_all_notification_to_761be1 import GetAllNotificationTopicsV1Admin
+from .get_my_notifications import GetMyNotifications
 from .get_notification_topic__b8a441 import GetNotificationTopicV1Admin
 from .get_single_template_loc_d01d4b import GetSingleTemplateLocalizationV1Admin
 from .get_template_slug_local_385ba4 import GetTemplateSlugLocalizationsTemplateV1Admin
 from .get_topic_by_namespace import GetTopicByNamespace
 from .get_topic_by_topic_name import GetTopicByTopicName
 from .notification_with_templ_f80964 import NotificationWithTemplateByUserID
 from .publish_template_locali_b4f377 import PublishTemplateLocalizationV1Admin
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_tem_590da9.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_tem_590da9.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         409: Conflict - RestapiErrorResponseV1 (Conflict)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelCreateTemplateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_top_701ddd.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_notification_top_701ddd.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         403: Forbidden - RestapiErrorResponseV1 (Forbidden)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelCreateTopicRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/create_topic.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/create_topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         409: Conflict - RestapiErrorResponseBody (Conflict)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/topics"
+    _path: str = "/notification/namespaces/{namespace}/topics"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelCreateTopicRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_tem_8c8a06.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_tem_8c8a06.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,32 +69,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}"
     )
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}"
+    )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_top_00eb0a.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_top_00eb0a.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,32 +70,46 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     topic_name: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_template_localiz_55eb81.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/publish_template_locali_b4f377.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import RestapiErrorResponseV1
 
 
-class DeleteTemplateLocalizationV1Admin(Operation):
-    """delete template localization (deleteTemplateLocalizationV1Admin)
+class PublishTemplateLocalizationV1Admin(Operation):
+    """publish template localization draft (publishTemplateLocalizationV1Admin)
 
-    Delete template localization
+    Publish notification template draft. Empty draft can not be published.
 
-    Action Code: 50209
+    Action Code: 50210
 
     Properties:
-        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
+        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish
 
-        method: DELETE
+        method: POST
 
         tags: ["notification"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -68,34 +68,46 @@
         404: Not Found - RestapiErrorResponseV1 (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
-    _method: str = "DELETE"
+    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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
 
@@ -138,23 +150,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> DeleteTemplateLocalizationV1Admin:
+    def with_namespace(self, value: str) -> PublishTemplateLocalizationV1Admin:
         self.namespace = value
         return self
 
-    def with_template_language(self, value: str) -> DeleteTemplateLocalizationV1Admin:
+    def with_template_language(self, value: str) -> PublishTemplateLocalizationV1Admin:
         self.template_language = value
         return self
 
-    def with_template_slug(self, value: str) -> DeleteTemplateLocalizationV1Admin:
+    def with_template_slug(self, value: str) -> PublishTemplateLocalizationV1Admin:
         self.template_slug = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -225,27 +237,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, template_language: str, template_slug: str, **kwargs
-    ) -> DeleteTemplateLocalizationV1Admin:
+    ) -> PublishTemplateLocalizationV1Admin:
         instance = cls()
         instance.namespace = namespace
         instance.template_language = template_language
         instance.template_slug = template_slug
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> DeleteTemplateLocalizationV1Admin:
+    ) -> PublishTemplateLocalizationV1Admin:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "templateLanguage" in dict_ and dict_["templateLanguage"] is not None:
             instance.template_language = str(dict_["templateLanguage"])
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_topic_by_topic_name.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_topic_by_topic_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _path: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     topic: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/free_form_notification__54ba50.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/free_form_notification__54ba50.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,33 +68,45 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/users/{userId}/freeform"
+    _path: str = "/notification/namespaces/{namespace}/users/{userId}/freeform"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelFreeFormNotificationRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_te_0053f8.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_te_0053f8.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,31 +68,43 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_to_761be1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_to_761be1.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,34 +72,46 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     after: str  # OPTIONAL in [query]
     before: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_notification_topic__b8a441.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_notification_topic__b8a441.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,46 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     topic_name: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_single_template_loc_d01d4b.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/delete_template_localiz_55eb81.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,28 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelLocalization
 from ...models import RestapiErrorResponseV1
 
 
-class GetSingleTemplateLocalizationV1Admin(Operation):
-    """get a template localization (getSingleTemplateLocalizationV1Admin)
+class DeleteTemplateLocalizationV1Admin(Operation):
+    """delete template localization (deleteTemplateLocalizationV1Admin)
 
-    Get a template localization
+    Delete template localization
 
-    Action Code: 50207
+    Action Code: 50209
 
     Properties:
         url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
 
-        method: GET
+        method: DELETE
 
         tags: ["notification"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -56,47 +55,59 @@
         namespace: (namespace) REQUIRED str in path
 
         template_language: (templateLanguage) REQUIRED str in path
 
         template_slug: (templateSlug) REQUIRED str in path
 
     Responses:
-        200: OK - ModelLocalization (OK)
+        204: No Content - (No Content)
 
         401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
-    _method: str = "GET"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
+    _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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
 
@@ -139,25 +150,23 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> GetSingleTemplateLocalizationV1Admin:
+    def with_namespace(self, value: str) -> DeleteTemplateLocalizationV1Admin:
         self.namespace = value
         return self
 
-    def with_template_language(
-        self, value: str
-    ) -> GetSingleTemplateLocalizationV1Admin:
+    def with_template_language(self, value: str) -> DeleteTemplateLocalizationV1Admin:
         self.template_language = value
         return self
 
-    def with_template_slug(self, value: str) -> GetSingleTemplateLocalizationV1Admin:
+    def with_template_slug(self, value: str) -> DeleteTemplateLocalizationV1Admin:
         self.template_slug = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -180,21 +189,18 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelLocalization],
-        Union[None, HttpResponse, RestapiErrorResponseV1],
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseV1]]:
         """Parse the given response.
 
-        200: OK - ModelLocalization (OK)
+        204: No Content - (No Content)
 
         401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
 
@@ -209,16 +215,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return ModelLocalization.create_from_dict(content), None
+        if code == 204:
+            return None, None
         if code == 401:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 403:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 404:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 500:
@@ -231,27 +237,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, template_language: str, template_slug: str, **kwargs
-    ) -> GetSingleTemplateLocalizationV1Admin:
+    ) -> DeleteTemplateLocalizationV1Admin:
         instance = cls()
         instance.namespace = namespace
         instance.template_language = template_language
         instance.template_slug = template_slug
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> GetSingleTemplateLocalizationV1Admin:
+    ) -> DeleteTemplateLocalizationV1Admin:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "templateLanguage" in dict_ and dict_["templateLanguage"] is not None:
             instance.template_language = str(dict_["templateLanguage"])
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_template_slug_local_385ba4.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_template_slug_local_385ba4.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}"
     )
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
     after: str  # OPTIONAL in [query]
     before: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
 
     # endregion fields
@@ -97,14 +103,22 @@
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_namespace.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,34 +70,46 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/topics"
+    _path: str = "/notification/namespaces/{namespace}/topics"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     after: str  # OPTIONAL in [query]
     before: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_topic_name.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_topic_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,32 +66,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _path: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     topic: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/notification_with_templ_f80964.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/notification_with_templ_f80964.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,33 +73,45 @@
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/users/{userId}/templated"
+    _path: str = "/notification/namespaces/{namespace}/users/{userId}/templated"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelNotificationWithTemplateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/publish_template_locali_b4f377.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/get_single_template_loc_d01d4b.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,28 +25,29 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
+from ...models import ModelLocalization
 from ...models import RestapiErrorResponseV1
 
 
-class PublishTemplateLocalizationV1Admin(Operation):
-    """publish template localization draft (publishTemplateLocalizationV1Admin)
+class GetSingleTemplateLocalizationV1Admin(Operation):
+    """get a template localization (getSingleTemplateLocalizationV1Admin)
 
-    Publish notification template draft. Empty draft can not be published.
+    Get a template localization
 
-    Action Code: 50210
+    Action Code: 50207
 
     Properties:
-        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish
+        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
 
-        method: POST
+        method: GET
 
         tags: ["notification"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
@@ -55,47 +56,59 @@
         namespace: (namespace) REQUIRED str in path
 
         template_language: (templateLanguage) REQUIRED str in path
 
         template_slug: (templateSlug) REQUIRED str in path
 
     Responses:
-        204: No Content - (No Content)
+        200: OK - ModelLocalization (OK)
 
         401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}/publish"
-    _method: str = "POST"
+    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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
 
@@ -138,23 +151,25 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublishTemplateLocalizationV1Admin:
+    def with_namespace(self, value: str) -> GetSingleTemplateLocalizationV1Admin:
         self.namespace = value
         return self
 
-    def with_template_language(self, value: str) -> PublishTemplateLocalizationV1Admin:
+    def with_template_language(
+        self, value: str
+    ) -> GetSingleTemplateLocalizationV1Admin:
         self.template_language = value
         return self
 
-    def with_template_slug(self, value: str) -> PublishTemplateLocalizationV1Admin:
+    def with_template_slug(self, value: str) -> GetSingleTemplateLocalizationV1Admin:
         self.template_slug = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -177,18 +192,21 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseV1]]:
+    ) -> Tuple[
+        Union[None, ModelLocalization],
+        Union[None, HttpResponse, RestapiErrorResponseV1],
+    ]:
         """Parse the given response.
 
-        204: No Content - (No Content)
+        200: OK - ModelLocalization (OK)
 
         401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseV1 (Forbidden)
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
 
@@ -203,16 +221,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return ModelLocalization.create_from_dict(content), None
         if code == 401:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 403:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 404:
             return None, RestapiErrorResponseV1.create_from_dict(content)
         if code == 500:
@@ -225,27 +243,27 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, namespace: str, template_language: str, template_slug: str, **kwargs
-    ) -> PublishTemplateLocalizationV1Admin:
+    ) -> GetSingleTemplateLocalizationV1Admin:
         instance = cls()
         instance.namespace = namespace
         instance.template_language = template_language
         instance.template_slug = template_slug
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublishTemplateLocalizationV1Admin:
+    ) -> GetSingleTemplateLocalizationV1Admin:
         instance = cls()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         if "templateLanguage" in dict_ and dict_["templateLanguage"] is not None:
             instance.template_language = str(dict_["templateLanguage"])
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_multiple_users_fre_78d5b0.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_multiple_users_fre_78d5b0.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,32 +67,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/notification/namespaces/{namespace}/bulkUsers/freeform/notify"
     )
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/bulkUsers/freeform/notify"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelBulkUsersFreeFormNotificationRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_freeform_not_1f36fa.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_freeform_not_1f36fa.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,33 +68,45 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/parties/{partyId}/freeform/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/parties/{partyId}/freeform/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelFreeFormNotificationRequestV1  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_templated_no_8a9ca4.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_party_templated_no_8a9ca4.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,33 +73,45 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/parties/{partyId}/templates/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/parties/{partyId}/templates/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelNotificationWithTemplateRequestV1  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_free_3a173d.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_free_3a173d.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,33 +69,45 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/users/{userId}/freeform/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/users/{userId}/freeform/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelFreeFormNotificationRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_temp_0499f2.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_specific_user_temp_0499f2.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,33 +75,45 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/users/{userId}/templates/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/users/{userId}/templates/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelNotificationWithTemplateRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_freeform_not_3d805f.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_freeform_not_3d805f.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/freeform/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/freeform/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelFreeFormNotificationRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_templated_no_9d39cc.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/send_users_templated_no_9d39cc.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,32 +73,44 @@
 
         404: Not Found - RestapiErrorResponseV1 (Not Found)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/notify"
+    _path: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/notify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelNotificationWithTemplateRequestV1  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_notification_top_0e4c05.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_notification_top_0e4c05.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,33 +75,47 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    _path: str = (
+        "/lobby/v1/admin/notification/namespaces/{namespace}/topics/{topicName}"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUpdateTopicRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     topic_name: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_template_localiz_cc6e6e.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/admin/update_localization_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,30 +26,28 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ModelUpdateTemplateRequest
-from ...models import RestapiErrorResponseV1
+from ...models import RestapiErrorResponseBody
 
 
-class UpdateTemplateLocalizationV1Admin(Operation):
-    """update template localization (updateTemplateLocalizationV1Admin)
+class UpdateLocalizationTemplate(Operation):
+    """update template draft (updateLocalizationTemplate)
 
-    Update template localization
-
-    Action Code: 50208
+    Modify draft template
 
     Properties:
-        url: /lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
+        url: /notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}
 
         method: PUT
 
-        tags: ["notification"]
+        tags: ["admin", "notification"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
@@ -60,48 +58,58 @@
         template_language: (templateLanguage) REQUIRED str in path
 
         template_slug: (templateSlug) REQUIRED str in path
 
     Responses:
         204: No Content - (No Content)
 
-        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
-
-        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
+        400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
-        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
+        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
-        404: Not Found - RestapiErrorResponseV1 (Not Found)
+        403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
-        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
+        404: Not Found - RestapiErrorResponseBody (Not Found)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/admin/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _url: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _path: str = "/notification/namespaces/{namespace}/templates/{templateSlug}/languages/{templateLanguage}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUpdateTemplateRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     template_language: str  # REQUIRED in [path]
     template_slug: str  # REQUIRED in [path]
 
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
 
@@ -152,27 +160,27 @@
 
     # endregion is/has methods
 
     # region with_x methods
 
     def with_body(
         self, value: ModelUpdateTemplateRequest
-    ) -> UpdateTemplateLocalizationV1Admin:
+    ) -> UpdateLocalizationTemplate:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> UpdateTemplateLocalizationV1Admin:
+    def with_namespace(self, value: str) -> UpdateLocalizationTemplate:
         self.namespace = value
         return self
 
-    def with_template_language(self, value: str) -> UpdateTemplateLocalizationV1Admin:
+    def with_template_language(self, value: str) -> UpdateLocalizationTemplate:
         self.template_language = value
         return self
 
-    def with_template_slug(self, value: str) -> UpdateTemplateLocalizationV1Admin:
+    def with_template_slug(self, value: str) -> UpdateLocalizationTemplate:
         self.template_slug = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -199,28 +207,26 @@
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
-    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseV1]]:
+    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
         """Parse the given response.
 
         204: No Content - (No Content)
 
-        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
-
-        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
+        400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
-        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
+        401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
-        404: Not Found - RestapiErrorResponseV1 (Not Found)
+        403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
-        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
+        404: Not Found - RestapiErrorResponseBody (Not Found)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -230,23 +236,21 @@
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 204:
             return None, None
         if code == 400:
-            return None, RestapiErrorResponseV1.create_from_dict(content)
+            return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 401:
-            return None, RestapiErrorResponseV1.create_from_dict(content)
+            return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 403:
-            return None, RestapiErrorResponseV1.create_from_dict(content)
+            return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 404:
-            return None, RestapiErrorResponseV1.create_from_dict(content)
-        if code == 500:
-            return None, RestapiErrorResponseV1.create_from_dict(content)
+            return None, RestapiErrorResponseBody.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
@@ -256,28 +260,28 @@
     def create(
         cls,
         body: ModelUpdateTemplateRequest,
         namespace: str,
         template_language: str,
         template_slug: str,
         **kwargs,
-    ) -> UpdateTemplateLocalizationV1Admin:
+    ) -> UpdateLocalizationTemplate:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         instance.template_language = template_language
         instance.template_slug = template_slug
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> UpdateTemplateLocalizationV1Admin:
+    ) -> UpdateLocalizationTemplate:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
             instance.body = ModelUpdateTemplateRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
             instance.body = ModelUpdateTemplateRequest()
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/notification/update_topic_by_topic_name.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/notification/update_topic_by_topic_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,33 +71,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _path: str = "/notification/namespaces/{namespace}/topics/{topic}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelUpdateTopicRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     topic: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_party_data_v1 import AdminGetPartyDataV1
 from .admin_get_user_party_v1 import AdminGetUserPartyV1
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_party_data_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_party_data_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}"
+    _path: str = "/lobby/v1/admin/party/namespaces/{namespace}/parties/{partyId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_user_party_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/admin_get_user_party_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/party/namespaces/{namespace}/users/{userId}/party"
+    _path: str = "/lobby/v1/admin/party/namespaces/{namespace}/users/{userId}/party"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_get_party_data_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_get_party_data_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,32 +73,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}"
+    _path: str = "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_set_party_limit_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_set_party_limit_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,33 +73,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}/limit"
+    _path: str = "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}/limit"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsPartyPUTLimitSizeRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/party/public_update_party_att_aeeff0.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/party/public_update_party_att_aeeff0.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,33 +78,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}/attributes"
     )
+    _path: str = (
+        "/lobby/v1/public/party/namespaces/{namespace}/parties/{partyId}/attributes"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsPartyPUTCustomAttributesRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     party_id: str  # REQUIRED in [path]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_bulk_block_players_v1 import AdminBulkBlockPlayersV1
 from .admin_get_all_player_se_b925d7 import AdminGetAllPlayerSessionAttribute
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_bulk_block_players_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_bulk_block_players_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,33 +70,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/bulk/block"
     )
+    _path: str = (
+        "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/bulk/block"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsListBlockedPlayerRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_all_player_se_b925d7.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_all_player_se_b925d7.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,32 +66,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes"
     )
+    _path: str = (
+        "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_bulk_player_b_0addc5.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_bulk_player_b_0addc5.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/bulk/blocked"
+    _path: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/bulk/blocked"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsGetBulkAllPlayerBlockedUsersRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_lobby_ccu.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_lobby_ccu.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,31 +66,43 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/player/namespaces/{namespace}/ccu"
+    _path: str = "/lobby/v1/admin/player/namespaces/{namespace}/ccu"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_7da3f3.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_7da3f3.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/blocked"
+    _path: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/blocked"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_8955db.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_blocke_8955db.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,32 +70,46 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/blocked-by"
     )
+    _path: str = (
+        "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/blocked-by"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_sessio_625ce8.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_get_player_sessio_625ce8.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes/{attribute}"
+    _path: str = "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes/{attribute}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     attribute: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/admin_set_player_sessio_1bc722.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/admin_set_player_sessio_1bc722.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,33 +72,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes"
     )
+    _path: str = (
+        "/lobby/v1/admin/player/namespaces/{namespace}/users/{userId}/attributes"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsSetPlayerSessionAttributeRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_0dc6b7.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_0dc6b7.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,31 +71,43 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/blocked-by"
+    _path: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/blocked-by"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_55d58a.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_player_block_players_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,77 +25,90 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsGetAllPlayerBlockedUsersResponse
+from ...models import ModelsBlockPlayerRequest
 from ...models import RestapiErrorResponseBody
 
 
-class PublicGetPlayerBlockedPlayersV1(Operation):
-    """get blocked players by user id (publicGetPlayerBlockedPlayersV1)
+class PublicPlayerBlockPlayersV1(Operation):
+    """block player by user id (publicPlayerBlockPlayersV1)
 
     Required valid user authorization
 
 
-    load blocked players in a namespace based on user id
-
-    Action Code: 50101
+    add blocked players in a namespace based on user id
 
     Properties:
-        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/blocked
+        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/block
 
-        method: GET
+        method: POST
 
         tags: ["player"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelsBlockPlayerRequest in body
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelsGetAllPlayerBlockedUsersResponse (OK)
+        201: Created - (Created)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/blocked"
-    _method: str = "GET"
+    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/block"
+    _path: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/block"
+    _base_path: str = ""
+    _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
+    body: ModelsBlockPlayerRequest  # REQUIRED in [body]
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
 
@@ -117,61 +130,74 @@
 
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
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_namespace(self, value: str) -> PublicGetPlayerBlockedPlayersV1:
+    def with_body(self, value: ModelsBlockPlayerRequest) -> PublicPlayerBlockPlayersV1:
+        self.body = value
+        return self
+
+    def with_namespace(self, value: str) -> PublicPlayerBlockPlayersV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["body"] = ModelsBlockPlayerRequest()
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
-        Union[None, ModelsGetAllPlayerBlockedUsersResponse],
-        Union[None, HttpResponse, RestapiErrorResponseBody],
+        Union[None, Optional[str]], Union[None, HttpResponse, RestapiErrorResponseBody]
     ]:
         """Parse the given response.
 
-        200: OK - ModelsGetAllPlayerBlockedUsersResponse (OK)
+        201: Created - (Created)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
@@ -188,19 +214,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 200:
-            return (
-                ModelsGetAllPlayerBlockedUsersResponse.create_from_dict(content),
-                None,
-            )
+        if code == 201:
+            return HttpResponse.create(code, "Created"), None
         if code == 400:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 401:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 403:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 404:
@@ -213,38 +236,49 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(cls, namespace: str, **kwargs) -> PublicGetPlayerBlockedPlayersV1:
+    def create(
+        cls, body: ModelsBlockPlayerRequest, namespace: str, **kwargs
+    ) -> PublicPlayerBlockPlayersV1:
         instance = cls()
+        instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicGetPlayerBlockedPlayersV1:
+    ) -> PublicPlayerBlockPlayersV1:
         instance = cls()
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelsBlockPlayerRequest.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.body = ModelsBlockPlayerRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "body": "body",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "body": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_player_block_players_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_unblock_player_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,78 +25,89 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsBlockPlayerRequest
+from ...models import ModelsUnblockPlayerRequest
 from ...models import RestapiErrorResponseBody
 
 
-class PublicPlayerBlockPlayersV1(Operation):
-    """block player by user id (publicPlayerBlockPlayersV1)
+class PublicUnblockPlayerV1(Operation):
+    """unblock player by user id (publicUnblockPlayerV1)
 
     Required valid user authorization
 
-
-    add blocked players in a namespace based on user id
+    unblock player in a namespace based on user id
 
     Properties:
-        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/block
+        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/unblock
 
         method: POST
 
         tags: ["player"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsBlockPlayerRequest in body
+        body: (body) REQUIRED ModelsUnblockPlayerRequest in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        201: Created - (Created)
+        204: No Content - (No Content)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/block"
+    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/unblock"
+    _path: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/unblock"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsBlockPlayerRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "lobby"
+
+    body: ModelsUnblockPlayerRequest  # REQUIRED in [body]
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
 
@@ -141,51 +152,49 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsBlockPlayerRequest) -> PublicPlayerBlockPlayersV1:
+    def with_body(self, value: ModelsUnblockPlayerRequest) -> PublicUnblockPlayerV1:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> PublicPlayerBlockPlayersV1:
+    def with_namespace(self, value: str) -> PublicUnblockPlayerV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelsBlockPlayerRequest()
+            result["body"] = ModelsUnblockPlayerRequest()
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
-        Union[None, Optional[str]], Union[None, HttpResponse, RestapiErrorResponseBody]
-    ]:
+    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
         """Parse the given response.
 
-        201: Created - (Created)
+        204: No Content - (No Content)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
@@ -202,16 +211,16 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 201:
-            return HttpResponse.create(code, "Created"), None
+        if code == 204:
+            return None, None
         if code == 400:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 401:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 403:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 404:
@@ -225,34 +234,34 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, body: ModelsBlockPlayerRequest, namespace: str, **kwargs
-    ) -> PublicPlayerBlockPlayersV1:
+        cls, body: ModelsUnblockPlayerRequest, namespace: str, **kwargs
+    ) -> PublicUnblockPlayerV1:
         instance = cls()
         instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicPlayerBlockPlayersV1:
+    ) -> PublicUnblockPlayerV1:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsBlockPlayerRequest.create_from_dict(
+            instance.body = ModelsUnblockPlayerRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelsBlockPlayerRequest()
+            instance.body = ModelsUnblockPlayerRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/player/public_unblock_player_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/player/public_get_player_block_55d58a.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,77 +25,89 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import ModelsUnblockPlayerRequest
+from ...models import ModelsGetAllPlayerBlockedUsersResponse
 from ...models import RestapiErrorResponseBody
 
 
-class PublicUnblockPlayerV1(Operation):
-    """unblock player by user id (publicUnblockPlayerV1)
+class PublicGetPlayerBlockedPlayersV1(Operation):
+    """get blocked players by user id (publicGetPlayerBlockedPlayersV1)
 
     Required valid user authorization
 
-    unblock player in a namespace based on user id
+
+    load blocked players in a namespace based on user id
+
+    Action Code: 50101
 
     Properties:
-        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/unblock
+        url: /lobby/v1/public/player/namespaces/{namespace}/users/me/blocked
 
-        method: POST
+        method: GET
 
         tags: ["player"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelsUnblockPlayerRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (No Content)
+        200: OK - ModelsGetAllPlayerBlockedUsersResponse (OK)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
         404: Not Found - RestapiErrorResponseBody (Not Found)
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/unblock"
-    _method: str = "POST"
+    _url: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/blocked"
+    _path: str = "/lobby/v1/public/player/namespaces/{namespace}/users/me/blocked"
+    _base_path: str = ""
+    _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelsUnblockPlayerRequest  # REQUIRED in [body]
+    service_name: Optional[str] = "lobby"
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
 
@@ -117,72 +129,61 @@
 
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
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelsUnblockPlayerRequest) -> PublicUnblockPlayerV1:
-        self.body = value
-        return self
-
-    def with_namespace(self, value: str) -> PublicUnblockPlayerV1:
+    def with_namespace(self, value: str) -> PublicGetPlayerBlockedPlayersV1:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelsUnblockPlayerRequest()
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
-    ) -> Tuple[None, Union[None, HttpResponse, RestapiErrorResponseBody]]:
+    ) -> Tuple[
+        Union[None, ModelsGetAllPlayerBlockedUsersResponse],
+        Union[None, HttpResponse, RestapiErrorResponseBody],
+    ]:
         """Parse the given response.
 
-        204: No Content - (No Content)
+        200: OK - ModelsGetAllPlayerBlockedUsersResponse (OK)
 
         400: Bad Request - RestapiErrorResponseBody (Bad Request)
 
         401: Unauthorized - RestapiErrorResponseBody (Unauthorized)
 
         403: Forbidden - RestapiErrorResponseBody (Forbidden)
 
@@ -199,16 +200,19 @@
         pre_processed_response, error = self.pre_process_response(
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
-        if code == 204:
-            return None, None
+        if code == 200:
+            return (
+                ModelsGetAllPlayerBlockedUsersResponse.create_from_dict(content),
+                None,
+            )
         if code == 400:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 401:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 403:
             return None, RestapiErrorResponseBody.create_from_dict(content)
         if code == 404:
@@ -221,49 +225,38 @@
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
-    def create(
-        cls, body: ModelsUnblockPlayerRequest, namespace: str, **kwargs
-    ) -> PublicUnblockPlayerV1:
+    def create(cls, namespace: str, **kwargs) -> PublicGetPlayerBlockedPlayersV1:
         instance = cls()
-        instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicUnblockPlayerV1:
+    ) -> PublicGetPlayerBlockedPlayersV1:
         instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelsUnblockPlayerRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelsUnblockPlayerRequest()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "body": "body",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "body": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/presence/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/presence/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .users_presence_handler_v1 import UsersPresenceHandlerV1
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/presence/users_presence_handler_v1.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/presence/users_presence_handler_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,33 +66,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/public/presence/namespaces/{namespace}/users/presence"
+    _path: str = "/lobby/v1/public/presence/namespaces/{namespace}/users/presence"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     namespace: str  # REQUIRED in [path]
     count_only: bool  # OPTIONAL in [query]
     user_ids: str  # REQUIRED in [query]
 
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_add_profanity_fil_e31341 import AdminAddProfanityFilterIntoList
 from .admin_add_profanity_filters import AdminAddProfanityFilters
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_fil_e31341.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_fil_e31341.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminAddProfanityFilterIntoListRequest  # REQUIRED in [body]
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_filters.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_add_profanity_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,33 +72,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/bulk"
     )
+    _path: str = (
+        "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/bulk"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminAddProfanityFiltersRequest  # REQUIRED in [body]
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_create_profanity_list.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_create_profanity_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminCreateProfanityListRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_debug_profanity_filters.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_debug_profanity_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/filters/debug"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/filters/debug"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsDebugProfanityFilterRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_filter.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,33 +73,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/delete"
     )
+    _path: str = (
+        "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/delete"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminDeleteProfanityFilterRequest  # REQUIRED in [body]
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_list.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_delete_profanity_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists/{list}"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists/{list}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lis_fd0d45.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lis_fd0d45.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lists.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,31 +66,43 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_rule.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_get_profanity_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,31 +66,43 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/rule"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/rule"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_import_profanity__286711.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_import_profanity__286711.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,33 +71,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/bulk-file"
     )
+    _path: str = (
+        "/lobby/v1/admin/profanity/namespaces/{namespace}/list/{list}/filters/bulk-file"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: List[int]  # REQUIRED in [body]
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_set_profanity_rul_e9d9e0.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_set_profanity_rul_e9d9e0.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/rule"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/rule"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminSetProfanityRuleForNamespaceRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_update_profanity_list.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_update_profanity_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,33 +70,45 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists/{list}"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/lists/{list}"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminUpdateProfanityList  # REQUIRED in [body]
     list_: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_verify_message_pr_169572.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/profanity/admin_verify_message_pr_169572.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - RestapiErrorResponseBody (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/verify"
+    _path: str = "/lobby/v1/admin/profanity/namespaces/{namespace}/verify"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsAdminVerifyMessageProfanityRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_third_part_225a9c import AdminCreateThirdPartyConfig
 from .admin_delete_third_part_c9d441 import AdminDeleteThirdPartyConfig
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_create_third_part_225a9c.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_create_third_part_225a9c.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,32 +69,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _path: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsCreateConfigRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_delete_third_part_c9d441.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_delete_third_part_c9d441.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,31 +71,43 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _path: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_get_third_party_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_get_third_party_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,31 +64,43 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _path: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_update_third_part_9b81f7.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/operations/third_party/admin_update_third_part_9b81f7.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _path: str = "/lobby/v1/admin/thirdparty/namespaces/{namespace}/config/steam"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "lobby"
+
     body: ModelsUpdateConfigRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Lobby Server."""
 
-__version__ = "3.35.0"
+__version__ = "3.35.5"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin import admin_delete_global_config
 from ._admin import admin_delete_global_config_async
@@ -37,14 +37,17 @@
 from ._admin import notification_with_template
 from ._admin import notification_with_template_async
 from ._admin import publish_template
 from ._admin import publish_template_async
 from ._admin import update_localization_template
 from ._admin import update_localization_template_async
 
+from ._blocks import sync_native_blocked_user
+from ._blocks import sync_native_blocked_user_async
+
 from ._config import admin_export_config_v1
 from ._config import admin_export_config_v1_async
 from ._config import admin_get_all_config_v1
 from ._config import admin_get_all_config_v1_async
 from ._config import admin_get_config_v1
 from ._config import admin_get_config_v1_async
 from ._config import admin_import_config_v1
@@ -114,14 +117,16 @@
 from ._notification import delete_topic_by_topic_name_async
 from ._notification import free_form_notification_by_user_id
 from ._notification import free_form_notification_by_user_id_async
 from ._notification import get_all_notification_templates_v1_admin
 from ._notification import get_all_notification_templates_v1_admin_async
 from ._notification import get_all_notification_topics_v1_admin
 from ._notification import get_all_notification_topics_v1_admin_async
+from ._notification import get_my_notifications
+from ._notification import get_my_notifications_async
 from ._notification import get_notification_topic_v1_admin
 from ._notification import get_notification_topic_v1_admin_async
 from ._notification import get_single_template_localization_v1_admin
 from ._notification import get_single_template_localization_v1_admin_async
 from ._notification import get_template_slug_localizations_template_v1_admin
 from ._notification import get_template_slug_localizations_template_v1_admin_async
 from ._notification import get_topic_by_namespace
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_admin.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_admin.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_config.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_friends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1492,21 +1492,22 @@
     body: List[ModelNativeFriendRequest],
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """sync friends using server to server call to native first party server. (syncNativeFriends)
 
-    Sync friends using server to server call to native first party servere.
+    Sync friends using server to server call to native first party server.
     Supported platforms:
     steam: The platform_tokenâs value is the binary ticket returned by Steam.
     If this ticket was generated by Steam GetAuthTicketForWebApi with version >= 1.57, then platform token should use this style: {identity}:{ticket}
     the {identity} was the parameter to call GetAuthTicketForWebApi when the ticket was created. Note: Do not contain : in this {identity}
     ps4: The platform_tokenâs value is the authorization code returned by Sony OAuth.
     ps5: The platform_tokenâs value is the authorization code returned by Sony OAuth.
+    pspc: The platform_tokenâs value is the authorization code returned by Sony OAuth.
 
     Properties:
         url: /friends/sync/namespaces/{namespace}/me
 
         method: PATCH
 
         tags: ["friends", "public"]
@@ -1548,21 +1549,22 @@
     body: List[ModelNativeFriendRequest],
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """sync friends using server to server call to native first party server. (syncNativeFriends)
 
-    Sync friends using server to server call to native first party servere.
+    Sync friends using server to server call to native first party server.
     Supported platforms:
     steam: The platform_tokenâs value is the binary ticket returned by Steam.
     If this ticket was generated by Steam GetAuthTicketForWebApi with version >= 1.57, then platform token should use this style: {identity}:{ticket}
     the {identity} was the parameter to call GetAuthTicketForWebApi when the ticket was created. Note: Do not contain : in this {identity}
     ps4: The platform_tokenâs value is the authorization code returned by Sony OAuth.
     ps5: The platform_tokenâs value is the authorization code returned by Sony OAuth.
+    pspc: The platform_tokenâs value is the authorization code returned by Sony OAuth.
 
     Properties:
         url: /friends/sync/namespaces/{namespace}/me
 
         method: PATCH
 
         tags: ["friends", "public"]
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_lobby_operations.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_lobby_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_notification.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from ..models import ModelCreateTopicRequest
 from ..models import ModelCreateTopicRequestV1
 from ..models import ModelFreeFormNotificationRequest
 from ..models import ModelFreeFormNotificationRequestV1
 from ..models import ModelGetAllNotificationTemplateSlugResp
 from ..models import ModelGetAllNotificationTopicsResponse
 from ..models import ModelLocalization
+from ..models import ModelNotificationResponse
 from ..models import ModelNotificationTemplateResponse
 from ..models import ModelNotificationTopicResponse
 from ..models import ModelNotificationTopicResponseV1
 from ..models import ModelNotificationWithTemplateRequest
 from ..models import ModelNotificationWithTemplateRequestV1
 from ..models import ModelTopicByNamespacesResponse
 from ..models import ModelUpdateTemplateRequest
@@ -55,14 +56,15 @@
 from ..operations.notification import DeleteNotificationTemplateSlugV1Admin
 from ..operations.notification import DeleteNotificationTopicV1Admin
 from ..operations.notification import DeleteTemplateLocalizationV1Admin
 from ..operations.notification import DeleteTopicByTopicName
 from ..operations.notification import FreeFormNotificationByUserID
 from ..operations.notification import GetAllNotificationTemplatesV1Admin
 from ..operations.notification import GetAllNotificationTopicsV1Admin
+from ..operations.notification import GetMyNotifications
 from ..operations.notification import GetNotificationTopicV1Admin
 from ..operations.notification import GetSingleTemplateLocalizationV1Admin
 from ..operations.notification import GetTemplateSlugLocalizationsTemplateV1Admin
 from ..operations.notification import GetTopicByNamespace
 from ..operations.notification import GetTopicByTopicName
 from ..operations.notification import NotificationWithTemplateByUserID
 from ..operations.notification import PublishTemplateLocalizationV1Admin
@@ -1182,14 +1184,148 @@
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
+@same_doc_as(GetMyNotifications)
+def get_my_notifications(
+    end_time: Optional[int] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    start_time: Optional[int] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get list of notifications (getMyNotifications)
+
+    Get list of notifications in a namespace.
+    The query parameters **startTime** and **endTime** can be filled with the **sequenceID** value in the notification, where the value is an epoch timestamp.
+    Example **sequenceID** or epoch timestamp value: **1706595813**
+
+    Properties:
+        url: /notification/namespaces/{namespace}/me
+
+        method: GET
+
+        tags: ["notification", "public"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        end_time: (endTime) OPTIONAL int in query
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        start_time: (startTime) OPTIONAL int in query
+
+    Responses:
+        200: OK - ModelNotificationResponse (OK)
+
+        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
+
+        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
+
+        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
+
+        404: Not Found - RestapiErrorResponseV1 (Not Found)
+
+        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetMyNotifications.create(
+        end_time=end_time,
+        limit=limit,
+        offset=offset,
+        start_time=start_time,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(GetMyNotifications)
+async def get_my_notifications_async(
+    end_time: Optional[int] = None,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    start_time: Optional[int] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Get list of notifications (getMyNotifications)
+
+    Get list of notifications in a namespace.
+    The query parameters **startTime** and **endTime** can be filled with the **sequenceID** value in the notification, where the value is an epoch timestamp.
+    Example **sequenceID** or epoch timestamp value: **1706595813**
+
+    Properties:
+        url: /notification/namespaces/{namespace}/me
+
+        method: GET
+
+        tags: ["notification", "public"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        end_time: (endTime) OPTIONAL int in query
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        start_time: (startTime) OPTIONAL int in query
+
+    Responses:
+        200: OK - ModelNotificationResponse (OK)
+
+        400: Bad Request - RestapiErrorResponseV1 (Bad Request)
+
+        401: Unauthorized - RestapiErrorResponseV1 (Unauthorized)
+
+        403: Forbidden - RestapiErrorResponseV1 (Forbidden)
+
+        404: Not Found - RestapiErrorResponseV1 (Not Found)
+
+        500: Internal Server Error - RestapiErrorResponseV1 (Internal Server Error)
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetMyNotifications.create(
+        end_time=end_time,
+        limit=limit,
+        offset=offset,
+        start_time=start_time,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
 @same_doc_as(GetNotificationTopicV1Admin)
 def get_notification_topic_v1_admin(
     topic_name: str,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_party.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_player.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_player.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_presence.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_presence.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_profanity.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_profanity.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wrappers/_third_party.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wrappers/_third_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/__init__.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/accept_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/block_player_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/cancel_matchmaking_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/channel_chat_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/channel_chat_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/client_reset_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/client_reset_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/connect_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/connect_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/disconnect_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/disconnect_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/ds_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/ds_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/error_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/error_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/exit_all_channel.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/exit_all_channel.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/friends_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_all_session_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_friendship_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/get_session_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/heartbeat.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/heartbeat.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/join_default_channel_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_incoming_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_of_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_online_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_online_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/list_outgoing_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/matchmaking_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/matchmaking_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/message_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/message_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/message_session_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/message_session_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/offline_notification_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/online_friends.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/online_friends.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_chat_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_data_update_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_data_update_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_get_invited_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_get_invited_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_info_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_invite_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_join_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_kick_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_leave_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_promote_leader_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/party_reject_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_history_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/personal_chat_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/refresh_token_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/reject_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/rematchmaking_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/rematchmaking_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/request_friends_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/send_channel_chat_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_ready_consent_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_session_attribute_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/set_user_status_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/shutdown_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/shutdown_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/signaling_p2p_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/signaling_p2p_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/start_matchmaking_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unblock_player_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/unfriend_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_banned_notification.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_banned_notification.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_request.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_response.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_metric_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk/api/lobby/wss_models/user_status_notif.py` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk/api/lobby/wss_models/user_status_notif.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-lobby
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Lobby Server
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Lobby Server
-* Version: 3.35.0
+* Version: 3.35.5
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-lobby-0.8.0/accelbyte_py_sdk_service_lobby.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_lobby-0.9.0/accelbyte_py_sdk_service_lobby.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 accelbyte_py_sdk/api/lobby/models/model_incoming_friends_with_time_data.py
 accelbyte_py_sdk/api/lobby/models/model_list_bulk_user_platforms_response.py
 accelbyte_py_sdk/api/lobby/models/model_load_incoming_friends_with_time_response.py
 accelbyte_py_sdk/api/lobby/models/model_load_outgoing_friends_with_time_response.py
 accelbyte_py_sdk/api/lobby/models/model_localization.py
 accelbyte_py_sdk/api/lobby/models/model_native_friend_request.py
 accelbyte_py_sdk/api/lobby/models/model_native_friend_sync_response.py
+accelbyte_py_sdk/api/lobby/models/model_native_user_block_request.py
+accelbyte_py_sdk/api/lobby/models/model_native_user_block_response.py
+accelbyte_py_sdk/api/lobby/models/model_notification_response.py
 accelbyte_py_sdk/api/lobby/models/model_notification_template_response.py
 accelbyte_py_sdk/api/lobby/models/model_notification_topic_response.py
 accelbyte_py_sdk/api/lobby/models/model_notification_topic_response_v1.py
 accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request.py
 accelbyte_py_sdk/api/lobby/models/model_notification_with_template_request_v1.py
 accelbyte_py_sdk/api/lobby/models/model_outgoing_friends_with_time_data.py
 accelbyte_py_sdk/api/lobby/models/model_pagination.py
@@ -106,14 +109,16 @@
 accelbyte_py_sdk/api/lobby/operations/admin/free_form_notification.py
 accelbyte_py_sdk/api/lobby/operations/admin/get_game_template.py
 accelbyte_py_sdk/api/lobby/operations/admin/get_localization_template.py
 accelbyte_py_sdk/api/lobby/operations/admin/get_slug_template.py
 accelbyte_py_sdk/api/lobby/operations/admin/notification_with_template.py
 accelbyte_py_sdk/api/lobby/operations/admin/publish_template.py
 accelbyte_py_sdk/api/lobby/operations/admin/update_localization_template.py
+accelbyte_py_sdk/api/lobby/operations/blocks/__init__.py
+accelbyte_py_sdk/api/lobby/operations/blocks/sync_native_blocked_user.py
 accelbyte_py_sdk/api/lobby/operations/config/__init__.py
 accelbyte_py_sdk/api/lobby/operations/config/admin_export_config_v1.py
 accelbyte_py_sdk/api/lobby/operations/config/admin_get_all_config_v1.py
 accelbyte_py_sdk/api/lobby/operations/config/admin_get_config_v1.py
 accelbyte_py_sdk/api/lobby/operations/config/admin_import_config_v1.py
 accelbyte_py_sdk/api/lobby/operations/config/admin_update_config_v1.py
 accelbyte_py_sdk/api/lobby/operations/friends/__init__.py
@@ -147,14 +152,15 @@
 accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_tem_8c8a06.py
 accelbyte_py_sdk/api/lobby/operations/notification/delete_notification_top_00eb0a.py
 accelbyte_py_sdk/api/lobby/operations/notification/delete_template_localiz_55eb81.py
 accelbyte_py_sdk/api/lobby/operations/notification/delete_topic_by_topic_name.py
 accelbyte_py_sdk/api/lobby/operations/notification/free_form_notification__54ba50.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_te_0053f8.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_all_notification_to_761be1.py
+accelbyte_py_sdk/api/lobby/operations/notification/get_my_notifications.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_notification_topic__b8a441.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_single_template_loc_d01d4b.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_template_slug_local_385ba4.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_namespace.py
 accelbyte_py_sdk/api/lobby/operations/notification/get_topic_by_topic_name.py
 accelbyte_py_sdk/api/lobby/operations/notification/notification_with_templ_f80964.py
 accelbyte_py_sdk/api/lobby/operations/notification/publish_template_locali_b4f377.py
@@ -206,14 +212,15 @@
 accelbyte_py_sdk/api/lobby/operations/third_party/__init__.py
 accelbyte_py_sdk/api/lobby/operations/third_party/admin_create_third_part_225a9c.py
 accelbyte_py_sdk/api/lobby/operations/third_party/admin_delete_third_part_c9d441.py
 accelbyte_py_sdk/api/lobby/operations/third_party/admin_get_third_party_config.py
 accelbyte_py_sdk/api/lobby/operations/third_party/admin_update_third_part_9b81f7.py
 accelbyte_py_sdk/api/lobby/wrappers/__init__.py
 accelbyte_py_sdk/api/lobby/wrappers/_admin.py
+accelbyte_py_sdk/api/lobby/wrappers/_blocks.py
 accelbyte_py_sdk/api/lobby/wrappers/_config.py
 accelbyte_py_sdk/api/lobby/wrappers/_friends.py
 accelbyte_py_sdk/api/lobby/wrappers/_lobby_operations.py
 accelbyte_py_sdk/api/lobby/wrappers/_notification.py
 accelbyte_py_sdk/api/lobby/wrappers/_party.py
 accelbyte_py_sdk/api/lobby/wrappers/_player.py
 accelbyte_py_sdk/api/lobby/wrappers/_presence.py
```

