# Comparing `tmp/accelbyte-py-sdk-service-match2-0.8.0.tar.gz` & `tmp/accelbyte_py_sdk_service_match2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-match2-0.8.0.tar", last modified: Tue Mar 26 05:43:30 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_match2-0.9.0.tar", last modified: Tue May  7 06:29:03 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-match2-0.8.0.tar` & `accelbyte_py_sdk_service_match2-0.9.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.581615 accelbyte-py-sdk-service-match2-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-26 05:43:30.581615 accelbyte-py-sdk-service-match2-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      873 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.569616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.569616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.573616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/
--rw-rw-r--   0 root         (0) root         (0)     3610 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/
--rw-rw-r--   0 root         (0) root         (0)     3190 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4464 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_accept_request.py
--rw-rw-r--   0 root         (0) root         (0)     4558 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_create_request.py
--rw-rw-r--   0 root         (0) root         (0)     4464 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_reject_request.py
--rw-rw-r--   0 root         (0) root         (0)     3732 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_create_response.py
--rw-rw-r--   0 root         (0) root         (0)     7284 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_get_response.py
--rw-rw-r--   0 root         (0) root         (0)     9352 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_proposal_response.py
--rw-rw-r--   0 root         (0) root         (0)     4332 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_environment_variables_response.py
--rw-rw-r--   0 root         (0) root         (0)     6038 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_functions_response.py
--rw-rw-r--   0 root         (0) root         (0)     6051 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_pool_tickets_response.py
--rw-rw-r--   0 root         (0) root         (0)     5163 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_pools_response.py
--rw-rw-r--   0 root         (0) root         (0)     5271 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_rule_sets_response.py
--rw-rw-r--   0 root         (0) root         (0)     9078 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match.py
--rw-rw-r--   0 root         (0) root         (0)     5376 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_config.py
--rw-rw-r--   0 root         (0) root         (0)     7304 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_override.py
--rw-rw-r--   0 root         (0) root         (0)     5389 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_request.py
--rw-rw-r--   0 root         (0) root         (0)    13957 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_pool.py
--rw-rw-r--   0 root         (0) root         (0)    13555 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_pool_config.py
--rw-rw-r--   0 root         (0) root         (0)     3741 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_rule_set_name_data.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_request.py
--rw-rw-r--   0 root         (0) root         (0)     4623 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_response.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_status.py
--rw-rw-r--   0 root         (0) root         (0)     5132 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_statuses.py
--rw-rw-r--   0 root         (0) root         (0)     4262 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_namespace_config_list.py
--rw-rw-r--   0 root         (0) root         (0)     4440 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_party.py
--rw-rw-r--   0 root         (0) root         (0)     4360 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_patch_namespace_config_request.py
--rw-rw-r--   0 root         (0) root         (0)     5348 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_player_data.py
--rw-rw-r--   0 root         (0) root         (0)     3919 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_player_metric_record.py
--rw-rw-r--   0 root         (0) root         (0)     5325 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_proposed_proposal.py
--rw-rw-r--   0 root         (0) root         (0)     5521 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_rule_set_payload.py
--rw-rw-r--   0 root         (0) root         (0)     4689 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_team.py
--rw-rw-r--   0 root         (0) root         (0)     9670 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     3894 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_ticket_metric_result_record.py
--rw-rw-r--   0 root         (0) root         (0)     6166 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/config_environment_variable.py
--rw-rw-r--   0 root         (0) root         (0)     5022 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/configmodels_namespace_config.py
--rw-rw-r--   0 root         (0) root         (0)     9692 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_match_ticket_record.py
--rw-rw-r--   0 root         (0) root         (0)     4538 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_party.py
--rw-rw-r--   0 root         (0) root         (0)     5231 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_proposed_proposal.py
--rw-rw-r--   0 root         (0) root         (0)     4836 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_team.py
--rw-rw-r--   0 root         (0) root         (0)    10585 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_ticket.py
--rw-rw-r--   0 root         (0) root         (0)    10304 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     6890 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_ds_information.py
--rw-rw-r--   0 root         (0) root         (0)    15253 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_game_session.py
--rw-rw-r--   0 root         (0) root         (0)     5437 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)    14798 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_server.py
--rw-rw-r--   0 root         (0) root         (0)     6311 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_user.py
--rw-rw-r--   0 root         (0) root         (0)     5920 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/player_player_data.py
--rw-rw-r--   0 root         (0) root         (0)     4436 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/
--rw-rw-r--   0 root         (0) root         (0)      739 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8500 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/accept_backfill.py
--rw-rw-r--   0 root         (0) root         (0)     7850 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/create_backfill.py
--rw-rw-r--   0 root         (0) root         (0)     7010 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/delete_backfill.py
--rw-rw-r--   0 root         (0) root         (0)     7326 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill.py
--rw-rw-r--   0 root         (0) root         (0)     7517 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill_proposal.py
--rw-rw-r--   0 root         (0) root         (0)     8392 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/reject_backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/
--rw-rw-r--   0 root         (0) root         (0)      631 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5229 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_all_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     6171 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_config_v1.py
--rw-rw-r--   0 root         (0) root         (0)     7458 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_patch_config_v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/environment_variables/
--rw-rw-r--   0 root         (0) root         (0)      533 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/environment_variables/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5055 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/environment_variables/environment_variable_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/
--rw-rw-r--   0 root         (0) root         (0)      686 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7569 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/create_match_function.py
--rw-rw-r--   0 root         (0) root         (0)     6922 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/delete_match_function.py
--rw-rw-r--   0 root         (0) root         (0)     7904 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/match_function_list.py
--rw-rw-r--   0 root         (0) root         (0)     8358 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/update_match_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/
--rw-rw-r--   0 root         (0) root         (0)      864 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8953 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/admin_get_match_pool_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     8480 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/create_match_pool.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/delete_match_pool.py
--rw-rw-r--   0 root         (0) root         (0)     7076 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/get_player_metric.py
--rw-rw-r--   0 root         (0) root         (0)     6787 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_details.py
--rw-rw-r--   0 root         (0) root         (0)     8529 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_list.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_metric.py
--rw-rw-r--   0 root         (0) root         (0)     9068 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/update_match_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/
--rw-rw-r--   0 root         (0) root         (0)      677 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9990 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/create_match_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     6995 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/delete_match_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     8702 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/get_my_match_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     7161 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/match_ticket_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/
--rw-rw-r--   0 root         (0) root         (0)      636 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4179 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info_v1.py
--rw-rw-r--   0 root         (0) root         (0)     4198 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/version_check_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.577616 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/
--rw-rw-r--   0 root         (0) root         (0)      683 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7782 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/create_rule_set.py
--rw-rw-r--   0 root         (0) root         (0)     6916 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/delete_rule_set.py
--rw-rw-r--   0 root         (0) root         (0)     6880 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_details.py
--rw-rw-r--   0 root         (0) root         (0)     8490 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_list.py
--rw-rw-r--   0 root         (0) root         (0)     8361 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/update_rule_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.581615 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     3741 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18219 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_backfill.py
--rw-rw-r--   0 root         (0) root         (0)     8291 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_config.py
--rw-rw-r--   0 root         (0) root         (0)     2934 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_environment_variables.py
--rw-rw-r--   0 root         (0) root         (0)    12370 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_functions.py
--rw-rw-r--   0 root         (0) root         (0)    27314 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_pools.py
--rw-rw-r--   0 root         (0) root         (0)    16676 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     4519 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_operations.py
--rw-rw-r--   0 root         (0) root         (0)    15486 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_rule_sets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:43:30.581615 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-26 05:43:30.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6809 2024-03-26 05:43:30.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:43:30.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:43:30.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:43:30.000000 accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      359 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-match2-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:43:30.581615 accelbyte-py-sdk-service-match2-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.735961 accelbyte_py_sdk_service_match2-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-07 06:29:03.735961 accelbyte_py_sdk_service_match2-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      873 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.723961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.723961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.723961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/
+-rw-rw-r--   0 root         (0) root         (0)     3610 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.727961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/
+-rw-rw-r--   0 root         (0) root         (0)     3190 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4464 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_accept_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4558 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_create_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4464 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_reject_request.py
+-rw-rw-r--   0 root         (0) root         (0)     3732 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_create_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7284 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_get_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9352 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_proposal_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4332 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_environment_variables_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6038 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_functions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6051 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_pool_tickets_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5163 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_pools_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5271 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_rule_sets_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9078 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match.py
+-rw-rw-r--   0 root         (0) root         (0)     5376 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_config.py
+-rw-rw-r--   0 root         (0) root         (0)     7304 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_override.py
+-rw-rw-r--   0 root         (0) root         (0)     5389 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_request.py
+-rw-rw-r--   0 root         (0) root         (0)    13957 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_pool.py
+-rw-rw-r--   0 root         (0) root         (0)    13555 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_pool_config.py
+-rw-rw-r--   0 root         (0) root         (0)     3741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_rule_set_name_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4623 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7370 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_status.py
+-rw-rw-r--   0 root         (0) root         (0)     5132 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_statuses.py
+-rw-rw-r--   0 root         (0) root         (0)     4262 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_namespace_config_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4440 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_party.py
+-rw-rw-r--   0 root         (0) root         (0)     4360 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_patch_namespace_config_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5348 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_player_data.py
+-rw-rw-r--   0 root         (0) root         (0)     3919 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_player_metric_record.py
+-rw-rw-r--   0 root         (0) root         (0)     5325 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_proposed_proposal.py
+-rw-rw-r--   0 root         (0) root         (0)     5521 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_rule_set_payload.py
+-rw-rw-r--   0 root         (0) root         (0)     4689 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_team.py
+-rw-rw-r--   0 root         (0) root         (0)     9670 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     3894 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_ticket_metric_result_record.py
+-rw-rw-r--   0 root         (0) root         (0)     6166 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/config_environment_variable.py
+-rw-rw-r--   0 root         (0) root         (0)     5022 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/configmodels_namespace_config.py
+-rw-rw-r--   0 root         (0) root         (0)     9692 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_match_ticket_record.py
+-rw-rw-r--   0 root         (0) root         (0)     4538 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_party.py
+-rw-rw-r--   0 root         (0) root         (0)     5231 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_proposed_proposal.py
+-rw-rw-r--   0 root         (0) root         (0)     4836 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_team.py
+-rw-rw-r--   0 root         (0) root         (0)    10585 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)    10304 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     6890 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_ds_information.py
+-rw-rw-r--   0 root         (0) root         (0)    15253 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_game_session.py
+-rw-rw-r--   0 root         (0) root         (0)     5437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)    14798 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_server.py
+-rw-rw-r--   0 root         (0) root         (0)     6311 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_user.py
+-rw-rw-r--   0 root         (0) root         (0)     5920 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/player_player_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4436 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.727961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/
+-rw-rw-r--   0 root         (0) root         (0)      739 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/accept_backfill.py
+-rw-rw-r--   0 root         (0) root         (0)     8127 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/create_backfill.py
+-rw-rw-r--   0 root         (0) root         (0)     7300 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/delete_backfill.py
+-rw-rw-r--   0 root         (0) root         (0)     7616 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill.py
+-rw-rw-r--   0 root         (0) root         (0)     7803 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill_proposal.py
+-rw-rw-r--   0 root         (0) root         (0)     8714 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/reject_backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/
+-rw-rw-r--   0 root         (0) root         (0)      631 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5481 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_all_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     6446 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_config_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     7733 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_patch_config_v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/environment_variables/
+-rw-rw-r--   0 root         (0) root         (0)      533 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/environment_variables/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5322 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/environment_variables/environment_variable_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/
+-rw-rw-r--   0 root         (0) root         (0)      686 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7853 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/create_match_function.py
+-rw-rw-r--   0 root         (0) root         (0)     7213 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/delete_match_function.py
+-rw-rw-r--   0 root         (0) root         (0)     8188 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/match_function_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8649 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/update_match_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/admin_get_match_pool_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     8760 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/create_match_pool.py
+-rw-rw-r--   0 root         (0) root         (0)     7155 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/delete_match_pool.py
+-rw-rw-r--   0 root         (0) root         (0)     7378 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/get_player_metric.py
+-rw-rw-r--   0 root         (0) root         (0)     7074 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_details.py
+-rw-rw-r--   0 root         (0) root         (0)     8809 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_list.py
+-rw-rw-r--   0 root         (0) root         (0)     7417 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_metric.py
+-rw-rw-r--   0 root         (0) root         (0)     9355 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/update_match_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/
+-rw-rw-r--   0 root         (0) root         (0)      677 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10272 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/create_match_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     7288 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/delete_match_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     8987 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/get_my_match_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     7454 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/match_ticket_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/
+-rw-rw-r--   0 root         (0) root         (0)      636 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4422 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4454 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     4448 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/version_check_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.731961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/
+-rw-rw-r--   0 root         (0) root         (0)      683 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8169 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/create_rule_set.py
+-rw-rw-r--   0 root         (0) root         (0)     7203 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/delete_rule_set.py
+-rw-rw-r--   0 root         (0) root         (0)     7167 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_details.py
+-rw-rw-r--   0 root         (0) root         (0)     8767 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/update_rule_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.735961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     3741 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18219 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_backfill.py
+-rw-rw-r--   0 root         (0) root         (0)     8291 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_config.py
+-rw-rw-r--   0 root         (0) root         (0)     2934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_environment_variables.py
+-rw-rw-r--   0 root         (0) root         (0)    12370 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_functions.py
+-rw-rw-r--   0 root         (0) root         (0)    27314 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_pools.py
+-rw-rw-r--   0 root         (0) root         (0)    16676 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     4519 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_operations.py
+-rw-rw-r--   0 root         (0) root         (0)    15926 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_rule_sets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:03.735961 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-07 06:29:03.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6809 2024-05-07 06:29:03.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:29:03.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:29:03.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:29:03.000000 accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      359 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_match2-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:29:03.735961 accelbyte_py_sdk_service_match2-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/PKG-INFO` & `accelbyte_py_sdk_service_match2-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-match2
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Match Service V2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Match Service V2
-* Version: 2.18.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/README.md` & `accelbyte_py_sdk_service_match2-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Match Service V2
-* Version: 2.18.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # backfill
 from .wrappers import accept_backfill
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .api_back_fill_accept_request import ApiBackFillAcceptRequest
 from .api_back_fill_create_request import ApiBackFillCreateRequest
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_accept_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_accept_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_create_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_create_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_back_fill_reject_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_back_fill_reject_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_create_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_create_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_get_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_get_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_backfill_proposal_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_backfill_proposal_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_environment_variables_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_environment_variables_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_functions_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_functions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_pool_tickets_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_pool_tickets_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_match_pools_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_match_pools_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_list_rule_sets_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_list_rule_sets_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_config.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_override.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_override.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_function_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_function_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_pool.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,30 +50,30 @@
 
         session_template: (session_template) REQUIRED str
 
         ticket_expiration_seconds: (ticket_expiration_seconds) REQUIRED int
 
         crossplay_disabled: (crossplay_disabled) OPTIONAL bool
 
-        platfrom_group_enabled: (platfrom_group_enabled) OPTIONAL bool
+        platform_group_enabled: (platform_group_enabled) OPTIONAL bool
     """
 
     # region fields
 
     auto_accept_backfill_proposal: bool  # REQUIRED
     backfill_proposal_expiration_seconds: int  # REQUIRED
     backfill_ticket_expiration_seconds: int  # REQUIRED
     match_function: str  # REQUIRED
     match_function_override: ApiMatchFunctionOverride  # REQUIRED
     name: str  # REQUIRED
     rule_set: str  # REQUIRED
     session_template: str  # REQUIRED
     ticket_expiration_seconds: int  # REQUIRED
     crossplay_disabled: bool  # OPTIONAL
-    platfrom_group_enabled: bool  # OPTIONAL
+    platform_group_enabled: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_auto_accept_backfill_proposal(self, value: bool) -> ApiMatchPool:
         self.auto_accept_backfill_proposal = value
@@ -113,16 +113,16 @@
         self.ticket_expiration_seconds = value
         return self
 
     def with_crossplay_disabled(self, value: bool) -> ApiMatchPool:
         self.crossplay_disabled = value
         return self
 
-    def with_platfrom_group_enabled(self, value: bool) -> ApiMatchPool:
-        self.platfrom_group_enabled = value
+    def with_platform_group_enabled(self, value: bool) -> ApiMatchPool:
+        self.platform_group_enabled = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
@@ -171,18 +171,18 @@
             result["ticket_expiration_seconds"] = int(self.ticket_expiration_seconds)
         elif include_empty:
             result["ticket_expiration_seconds"] = 0
         if hasattr(self, "crossplay_disabled"):
             result["crossplay_disabled"] = bool(self.crossplay_disabled)
         elif include_empty:
             result["crossplay_disabled"] = False
-        if hasattr(self, "platfrom_group_enabled"):
-            result["platfrom_group_enabled"] = bool(self.platfrom_group_enabled)
+        if hasattr(self, "platform_group_enabled"):
+            result["platform_group_enabled"] = bool(self.platform_group_enabled)
         elif include_empty:
-            result["platfrom_group_enabled"] = False
+            result["platform_group_enabled"] = False
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -194,15 +194,15 @@
         match_function: str,
         match_function_override: ApiMatchFunctionOverride,
         name: str,
         rule_set: str,
         session_template: str,
         ticket_expiration_seconds: int,
         crossplay_disabled: Optional[bool] = None,
-        platfrom_group_enabled: Optional[bool] = None,
+        platform_group_enabled: Optional[bool] = None,
         **kwargs,
     ) -> ApiMatchPool:
         instance = cls()
         instance.auto_accept_backfill_proposal = auto_accept_backfill_proposal
         instance.backfill_proposal_expiration_seconds = (
             backfill_proposal_expiration_seconds
         )
@@ -211,16 +211,16 @@
         instance.match_function_override = match_function_override
         instance.name = name
         instance.rule_set = rule_set
         instance.session_template = session_template
         instance.ticket_expiration_seconds = ticket_expiration_seconds
         if crossplay_disabled is not None:
             instance.crossplay_disabled = crossplay_disabled
-        if platfrom_group_enabled is not None:
-            instance.platfrom_group_enabled = platfrom_group_enabled
+        if platform_group_enabled is not None:
+            instance.platform_group_enabled = platform_group_enabled
         return instance
 
     @classmethod
     def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> ApiMatchPool:
         instance = cls()
         if not dict_:
             return instance
@@ -286,20 +286,20 @@
         elif include_empty:
             instance.ticket_expiration_seconds = 0
         if "crossplay_disabled" in dict_ and dict_["crossplay_disabled"] is not None:
             instance.crossplay_disabled = bool(dict_["crossplay_disabled"])
         elif include_empty:
             instance.crossplay_disabled = False
         if (
-            "platfrom_group_enabled" in dict_
-            and dict_["platfrom_group_enabled"] is not None
+            "platform_group_enabled" in dict_
+            and dict_["platform_group_enabled"] is not None
         ):
-            instance.platfrom_group_enabled = bool(dict_["platfrom_group_enabled"])
+            instance.platform_group_enabled = bool(dict_["platform_group_enabled"])
         elif include_empty:
-            instance.platfrom_group_enabled = False
+            instance.platform_group_enabled = False
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ApiMatchPool]:
         return (
@@ -341,15 +341,15 @@
             "match_function": "match_function",
             "match_function_override": "match_function_override",
             "name": "name",
             "rule_set": "rule_set",
             "session_template": "session_template",
             "ticket_expiration_seconds": "ticket_expiration_seconds",
             "crossplay_disabled": "crossplay_disabled",
-            "platfrom_group_enabled": "platfrom_group_enabled",
+            "platform_group_enabled": "platform_group_enabled",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "auto_accept_backfill_proposal": True,
             "backfill_proposal_expiration_seconds": True,
@@ -357,11 +357,11 @@
             "match_function": True,
             "match_function_override": True,
             "name": True,
             "rule_set": True,
             "session_template": True,
             "ticket_expiration_seconds": True,
             "crossplay_disabled": False,
-            "platfrom_group_enabled": False,
+            "platform_group_enabled": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_pool_config.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_pool_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,29 +48,29 @@
 
         session_template: (session_template) REQUIRED str
 
         ticket_expiration_seconds: (ticket_expiration_seconds) REQUIRED int
 
         crossplay_disabled: (crossplay_disabled) OPTIONAL bool
 
-        platfrom_group_enabled: (platfrom_group_enabled) OPTIONAL bool
+        platform_group_enabled: (platform_group_enabled) OPTIONAL bool
     """
 
     # region fields
 
     auto_accept_backfill_proposal: bool  # REQUIRED
     backfill_proposal_expiration_seconds: int  # REQUIRED
     backfill_ticket_expiration_seconds: int  # REQUIRED
     match_function: str  # REQUIRED
     match_function_override: ApiMatchFunctionOverride  # REQUIRED
     rule_set: str  # REQUIRED
     session_template: str  # REQUIRED
     ticket_expiration_seconds: int  # REQUIRED
     crossplay_disabled: bool  # OPTIONAL
-    platfrom_group_enabled: bool  # OPTIONAL
+    platform_group_enabled: bool  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_auto_accept_backfill_proposal(self, value: bool) -> ApiMatchPoolConfig:
         self.auto_accept_backfill_proposal = value
@@ -108,16 +108,16 @@
         self.ticket_expiration_seconds = value
         return self
 
     def with_crossplay_disabled(self, value: bool) -> ApiMatchPoolConfig:
         self.crossplay_disabled = value
         return self
 
-    def with_platfrom_group_enabled(self, value: bool) -> ApiMatchPoolConfig:
-        self.platfrom_group_enabled = value
+    def with_platform_group_enabled(self, value: bool) -> ApiMatchPoolConfig:
+        self.platform_group_enabled = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
@@ -162,18 +162,18 @@
             result["ticket_expiration_seconds"] = int(self.ticket_expiration_seconds)
         elif include_empty:
             result["ticket_expiration_seconds"] = 0
         if hasattr(self, "crossplay_disabled"):
             result["crossplay_disabled"] = bool(self.crossplay_disabled)
         elif include_empty:
             result["crossplay_disabled"] = False
-        if hasattr(self, "platfrom_group_enabled"):
-            result["platfrom_group_enabled"] = bool(self.platfrom_group_enabled)
+        if hasattr(self, "platform_group_enabled"):
+            result["platform_group_enabled"] = bool(self.platform_group_enabled)
         elif include_empty:
-            result["platfrom_group_enabled"] = False
+            result["platform_group_enabled"] = False
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -184,15 +184,15 @@
         backfill_ticket_expiration_seconds: int,
         match_function: str,
         match_function_override: ApiMatchFunctionOverride,
         rule_set: str,
         session_template: str,
         ticket_expiration_seconds: int,
         crossplay_disabled: Optional[bool] = None,
-        platfrom_group_enabled: Optional[bool] = None,
+        platform_group_enabled: Optional[bool] = None,
         **kwargs,
     ) -> ApiMatchPoolConfig:
         instance = cls()
         instance.auto_accept_backfill_proposal = auto_accept_backfill_proposal
         instance.backfill_proposal_expiration_seconds = (
             backfill_proposal_expiration_seconds
         )
@@ -200,16 +200,16 @@
         instance.match_function = match_function
         instance.match_function_override = match_function_override
         instance.rule_set = rule_set
         instance.session_template = session_template
         instance.ticket_expiration_seconds = ticket_expiration_seconds
         if crossplay_disabled is not None:
             instance.crossplay_disabled = crossplay_disabled
-        if platfrom_group_enabled is not None:
-            instance.platfrom_group_enabled = platfrom_group_enabled
+        if platform_group_enabled is not None:
+            instance.platform_group_enabled = platform_group_enabled
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ApiMatchPoolConfig:
         instance = cls()
@@ -273,20 +273,20 @@
         elif include_empty:
             instance.ticket_expiration_seconds = 0
         if "crossplay_disabled" in dict_ and dict_["crossplay_disabled"] is not None:
             instance.crossplay_disabled = bool(dict_["crossplay_disabled"])
         elif include_empty:
             instance.crossplay_disabled = False
         if (
-            "platfrom_group_enabled" in dict_
-            and dict_["platfrom_group_enabled"] is not None
+            "platform_group_enabled" in dict_
+            and dict_["platform_group_enabled"] is not None
         ):
-            instance.platfrom_group_enabled = bool(dict_["platfrom_group_enabled"])
+            instance.platform_group_enabled = bool(dict_["platform_group_enabled"])
         elif include_empty:
-            instance.platfrom_group_enabled = False
+            instance.platform_group_enabled = False
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ApiMatchPoolConfig]:
         return (
@@ -329,26 +329,26 @@
             "backfill_ticket_expiration_seconds": "backfill_ticket_expiration_seconds",
             "match_function": "match_function",
             "match_function_override": "match_function_override",
             "rule_set": "rule_set",
             "session_template": "session_template",
             "ticket_expiration_seconds": "ticket_expiration_seconds",
             "crossplay_disabled": "crossplay_disabled",
-            "platfrom_group_enabled": "platfrom_group_enabled",
+            "platform_group_enabled": "platform_group_enabled",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "auto_accept_backfill_proposal": True,
             "backfill_proposal_expiration_seconds": True,
             "backfill_ticket_expiration_seconds": True,
             "match_function": True,
             "match_function_override": True,
             "rule_set": True,
             "session_template": True,
             "ticket_expiration_seconds": True,
             "crossplay_disabled": False,
-            "platfrom_group_enabled": False,
+            "platform_group_enabled": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_rule_set_name_data.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_rule_set_name_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_response.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_status.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_status.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_statuses.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_match_ticket_statuses.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_namespace_config_list.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_namespace_config_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_party.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_patch_namespace_config_request.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_patch_namespace_config_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_player_data.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_player_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_player_metric_record.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_player_metric_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_proposed_proposal.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_proposed_proposal.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_rule_set_payload.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_rule_set_payload.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_team.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_ticket.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/api_ticket_metric_result_record.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/api_ticket_metric_result_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/config_environment_variable.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/config_environment_variable.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/configmodels_namespace_config.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/configmodels_namespace_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_match_ticket_record.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_match_ticket_record.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_party.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_party.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_proposed_proposal.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_proposed_proposal.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_team.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_team.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/matchmaker_ticket.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/matchmaker_ticket.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_configuration.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_configuration.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_ds_information.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_ds_information.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_game_session.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_game_session.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_pagination.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_server.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_server.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/models_user.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/models_user.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/player_player_data.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/player_player_data.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/models/response_error.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .accept_backfill import AcceptBackfill
 from .create_backfill import CreateBackfill
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/accept_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/accept_backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,33 +73,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/match2/v1/namespaces/{namespace}/backfill/{backfillID}/proposal/accept"
     )
+    _path: str = (
+        "/match2/v1/namespaces/{namespace}/backfill/{backfillID}/proposal/accept"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiBackFillAcceptRequest  # REQUIRED in [body]
     backfill_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/create_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/create_backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/backfill"
+    _path: str = "/match2/v1/namespaces/{namespace}/backfill"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiBackFillCreateRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/delete_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/delete_backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/backfill/{backfillID}"
+    _path: str = "/match2/v1/namespaces/{namespace}/backfill/{backfillID}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     backfill_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/backfill/{backfillID}"
+    _path: str = "/match2/v1/namespaces/{namespace}/backfill/{backfillID}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     backfill_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill_proposal.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/get_backfill_proposal.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/backfill/proposal"
+    _path: str = "/match2/v1/namespaces/{namespace}/backfill/proposal"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     session_id: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/backfill/reject_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/backfill/reject_backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,33 +72,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/match2/v1/namespaces/{namespace}/backfill/{backfillID}/proposal/reject"
     )
+    _path: str = (
+        "/match2/v1/namespaces/{namespace}/backfill/{backfillID}/proposal/reject"
+    )
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiBackFillRejectRequest  # REQUIRED in [body]
     backfill_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_all_config_v1 import AdminGetAllConfigV1
 from .admin_get_config_v1 import AdminGetConfigV1
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_all_config_v1.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_all_config_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,29 +60,41 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/config"
+    _path: str = "/match2/v1/config"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_config_v1.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_get_config_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,43 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/config/namespaces/{namespace}"
+    _path: str = "/match2/v1/config/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/config/admin_patch_config_v1.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/config/admin_patch_config_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/config/namespaces/{namespace}"
+    _path: str = "/match2/v1/config/namespaces/{namespace}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiPatchNamespaceConfigRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/environment_variables/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
-from .environment_variable_list import EnvironmentVariableList
+from .get_healthcheck_info import GetHealthcheckInfo
+from .get_healthcheck_info_v1 import GetHealthcheckInfoV1
+from .version_check_handler import VersionCheckHandler
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/environment_variables/environment_variable_list.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/environment_variables/environment_variable_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,29 +58,41 @@
 
         403: Forbidden - ResponseError (Forbidden)
     """
 
     # region fields
 
     _url: str = "/match2/v1/environment-variables"
+    _path: str = "/match2/v1/environment-variables"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_match_function import CreateMatchFunction
 from .delete_match_function import DeleteMatchFunction
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/create_match_function.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/create_match_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-functions"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-functions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiMatchFunctionRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/delete_match_function.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/delete_match_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-functions/{name}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-functions/{name}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/match_function_list.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/match_function_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,33 +66,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-functions"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-functions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_functions/update_match_function.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_functions/update_match_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,33 +71,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-functions/{name}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-functions/{name}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiMatchFunctionRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_match_pool_tickets import AdminGetMatchPoolTickets
 from .create_match_pool import CreateMatchPool
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/admin_get_match_pool_tickets.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/admin_get_match_pool_tickets.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,34 +72,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/tickets"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/tickets"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/create_match_pool.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/create_match_pool.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,32 +86,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiMatchPool  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/delete_match_pool.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/delete_match_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/get_player_metric.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/get_player_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,32 +66,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/metrics/player"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/metrics/player"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_details.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,32 +64,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_list.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,34 +68,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     name: str  # OPTIONAL in [query]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_metric.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/match_pool_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/metrics"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}/metrics"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_pools/update_match_pool.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_pools/update_match_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,33 +86,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-pools/{pool}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiMatchPoolConfig  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     pool: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_match_ticket import CreateMatchTicket
 from .delete_match_ticket import DeleteMatchTicket
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/create_match_ticket.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/create_match_ticket.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,33 +35,33 @@
 
 
 class CreateMatchTicket(Operation):
     """Create a matchmaking ticket (CreateMatchTicket)
 
     Creates a new request for matchmaking.
 
-    Cross Platform: Allow player to play game with "any" registered platforms.
+    Cross Platform: Allow player to play game with "all" registered platforms.
     1. Cross Platform can be enabled through session service or create match ticket.
     a. via ticket: specify several cross_platform on create match ticket attributes. **[DEPRECATED]** client should not send from attribute `cross_platform` will be populated from backend
     This value will override player attributes in session service. e.g. cross_platform:[xbox,psn,steam]
     b. via session service: set player/party cross_platform attributes.
-    c. Enable match options ruleset with name cross_platform and type "any".
+    c. Enable match options ruleset with name cross_platform and type "all".
     ```
     {
     "name": "co-op",
     "data": {
     "alliance": {
     "min_number": 1,
     "max_number": 1,
     "player_min_number": 1,
     "player_max_number": 4
     },
     "match_options": {
     "options": [
-    {"name": "cross_platform", "type": "any"}
+    {"name": "cross_platform", "type": "all"}
     ]
     }
     }
     }
     ```
     2. Cross Platform can be disabled from the matchpool configuration `crossplay_disabled=true`
     3. When matchpool `crossplay_disabled=false`
@@ -106,32 +106,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-tickets"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-tickets"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiMatchTicketRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/delete_match_ticket.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/delete_match_ticket.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-tickets/{ticketid}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-tickets/{ticketid}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     ticketid: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/get_my_match_tickets.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/get_my_match_tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,34 +68,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-tickets/me"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-tickets/me"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     match_pool: str  # OPTIONAL in [query]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/match_tickets/match_ticket_details.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/match_tickets/match_ticket_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,32 +66,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/match-tickets/{ticketid}"
+    _path: str = "/match2/v1/namespaces/{namespace}/match-tickets/{ticketid}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     ticketid: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info.py`

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
     _produces: List[str] = []
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info_v1.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/get_healthcheck_info_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,29 +50,41 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/match2/healthz"
+    _path: str = "/match2/healthz"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = []
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/operations/version_check_handler.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/operations/version_check_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,29 +50,41 @@
     Responses:
         200: OK - (OK)
     """
 
     # region fields
 
     _url: str = "/match2/version"
+    _path: str = "/match2/version"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = []
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_rule_set import CreateRuleSet
 from .delete_rule_set import DeleteRuleSet
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/create_rule_set.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/create_rule_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     Creates a new rules set.
 
     A rule set has a name and contains arbitrary data which is meaningful to some particular match function(s)
     The name is used for a match pool to select the ruleset data that should be sent to the match function when matchmaking in that pool.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets
 
         method: POST
 
         tags: ["Rule-Sets", "admin"]
 
@@ -73,32 +75,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/rulesets"
+    _path: str = "/match2/v1/namespaces/{namespace}/rulesets"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiRuleSetPayload  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/delete_rule_set.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/delete_rule_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _path: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     ruleset: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_details.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,32 +64,44 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _path: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     ruleset: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_list.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/rule_set_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,34 +68,46 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/rulesets"
+    _path: str = "/match2/v1/namespaces/{namespace}/rulesets"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     name: str  # OPTIONAL in [query]
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

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/operations/rule_sets/update_rule_set.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/operations/rule_sets/update_rule_set.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 class UpdateRuleSet(Operation):
     """Update a match rule set (UpdateRuleSet)
 
     Updates an existing matchmaking rule set.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets/{ruleset}
 
         method: PUT
 
         tags: ["Rule-Sets", "admin"]
 
@@ -72,33 +74,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _path: str = "/match2/v1/namespaces/{namespace}/rulesets/{ruleset}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "match2"
+
     body: ApiRuleSetPayload  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     ruleset: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/__init__.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Match Service V2."""
 
-__version__ = "2.18.1"
+__version__ = "2.19.2"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._backfill import accept_backfill
 from ._backfill import accept_backfill_async
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_backfill.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_backfill.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_config.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_config.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_environment_variables.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_environment_variables.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_functions.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_functions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_pools.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_pools.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_match_tickets.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_match_tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,33 +48,33 @@
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a matchmaking ticket (CreateMatchTicket)
 
     Creates a new request for matchmaking.
 
-    Cross Platform: Allow player to play game with "any" registered platforms.
+    Cross Platform: Allow player to play game with "all" registered platforms.
     1. Cross Platform can be enabled through session service or create match ticket.
     a. via ticket: specify several cross_platform on create match ticket attributes. **[DEPRECATED]** client should not send from attribute `cross_platform` will be populated from backend
     This value will override player attributes in session service. e.g. cross_platform:[xbox,psn,steam]
     b. via session service: set player/party cross_platform attributes.
-    c. Enable match options ruleset with name cross_platform and type "any".
+    c. Enable match options ruleset with name cross_platform and type "all".
     ```
     {
     "name": "co-op",
     "data": {
     "alliance": {
     "min_number": 1,
     "max_number": 1,
     "player_min_number": 1,
     "player_max_number": 4
     },
     "match_options": {
     "options": [
-    {"name": "cross_platform", "type": "any"}
+    {"name": "cross_platform", "type": "all"}
     ]
     }
     }
     }
     ```
     2. Cross Platform can be disabled from the matchpool configuration `crossplay_disabled=true`
     3. When matchpool `crossplay_disabled=false`
@@ -137,33 +137,33 @@
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Create a matchmaking ticket (CreateMatchTicket)
 
     Creates a new request for matchmaking.
 
-    Cross Platform: Allow player to play game with "any" registered platforms.
+    Cross Platform: Allow player to play game with "all" registered platforms.
     1. Cross Platform can be enabled through session service or create match ticket.
     a. via ticket: specify several cross_platform on create match ticket attributes. **[DEPRECATED]** client should not send from attribute `cross_platform` will be populated from backend
     This value will override player attributes in session service. e.g. cross_platform:[xbox,psn,steam]
     b. via session service: set player/party cross_platform attributes.
-    c. Enable match options ruleset with name cross_platform and type "any".
+    c. Enable match options ruleset with name cross_platform and type "all".
     ```
     {
     "name": "co-op",
     "data": {
     "alliance": {
     "min_number": 1,
     "max_number": 1,
     "player_min_number": 1,
     "player_max_number": 4
     },
     "match_options": {
     "options": [
-    {"name": "cross_platform", "type": "any"}
+    {"name": "cross_platform", "type": "all"}
     ]
     }
     }
     }
     ```
     2. Cross Platform can be disabled from the matchpool configuration `crossplay_disabled=true`
     3. When matchpool `crossplay_disabled=false`
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_operations.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_operations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk/api/match2/wrappers/_rule_sets.py` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk/api/match2/wrappers/_rule_sets.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     Creates a new rules set.
 
     A rule set has a name and contains arbitrary data which is meaningful to some particular match function(s)
     The name is used for a match pool to select the ruleset data that should be sent to the match function when matchmaking in that pool.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets
 
         method: POST
 
         tags: ["Rule-Sets", "admin"]
 
@@ -109,14 +111,16 @@
     Creates a new rules set.
 
     A rule set has a name and contains arbitrary data which is meaningful to some particular match function(s)
     The name is used for a match pool to select the ruleset data that should be sent to the match function when matchmaking in that pool.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets
 
         method: POST
 
         tags: ["Rule-Sets", "admin"]
 
@@ -480,14 +484,16 @@
 ):
     """Update a match rule set (UpdateRuleSet)
 
     Updates an existing matchmaking rule set.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets/{ruleset}
 
         method: PUT
 
         tags: ["Rule-Sets", "admin"]
 
@@ -538,14 +544,16 @@
 ):
     """Update a match rule set (UpdateRuleSet)
 
     Updates an existing matchmaking rule set.
 
     To use custom rules set please set enable_custom_match_function=true. Default (false).
 
+    When custom enable_custom_match_function=true, the ruleset will only validate if the rule is valid json.
+
     Properties:
         url: /match2/v1/namespaces/{namespace}/rulesets/{ruleset}
 
         method: PUT
 
         tags: ["Rule-Sets", "admin"]
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-match2
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Match Service V2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Match Service V2
-* Version: 2.18.1
+* Version: 2.19.2
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-match2-0.8.0/accelbyte_py_sdk_service_match2.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_match2-0.9.0/accelbyte_py_sdk_service_match2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

