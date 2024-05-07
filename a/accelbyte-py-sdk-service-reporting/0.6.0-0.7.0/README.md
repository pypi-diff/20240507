# Comparing `tmp/accelbyte-py-sdk-service-reporting-0.6.0.tar.gz` & `tmp/accelbyte_py_sdk_service_reporting-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-reporting-0.6.0.tar", last modified: Tue Feb 27 05:41:22 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_reporting-0.7.0.tar", last modified: Tue May  7 06:29:50 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-reporting-0.6.0.tar` & `accelbyte_py_sdk_service_reporting-0.7.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.384230 accelbyte-py-sdk-service-reporting-0.6.0/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-02-27 05:41:22.384230 accelbyte-py-sdk-service-reporting-0.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      877 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.372230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.372230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.372230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/
--rw-rw-r--   0 root         (0) root         (0)     3814 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.376230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/
--rw-rw-r--   0 root         (0) root         (0)     4317 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5226 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py
--rw-rw-r--   0 root         (0) root         (0)     5239 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4250 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4293 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py
--rw-rw-r--   0 root         (0) root         (0)     5171 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     8332 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py
--rw-rw-r--   0 root         (0) root         (0)     6548 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py
--rw-rw-r--   0 root         (0) root         (0)     6563 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py
--rw-rw-r--   0 root         (0) root         (0)     5534 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py
--rw-rw-r--   0 root         (0) root         (0)     5672 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py
--rw-rw-r--   0 root         (0) root         (0)     4662 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     5235 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py
--rw-rw-r--   0 root         (0) root         (0)     4567 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py
--rw-rw-r--   0 root         (0) root         (0)     5945 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py
--rw-rw-r--   0 root         (0) root         (0)     5972 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     4459 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py
--rw-rw-r--   0 root         (0) root         (0)     7157 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py
--rw-rw-r--   0 root         (0) root         (0)     7180 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py
--rw-rw-r--   0 root         (0) root         (0)     3914 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py
--rw-rw-r--   0 root         (0) root         (0)     9274 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py
--rw-rw-r--   0 root         (0) root         (0)    11237 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py
--rw-rw-r--   0 root         (0) root         (0)     5168 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py
--rw-rw-r--   0 root         (0) root         (0)     5466 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     4408 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     5215 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     4530 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py
--rw-rw-r--   0 root         (0) root         (0)     5248 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     5521 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    13341 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py
--rw-rw-r--   0 root         (0) root         (0)     6299 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py
--rw-rw-r--   0 root         (0) root         (0)     9713 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py
--rw-rw-r--   0 root         (0) root         (0)    10961 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py
--rw-rw-r--   0 root         (0) root         (0)    12043 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py
--rw-rw-r--   0 root         (0) root         (0)     5431 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py
--rw-rw-r--   0 root         (0) root         (0)     4364 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py
--rw-rw-r--   0 root         (0) root         (0)     4662 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.376230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/
--rw-rw-r--   0 root         (0) root         (0)      438 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.376230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/
--rw-rw-r--   0 root         (0) root         (0)      577 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7142 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py
--rw-rw-r--   0 root         (0) root         (0)     7095 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/
--rw-rw-r--   0 root         (0) root         (0)      899 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6382 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py
--rw-rw-r--   0 root         (0) root         (0)     6173 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py
--rw-rw-r--   0 root         (0) root         (0)     5057 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/
--rw-rw-r--   0 root         (0) root         (0)      831 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7606 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     6645 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     6843 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py
--rw-rw-r--   0 root         (0) root         (0)     9855 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py
--rw-rw-r--   0 root         (0) root         (0)     8702 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)     8179 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/
--rw-rw-r--   0 root         (0) root         (0)     1055 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5811 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     6739 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py
--rw-rw-r--   0 root         (0) root         (0)     9159 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     8153 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     7621 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py
--rw-rw-r--   0 root         (0) root         (0)     7277 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py
--rw-rw-r--   0 root         (0) root         (0)     7551 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     6349 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py
--rw-rw-r--   0 root         (0) root         (0)     6382 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     6671 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py
--rw-rw-r--   0 root         (0) root         (0)     8072 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py
--rw-rw-r--   0 root         (0) root         (0)     8367 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/
--rw-rw-r--   0 root         (0) root         (0)      560 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7759 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py
--rw-rw-r--   0 root         (0) root         (0)    10167 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6536 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     8296 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py
--rw-rw-r--   0 root         (0) root         (0)     6729 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py
--rw-rw-r--   0 root         (0) root         (0)    12745 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     7824 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py
--rw-rw-r--   0 root         (0) root         (0)     7963 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/
--rw-rw-r--   0 root         (0) root         (0)      582 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9130 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     7559 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.380230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reports/
--rw-rw-r--   0 root         (0) root         (0)      511 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7973 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.384230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     4578 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6347 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py
--rw-rw-r--   0 root         (0) root         (0)    10312 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py
--rw-rw-r--   0 root         (0) root         (0)    19611 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py
--rw-rw-r--   0 root         (0) root         (0)    32822 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     8390 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py
--rw-rw-r--   0 root         (0) root         (0)    18658 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py
--rw-rw-r--   0 root         (0) root         (0)     6758 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py
--rw-rw-r--   0 root         (0) root         (0)     5020 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:41:22.384230 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2024-02-27 05:41:22.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7486 2024-02-27 05:41:22.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:41:22.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:41:22.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:41:22.000000 accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-02-27 05:33:51.000000 accelbyte-py-sdk-service-reporting-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:41:22.384230 accelbyte-py-sdk-service-reporting-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      877 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.742686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/
+-rw-rw-r--   0 root         (0) root         (0)     3814 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/
+-rw-rw-r--   0 root         (0) root         (0)     4317 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5226 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5239 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4250 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5171 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8332 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6548 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6563 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5534 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     5672 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5235 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4567 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5945 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5972 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4459 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7157 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7180 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3914 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9274 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py
+-rw-rw-r--   0 root         (0) root         (0)    11237 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5168 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py
+-rw-rw-r--   0 root         (0) root         (0)     5466 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     4408 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5215 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5248 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5521 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    13341 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6299 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     9713 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py
+-rw-rw-r--   0 root         (0) root         (0)    10961 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12043 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5431 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4364 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4662 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/
+-rw-rw-r--   0 root         (0) root         (0)      577 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py
+-rw-rw-r--   0 root         (0) root         (0)     7390 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/
+-rw-rw-r--   0 root         (0) root         (0)      899 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6659 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py
+-rw-rw-r--   0 root         (0) root         (0)     5331 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py
+-rw-rw-r--   0 root         (0) root         (0)     8063 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/
+-rw-rw-r--   0 root         (0) root         (0)      831 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7891 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     6939 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     7138 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py
+-rw-rw-r--   0 root         (0) root         (0)    10141 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py
+-rw-rw-r--   0 root         (0) root         (0)     8996 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     8480 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6103 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7038 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     9447 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     8448 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7914 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py
+-rw-rw-r--   0 root         (0) root         (0)     7565 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     7844 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     6685 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     6974 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py
+-rw-rw-r--   0 root         (0) root         (0)     8371 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py
+-rw-rw-r--   0 root         (0) root         (0)     8670 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.746686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/
+-rw-rw-r--   0 root         (0) root         (0)      560 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8047 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py
+-rw-rw-r--   0 root         (0) root         (0)    10455 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6835 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     8603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py
+-rw-rw-r--   0 root         (0) root         (0)     7028 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py
+-rw-rw-r--   0 root         (0) root         (0)    13033 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     8122 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py
+-rw-rw-r--   0 root         (0) root         (0)     8290 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/
+-rw-rw-r--   0 root         (0) root         (0)      582 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9419 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     7853 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/
+-rw-rw-r--   0 root         (0) root         (0)      511 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8262 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     4578 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6347 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py
+-rw-rw-r--   0 root         (0) root         (0)    10312 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py
+-rw-rw-r--   0 root         (0) root         (0)    19611 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py
+-rw-rw-r--   0 root         (0) root         (0)    32822 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     8390 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py
+-rw-rw-r--   0 root         (0) root         (0)    18658 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py
+-rw-rw-r--   0 root         (0) root         (0)     6758 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py
+-rw-rw-r--   0 root         (0) root         (0)     5020 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:29:50.000000 accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_reporting-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:29:50.750686 accelbyte_py_sdk_service_reporting-0.7.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/PKG-INFO` & `accelbyte_py_sdk_service_reporting-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-reporting
-Version: 0.6.0
+Version: 0.7.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Reporting Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.32
+* Version: 0.1.34
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/README.md` & `accelbyte_py_sdk_service_reporting-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.32
+* Version: 0.1.34
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # admin_configurations
 from .wrappers import get
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .restapi_action_api_request import RestapiActionApiRequest
 from .restapi_action_api_response import RestapiActionApiResponse
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_action_list_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_all_reasons_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_admin_reason_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ban_account_action_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_category_limit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_create_reason_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_extension_category_list_api_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_actions_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_active_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rule_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_moderation_rules_list.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_public_reason_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reason_group_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_report_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_reporting_limit.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_submit_report_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_ticket_statistic_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_unused_reason_list_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_reason_group_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/models/restapi_update_ticket_resolutions_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .get import Get
 from .get import (
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/configurations"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/configurations"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     category: Union[str, CategoryEnum]  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_configurations/upsert.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/configurations"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/configurations"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiReportingLimit  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_extension__954f3a import AdminCreateExtensionCategory
 from .admin_create_mod_action import AdminCreateModAction
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_extension__954f3a.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,31 +61,43 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/extensionCategories"
+    _path: str = "/reporting/v1/admin/extensionCategories"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiExtensionCategoryApiRequest  # REQUIRED in [body]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_create_mod_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,31 +61,43 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/extensionActions"
+    _path: str = "/reporting/v1/admin/extensionActions"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiActionApiRequest  # REQUIRED in [body]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_action_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,29 +58,41 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/extensionActions"
+    _path: str = "/reporting/v1/admin/extensionActions"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_extension_categories_and_auto_moderation_actions/admin_find_extension_ca_6e8210.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,32 +75,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/extensionCategories"
+    _path: str = "/reporting/v1/admin/extensionCategories"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     order: Union[str, OrderEnum]  # OPTIONAL in [query]
     sort_by: Union[str, SortByEnum]  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .create_moderation_rule import CreateModerationRule
 from .delete_moderation_rule import DeleteModerationRule
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/create_moderation_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,32 +74,44 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rule"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rule"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiModerationRuleRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/delete_moderation_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,32 +61,44 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     rule_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rule_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,32 +62,44 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rules/{ruleId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rules/{ruleId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     rule_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/get_moderation_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,20 +70,24 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rules"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rules"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     category: str  # OPTIONAL in [query]
     extension_category: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
 
     # endregion fields
@@ -91,14 +95,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,33 +77,45 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiModerationRuleRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     rule_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_moderation_rule/update_moderation_rule_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,33 +66,45 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}/status"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/rule/{ruleId}/status"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiModerationRuleActiveRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     rule_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_get_all_reasons import AdminGetAllReasons
 from .admin_get_reason import AdminGetReason
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_all_reasons.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,31 +58,43 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/all"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/all"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reason.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,32 +62,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     reason_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_reasons.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,20 +68,24 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     group: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     title: str  # OPTIONAL in [query]
 
     # endregion fields
@@ -89,14 +93,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_get_unused_reasons.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,33 +64,45 @@
 
         500: Internal Server Error - RestapiErrorResponse (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/unused"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/unused"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     extension_category: str  # OPTIONAL in [query]
     category: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/admin_list_reason_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,33 +63,45 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiCreateReasonRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/create_reason_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,32 +67,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiCreateReasonGroupRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     reason_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/delete_reason_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,32 +59,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     group_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/get_reason_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,32 +61,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     group_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,33 +67,45 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasons/{reasonId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiCreateReasonRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     reason_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reasons/update_reason_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,33 +68,45 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reasonGroups/{groupId}"
+    _base_path: str = ""
     _method: str = "PATCH"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiUpdateReasonGroupRequest  # REQUIRED in [body]
     group_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_submit_report import AdminSubmitReport
 from .list_reports import ListReports
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/admin_submit_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,32 +72,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reports"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reports"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiSubmitReportRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_reports/list_reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,20 +74,24 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/reports"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/reports"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     category: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     reported_user_id: str  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .delete_ticket import DeleteTicket
 from .get_reports_by_ticket import GetReportsByTicket
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/delete_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,32 +61,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     ticket_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_reports_by_ticket.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,34 +64,46 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}/reports"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}/reports"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     ticket_id: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/get_ticket_detail.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,32 +62,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     ticket_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/list_tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,20 +77,24 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/tickets"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/tickets"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     category: str  # OPTIONAL in [query]
     extension_category: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     order: str  # OPTIONAL in [query]
     reported_user_id: str  # OPTIONAL in [query]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/ticket_statistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,33 +64,45 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/statistic"
+    _path: str = "/reporting/v1/admin/namespaces/{namespace}/tickets/statistic"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     extension_category: str  # OPTIONAL in [query]
     category: str  # REQUIRED in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/admin_tickets/update_ticket_resolutions.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,33 +65,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}/resolutions"
     )
+    _path: str = (
+        "/reporting/v1/admin/namespaces/{namespace}/tickets/{ticketId}/resolutions"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiUpdateTicketResolutionsRequest  # REQUIRED in [body]
     namespace: str  # REQUIRED in [path]
     ticket_id: str  # REQUIRED in [path]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .public_get_reasons import PublicGetReasons
 from .public_list_reason_groups import PublicListReasonGroups
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_get_reasons.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,20 +67,24 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/public/namespaces/{namespace}/reasons"
+    _path: str = "/reporting/v1/public/namespaces/{namespace}/reasons"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     namespace: str  # REQUIRED in [path]
     group: str  # OPTIONAL in [query]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     title: str  # OPTIONAL in [query]
 
     # endregion fields
@@ -88,14 +92,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reasons/public_list_reason_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,33 +62,45 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/public/namespaces/{namespace}/reasonGroups"
+    _path: str = "/reporting/v1/public/namespaces/{namespace}/reasonGroups"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/operations/public_reports/submit_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,32 +75,44 @@
 
         500: Internal Server Error - RestapiErrorResponse
     """
 
     # region fields
 
     _url: str = "/reporting/v1/public/namespaces/{namespace}/reports"
+    _path: str = "/reporting/v1/public/namespaces/{namespace}/reports"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "reporting"
+
     body: RestapiSubmitReportRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Reporting Service."""
 
-__version__ = "0.1.32"
+__version__ = "0.1.34"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._admin_configurations import get
 from ._admin_configurations import get_async
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_configurations.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_extension_categories_and_auto_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_moderation_rule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_reports.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_admin_tickets.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reasons.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk/api/reporting/wrappers/_public_reports.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-reporting
-Version: 0.6.0
+Version: 0.7.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Reporting Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Reporting Service
-* Version: 0.1.32
+* Version: 0.1.34
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-reporting-0.6.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_reporting-0.7.0/accelbyte_py_sdk_service_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

