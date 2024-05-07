# Comparing `tmp/accelbyte-py-sdk-service-achievement-0.8.0.tar.gz` & `tmp/accelbyte-py-sdk-service-achievement-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-achievement-0.8.0.tar", last modified: Tue Feb 27 05:34:34 2024, max compression
+gzip compressed data, was "accelbyte-py-sdk-service-achievement-0.9.0.tar", last modified: Wed Mar 13 06:09:30 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-achievement-0.8.0.tar` & `accelbyte-py-sdk-service-achievement-0.9.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     1142 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      882 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.878007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.878007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.882007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/
--rw-rw-r--   0 root         (0) root         (0)     3262 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.882007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/
--rw-rw-r--   0 root         (0) root         (0)     2098 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4025 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_order_update_request.py
--rw-rw-r--   0 root         (0) root         (0)    13553 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_request.py
--rw-rw-r--   0 root         (0) root         (0)    17066 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)    12919 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_update_request.py
--rw-rw-r--   0 root         (0) root         (0)     6423 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_additional_info.py
--rw-rw-r--   0 root         (0) root         (0)     8164 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_contributor_response.py
--rw-rw-r--   0 root         (0) root         (0)     9627 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_global_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     4087 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_icon.py
--rw-rw-r--   0 root         (0) root         (0)     5217 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     5217 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_contributor_response.py
--rw-rw-r--   0 root         (0) root         (0)     5358 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_global_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     4999 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_tag_response.py
--rw-rw-r--   0 root         (0) root         (0)     6335 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     5339 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_contribution_response.py
--rw-rw-r--   0 root         (0) root         (0)     4284 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_pagination.py
--rw-rw-r--   0 root         (0) root         (0)    16155 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_public_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     5247 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_public_achievements_response.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_tag_response.py
--rw-rw-r--   0 root         (0) root         (0)     7404 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_user_achievement_response.py
--rw-rw-r--   0 root         (0) root         (0)     8321 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_user_contribution_response.py
--rw-rw-r--   0 root         (0) root         (0)     4439 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/response_error.py
--rw-rw-r--   0 root         (0) root         (0)     6541 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/service_import_config_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.882007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/
--rw-rw-r--   0 root         (0) root         (0)      441 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.882007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/
--rw-rw-r--   0 root         (0) root         (0)     1262 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8638 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_create_new_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     7455 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_delete_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     7587 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_get_achievement.py
--rw-rw-r--   0 root         (0) root         (0)    11809 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_list_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8767 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievemen_d288a7.py
--rw-rw-r--   0 root         (0) root         (0)     8815 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     7444 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/export_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8777 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/import_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8519 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_get_achievement.py
--rw-rw-r--   0 root         (0) root         (0)    12577 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_list_achievements.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.882007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/anonymization/
--rw-rw-r--   0 root         (0) root         (0)      548 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/anonymization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6929 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/anonymization/admin_anonymize_user_ac_c61ab2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/
--rw-rw-r--   0 root         (0) root         (0)     1043 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10172 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achie_0b49fb.py
--rw-rw-r--   0 root         (0) root         (0)    12035 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achievements.py
--rw-rw-r--   0 root         (0) root         (0)    11927 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_user_contributions.py
--rw-rw-r--   0 root         (0) root         (0)     8297 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/claim_global_achievemen_1ea8df.py
--rw-rw-r--   0 root         (0) root         (0)    10097 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_global_achievement_b19e66.py
--rw-rw-r--   0 root         (0) root         (0)    11856 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_user_contributions.py
--rw-rw-r--   0 root         (0) root         (0)    12030 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/public_list_global_achi_9c838b.py
--rw-rw-r--   0 root         (0) root         (0)     7303 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/reset_global_achievement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/
--rw-rw-r--   0 root         (0) root         (0)      562 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9718 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/admin_list_tags.py
--rw-rw-r--   0 root         (0) root         (0)     9717 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/public_list_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/
--rw-rw-r--   0 root         (0) root         (0)      795 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12291 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_list_user_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8270 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_reset_achievement.py
--rw-rw-r--   0 root         (0) root         (0)     8289 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_unlock_achievement.py
--rw-rw-r--   0 root         (0) root         (0)    12292 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_list_user_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8286 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_unlock_achievement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     3574 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38615 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     4145 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_anonymization.py
--rw-rw-r--   0 root         (0) root         (0)    33694 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_global_achievements.py
--rw-rw-r--   0 root         (0) root         (0)     8223 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_tags.py
--rw-rw-r--   0 root         (0) root         (0)    21385 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_user_achievements.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1142 2024-02-27 05:34:34.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5115 2024-02-27 05:34:34.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 05:34:34.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-27 05:34:34.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 05:34:34.000000 accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-27 05:33:50.000000 accelbyte-py-sdk-service-achievement-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 05:34:34.886007 accelbyte-py-sdk-service-achievement-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.042318 accelbyte-py-sdk-service-achievement-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-03-13 06:09:30.042318 accelbyte-py-sdk-service-achievement-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      882 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.034318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.034318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.034318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/
+-rw-rw-r--   0 root         (0) root         (0)     3262 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/
+-rw-rw-r--   0 root         (0) root         (0)     2098 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4025 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_order_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)    13553 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_request.py
+-rw-rw-r--   0 root         (0) root         (0)    17066 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12919 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_update_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6423 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_additional_info.py
+-rw-rw-r--   0 root         (0) root         (0)     8164 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_contributor_response.py
+-rw-rw-r--   0 root         (0) root         (0)     9627 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_global_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4087 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_icon.py
+-rw-rw-r--   0 root         (0) root         (0)     5217 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5217 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_contributor_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5358 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_global_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4999 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_tag_response.py
+-rw-rw-r--   0 root         (0) root         (0)     6335 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5339 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_contribution_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4284 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)    16155 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_public_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5247 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_public_achievements_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_tag_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7404 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_user_achievement_response.py
+-rw-rw-r--   0 root         (0) root         (0)     8321 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_user_contribution_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4439 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/response_error.py
+-rw-rw-r--   0 root         (0) root         (0)     6541 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/service_import_config_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/
+-rw-rw-r--   0 root         (0) root         (0)      441 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/
+-rw-rw-r--   0 root         (0) root         (0)     1262 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8638 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_create_new_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     7455 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_delete_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     7587 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_get_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)    11809 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_list_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8767 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievemen_d288a7.py
+-rw-rw-r--   0 root         (0) root         (0)     8815 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     7444 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/export_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8777 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/import_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8519 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_get_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)    12577 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_list_achievements.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/anonymization/
+-rw-rw-r--   0 root         (0) root         (0)      548 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/anonymization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6929 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/anonymization/admin_anonymize_user_ac_c61ab2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/
+-rw-rw-r--   0 root         (0) root         (0)     1043 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10172 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achie_0b49fb.py
+-rw-rw-r--   0 root         (0) root         (0)    12035 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)    11927 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_user_contributions.py
+-rw-rw-r--   0 root         (0) root         (0)     8297 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/claim_global_achievemen_1ea8df.py
+-rw-rw-r--   0 root         (0) root         (0)    10097 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_global_achievement_b19e66.py
+-rw-rw-r--   0 root         (0) root         (0)    11856 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_user_contributions.py
+-rw-rw-r--   0 root         (0) root         (0)    12030 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/public_list_global_achi_9c838b.py
+-rw-rw-r--   0 root         (0) root         (0)     7303 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/reset_global_achievement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9718 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/admin_list_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     9717 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/public_list_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.038318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/
+-rw-rw-r--   0 root         (0) root         (0)      795 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12291 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_list_user_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8270 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_reset_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)     8289 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_unlock_achievement.py
+-rw-rw-r--   0 root         (0) root         (0)    12292 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_list_user_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8286 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_unlock_achievement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.042318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     3574 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38615 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     4145 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_anonymization.py
+-rw-rw-r--   0 root         (0) root         (0)    33694 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_global_achievements.py
+-rw-rw-r--   0 root         (0) root         (0)     8223 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_tags.py
+-rw-rw-r--   0 root         (0) root         (0)    21385 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_user_achievements.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 06:09:30.042318 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-03-13 06:09:30.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5115 2024-03-13 06:09:30.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 06:09:30.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-13 06:09:30.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-13 06:09:30.000000 accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-03-13 06:08:58.000000 accelbyte-py-sdk-service-achievement-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 06:09:30.042318 accelbyte-py-sdk-service-achievement-0.9.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/PKG-INFO` & `accelbyte-py-sdk-service-achievement-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-achievement
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Achievement Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Achievement Service
-* Version: 2.21.12
+* Version: 2.21.13
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/README.md` & `accelbyte-py-sdk-service-achievement-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Achievement Service
-* Version: 2.21.12
+* Version: 2.21.13
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: service-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 # achievements
 from .wrappers import admin_create_new_achievement
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: model-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .models_achievement_order_update_request import ModelsAchievementOrderUpdateRequest
 from .models_achievement_request import ModelsAchievementRequest
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_order_update_request.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_order_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_request.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_achievement_update_request.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_achievement_update_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_additional_info.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_additional_info.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_contributor_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_contributor_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_global_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_global_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_icon.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_icon.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_contributor_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_contributor_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_global_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_global_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_tag_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_tag_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_contribution_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_paginated_user_contribution_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_pagination.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_public_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_public_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_public_achievements_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_public_achievements_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_tag_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_tag_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_user_achievement_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_user_achievement_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/models_user_contribution_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/models_user_contribution_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/response_error.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/models/service_import_config_response.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/models/service_import_config_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_create_new_achievement import AdminCreateNewAchievement
 from .admin_delete_achievement import AdminDeleteAchievement
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_create_new_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_create_new_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_delete_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_delete_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_get_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_get_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_list_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_list_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievemen_d288a7.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievemen_d288a7.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/admin_update_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/export_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/export_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/import_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/import_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_get_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_get_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_list_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/achievements/public_list_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/anonymization/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/anonymization/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_anonymize_user_ac_c61ab2 import AdminAnonymizeUserAchievement
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/anonymization/admin_anonymize_user_ac_c61ab2.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/anonymization/admin_anonymize_user_ac_c61ab2.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_list_global_achie_0b49fb import AdminListGlobalAchievementContributors
 from .admin_list_global_achievements import AdminListGlobalAchievements
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achie_0b49fb.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achie_0b49fb.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_global_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_user_contributions.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/admin_list_user_contributions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/claim_global_achievemen_1ea8df.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/claim_global_achievemen_1ea8df.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_global_achievement_b19e66.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_global_achievement_b19e66.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_user_contributions.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/list_user_contributions.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/public_list_global_achi_9c838b.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/public_list_global_achi_9c838b.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/reset_global_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/global_achievements/reset_global_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_list_tags import AdminListTags
 from .public_list_tags import PublicListTags
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/admin_list_tags.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/admin_list_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/tags/public_list_tags.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/tags/public_list_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: operation-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from .admin_list_user_achievements import AdminListUserAchievements
 from .admin_reset_achievement import AdminResetAchievement
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_list_user_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_list_user_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_reset_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_reset_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_unlock_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/admin_unlock_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_list_user_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_list_user_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_unlock_achievement.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/operations/user_achievements/public_unlock_achievement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/__init__.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Code generated. DO NOT EDIT!
 
 # template file: wrapper-init.j2
 
 """Auto-generated package that contains models used by the AccelByte Gaming Services Achievement Service."""
 
-__version__ = "2.21.12"
+__version__ = "2.21.13"
 __author__ = "AccelByte"
 __email__ = "dev@accelbyte.net"
 
 # pylint: disable=line-too-long
 
 from ._achievements import admin_create_new_achievement
 from ._achievements import admin_create_new_achievement_async
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_anonymization.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_anonymization.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_global_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_global_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_tags.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_tags.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk/api/achievement/wrappers/_user_achievements.py` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk/api/achievement/wrappers/_user_achievements.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/PKG-INFO` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-achievement
-Version: 0.8.0
+Version: 0.9.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Achievement Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
 
 # AccelByte Modular Python SDK - Service Module
 
 This is a service module for the [AccelByte Modular Python SDK](https://github.com/AccelByte/accelbyte-python-modular-sdk) package.
 
 ```text
 AccelByte Gaming Services Achievement Service
-* Version: 2.21.12
+* Version: 2.21.13
 ```
 
 ## Setup
 
 This SDK requires Python 3.9 to be installed.
 
 ### Install with Pip
```

### Comparing `accelbyte-py-sdk-service-achievement-0.8.0/accelbyte_py_sdk_service_achievement.egg-info/SOURCES.txt` & `accelbyte-py-sdk-service-achievement-0.9.0/accelbyte_py_sdk_service_achievement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

