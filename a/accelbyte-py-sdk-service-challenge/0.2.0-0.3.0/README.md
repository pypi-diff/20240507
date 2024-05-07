# Comparing `tmp/accelbyte-py-sdk-service-challenge-0.2.0.tar.gz` & `tmp/accelbyte_py_sdk_service_challenge-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelbyte-py-sdk-service-challenge-0.2.0.tar", last modified: Tue Mar 26 05:40:24 2024, max compression
+gzip compressed data, was "accelbyte_py_sdk_service_challenge-0.3.0.tar", last modified: Tue May  7 06:26:10 2024, max compression
```

## Comparing `accelbyte-py-sdk-service-challenge-0.2.0.tar` & `accelbyte_py_sdk_service_challenge-0.3.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.086062 accelbyte-py-sdk-service-challenge-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-03-26 05:40:24.086062 accelbyte-py-sdk-service-challenge-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      876 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.078062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.078062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.078062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/
--rw-rw-r--   0 root         (0) root         (0)     2538 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/
--rw-rw-r--   0 root         (0) root         (0)     3600 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4474 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py
--rw-rw-r--   0 root         (0) root         (0)    13818 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py
--rw-rw-r--   0 root         (0) root         (0)     3930 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py
--rw-rw-r--   0 root         (0) root         (0)    11814 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py
--rw-rw-r--   0 root         (0) root         (0)     9703 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py
--rw-rw-r--   0 root         (0) root         (0)     4090 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py
--rw-rw-r--   0 root         (0) root         (0)     8159 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)    12214 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py
--rw-rw-r--   0 root         (0) root         (0)     5051 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py
--rw-rw-r--   0 root         (0) root         (0)     5037 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py
--rw-rw-r--   0 root         (0) root         (0)     4999 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py
--rw-rw-r--   0 root         (0) root         (0)     6987 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py
--rw-rw-r--   0 root         (0) root         (0)     5094 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py
--rw-rw-r--   0 root         (0) root         (0)     6282 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)     5814 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_reward.py
--rw-rw-r--   0 root         (0) root         (0)     8061 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py
--rw-rw-r--   0 root         (0) root         (0)     8900 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py
--rw-rw-r--   0 root         (0) root         (0)     5306 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py
--rw-rw-r--   0 root         (0) root         (0)     7227 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py
--rw-rw-r--   0 root         (0) root         (0)    10051 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py
--rw-rw-r--   0 root         (0) root         (0)     4882 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/models_period.py
--rw-rw-r--   0 root         (0) root         (0)    11555 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6530 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/response_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/
--rw-rw-r--   0 root         (0) root         (0)      437 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/
--rw-rw-r--   0 root         (0) root         (0)     1007 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9470 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     7627 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     7799 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     7573 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py
--rw-rw-r--   0 root         (0) root         (0)    10132 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py
--rw-rw-r--   0 root         (0) root         (0)     9302 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py
--rw-rw-r--   0 root         (0) root         (0)     7769 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py
--rw-rw-r--   0 root         (0) root         (0)     9284 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/
--rw-rw-r--   0 root         (0) root         (0)      651 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10068 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py
--rw-rw-r--   0 root         (0) root         (0)    10064 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/
--rw-rw-r--   0 root         (0) root         (0)      648 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7836 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py
--rw-rw-r--   0 root         (0) root         (0)     6357 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py
--rw-rw-r--   0 root         (0) root         (0)     8724 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/
--rw-rw-r--   0 root         (0) root         (0)      697 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9809 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py
--rw-rw-r--   0 root         (0) root         (0)     7808 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py
--rw-rw-r--   0 root         (0) root         (0)     8140 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py
--rw-rw-r--   0 root         (0) root         (0)    10054 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py
--rw-rw-r--   0 root         (0) root         (0)     8800 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.082062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/
--rw-rw-r--   0 root         (0) root         (0)      826 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10912 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py
--rw-rw-r--   0 root         (0) root         (0)     7872 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py
--rw-rw-r--   0 root         (0) root         (0)    10171 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.086062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/
--rw-rw-r--   0 root         (0) root         (0)     2948 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32517 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     8446 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py
--rw-rw-r--   0 root         (0) root         (0)    10668 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py
--rw-rw-r--   0 root         (0) root         (0)    19394 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py
--rw-rw-r--   0 root         (0) root         (0)    12111 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 05:40:24.086062 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-03-26 05:40:24.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4792 2024-03-26 05:40:24.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 05:40:24.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 05:40:24.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 05:40:24.000000 accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      363 2024-03-26 05:39:06.000000 accelbyte-py-sdk-service-challenge-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 05:40:24.086062 accelbyte-py-sdk-service-challenge-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.788635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/
+-rw-rw-r--   0 root         (0) root         (0)     2538 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/
+-rw-rw-r--   0 root         (0) root         (0)     3643 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4474 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py
+-rw-rw-r--   0 root         (0) root         (0)    14602 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py
+-rw-rw-r--   0 root         (0) root         (0)     3930 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py
+-rw-rw-r--   0 root         (0) root         (0)    12603 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     9703 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4090 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7676 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_meta.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py
+-rw-rw-r--   0 root         (0) root         (0)     9022 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)    12214 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5051 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py
+-rw-rw-r--   0 root         (0) root         (0)     5037 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py
+-rw-rw-r--   0 root         (0) root         (0)     4999 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py
+-rw-rw-r--   0 root         (0) root         (0)     6987 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py
+-rw-rw-r--   0 root         (0) root         (0)     5094 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py
+-rw-rw-r--   0 root         (0) root         (0)     8409 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)     5814 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     8061 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py
+-rw-rw-r--   0 root         (0) root         (0)     8956 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6179 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py
+-rw-rw-r--   0 root         (0) root         (0)     7227 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py
+-rw-rw-r--   0 root         (0) root         (0)    10051 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py
+-rw-rw-r--   0 root         (0) root         (0)     4882 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_period.py
+-rw-rw-r--   0 root         (0) root         (0)    12345 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6530 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/response_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/
+-rw-rw-r--   0 root         (0) root         (0)      437 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/
+-rw-rw-r--   0 root         (0) root         (0)     1007 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9908 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     7934 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     8127 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     7880 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)    10423 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py
+-rw-rw-r--   0 root         (0) root         (0)     9633 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py
+-rw-rw-r--   0 root         (0) root         (0)     8086 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     9591 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10360 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py
+-rw-rw-r--   0 root         (0) root         (0)    10394 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/
+-rw-rw-r--   0 root         (0) root         (0)      648 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8134 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     6681 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py
+-rw-rw-r--   0 root         (0) root         (0)    11538 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/
+-rw-rw-r--   0 root         (0) root         (0)      697 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10497 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py
+-rw-rw-r--   0 root         (0) root         (0)     8128 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py
+-rw-rw-r--   0 root         (0) root         (0)     8460 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py
+-rw-rw-r--   0 root         (0) root         (0)    10383 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py
+-rw-rw-r--   0 root         (0) root         (0)    10047 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/
+-rw-rw-r--   0 root         (0) root         (0)      826 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11215 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)     8164 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py
+-rw-rw-r--   0 root         (0) root         (0)    10457 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/
+-rw-rw-r--   0 root         (0) root         (0)     2948 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    32811 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     8446 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py
+-rw-rw-r--   0 root         (0) root         (0)    11292 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py
+-rw-rw-r--   0 root         (0) root         (0)    21624 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)    12063 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4849 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 06:26:10.000000 accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-07 06:24:47.000000 accelbyte_py_sdk_service_challenge-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 06:26:10.792635 accelbyte_py_sdk_service_challenge-0.3.0/setup.cfg
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/PKG-INFO` & `accelbyte_py_sdk_service_challenge-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-challenge
-Version: 0.2.0
+Version: 0.3.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Challenge Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/README.md` & `accelbyte_py_sdk_service_challenge-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     RotationEnum as ModelCreateChallengeRequestRotationEnum,
 )
 from .model_create_goal_request import ModelCreateGoalRequest
 from .model_evaluate_player_progression_request import (
     ModelEvaluatePlayerProgressionRequest,
 )
 from .model_get_goals_response import ModelGetGoalsResponse
+from .model_goal_meta import ModelGoalMeta
 from .model_goal_order import ModelGoalOrder
 from .model_goal_progression_response import ModelGoalProgressionResponse
 from .model_goal_progression_response import (
     StatusEnum as ModelGoalProgressionResponseStatusEnum,
 )
 from .model_goal_response import ModelGoalResponse
 from .model_goal_schedule import ModelGoalSchedule
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/iam_error_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_challenge_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
         status: (status) REQUIRED Union[str, StatusEnum]
 
         updated_at: (updatedAt) REQUIRED str
 
         end_after: (endAfter) OPTIONAL int
 
         end_date: (endDate) OPTIONAL str
+
+        repeat_after: (repeatAfter) OPTIONAL int
     """
 
     # region fields
 
     active_goals_per_rotation: int  # REQUIRED
     assignment_rule: Union[str, AssignmentRuleEnum]  # REQUIRED
     code: str  # REQUIRED
@@ -95,14 +97,15 @@
     name: str  # REQUIRED
     rotation: Union[str, RotationEnum]  # REQUIRED
     start_date: str  # REQUIRED
     status: Union[str, StatusEnum]  # REQUIRED
     updated_at: str  # REQUIRED
     end_after: int  # OPTIONAL
     end_date: str  # OPTIONAL
+    repeat_after: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_active_goals_per_rotation(self, value: int) -> ModelChallengeResponse:
         self.active_goals_per_rotation = value
@@ -156,14 +159,18 @@
         self.end_after = value
         return self
 
     def with_end_date(self, value: str) -> ModelChallengeResponse:
         self.end_date = value
         return self
 
+    def with_repeat_after(self, value: int) -> ModelChallengeResponse:
+        self.repeat_after = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "active_goals_per_rotation"):
@@ -214,14 +221,18 @@
             result["endAfter"] = int(self.end_after)
         elif include_empty:
             result["endAfter"] = 0
         if hasattr(self, "end_date"):
             result["endDate"] = str(self.end_date)
         elif include_empty:
             result["endDate"] = ""
+        if hasattr(self, "repeat_after"):
+            result["repeatAfter"] = int(self.repeat_after)
+        elif include_empty:
+            result["repeatAfter"] = 0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -236,14 +247,15 @@
         name: str,
         rotation: Union[str, RotationEnum],
         start_date: str,
         status: Union[str, StatusEnum],
         updated_at: str,
         end_after: Optional[int] = None,
         end_date: Optional[str] = None,
+        repeat_after: Optional[int] = None,
         **kwargs,
     ) -> ModelChallengeResponse:
         instance = cls()
         instance.active_goals_per_rotation = active_goals_per_rotation
         instance.assignment_rule = assignment_rule
         instance.code = code
         instance.created_at = created_at
@@ -254,14 +266,16 @@
         instance.start_date = start_date
         instance.status = status
         instance.updated_at = updated_at
         if end_after is not None:
             instance.end_after = end_after
         if end_date is not None:
             instance.end_date = end_date
+        if repeat_after is not None:
+            instance.repeat_after = repeat_after
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelChallengeResponse:
         instance = cls()
@@ -318,14 +332,18 @@
             instance.end_after = int(dict_["endAfter"])
         elif include_empty:
             instance.end_after = 0
         if "endDate" in dict_ and dict_["endDate"] is not None:
             instance.end_date = str(dict_["endDate"])
         elif include_empty:
             instance.end_date = ""
+        if "repeatAfter" in dict_ and dict_["repeatAfter"] is not None:
+            instance.repeat_after = int(dict_["repeatAfter"])
+        elif include_empty:
+            instance.repeat_after = 0
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelChallengeResponse]:
         return (
@@ -374,14 +392,15 @@
             "name": "name",
             "rotation": "rotation",
             "startDate": "start_date",
             "status": "status",
             "updatedAt": "updated_at",
             "endAfter": "end_after",
             "endDate": "end_date",
+            "repeatAfter": "repeat_after",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "activeGoalsPerRotation": True,
             "assignmentRule": True,
@@ -392,14 +411,15 @@
             "name": True,
             "rotation": True,
             "startDate": True,
             "status": True,
             "updatedAt": True,
             "endAfter": False,
             "endDate": False,
+            "repeatAfter": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "assignmentRule": ["FIXED", "RANDOMIZED", "UNSCHEDULED"],
             "goalsVisibility": ["PERIODONLY", "SHOWALL"],
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,28 +66,31 @@
         active_goals_per_rotation: (activeGoalsPerRotation) OPTIONAL int
 
         description: (description) OPTIONAL str
 
         end_after: (endAfter) OPTIONAL int
 
         end_date: (endDate) OPTIONAL str
+
+        repeat_after: (repeatAfter) OPTIONAL int
     """
 
     # region fields
 
     assignment_rule: Union[str, AssignmentRuleEnum]  # REQUIRED
     code: str  # REQUIRED
     goals_visibility: Union[str, GoalsVisibilityEnum]  # REQUIRED
     name: str  # REQUIRED
     rotation: Union[str, RotationEnum]  # REQUIRED
     start_date: str  # REQUIRED
     active_goals_per_rotation: int  # OPTIONAL
     description: str  # OPTIONAL
     end_after: int  # OPTIONAL
     end_date: str  # OPTIONAL
+    repeat_after: int  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_assignment_rule(
         self, value: Union[str, AssignmentRuleEnum]
@@ -131,14 +134,18 @@
         self.end_after = value
         return self
 
     def with_end_date(self, value: str) -> ModelCreateChallengeRequest:
         self.end_date = value
         return self
 
+    def with_repeat_after(self, value: int) -> ModelCreateChallengeRequest:
+        self.repeat_after = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "assignment_rule"):
@@ -177,14 +184,18 @@
             result["endAfter"] = int(self.end_after)
         elif include_empty:
             result["endAfter"] = 0
         if hasattr(self, "end_date"):
             result["endDate"] = str(self.end_date)
         elif include_empty:
             result["endDate"] = ""
+        if hasattr(self, "repeat_after"):
+            result["repeatAfter"] = int(self.repeat_after)
+        elif include_empty:
+            result["repeatAfter"] = 0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
@@ -196,14 +207,15 @@
         name: str,
         rotation: Union[str, RotationEnum],
         start_date: str,
         active_goals_per_rotation: Optional[int] = None,
         description: Optional[str] = None,
         end_after: Optional[int] = None,
         end_date: Optional[str] = None,
+        repeat_after: Optional[int] = None,
         **kwargs,
     ) -> ModelCreateChallengeRequest:
         instance = cls()
         instance.assignment_rule = assignment_rule
         instance.code = code
         instance.goals_visibility = goals_visibility
         instance.name = name
@@ -213,14 +225,16 @@
             instance.active_goals_per_rotation = active_goals_per_rotation
         if description is not None:
             instance.description = description
         if end_after is not None:
             instance.end_after = end_after
         if end_date is not None:
             instance.end_date = end_date
+        if repeat_after is not None:
+            instance.repeat_after = repeat_after
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelCreateChallengeRequest:
         instance = cls()
@@ -265,14 +279,18 @@
             instance.end_after = int(dict_["endAfter"])
         elif include_empty:
             instance.end_after = 0
         if "endDate" in dict_ and dict_["endDate"] is not None:
             instance.end_date = str(dict_["endDate"])
         elif include_empty:
             instance.end_date = ""
+        if "repeatAfter" in dict_ and dict_["repeatAfter"] is not None:
+            instance.repeat_after = int(dict_["repeatAfter"])
+        elif include_empty:
+            instance.repeat_after = 0
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelCreateChallengeRequest]:
         return (
@@ -318,14 +336,15 @@
             "name": "name",
             "rotation": "rotation",
             "startDate": "start_date",
             "activeGoalsPerRotation": "active_goals_per_rotation",
             "description": "description",
             "endAfter": "end_after",
             "endDate": "end_date",
+            "repeatAfter": "repeat_after",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "assignmentRule": True,
             "code": True,
@@ -333,14 +352,15 @@
             "name": True,
             "rotation": True,
             "startDate": True,
             "activeGoalsPerRotation": False,
             "description": False,
             "endAfter": False,
             "endDate": False,
+            "repeatAfter": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
             "assignmentRule": ["FIXED", "RANDOMIZED", "UNSCHEDULED"],
             "goalsVisibility": ["PERIODONLY", "SHOWALL"],
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_order.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,56 +24,65 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 from accelbyte_py_sdk.core import StrEnum
 
+from ..models.model_goal_meta import ModelGoalMeta
 from ..models.model_requirement_progression_response import (
     ModelRequirementProgressionResponse,
 )
 
 
 class StatusEnum(StrEnum):
     ACTIVE = "ACTIVE"
     COMPLETED = "COMPLETED"
+    NOT_STARTED = "NOT_STARTED"
     RETIRED = "RETIRED"
 
 
 class ModelGoalProgressionResponse(Model):
     """Model goal progression response (model.GoalProgressionResponse)
 
     Properties:
         challenge_code: (challengeCode) REQUIRED str
 
+        goal: (goal) REQUIRED ModelGoalMeta
+
         goal_code: (goalCode) REQUIRED str
 
         goal_progression_id: (goalProgressionId) REQUIRED str
 
         requirement_progressions: (requirementProgressions) REQUIRED List[ModelRequirementProgressionResponse]
 
         status: (status) REQUIRED Union[str, StatusEnum]
     """
 
     # region fields
 
     challenge_code: str  # REQUIRED
+    goal: ModelGoalMeta  # REQUIRED
     goal_code: str  # REQUIRED
     goal_progression_id: str  # REQUIRED
     requirement_progressions: List[ModelRequirementProgressionResponse]  # REQUIRED
     status: Union[str, StatusEnum]  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_challenge_code(self, value: str) -> ModelGoalProgressionResponse:
         self.challenge_code = value
         return self
 
+    def with_goal(self, value: ModelGoalMeta) -> ModelGoalProgressionResponse:
+        self.goal = value
+        return self
+
     def with_goal_code(self, value: str) -> ModelGoalProgressionResponse:
         self.goal_code = value
         return self
 
     def with_goal_progression_id(self, value: str) -> ModelGoalProgressionResponse:
         self.goal_progression_id = value
         return self
@@ -96,14 +105,18 @@
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "challenge_code"):
             result["challengeCode"] = str(self.challenge_code)
         elif include_empty:
             result["challengeCode"] = ""
+        if hasattr(self, "goal"):
+            result["goal"] = self.goal.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["goal"] = ModelGoalMeta()
         if hasattr(self, "goal_code"):
             result["goalCode"] = str(self.goal_code)
         elif include_empty:
             result["goalCode"] = ""
         if hasattr(self, "goal_progression_id"):
             result["goalProgressionId"] = str(self.goal_progression_id)
         elif include_empty:
@@ -125,22 +138,24 @@
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         challenge_code: str,
+        goal: ModelGoalMeta,
         goal_code: str,
         goal_progression_id: str,
         requirement_progressions: List[ModelRequirementProgressionResponse],
         status: Union[str, StatusEnum],
         **kwargs,
     ) -> ModelGoalProgressionResponse:
         instance = cls()
         instance.challenge_code = challenge_code
+        instance.goal = goal
         instance.goal_code = goal_code
         instance.goal_progression_id = goal_progression_id
         instance.requirement_progressions = requirement_progressions
         instance.status = status
         return instance
 
     @classmethod
@@ -150,14 +165,20 @@
         instance = cls()
         if not dict_:
             return instance
         if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
             instance.challenge_code = str(dict_["challengeCode"])
         elif include_empty:
             instance.challenge_code = ""
+        if "goal" in dict_ and dict_["goal"] is not None:
+            instance.goal = ModelGoalMeta.create_from_dict(
+                dict_["goal"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.goal = ModelGoalMeta()
         if "goalCode" in dict_ and dict_["goalCode"] is not None:
             instance.goal_code = str(dict_["goalCode"])
         elif include_empty:
             instance.goal_code = ""
         if "goalProgressionId" in dict_ and dict_["goalProgressionId"] is not None:
             instance.goal_progression_id = str(dict_["goalProgressionId"])
         elif include_empty:
@@ -218,30 +239,32 @@
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "challengeCode": "challenge_code",
+            "goal": "goal",
             "goalCode": "goal_code",
             "goalProgressionId": "goal_progression_id",
             "requirementProgressions": "requirement_progressions",
             "status": "status",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "challengeCode": True,
+            "goal": True,
             "goalCode": True,
             "goalProgressionId": True,
             "requirementProgressions": True,
             "status": True,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
-            "status": ["ACTIVE", "COMPLETED", "RETIRED"],
+            "status": ["ACTIVE", "COMPLETED", "NOT_STARTED", "RETIRED"],
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_pagination.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_predicate.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_requirement_progression_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,119 +28,169 @@
 from accelbyte_py_sdk.core import Model
 
 
 class ModelRequirementProgressionResponse(Model):
     """Model requirement progression response (model.RequirementProgressionResponse)
 
     Properties:
+        current_value: (currentValue) REQUIRED float
+
         id_: (id) REQUIRED str
 
+        matcher: (matcher) REQUIRED str
+
+        parameter_name: (parameterName) REQUIRED str
+
+        parameter_type: (parameterType) REQUIRED str
+
         target_value: (targetValue) REQUIRED float
 
         completed_at: (completedAt) OPTIONAL str
-
-        currrent_value: (currrentValue) OPTIONAL float
     """
 
     # region fields
 
+    current_value: float  # REQUIRED
     id_: str  # REQUIRED
+    matcher: str  # REQUIRED
+    parameter_name: str  # REQUIRED
+    parameter_type: str  # REQUIRED
     target_value: float  # REQUIRED
     completed_at: str  # OPTIONAL
-    currrent_value: float  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
+    def with_current_value(self, value: float) -> ModelRequirementProgressionResponse:
+        self.current_value = value
+        return self
+
     def with_id(self, value: str) -> ModelRequirementProgressionResponse:
         self.id_ = value
         return self
 
+    def with_matcher(self, value: str) -> ModelRequirementProgressionResponse:
+        self.matcher = value
+        return self
+
+    def with_parameter_name(self, value: str) -> ModelRequirementProgressionResponse:
+        self.parameter_name = value
+        return self
+
+    def with_parameter_type(self, value: str) -> ModelRequirementProgressionResponse:
+        self.parameter_type = value
+        return self
+
     def with_target_value(self, value: float) -> ModelRequirementProgressionResponse:
         self.target_value = value
         return self
 
     def with_completed_at(self, value: str) -> ModelRequirementProgressionResponse:
         self.completed_at = value
         return self
 
-    def with_currrent_value(self, value: float) -> ModelRequirementProgressionResponse:
-        self.currrent_value = value
-        return self
-
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
+        if hasattr(self, "current_value"):
+            result["currentValue"] = float(self.current_value)
+        elif include_empty:
+            result["currentValue"] = 0.0
         if hasattr(self, "id_"):
             result["id"] = str(self.id_)
         elif include_empty:
             result["id"] = ""
+        if hasattr(self, "matcher"):
+            result["matcher"] = str(self.matcher)
+        elif include_empty:
+            result["matcher"] = ""
+        if hasattr(self, "parameter_name"):
+            result["parameterName"] = str(self.parameter_name)
+        elif include_empty:
+            result["parameterName"] = ""
+        if hasattr(self, "parameter_type"):
+            result["parameterType"] = str(self.parameter_type)
+        elif include_empty:
+            result["parameterType"] = ""
         if hasattr(self, "target_value"):
             result["targetValue"] = float(self.target_value)
         elif include_empty:
             result["targetValue"] = 0.0
         if hasattr(self, "completed_at"):
             result["completedAt"] = str(self.completed_at)
         elif include_empty:
             result["completedAt"] = ""
-        if hasattr(self, "currrent_value"):
-            result["currrentValue"] = float(self.currrent_value)
-        elif include_empty:
-            result["currrentValue"] = 0.0
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
+        current_value: float,
         id_: str,
+        matcher: str,
+        parameter_name: str,
+        parameter_type: str,
         target_value: float,
         completed_at: Optional[str] = None,
-        currrent_value: Optional[float] = None,
         **kwargs,
     ) -> ModelRequirementProgressionResponse:
         instance = cls()
+        instance.current_value = current_value
         instance.id_ = id_
+        instance.matcher = matcher
+        instance.parameter_name = parameter_name
+        instance.parameter_type = parameter_type
         instance.target_value = target_value
         if completed_at is not None:
             instance.completed_at = completed_at
-        if currrent_value is not None:
-            instance.currrent_value = currrent_value
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelRequirementProgressionResponse:
         instance = cls()
         if not dict_:
             return instance
+        if "currentValue" in dict_ and dict_["currentValue"] is not None:
+            instance.current_value = float(dict_["currentValue"])
+        elif include_empty:
+            instance.current_value = 0.0
         if "id" in dict_ and dict_["id"] is not None:
             instance.id_ = str(dict_["id"])
         elif include_empty:
             instance.id_ = ""
+        if "matcher" in dict_ and dict_["matcher"] is not None:
+            instance.matcher = str(dict_["matcher"])
+        elif include_empty:
+            instance.matcher = ""
+        if "parameterName" in dict_ and dict_["parameterName"] is not None:
+            instance.parameter_name = str(dict_["parameterName"])
+        elif include_empty:
+            instance.parameter_name = ""
+        if "parameterType" in dict_ and dict_["parameterType"] is not None:
+            instance.parameter_type = str(dict_["parameterType"])
+        elif include_empty:
+            instance.parameter_type = ""
         if "targetValue" in dict_ and dict_["targetValue"] is not None:
             instance.target_value = float(dict_["targetValue"])
         elif include_empty:
             instance.target_value = 0.0
         if "completedAt" in dict_ and dict_["completedAt"] is not None:
             instance.completed_at = str(dict_["completedAt"])
         elif include_empty:
             instance.completed_at = ""
-        if "currrentValue" in dict_ and dict_["currrentValue"] is not None:
-            instance.currrent_value = float(dict_["currrentValue"])
-        elif include_empty:
-            instance.currrent_value = 0.0
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelRequirementProgressionResponse]:
         return (
@@ -176,23 +226,29 @@
                 raise ValueError()
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
+            "currentValue": "current_value",
             "id": "id_",
+            "matcher": "matcher",
+            "parameterName": "parameter_name",
+            "parameterType": "parameter_type",
             "targetValue": "target_value",
             "completedAt": "completed_at",
-            "currrentValue": "currrent_value",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
+            "currentValue": True,
             "id": True,
+            "matcher": True,
+            "parameterName": True,
+            "parameterType": True,
             "targetValue": True,
             "completedAt": False,
-            "currrentValue": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_reward.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_schedule.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_update_goal_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,49 +34,45 @@
 
 class ModelUpdateGoalRequest(Model):
     """Model update goal request (model.UpdateGoalRequest)
 
     Properties:
         description: (description) REQUIRED str
 
-        is_active: (isActive) REQUIRED bool
-
         name: (name) REQUIRED str
 
         requirement_groups: (requirementGroups) REQUIRED List[ModelRequirement]
 
         rewards: (rewards) REQUIRED List[ModelReward]
 
         tags: (tags) REQUIRED List[str]
 
+        is_active: (isActive) OPTIONAL bool
+
         schedule: (schedule) OPTIONAL ModelGoalSchedule
     """
 
     # region fields
 
     description: str  # REQUIRED
-    is_active: bool  # REQUIRED
     name: str  # REQUIRED
     requirement_groups: List[ModelRequirement]  # REQUIRED
     rewards: List[ModelReward]  # REQUIRED
     tags: List[str]  # REQUIRED
+    is_active: bool  # OPTIONAL
     schedule: ModelGoalSchedule  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
     def with_description(self, value: str) -> ModelUpdateGoalRequest:
         self.description = value
         return self
 
-    def with_is_active(self, value: bool) -> ModelUpdateGoalRequest:
-        self.is_active = value
-        return self
-
     def with_name(self, value: str) -> ModelUpdateGoalRequest:
         self.name = value
         return self
 
     def with_requirement_groups(
         self, value: List[ModelRequirement]
     ) -> ModelUpdateGoalRequest:
@@ -87,32 +83,32 @@
         self.rewards = value
         return self
 
     def with_tags(self, value: List[str]) -> ModelUpdateGoalRequest:
         self.tags = value
         return self
 
+    def with_is_active(self, value: bool) -> ModelUpdateGoalRequest:
+        self.is_active = value
+        return self
+
     def with_schedule(self, value: ModelGoalSchedule) -> ModelUpdateGoalRequest:
         self.schedule = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "description"):
             result["description"] = str(self.description)
         elif include_empty:
             result["description"] = ""
-        if hasattr(self, "is_active"):
-            result["isActive"] = bool(self.is_active)
-        elif include_empty:
-            result["isActive"] = False
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
         if hasattr(self, "requirement_groups"):
             result["requirementGroups"] = [
                 i0.to_dict(include_empty=include_empty)
@@ -126,43 +122,48 @@
             ]
         elif include_empty:
             result["rewards"] = []
         if hasattr(self, "tags"):
             result["tags"] = [str(i0) for i0 in self.tags]
         elif include_empty:
             result["tags"] = []
+        if hasattr(self, "is_active"):
+            result["isActive"] = bool(self.is_active)
+        elif include_empty:
+            result["isActive"] = False
         if hasattr(self, "schedule"):
             result["schedule"] = self.schedule.to_dict(include_empty=include_empty)
         elif include_empty:
             result["schedule"] = ModelGoalSchedule()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         description: str,
-        is_active: bool,
         name: str,
         requirement_groups: List[ModelRequirement],
         rewards: List[ModelReward],
         tags: List[str],
+        is_active: Optional[bool] = None,
         schedule: Optional[ModelGoalSchedule] = None,
         **kwargs,
     ) -> ModelUpdateGoalRequest:
         instance = cls()
         instance.description = description
-        instance.is_active = is_active
         instance.name = name
         instance.requirement_groups = requirement_groups
         instance.rewards = rewards
         instance.tags = tags
+        if is_active is not None:
+            instance.is_active = is_active
         if schedule is not None:
             instance.schedule = schedule
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
@@ -170,18 +171,14 @@
         instance = cls()
         if not dict_:
             return instance
         if "description" in dict_ and dict_["description"] is not None:
             instance.description = str(dict_["description"])
         elif include_empty:
             instance.description = ""
-        if "isActive" in dict_ and dict_["isActive"] is not None:
-            instance.is_active = bool(dict_["isActive"])
-        elif include_empty:
-            instance.is_active = False
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
         if "requirementGroups" in dict_ and dict_["requirementGroups"] is not None:
             instance.requirement_groups = [
                 ModelRequirement.create_from_dict(i0, include_empty=include_empty)
@@ -196,14 +193,18 @@
             ]
         elif include_empty:
             instance.rewards = []
         if "tags" in dict_ and dict_["tags"] is not None:
             instance.tags = [str(i0) for i0 in dict_["tags"]]
         elif include_empty:
             instance.tags = []
+        if "isActive" in dict_ and dict_["isActive"] is not None:
+            instance.is_active = bool(dict_["isActive"])
+        elif include_empty:
+            instance.is_active = False
         if "schedule" in dict_ and dict_["schedule"] is not None:
             instance.schedule = ModelGoalSchedule.create_from_dict(
                 dict_["schedule"], include_empty=include_empty
             )
         elif include_empty:
             instance.schedule = ModelGoalSchedule()
         return instance
@@ -246,28 +247,28 @@
         else:
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "description": "description",
-            "isActive": "is_active",
             "name": "name",
             "requirementGroups": "requirement_groups",
             "rewards": "rewards",
             "tags": "tags",
+            "isActive": "is_active",
             "schedule": "schedule",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "description": True,
-            "isActive": True,
             "name": True,
             "requirementGroups": True,
             "rewards": True,
             "tags": True,
+            "isActive": False,
             "schedule": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,32 +24,36 @@
 
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Model
 
 from ..models.model_goal_progression_response import ModelGoalProgressionResponse
+from ..models.model_pagination import ModelPagination
 from ..models.model_user_progression_response_meta import (
     ModelUserProgressionResponseMeta,
 )
 
 
 class ModelUserProgressionResponse(Model):
     """Model user progression response (model.UserProgressionResponse)
 
     Properties:
         data: (data) REQUIRED List[ModelGoalProgressionResponse]
 
         meta: (meta) REQUIRED ModelUserProgressionResponseMeta
+
+        paging: (paging) REQUIRED ModelPagination
     """
 
     # region fields
 
     data: List[ModelGoalProgressionResponse]  # REQUIRED
     meta: ModelUserProgressionResponseMeta  # REQUIRED
+    paging: ModelPagination  # REQUIRED
 
     # endregion fields
 
     # region with_x methods
 
     def with_data(
         self, value: List[ModelGoalProgressionResponse]
@@ -59,14 +63,18 @@
 
     def with_meta(
         self, value: ModelUserProgressionResponseMeta
     ) -> ModelUserProgressionResponse:
         self.meta = value
         return self
 
+    def with_paging(self, value: ModelPagination) -> ModelUserProgressionResponse:
+        self.paging = value
+        return self
+
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "data"):
@@ -75,30 +83,36 @@
             ]
         elif include_empty:
             result["data"] = []
         if hasattr(self, "meta"):
             result["meta"] = self.meta.to_dict(include_empty=include_empty)
         elif include_empty:
             result["meta"] = ModelUserProgressionResponseMeta()
+        if hasattr(self, "paging"):
+            result["paging"] = self.paging.to_dict(include_empty=include_empty)
+        elif include_empty:
+            result["paging"] = ModelPagination()
         return result
 
     # endregion to methods
 
     # region static methods
 
     @classmethod
     def create(
         cls,
         data: List[ModelGoalProgressionResponse],
         meta: ModelUserProgressionResponseMeta,
+        paging: ModelPagination,
         **kwargs,
     ) -> ModelUserProgressionResponse:
         instance = cls()
         instance.data = data
         instance.meta = meta
+        instance.paging = paging
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> ModelUserProgressionResponse:
         instance = cls()
@@ -115,14 +129,20 @@
             instance.data = []
         if "meta" in dict_ and dict_["meta"] is not None:
             instance.meta = ModelUserProgressionResponseMeta.create_from_dict(
                 dict_["meta"], include_empty=include_empty
             )
         elif include_empty:
             instance.meta = ModelUserProgressionResponseMeta()
+        if "paging" in dict_ and dict_["paging"] is not None:
+            instance.paging = ModelPagination.create_from_dict(
+                dict_["paging"], include_empty=include_empty
+            )
+        elif include_empty:
+            instance.paging = ModelPagination()
         return instance
 
     @classmethod
     def create_many_from_dict(
         cls, dict_: dict, include_empty: bool = False
     ) -> Dict[str, ModelUserProgressionResponse]:
         return (
@@ -160,17 +180,19 @@
             return cls.create_from_dict(any_, include_empty=include_empty)
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "data": "data",
             "meta": "meta",
+            "paging": "paging",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "data": True,
             "meta": True,
+            "paging": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_progression_response_meta.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/model_user_reward.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/models_period.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_period.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/models_update_challenge_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,28 +61,31 @@
 
         end_date: (endDate) OPTIONAL str
 
         goals_visibility: (goalsVisibility) OPTIONAL Union[str, GoalsVisibilityEnum]
 
         name: (name) OPTIONAL str
 
+        repeat_after: (repeatAfter) OPTIONAL int
+
         rotation: (rotation) OPTIONAL Union[str, RotationEnum]
 
         start_date: (startDate) OPTIONAL str
     """
 
     # region fields
 
     active_goals_per_rotation: int  # OPTIONAL
     assignment_rule: Union[str, AssignmentRuleEnum]  # OPTIONAL
     description: str  # OPTIONAL
     end_after: int  # OPTIONAL
     end_date: str  # OPTIONAL
     goals_visibility: Union[str, GoalsVisibilityEnum]  # OPTIONAL
     name: str  # OPTIONAL
+    repeat_after: int  # OPTIONAL
     rotation: Union[str, RotationEnum]  # OPTIONAL
     start_date: str  # OPTIONAL
 
     # endregion fields
 
     # region with_x methods
 
@@ -116,14 +119,18 @@
         self.goals_visibility = value
         return self
 
     def with_name(self, value: str) -> ModelsUpdateChallengeRequest:
         self.name = value
         return self
 
+    def with_repeat_after(self, value: int) -> ModelsUpdateChallengeRequest:
+        self.repeat_after = value
+        return self
+
     def with_rotation(
         self, value: Union[str, RotationEnum]
     ) -> ModelsUpdateChallengeRequest:
         self.rotation = value
         return self
 
     def with_start_date(self, value: str) -> ModelsUpdateChallengeRequest:
@@ -160,14 +167,18 @@
             result["goalsVisibility"] = str(self.goals_visibility)
         elif include_empty:
             result["goalsVisibility"] = Union[str, GoalsVisibilityEnum]()
         if hasattr(self, "name"):
             result["name"] = str(self.name)
         elif include_empty:
             result["name"] = ""
+        if hasattr(self, "repeat_after"):
+            result["repeatAfter"] = int(self.repeat_after)
+        elif include_empty:
+            result["repeatAfter"] = 0
         if hasattr(self, "rotation"):
             result["rotation"] = str(self.rotation)
         elif include_empty:
             result["rotation"] = Union[str, RotationEnum]()
         if hasattr(self, "start_date"):
             result["startDate"] = str(self.start_date)
         elif include_empty:
@@ -184,14 +195,15 @@
         active_goals_per_rotation: Optional[int] = None,
         assignment_rule: Optional[Union[str, AssignmentRuleEnum]] = None,
         description: Optional[str] = None,
         end_after: Optional[int] = None,
         end_date: Optional[str] = None,
         goals_visibility: Optional[Union[str, GoalsVisibilityEnum]] = None,
         name: Optional[str] = None,
+        repeat_after: Optional[int] = None,
         rotation: Optional[Union[str, RotationEnum]] = None,
         start_date: Optional[str] = None,
         **kwargs,
     ) -> ModelsUpdateChallengeRequest:
         instance = cls()
         if active_goals_per_rotation is not None:
             instance.active_goals_per_rotation = active_goals_per_rotation
@@ -203,14 +215,16 @@
             instance.end_after = end_after
         if end_date is not None:
             instance.end_date = end_date
         if goals_visibility is not None:
             instance.goals_visibility = goals_visibility
         if name is not None:
             instance.name = name
+        if repeat_after is not None:
+            instance.repeat_after = repeat_after
         if rotation is not None:
             instance.rotation = rotation
         if start_date is not None:
             instance.start_date = start_date
         return instance
 
     @classmethod
@@ -247,14 +261,18 @@
             instance.goals_visibility = str(dict_["goalsVisibility"])
         elif include_empty:
             instance.goals_visibility = Union[str, GoalsVisibilityEnum]()
         if "name" in dict_ and dict_["name"] is not None:
             instance.name = str(dict_["name"])
         elif include_empty:
             instance.name = ""
+        if "repeatAfter" in dict_ and dict_["repeatAfter"] is not None:
+            instance.repeat_after = int(dict_["repeatAfter"])
+        elif include_empty:
+            instance.repeat_after = 0
         if "rotation" in dict_ and dict_["rotation"] is not None:
             instance.rotation = str(dict_["rotation"])
         elif include_empty:
             instance.rotation = Union[str, RotationEnum]()
         if "startDate" in dict_ and dict_["startDate"] is not None:
             instance.start_date = str(dict_["startDate"])
         elif include_empty:
@@ -305,28 +323,30 @@
             "activeGoalsPerRotation": "active_goals_per_rotation",
             "assignmentRule": "assignment_rule",
             "description": "description",
             "endAfter": "end_after",
             "endDate": "end_date",
             "goalsVisibility": "goals_visibility",
             "name": "name",
+            "repeatAfter": "repeat_after",
             "rotation": "rotation",
             "startDate": "start_date",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "activeGoalsPerRotation": False,
             "assignmentRule": False,
             "description": False,
             "endAfter": False,
             "endDate": False,
             "goalsVisibility": False,
             "name": False,
+            "repeatAfter": False,
             "rotation": False,
             "startDate": False,
         }
 
     @staticmethod
     def get_enum_map() -> Dict[str, List[Any]]:
         return {
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/models/response_error.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/models/response_error.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_create_challenge.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
       * code: only lowercase letters, numbers, and the separator - are allowed; must start and end with letter
       * name: name of the challenge
       * description: text describing about the challenge (optional)
       * startDate: timestamp of when the challenge is started
       * endDate: timestamp of when the challenge is ended (optional)
       * endAfter: describe number of period challenge will be retired after (optional)
     To configure challenge that never end, leave the endDate and endAfter field null/empty.
+      * repeatAfter: describe number of period challenge's goals will be repeated after. Leave it empty if you don't want to repeat the challenge.
       * rotation: describe how long goals in a challenge will be available for players to progress before rotated with another goals. (DAILY|WEEKLY|MONTHLY|NONE)
       * activeGoalsPerRotation: number of goals per rotation (currently only applicable for RANDOMIZE assignment)
       * assignmentRule: describe how the goals will be assigned and scheduled to users. (FIXED|RANDOMIZED|UNSCHEDULED)
       * goalsVisibility: describe whether users can see all goals under challenge, or only active goal in one rotation period only. (SHOWALL|PERIODONLY)
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
@@ -89,32 +90,44 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     body: ModelCreateChallengeRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteChallenge(Operation):
-    """Delete a Challenge (adminDeleteChallenge)
+class AdminDeleteTiedChallenge(Operation):
+    """Delete Tied Challenge (adminDeleteTiedChallenge)
 
     * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
+        * This endpoint will delete the combination of related data: CHALLENGES, GOALS, SCHEDULES, PLAYER PROGRESSIONS
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}
+        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/tied
 
         method: DELETE
 
         tags: ["Challenge Configuration"]
 
         consumes: []
 
@@ -69,33 +70,49 @@
         404: Not Found - ResponseError (20029: not found)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
-    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _url: str = (
+        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/tied"
+    )
+    _path: str = (
+        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/tied"
+    )
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
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
 
@@ -136,19 +153,19 @@
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_challenge_code(self, value: str) -> AdminDeleteChallenge:
+    def with_challenge_code(self, value: str) -> AdminDeleteTiedChallenge:
         self.challenge_code = value
         return self
 
-    def with_namespace(self, value: str) -> AdminDeleteChallenge:
+    def with_namespace(self, value: str) -> AdminDeleteTiedChallenge:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
@@ -219,26 +236,26 @@
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
         cls, challenge_code: str, namespace: str, **kwargs
-    ) -> AdminDeleteChallenge:
+    ) -> AdminDeleteTiedChallenge:
         instance = cls()
         instance.challenge_code = challenge_code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteChallenge:
+    ) -> AdminDeleteTiedChallenge:
         instance = cls()
         if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
             instance.challenge_code = str(dict_["challengeCode"])
         elif include_empty:
             instance.challenge_code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_tied_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,77 +28,85 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteTiedChallenge(Operation):
-    """Delete Tied Challenge (adminDeleteTiedChallenge)
+class AdminDeleteGoal(Operation):
+    """Delete Goal (adminDeleteGoal)
 
     * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
-        * This endpoint will delete the combination of related data: CHALLENGES, GOALS, SCHEDULES, PLAYER PROGRESSIONS
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/tied
+        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
 
         method: DELETE
 
-        tags: ["Challenge Configuration"]
+        tags: ["Goal Configuration"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         challenge_code: (challengeCode) REQUIRED str in path
 
+        code: (code) REQUIRED str in path
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         204: No Content - (No Content)
 
         400: Bad Request - ResponseError (20018: bad request: {{message}})
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
-
-        403: Forbidden - ResponseError (20013: insufficient permission)
-
         404: Not Found - ResponseError (20029: not found)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
-    _url: str = (
-        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/tied"
-    )
+    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
+    code: str  # REQUIRED in [path]
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
 
@@ -127,44 +135,54 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "challenge_code"):
             result["challengeCode"] = self.challenge_code
+        if hasattr(self, "code"):
+            result["code"] = self.code
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_challenge_code(self, value: str) -> AdminDeleteTiedChallenge:
+    def with_challenge_code(self, value: str) -> AdminDeleteGoal:
         self.challenge_code = value
         return self
 
-    def with_namespace(self, value: str) -> AdminDeleteTiedChallenge:
+    def with_code(self, value: str) -> AdminDeleteGoal:
+        self.code = value
+        return self
+
+    def with_namespace(self, value: str) -> AdminDeleteGoal:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "challenge_code") and self.challenge_code:
             result["challengeCode"] = str(self.challenge_code)
         elif include_empty:
             result["challengeCode"] = ""
+        if hasattr(self, "code") and self.code:
+            result["code"] = str(self.code)
+        elif include_empty:
+            result["code"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
@@ -177,18 +195,14 @@
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
         204: No Content - (No Content)
 
         400: Bad Request - ResponseError (20018: bad request: {{message}})
 
-        401: Unauthorized - ResponseError (20001: unauthorized access)
-
-        403: Forbidden - ResponseError (20013: insufficient permission)
-
         404: Not Found - ResponseError (20029: not found)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
@@ -202,18 +216,14 @@
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 204:
             return None, None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
-        if code == 401:
-            return None, ResponseError.create_from_dict(content)
-        if code == 403:
-            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
@@ -221,46 +231,53 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, challenge_code: str, namespace: str, **kwargs
-    ) -> AdminDeleteTiedChallenge:
+        cls, challenge_code: str, code: str, namespace: str, **kwargs
+    ) -> AdminDeleteGoal:
         instance = cls()
         instance.challenge_code = challenge_code
+        instance.code = code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteTiedChallenge:
+    ) -> AdminDeleteGoal:
         instance = cls()
         if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
             instance.challenge_code = str(dict_["challengeCode"])
         elif include_empty:
             instance.challenge_code = ""
+        if "code" in dict_ and dict_["code"] is not None:
+            instance.code = str(dict_["code"])
+        elif include_empty:
+            instance.code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "challengeCode": "challenge_code",
+            "code": "code",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "challengeCode": True,
+            "code": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_challenges.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,24 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
     status: Union[str, StatusEnum]  # OPTIONAL in [query]
 
     # endregion fields
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_get_periods.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,34 +76,48 @@
     """
 
     # region fields
 
     _url: str = (
         "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/periods"
     )
+    _path: str = (
+        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/periods"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_randomize_challenge.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,32 +71,44 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/randomize"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/randomize"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_update_challenge.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,33 +85,45 @@
 
         500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _base_path: str = ""
     _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     body: ModelsUpdateChallengeRequest  # REQUIRED in [body]
     challenge_code: str  # REQUIRED in [path]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/get_challenges.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,24 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/public/namespaces/{namespace}/challenges"
+    _path: str = "/challenge/v1/public/namespaces/{namespace}/challenges"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
     status: Union[str, StatusEnum]  # OPTIONAL in [query]
 
     # endregion fields
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_list/public_get_scheduled_goals.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,20 +76,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals"
     )
+    _path: str = (
+        "/challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     tags: List[str]  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/admin_evaluate_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,32 +70,44 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/progress/evaluate"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/progress/evaluate"
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     body: ModelEvaluatePlayerProgressionRequest  # REQUIRED in [body]
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/evaluate_my_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,31 +65,45 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate"
+    _path: str = (
+        "/challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/challenge_progression/public_get_user_progression.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,81 +26,91 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import IamErrorResponse
-from ...models import ModelUserProgressionResponse
+from ...models import ModelGoalResponse
 from ...models import ResponseError
 
 
-class PublicGetUserProgression(Operation):
-    """List User's Progressions (publicGetUserProgression)
+class AdminGetGoal(Operation):
+    """Get Goal (adminGetGoal)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [READ]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE [READ]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}
+        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
 
         method: GET
 
-        tags: ["Challenge Progression"]
+        tags: ["Goal Configuration"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         challenge_code: (challengeCode) REQUIRED str in path
 
-        namespace: (namespace) REQUIRED str in path
+        code: (code) REQUIRED str in path
 
-        goal_code: (goalCode) OPTIONAL str in query
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelUserProgressionResponse (OK)
+        200: OK - ModelGoalResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - IamErrorResponse (20029: not found)
+        404: Not Found - ResponseError (Not Found)
 
-        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+        500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = (
-        "/challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}"
-    )
+    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
+    code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
-    goal_code: str  # OPTIONAL in [query]
 
     # endregion fields
 
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
 
@@ -123,93 +133,88 @@
     # endregion get methods
 
     # region get_x_params methods
 
     def get_all_params(self) -> dict:
         return {
             "path": self.get_path_params(),
-            "query": self.get_query_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "challenge_code"):
             result["challengeCode"] = self.challenge_code
+        if hasattr(self, "code"):
+            result["code"] = self.code
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
-    def get_query_params(self) -> dict:
-        result = {}
-        if hasattr(self, "goal_code"):
-            result["goalCode"] = self.goal_code
-        return result
-
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_challenge_code(self, value: str) -> PublicGetUserProgression:
+    def with_challenge_code(self, value: str) -> AdminGetGoal:
         self.challenge_code = value
         return self
 
-    def with_namespace(self, value: str) -> PublicGetUserProgression:
-        self.namespace = value
+    def with_code(self, value: str) -> AdminGetGoal:
+        self.code = value
         return self
 
-    def with_goal_code(self, value: str) -> PublicGetUserProgression:
-        self.goal_code = value
+    def with_namespace(self, value: str) -> AdminGetGoal:
+        self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "challenge_code") and self.challenge_code:
             result["challengeCode"] = str(self.challenge_code)
         elif include_empty:
             result["challengeCode"] = ""
+        if hasattr(self, "code") and self.code:
+            result["code"] = str(self.code)
+        elif include_empty:
+            result["code"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
-        if hasattr(self, "goal_code") and self.goal_code:
-            result["goalCode"] = str(self.goal_code)
-        elif include_empty:
-            result["goalCode"] = ""
         return result
 
     # endregion to methods
 
     # region response methods
 
     # noinspection PyMethodMayBeStatic
     def parse_response(
         self, code: int, content_type: str, content: Any
     ) -> Tuple[
-        Union[None, ModelUserProgressionResponse],
+        Union[None, ModelGoalResponse],
         Union[None, HttpResponse, IamErrorResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelUserProgressionResponse (OK)
+        200: OK - ModelGoalResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - IamErrorResponse (20029: not found)
+        404: Not Found - ResponseError (Not Found)
 
-        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+        500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -217,78 +222,71 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelUserProgressionResponse.create_from_dict(content), None
+            return ModelGoalResponse.create_from_dict(content), None
         if code == 401:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 403:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 404:
-            return None, IamErrorResponse.create_from_dict(content)
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
-        challenge_code: str,
-        namespace: str,
-        goal_code: Optional[str] = None,
-        **kwargs,
-    ) -> PublicGetUserProgression:
+        cls, challenge_code: str, code: str, namespace: str, **kwargs
+    ) -> AdminGetGoal:
         instance = cls()
         instance.challenge_code = challenge_code
+        instance.code = code
         instance.namespace = namespace
-        if goal_code is not None:
-            instance.goal_code = goal_code
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> PublicGetUserProgression:
+    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> AdminGetGoal:
         instance = cls()
         if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
             instance.challenge_code = str(dict_["challengeCode"])
         elif include_empty:
             instance.challenge_code = ""
+        if "code" in dict_ and dict_["code"] is not None:
+            instance.code = str(dict_["code"])
+        elif include_empty:
+            instance.code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
-        if "goalCode" in dict_ and dict_["goalCode"] is not None:
-            instance.goal_code = str(dict_["goalCode"])
-        elif include_empty:
-            instance.goal_code = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "challengeCode": "challenge_code",
+            "code": "code",
             "namespace": "namespace",
-            "goalCode": "goal_code",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "challengeCode": True,
+            "code": True,
             "namespace": True,
-            "goalCode": False,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_create_goal.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         * code: unique within a challenge
         * name: name of the goal
         * description: text describing the goal (optional)
         * schedule: a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
         * requirementGroups: list of conditions that conform with the goal progressions.
         * rewards: list of rewards that will be claimable once a goal is complete
         * tag: goal's labels
+        * isActive: when goal is in a schedule, isActive determine whether goal is active to progress or not
     Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
 
     Properties:
         url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals
@@ -71,14 +72,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelGoalResponse (Created)
 
+        400: Bad Request - IamErrorResponse (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         404: Not Found - ResponseError (20029: not found)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
@@ -87,33 +90,47 @@
     """
 
     # region fields
 
     _url: str = (
         "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals"
     )
+    _path: str = (
+        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals"
+    )
+    _base_path: str = ""
     _method: str = "POST"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     body: ModelCreateGoalRequest  # REQUIRED in [body]
     challenge_code: str  # REQUIRED in [path]
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
 
@@ -207,14 +224,16 @@
         Union[None, ModelGoalResponse],
         Union[None, HttpResponse, IamErrorResponse, ResponseError],
     ]:
         """Parse the given response.
 
         201: Created - ModelGoalResponse (Created)
 
+        400: Bad Request - IamErrorResponse (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         404: Not Found - ResponseError (20029: not found)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
@@ -232,14 +251,16 @@
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 201:
             return ModelGoalResponse.create_from_dict(content), None
+        if code == 400:
+            return None, IamErrorResponse.create_from_dict(content)
         if code == 401:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 403:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 409:
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_delete_goal.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/challenge_configuration/admin_delete_challenge.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,73 +28,86 @@
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import ResponseError
 
 
-class AdminDeleteGoal(Operation):
-    """Delete Goal (adminDeleteGoal)
+class AdminDeleteChallenge(Operation):
+    """Delete a Challenge (adminDeleteChallenge)
 
     * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [DELETE]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
+        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}
 
         method: DELETE
 
-        tags: ["Goal Configuration"]
+        tags: ["Challenge Configuration"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         challenge_code: (challengeCode) REQUIRED str in path
 
-        code: (code) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         204: No Content - (No Content)
 
         400: Bad Request - ResponseError (20018: bad request: {{message}})
 
+        401: Unauthorized - ResponseError (20001: unauthorized access)
+
+        403: Forbidden - ResponseError (20013: insufficient permission)
+
         404: Not Found - ResponseError (20029: not found)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
-    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}"
+    _base_path: str = ""
     _method: str = "DELETE"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
-    code: str  # REQUIRED in [path]
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
 
@@ -123,54 +136,44 @@
             "path": self.get_path_params(),
         }
 
     def get_path_params(self) -> dict:
         result = {}
         if hasattr(self, "challenge_code"):
             result["challengeCode"] = self.challenge_code
-        if hasattr(self, "code"):
-            result["code"] = self.code
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_challenge_code(self, value: str) -> AdminDeleteGoal:
+    def with_challenge_code(self, value: str) -> AdminDeleteChallenge:
         self.challenge_code = value
         return self
 
-    def with_code(self, value: str) -> AdminDeleteGoal:
-        self.code = value
-        return self
-
-    def with_namespace(self, value: str) -> AdminDeleteGoal:
+    def with_namespace(self, value: str) -> AdminDeleteChallenge:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "challenge_code") and self.challenge_code:
             result["challengeCode"] = str(self.challenge_code)
         elif include_empty:
             result["challengeCode"] = ""
-        if hasattr(self, "code") and self.code:
-            result["code"] = str(self.code)
-        elif include_empty:
-            result["code"] = ""
         if hasattr(self, "namespace") and self.namespace:
             result["namespace"] = str(self.namespace)
         elif include_empty:
             result["namespace"] = ""
         return result
 
     # endregion to methods
@@ -183,14 +186,18 @@
     ) -> Tuple[None, Union[None, HttpResponse, ResponseError]]:
         """Parse the given response.
 
         204: No Content - (No Content)
 
         400: Bad Request - ResponseError (20018: bad request: {{message}})
 
+        401: Unauthorized - ResponseError (20001: unauthorized access)
+
+        403: Forbidden - ResponseError (20013: insufficient permission)
+
         404: Not Found - ResponseError (20029: not found)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
@@ -204,14 +211,18 @@
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 204:
             return None, None
         if code == 400:
             return None, ResponseError.create_from_dict(content)
+        if code == 401:
+            return None, ResponseError.create_from_dict(content)
+        if code == 403:
+            return None, ResponseError.create_from_dict(content)
         if code == 404:
             return None, ResponseError.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
@@ -219,53 +230,46 @@
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, challenge_code: str, code: str, namespace: str, **kwargs
-    ) -> AdminDeleteGoal:
+        cls, challenge_code: str, namespace: str, **kwargs
+    ) -> AdminDeleteChallenge:
         instance = cls()
         instance.challenge_code = challenge_code
-        instance.code = code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> AdminDeleteGoal:
+    ) -> AdminDeleteChallenge:
         instance = cls()
         if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
             instance.challenge_code = str(dict_["challengeCode"])
         elif include_empty:
             instance.challenge_code = ""
-        if "code" in dict_ and dict_["code"] is not None:
-            instance.code = str(dict_["code"])
-        elif include_empty:
-            instance.code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "challengeCode": "challenge_code",
-            "code": "code",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "challengeCode": True,
-            "code": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goal.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,79 +26,89 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
 from ...models import IamErrorResponse
-from ...models import ModelGoalResponse
+from ...models import ModelClaimUserRewardsReq
+from ...models import ModelUserReward
 from ...models import ResponseError
 
 
-class AdminGetGoal(Operation):
-    """Get Goal (adminGetGoal)
+class PublicClaimUserRewards(Operation):
+    """Claim User's Rewards (publicClaimUserRewards)
 
-    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CHALLENGE [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim
 
-        method: GET
+        method: POST
 
-        tags: ["Goal Configuration"]
+        tags: ["Player Reward"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        challenge_code: (challengeCode) REQUIRED str in path
-
-        code: (code) REQUIRED str in path
+        body: (body) REQUIRED ModelClaimUserRewardsReq in body
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelGoalResponse (OK)
+        200: OK - List[ModelUserReward] (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - ResponseError (Not Found)
+        404: Not Found - IamErrorResponse (20029: not found)
 
-        500: Internal Server Error - ResponseError (Internal Server Error)
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
-    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
-    _method: str = "GET"
-    _consumes: List[str] = []
+    _url: str = "/challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim"
+    _path: str = "/challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim"
+    _base_path: str = ""
+    _method: str = "POST"
+    _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    challenge_code: str  # REQUIRED in [path]
-    code: str  # REQUIRED in [path]
+    service_name: Optional[str] = "challenge"
+
+    body: ModelClaimUserRewardsReq  # REQUIRED in [body]
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
 
@@ -120,89 +130,83 @@
 
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
-        if hasattr(self, "challenge_code"):
-            result["challengeCode"] = self.challenge_code
-        if hasattr(self, "code"):
-            result["code"] = self.code
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_challenge_code(self, value: str) -> AdminGetGoal:
-        self.challenge_code = value
+    def with_body(self, value: ModelClaimUserRewardsReq) -> PublicClaimUserRewards:
+        self.body = value
         return self
 
-    def with_code(self, value: str) -> AdminGetGoal:
-        self.code = value
-        return self
-
-    def with_namespace(self, value: str) -> AdminGetGoal:
+    def with_namespace(self, value: str) -> PublicClaimUserRewards:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
-        if hasattr(self, "challenge_code") and self.challenge_code:
-            result["challengeCode"] = str(self.challenge_code)
-        elif include_empty:
-            result["challengeCode"] = ""
-        if hasattr(self, "code") and self.code:
-            result["code"] = str(self.code)
+        if hasattr(self, "body") and self.body:
+            result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["code"] = ""
+            result["body"] = ModelClaimUserRewardsReq()
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
-        Union[None, ModelGoalResponse],
+        Union[None, List[ModelUserReward]],
         Union[None, HttpResponse, IamErrorResponse, ResponseError],
     ]:
         """Parse the given response.
 
-        200: OK - ModelGoalResponse (OK)
+        200: OK - List[ModelUserReward] (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - ResponseError (Not Found)
+        404: Not Found - IamErrorResponse (20029: not found)
 
-        500: Internal Server Error - ResponseError (Internal Server Error)
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -210,71 +214,68 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return ModelGoalResponse.create_from_dict(content), None
+            return [ModelUserReward.create_from_dict(i) for i in content], None
         if code == 401:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 403:
             return None, IamErrorResponse.create_from_dict(content)
         if code == 404:
-            return None, ResponseError.create_from_dict(content)
+            return None, IamErrorResponse.create_from_dict(content)
         if code == 500:
             return None, ResponseError.create_from_dict(content)
 
         return self.handle_undocumented_response(
             code=code, content_type=content_type, content=content
         )
 
     # endregion response methods
 
     # region static methods
 
     @classmethod
     def create(
-        cls, challenge_code: str, code: str, namespace: str, **kwargs
-    ) -> AdminGetGoal:
+        cls, body: ModelClaimUserRewardsReq, namespace: str, **kwargs
+    ) -> PublicClaimUserRewards:
         instance = cls()
-        instance.challenge_code = challenge_code
-        instance.code = code
+        instance.body = body
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
-    def create_from_dict(cls, dict_: dict, include_empty: bool = False) -> AdminGetGoal:
+    def create_from_dict(
+        cls, dict_: dict, include_empty: bool = False
+    ) -> PublicClaimUserRewards:
         instance = cls()
-        if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
-            instance.challenge_code = str(dict_["challengeCode"])
-        elif include_empty:
-            instance.challenge_code = ""
-        if "code" in dict_ and dict_["code"] is not None:
-            instance.code = str(dict_["code"])
+        if "body" in dict_ and dict_["body"] is not None:
+            instance.body = ModelClaimUserRewardsReq.create_from_dict(
+                dict_["body"], include_empty=include_empty
+            )
         elif include_empty:
-            instance.code = ""
+            instance.body = ModelClaimUserRewardsReq()
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
-            "challengeCode": "challenge_code",
-            "code": "code",
+            "body": "body",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
-            "challengeCode": True,
-            "code": True,
+            "body": True,
             "namespace": True,
         }
 
     # endregion static methods
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_get_goals.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,20 +78,26 @@
     """
 
     # region fields
 
     _url: str = (
         "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals"
     )
+    _path: str = (
+        "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals"
+    )
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     challenge_code: str  # REQUIRED in [path]
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
 
     # endregion fields
@@ -99,14 +105,22 @@
     # region properties
 
     @property
     def url(self) -> str:
         return self._url
 
     @property
+    def path(self) -> str:
+        return self._path
+
+    @property
+    def base_path(self) -> str:
+        return self._base_path
+
+    @property
     def method(self) -> str:
         return self._method
 
     @property
     def consumes(self) -> List[str]:
         return self._consumes
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,300 +1,297 @@
 # Copyright (c) 2021 AccelByte Inc. All Rights Reserved.
 # This is licensed software from AccelByte Inc, for limitations
 # and restrictions contact your company contract manager.
 #
 # Code generated. DO NOT EDIT!
 
-# template file: operation.j2
+# template file: wrapper.j2
 
 # pylint: disable=duplicate-code
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
+# pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 # pylint: disable=too-many-arguments
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-public-methods
 # pylint: disable=too-many-return-statements
 # pylint: disable=too-many-statements
 # pylint: disable=unused-import
 
-# AccelByte Gaming Services Challenge Service
-
-from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
-from accelbyte_py_sdk.core import HttpResponse
+from accelbyte_py_sdk.core import get_namespace as get_services_namespace
+from accelbyte_py_sdk.core import run_request
+from accelbyte_py_sdk.core import run_request_async
+from accelbyte_py_sdk.core import same_doc_as
+
+from ..models import IamErrorResponse
+from ..models import ModelGetGoalsResponse
+from ..models import ModelListChallengeResponse
+from ..models import ResponseError
+
+from ..operations.challenge_list import GetChallenges
+from ..operations.challenge_list import (
+    GetChallengesStatusEnum,
+)
+from ..operations.challenge_list import PublicGetScheduledGoals
+
+
+@same_doc_as(GetChallenges)
+def get_challenges(
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, GetChallengesStatusEnum]] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """List Challenges (GetChallenges)
+
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:CHALLENGE [READ]
 
-from ...models import ModelGoalResponse
-from ...models import ModelUpdateGoalRequest
-from ...models import ResponseError
+    Properties:
+        url: /challenge/v1/public/namespaces/{namespace}/challenges
+
+        method: GET
+
+        tags: ["Challenge List"]
 
+        consumes: []
+
+        produces: ["application/json"]
 
-class AdminUpdateGoals(Operation):
-    """Update Goal (adminUpdateGoals)
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
+
+    Responses:
+        200: OK - ModelListChallengeResponse (OK)
 
-    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetChallenges.create(
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(GetChallenges)
+async def get_challenges_async(
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, GetChallengesStatusEnum]] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """List Challenges (GetChallenges)
+
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
+        - NAMESPACE:{namespace}:CHALLENGE [READ]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
+        url: /challenge/v1/public/namespaces/{namespace}/challenges
 
-        method: PUT
+        method: GET
 
-        tags: ["Goal Configuration"]
+        tags: ["Challenge List"]
 
-        consumes: ["application/json"]
+        consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelUpdateGoalRequest in body
+        namespace: (namespace) REQUIRED str in path
 
-        challenge_code: (challengeCode) REQUIRED str in path
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
 
-        code: (code) REQUIRED str in path
+    Responses:
+        200: OK - ModelListChallengeResponse (OK)
+
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = GetChallenges.create(
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
+
+
+@same_doc_as(PublicGetScheduledGoals)
+def public_get_scheduled_goals(
+    challenge_code: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    tags: Optional[List[str]] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """List Goals of a Challenge (publicGetScheduledGoals)
+
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:CHALLENGE [READ]
+
+    Properties:
+        url: /challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals
+
+        method: GET
+
+        tags: ["Challenge List"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        tags: (tags) OPTIONAL List[str] in query
+
     Responses:
-        200: OK - ModelGoalResponse (OK)
+        200: OK - ModelGetGoalsResponse (OK)
+
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
-        404: Not Found - ResponseError (Not Found)
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        500: Internal Server Error - ResponseError (Internal Server Error)
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = PublicGetScheduledGoals.create(
+        challenge_code=challenge_code,
+        limit=limit,
+        offset=offset,
+        tags=tags,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(PublicGetScheduledGoals)
+async def public_get_scheduled_goals_async(
+    challenge_code: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    tags: Optional[List[str]] = None,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """List Goals of a Challenge (publicGetScheduledGoals)
+
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:CHALLENGE [READ]
+
+    Properties:
+        url: /challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals
+
+        method: GET
+
+        tags: ["Challenge List"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        challenge_code: (challengeCode) REQUIRED str in path
+
+        namespace: (namespace) REQUIRED str in path
 
-    # region fields
+        limit: (limit) OPTIONAL int in query
 
-    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
-    _method: str = "PUT"
-    _consumes: List[str] = ["application/json"]
-    _produces: List[str] = ["application/json"]
-    _securities: List[List[str]] = [["BEARER_AUTH"]]
-    _location_query: str = None
-
-    body: ModelUpdateGoalRequest  # REQUIRED in [body]
-    challenge_code: str  # REQUIRED in [path]
-    code: str  # REQUIRED in [path]
-    namespace: str  # REQUIRED in [path]
-
-    # endregion fields
-
-    # region properties
-
-    @property
-    def url(self) -> str:
-        return self._url
-
-    @property
-    def method(self) -> str:
-        return self._method
-
-    @property
-    def consumes(self) -> List[str]:
-        return self._consumes
-
-    @property
-    def produces(self) -> List[str]:
-        return self._produces
-
-    @property
-    def securities(self) -> List[List[str]]:
-        return self._securities
-
-    @property
-    def location_query(self) -> str:
-        return self._location_query
-
-    # endregion properties
-
-    # region get methods
-
-    # endregion get methods
-
-    # region get_x_params methods
-
-    def get_all_params(self) -> dict:
-        return {
-            "body": self.get_body_params(),
-            "path": self.get_path_params(),
-        }
-
-    def get_body_params(self) -> Any:
-        if not hasattr(self, "body") or self.body is None:
-            return None
-        return self.body.to_dict()
-
-    def get_path_params(self) -> dict:
-        result = {}
-        if hasattr(self, "challenge_code"):
-            result["challengeCode"] = self.challenge_code
-        if hasattr(self, "code"):
-            result["code"] = self.code
-        if hasattr(self, "namespace"):
-            result["namespace"] = self.namespace
-        return result
-
-    # endregion get_x_params methods
-
-    # region is/has methods
-
-    # endregion is/has methods
-
-    # region with_x methods
-
-    def with_body(self, value: ModelUpdateGoalRequest) -> AdminUpdateGoals:
-        self.body = value
-        return self
-
-    def with_challenge_code(self, value: str) -> AdminUpdateGoals:
-        self.challenge_code = value
-        return self
-
-    def with_code(self, value: str) -> AdminUpdateGoals:
-        self.code = value
-        return self
-
-    def with_namespace(self, value: str) -> AdminUpdateGoals:
-        self.namespace = value
-        return self
-
-    # endregion with_x methods
-
-    # region to methods
-
-    def to_dict(self, include_empty: bool = False) -> dict:
-        result: dict = {}
-        if hasattr(self, "body") and self.body:
-            result["body"] = self.body.to_dict(include_empty=include_empty)
-        elif include_empty:
-            result["body"] = ModelUpdateGoalRequest()
-        if hasattr(self, "challenge_code") and self.challenge_code:
-            result["challengeCode"] = str(self.challenge_code)
-        elif include_empty:
-            result["challengeCode"] = ""
-        if hasattr(self, "code") and self.code:
-            result["code"] = str(self.code)
-        elif include_empty:
-            result["code"] = ""
-        if hasattr(self, "namespace") and self.namespace:
-            result["namespace"] = str(self.namespace)
-        elif include_empty:
-            result["namespace"] = ""
-        return result
-
-    # endregion to methods
-
-    # region response methods
-
-    # noinspection PyMethodMayBeStatic
-    def parse_response(
-        self, code: int, content_type: str, content: Any
-    ) -> Tuple[
-        Union[None, ModelGoalResponse], Union[None, HttpResponse, ResponseError]
-    ]:
-        """Parse the given response.
-
-        200: OK - ModelGoalResponse (OK)
-
-        404: Not Found - ResponseError (Not Found)
-
-        500: Internal Server Error - ResponseError (Internal Server Error)
-
-        ---: HttpResponse (Undocumented Response)
-
-        ---: HttpResponse (Unexpected Content-Type Error)
-
-        ---: HttpResponse (Unhandled Error)
-        """
-        pre_processed_response, error = self.pre_process_response(
-            code=code, content_type=content_type, content=content
-        )
-        if error is not None:
-            return None, None if error.is_no_content() else error
-        code, content_type, content = pre_processed_response
-
-        if code == 200:
-            return ModelGoalResponse.create_from_dict(content), None
-        if code == 404:
-            return None, ResponseError.create_from_dict(content)
-        if code == 500:
-            return None, ResponseError.create_from_dict(content)
-
-        return self.handle_undocumented_response(
-            code=code, content_type=content_type, content=content
-        )
-
-    # endregion response methods
-
-    # region static methods
-
-    @classmethod
-    def create(
-        cls,
-        body: ModelUpdateGoalRequest,
-        challenge_code: str,
-        code: str,
-        namespace: str,
-        **kwargs,
-    ) -> AdminUpdateGoals:
-        instance = cls()
-        instance.body = body
-        instance.challenge_code = challenge_code
-        instance.code = code
-        instance.namespace = namespace
-        if x_flight_id := kwargs.get("x_flight_id", None):
-            instance.x_flight_id = x_flight_id
-        return instance
-
-    @classmethod
-    def create_from_dict(
-        cls, dict_: dict, include_empty: bool = False
-    ) -> AdminUpdateGoals:
-        instance = cls()
-        if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelUpdateGoalRequest.create_from_dict(
-                dict_["body"], include_empty=include_empty
-            )
-        elif include_empty:
-            instance.body = ModelUpdateGoalRequest()
-        if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
-            instance.challenge_code = str(dict_["challengeCode"])
-        elif include_empty:
-            instance.challenge_code = ""
-        if "code" in dict_ and dict_["code"] is not None:
-            instance.code = str(dict_["code"])
-        elif include_empty:
-            instance.code = ""
-        if "namespace" in dict_ and dict_["namespace"] is not None:
-            instance.namespace = str(dict_["namespace"])
-        elif include_empty:
-            instance.namespace = ""
-        return instance
-
-    @staticmethod
-    def get_field_info() -> Dict[str, str]:
-        return {
-            "body": "body",
-            "challengeCode": "challenge_code",
-            "code": "code",
-            "namespace": "namespace",
-        }
-
-    @staticmethod
-    def get_required_map() -> Dict[str, bool]:
-        return {
-            "body": True,
-            "challengeCode": True,
-            "code": True,
-            "namespace": True,
-        }
+        offset: (offset) OPTIONAL int in query
 
-    # endregion static methods
+        tags: (tags) OPTIONAL List[str] in query
+
+    Responses:
+        200: OK - ModelGetGoalsResponse (OK)
+
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = PublicGetScheduledGoals.create(
+        challenge_code=challenge_code,
+        limit=limit,
+        offset=offset,
+        tags=tags,
+        namespace=namespace,
+    )
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/admin_get_user_rewards.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,24 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/admin/namespaces/{namespace}/users/{userId}/rewards"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/users/{userId}/rewards"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     namespace: str  # REQUIRED in [path]
     user_id: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
     status: Union[str, StatusEnum]  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_claim_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/goal_configuration/admin_update_goals.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,78 +25,101 @@
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from accelbyte_py_sdk.core import Operation
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import HttpResponse
 
-from ...models import IamErrorResponse
-from ...models import ModelClaimUserRewardsReq
-from ...models import ModelUserReward
+from ...models import ModelGoalResponse
+from ...models import ModelUpdateGoalRequest
 from ...models import ResponseError
 
 
-class PublicClaimUserRewards(Operation):
-    """Claim User's Rewards (publicClaimUserRewards)
+class AdminUpdateGoals(Operation):
+    """Update Goal (adminUpdateGoals)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD:CLAIM [UPDATE]
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
+
+    Request body:
+        * name: name of the goal
+        * description: text describing the goal (optional)
+        * schedule (optional): a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
+        * requirementGroups: list of conditions that conform with the goal progressions.
+        * rewards: list of rewards that will be claimable once a goal is complete
+        * tag: goal's labels
+        * isActive (optional): when goal is in a schedule, isActive determine whether goal is active to progress or not
+    Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:REWARD:CLAIM [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim
+        url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
 
-        method: POST
+        method: PUT
 
-        tags: ["Player Reward"]
+        tags: ["Goal Configuration"]
 
         consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelClaimUserRewardsReq in body
+        body: (body) REQUIRED ModelUpdateGoalRequest in body
 
-        namespace: (namespace) REQUIRED str in path
+        challenge_code: (challengeCode) REQUIRED str in path
 
-    Responses:
-        200: OK - List[ModelUserReward] (OK)
+        code: (code) REQUIRED str in path
 
-        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+        namespace: (namespace) REQUIRED str in path
 
-        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+    Responses:
+        200: OK - ModelGoalResponse (OK)
 
-        404: Not Found - IamErrorResponse (20029: not found)
+        404: Not Found - ResponseError (Not Found)
 
-        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+        500: Internal Server Error - ResponseError (Internal Server Error)
     """
 
     # region fields
 
-    _url: str = "/challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim"
-    _method: str = "POST"
+    _url: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _path: str = "/challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}"
+    _base_path: str = ""
+    _method: str = "PUT"
     _consumes: List[str] = ["application/json"]
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
-    body: ModelClaimUserRewardsReq  # REQUIRED in [body]
+    service_name: Optional[str] = "challenge"
+
+    body: ModelUpdateGoalRequest  # REQUIRED in [body]
+    challenge_code: str  # REQUIRED in [path]
+    code: str  # REQUIRED in [path]
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
 
@@ -129,72 +152,87 @@
     def get_body_params(self) -> Any:
         if not hasattr(self, "body") or self.body is None:
             return None
         return self.body.to_dict()
 
     def get_path_params(self) -> dict:
         result = {}
+        if hasattr(self, "challenge_code"):
+            result["challengeCode"] = self.challenge_code
+        if hasattr(self, "code"):
+            result["code"] = self.code
         if hasattr(self, "namespace"):
             result["namespace"] = self.namespace
         return result
 
     # endregion get_x_params methods
 
     # region is/has methods
 
     # endregion is/has methods
 
     # region with_x methods
 
-    def with_body(self, value: ModelClaimUserRewardsReq) -> PublicClaimUserRewards:
+    def with_body(self, value: ModelUpdateGoalRequest) -> AdminUpdateGoals:
         self.body = value
         return self
 
-    def with_namespace(self, value: str) -> PublicClaimUserRewards:
+    def with_challenge_code(self, value: str) -> AdminUpdateGoals:
+        self.challenge_code = value
+        return self
+
+    def with_code(self, value: str) -> AdminUpdateGoals:
+        self.code = value
+        return self
+
+    def with_namespace(self, value: str) -> AdminUpdateGoals:
         self.namespace = value
         return self
 
     # endregion with_x methods
 
     # region to methods
 
     def to_dict(self, include_empty: bool = False) -> dict:
         result: dict = {}
         if hasattr(self, "body") and self.body:
             result["body"] = self.body.to_dict(include_empty=include_empty)
         elif include_empty:
-            result["body"] = ModelClaimUserRewardsReq()
+            result["body"] = ModelUpdateGoalRequest()
+        if hasattr(self, "challenge_code") and self.challenge_code:
+            result["challengeCode"] = str(self.challenge_code)
+        elif include_empty:
+            result["challengeCode"] = ""
+        if hasattr(self, "code") and self.code:
+            result["code"] = str(self.code)
+        elif include_empty:
+            result["code"] = ""
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
-        Union[None, List[ModelUserReward]],
-        Union[None, HttpResponse, IamErrorResponse, ResponseError],
+        Union[None, ModelGoalResponse], Union[None, HttpResponse, ResponseError]
     ]:
         """Parse the given response.
 
-        200: OK - List[ModelUserReward] (OK)
+        200: OK - ModelGoalResponse (OK)
 
-        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+        404: Not Found - ResponseError (Not Found)
 
-        403: Forbidden - IamErrorResponse (20013: insufficient permission)
-
-        404: Not Found - IamErrorResponse (20029: not found)
-
-        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+        500: Internal Server Error - ResponseError (Internal Server Error)
 
         ---: HttpResponse (Undocumented Response)
 
         ---: HttpResponse (Unexpected Content-Type Error)
 
         ---: HttpResponse (Unhandled Error)
         """
@@ -202,68 +240,83 @@
             code=code, content_type=content_type, content=content
         )
         if error is not None:
             return None, None if error.is_no_content() else error
         code, content_type, content = pre_processed_response
 
         if code == 200:
-            return [ModelUserReward.create_from_dict(i) for i in content], None
-        if code == 401:
-            return None, IamErrorResponse.create_from_dict(content)
-        if code == 403:
-            return None, IamErrorResponse.create_from_dict(content)
+            return ModelGoalResponse.create_from_dict(content), None
         if code == 404:
-            return None, IamErrorResponse.create_from_dict(content)
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
-        cls, body: ModelClaimUserRewardsReq, namespace: str, **kwargs
-    ) -> PublicClaimUserRewards:
+        cls,
+        body: ModelUpdateGoalRequest,
+        challenge_code: str,
+        code: str,
+        namespace: str,
+        **kwargs,
+    ) -> AdminUpdateGoals:
         instance = cls()
         instance.body = body
+        instance.challenge_code = challenge_code
+        instance.code = code
         instance.namespace = namespace
         if x_flight_id := kwargs.get("x_flight_id", None):
             instance.x_flight_id = x_flight_id
         return instance
 
     @classmethod
     def create_from_dict(
         cls, dict_: dict, include_empty: bool = False
-    ) -> PublicClaimUserRewards:
+    ) -> AdminUpdateGoals:
         instance = cls()
         if "body" in dict_ and dict_["body"] is not None:
-            instance.body = ModelClaimUserRewardsReq.create_from_dict(
+            instance.body = ModelUpdateGoalRequest.create_from_dict(
                 dict_["body"], include_empty=include_empty
             )
         elif include_empty:
-            instance.body = ModelClaimUserRewardsReq()
+            instance.body = ModelUpdateGoalRequest()
+        if "challengeCode" in dict_ and dict_["challengeCode"] is not None:
+            instance.challenge_code = str(dict_["challengeCode"])
+        elif include_empty:
+            instance.challenge_code = ""
+        if "code" in dict_ and dict_["code"] is not None:
+            instance.code = str(dict_["code"])
+        elif include_empty:
+            instance.code = ""
         if "namespace" in dict_ and dict_["namespace"] is not None:
             instance.namespace = str(dict_["namespace"])
         elif include_empty:
             instance.namespace = ""
         return instance
 
     @staticmethod
     def get_field_info() -> Dict[str, str]:
         return {
             "body": "body",
+            "challengeCode": "challenge_code",
+            "code": "code",
             "namespace": "namespace",
         }
 
     @staticmethod
     def get_required_map() -> Dict[str, bool]:
         return {
             "body": True,
+            "challengeCode": True,
+            "code": True,
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/operations/player_reward/public_get_user_rewards.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     CLAIMED = "CLAIMED"
     UNCLAIMED = "UNCLAIMED"
 
 
 class PublicGetUserRewards(Operation):
     """List User's Rewards (publicGetUserRewards)
 
-    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Properties:
         url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards
 
         method: GET
 
         tags: ["Player Reward"]
@@ -80,20 +80,24 @@
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
 
     # region fields
 
     _url: str = "/challenge/v1/public/namespaces/{namespace}/users/me/rewards"
+    _path: str = "/challenge/v1/public/namespaces/{namespace}/users/me/rewards"
+    _base_path: str = ""
     _method: str = "GET"
     _consumes: List[str] = []
     _produces: List[str] = ["application/json"]
     _securities: List[List[str]] = [["BEARER_AUTH"]]
     _location_query: str = None
 
+    service_name: Optional[str] = "challenge"
+
     namespace: str  # REQUIRED in [path]
     limit: int  # OPTIONAL in [query]
     offset: int  # OPTIONAL in [query]
     sort_by: str  # OPTIONAL in [query]
     status: Union[str, StatusEnum]  # OPTIONAL in [query]
 
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

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
       * code: only lowercase letters, numbers, and the separator - are allowed; must start and end with letter
       * name: name of the challenge
       * description: text describing about the challenge (optional)
       * startDate: timestamp of when the challenge is started
       * endDate: timestamp of when the challenge is ended (optional)
       * endAfter: describe number of period challenge will be retired after (optional)
     To configure challenge that never end, leave the endDate and endAfter field null/empty.
+      * repeatAfter: describe number of period challenge's goals will be repeated after. Leave it empty if you don't want to repeat the challenge.
       * rotation: describe how long goals in a challenge will be available for players to progress before rotated with another goals. (DAILY|WEEKLY|MONTHLY|NONE)
       * activeGoalsPerRotation: number of goals per rotation (currently only applicable for RANDOMIZE assignment)
       * assignmentRule: describe how the goals will be assigned and scheduled to users. (FIXED|RANDOMIZED|UNSCHEDULED)
       * goalsVisibility: describe whether users can see all goals under challenge, or only active goal in one rotation period only. (SHOWALL|PERIODONLY)
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
@@ -156,14 +157,15 @@
       * code: only lowercase letters, numbers, and the separator - are allowed; must start and end with letter
       * name: name of the challenge
       * description: text describing about the challenge (optional)
       * startDate: timestamp of when the challenge is started
       * endDate: timestamp of when the challenge is ended (optional)
       * endAfter: describe number of period challenge will be retired after (optional)
     To configure challenge that never end, leave the endDate and endAfter field null/empty.
+      * repeatAfter: describe number of period challenge's goals will be repeated after. Leave it empty if you don't want to repeat the challenge.
       * rotation: describe how long goals in a challenge will be available for players to progress before rotated with another goals. (DAILY|WEEKLY|MONTHLY|NONE)
       * activeGoalsPerRotation: number of goals per rotation (currently only applicable for RANDOMIZE assignment)
       * assignmentRule: describe how the goals will be assigned and scheduled to users. (FIXED|RANDOMIZED|UNSCHEDULED)
       * goalsVisibility: describe whether users can see all goals under challenge, or only active goal in one rotation period only. (SHOWALL|PERIODONLY)
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_list.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,271 +26,357 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import IamErrorResponse
-from ..models import ModelGetGoalsResponse
-from ..models import ModelListChallengeResponse
+from ..models import ModelEvaluatePlayerProgressionRequest
+from ..models import ModelUserProgressionResponse
 from ..models import ResponseError
 
-from ..operations.challenge_list import GetChallenges
-from ..operations.challenge_list import (
-    GetChallengesStatusEnum,
-)
-from ..operations.challenge_list import PublicGetScheduledGoals
+from ..operations.challenge_progression import AdminEvaluateProgress
+from ..operations.challenge_progression import EvaluateMyProgress
+from ..operations.challenge_progression import PublicGetUserProgression
 
 
-@same_doc_as(GetChallenges)
-def get_challenges(
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
-    sort_by: Optional[str] = None,
-    status: Optional[Union[str, GetChallengesStatusEnum]] = None,
+@same_doc_as(AdminEvaluateProgress)
+def admin_evaluate_progress(
+    body: ModelEvaluatePlayerProgressionRequest,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List Challenges (GetChallenges)
+    """Evaluate User's Progressions (adminEvaluateProgress)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE [READ]
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/challenges
+        url: /challenge/v1/admin/namespaces/{namespace}/progress/evaluate
 
-        method: GET
+        method: POST
 
-        tags: ["Challenge List"]
+        tags: ["Challenge Progression"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelEvaluatePlayerProgressionRequest in body
+
         namespace: (namespace) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
+    Responses:
+        204: No Content - (No Content)
+
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+
+        404: Not Found - ResponseError (20029: not found)
+
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = AdminEvaluateProgress.create(
+        body=body,
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
-        offset: (offset) OPTIONAL int in query
 
-        sort_by: (sortBy) OPTIONAL str in query
+@same_doc_as(AdminEvaluateProgress)
+async def admin_evaluate_progress_async(
+    body: ModelEvaluatePlayerProgressionRequest,
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Evaluate User's Progressions (adminEvaluateProgress)
+
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+
+    Required Permission(s):
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+
+    Properties:
+        url: /challenge/v1/admin/namespaces/{namespace}/progress/evaluate
 
-        status: (status) OPTIONAL Union[str, StatusEnum] in query
+        method: POST
+
+        tags: ["Challenge Progression"]
+
+        consumes: ["application/json"]
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        body: (body) REQUIRED ModelEvaluatePlayerProgressionRequest in body
+
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelListChallengeResponse (OK)
+        204: No Content - (No Content)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - ResponseError (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = GetChallenges.create(
-        limit=limit,
-        offset=offset,
-        sort_by=sort_by,
-        status=status,
+    request = AdminEvaluateProgress.create(
+        body=body,
         namespace=namespace,
     )
-    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+    return await run_request_async(
+        request, additional_headers=x_additional_headers, **kwargs
+    )
 
 
-@same_doc_as(GetChallenges)
-async def get_challenges_async(
-    limit: Optional[int] = None,
-    offset: Optional[int] = None,
-    sort_by: Optional[str] = None,
-    status: Optional[Union[str, GetChallengesStatusEnum]] = None,
+@same_doc_as(EvaluateMyProgress)
+def evaluate_my_progress(
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List Challenges (GetChallenges)
+    """Evaluate User's Challenge Progressions (EvaluateMyProgress)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/challenges
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate
 
-        method: GET
+        method: POST
 
-        tags: ["Challenge List"]
+        tags: ["Challenge Progression"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         namespace: (namespace) REQUIRED str in path
 
-        limit: (limit) OPTIONAL int in query
+    Responses:
+        204: No Content - (No Content)
 
-        offset: (offset) OPTIONAL int in query
+        401: Unauthorized - IamErrorResponse (20001: unauthorized access)
+
+        403: Forbidden - IamErrorResponse (20013: insufficient permission)
+
+        500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
+    """
+    if namespace is None:
+        namespace, error = get_services_namespace()
+        if error:
+            return None, error
+    request = EvaluateMyProgress.create(
+        namespace=namespace,
+    )
+    return run_request(request, additional_headers=x_additional_headers, **kwargs)
+
+
+@same_doc_as(EvaluateMyProgress)
+async def evaluate_my_progress_async(
+    namespace: Optional[str] = None,
+    x_additional_headers: Optional[Dict[str, str]] = None,
+    **kwargs
+):
+    """Evaluate User's Challenge Progressions (EvaluateMyProgress)
+
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+
+    Required Permission(s):
+        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+
+    Properties:
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate
 
-        sort_by: (sortBy) OPTIONAL str in query
+        method: POST
 
-        status: (status) OPTIONAL Union[str, StatusEnum] in query
+        tags: ["Challenge Progression"]
+
+        consumes: []
+
+        produces: ["application/json"]
+
+        securities: [BEARER_AUTH]
+
+        namespace: (namespace) REQUIRED str in path
 
     Responses:
-        200: OK - ModelListChallengeResponse (OK)
+        204: No Content - (No Content)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = GetChallenges.create(
-        limit=limit,
-        offset=offset,
-        sort_by=sort_by,
-        status=status,
+    request = EvaluateMyProgress.create(
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(PublicGetScheduledGoals)
-def public_get_scheduled_goals(
+@same_doc_as(PublicGetUserProgression)
+def public_get_user_progression(
     challenge_code: str,
+    goal_code: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     tags: Optional[List[str]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List Goals of a Challenge (publicGetScheduledGoals)
+    """List User's Progressions (publicGetUserProgression)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}
 
         method: GET
 
-        tags: ["Challenge List"]
+        tags: ["Challenge Progression"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        goal_code: (goalCode) OPTIONAL str in query
+
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
         tags: (tags) OPTIONAL List[str] in query
 
     Responses:
-        200: OK - ModelGetGoalsResponse (OK)
+        200: OK - ModelUserProgressionResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - IamErrorResponse (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = PublicGetScheduledGoals.create(
+    request = PublicGetUserProgression.create(
         challenge_code=challenge_code,
+        goal_code=goal_code,
         limit=limit,
         offset=offset,
         tags=tags,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(PublicGetScheduledGoals)
-async def public_get_scheduled_goals_async(
+@same_doc_as(PublicGetUserProgression)
+async def public_get_user_progression_async(
     challenge_code: str,
+    goal_code: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     tags: Optional[List[str]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List Goals of a Challenge (publicGetScheduledGoals)
+    """List User's Progressions (publicGetUserProgression)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/challenges/{challengeCode}/goals
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}
 
         method: GET
 
-        tags: ["Challenge List"]
+        tags: ["Challenge Progression"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
+        goal_code: (goalCode) OPTIONAL str in query
+
         limit: (limit) OPTIONAL int in query
 
         offset: (offset) OPTIONAL int in query
 
         tags: (tags) OPTIONAL List[str] in query
 
     Responses:
-        200: OK - ModelGetGoalsResponse (OK)
+        200: OK - ModelUserProgressionResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - IamErrorResponse (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = PublicGetScheduledGoals.create(
+    request = PublicGetUserProgression.create(
         challenge_code=challenge_code,
+        goal_code=goal_code,
         limit=limit,
         offset=offset,
         tags=tags,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_challenge_progression.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_player_reward.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,334 +26,393 @@
 from accelbyte_py_sdk.core import HeaderStr
 from accelbyte_py_sdk.core import get_namespace as get_services_namespace
 from accelbyte_py_sdk.core import run_request
 from accelbyte_py_sdk.core import run_request_async
 from accelbyte_py_sdk.core import same_doc_as
 
 from ..models import IamErrorResponse
-from ..models import ModelEvaluatePlayerProgressionRequest
-from ..models import ModelUserProgressionResponse
+from ..models import ModelClaimUserRewardsReq
+from ..models import ModelListUserRewardsResponse
+from ..models import ModelUserReward
 from ..models import ResponseError
 
-from ..operations.challenge_progression import AdminEvaluateProgress
-from ..operations.challenge_progression import EvaluateMyProgress
-from ..operations.challenge_progression import PublicGetUserProgression
-
-
-@same_doc_as(AdminEvaluateProgress)
-def admin_evaluate_progress(
-    body: ModelEvaluatePlayerProgressionRequest,
+from ..operations.player_reward import AdminGetUserRewards
+from ..operations.player_reward import (
+    AdminGetUserRewardsStatusEnum,
+)
+from ..operations.player_reward import PublicClaimUserRewards
+from ..operations.player_reward import PublicGetUserRewards
+from ..operations.player_reward import (
+    PublicGetUserRewardsStatusEnum,
+)
+
+
+@same_doc_as(AdminGetUserRewards)
+def admin_get_user_rewards(
+    user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, AdminGetUserRewardsStatusEnum]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Evaluate User's Progressions (adminEvaluateProgress)
+    """List User's Rewards (adminGetUserRewards)
 
-    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/progress/evaluate
+        url: /challenge/v1/admin/namespaces/{namespace}/users/{userId}/rewards
 
-        method: POST
+        method: GET
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
-        consumes: ["application/json"]
+        consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelEvaluatePlayerProgressionRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
+
     Responses:
-        204: No Content - (No Content)
+        200: OK - ModelListUserRewardsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - ResponseError (20029: not found)
-
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminEvaluateProgress.create(
-        body=body,
+    request = AdminGetUserRewards.create(
+        user_id=user_id,
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(AdminEvaluateProgress)
-async def admin_evaluate_progress_async(
-    body: ModelEvaluatePlayerProgressionRequest,
+@same_doc_as(AdminGetUserRewards)
+async def admin_get_user_rewards_async(
+    user_id: str,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, AdminGetUserRewardsStatusEnum]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Evaluate User's Progressions (adminEvaluateProgress)
+    """List User's Rewards (adminGetUserRewards)
 
-    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+    * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Required Permission(s):
-        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+        - ADMIN:NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Properties:
-        url: /challenge/v1/admin/namespaces/{namespace}/progress/evaluate
+        url: /challenge/v1/admin/namespaces/{namespace}/users/{userId}/rewards
 
-        method: POST
+        method: GET
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
-        consumes: ["application/json"]
+        consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        body: (body) REQUIRED ModelEvaluatePlayerProgressionRequest in body
-
         namespace: (namespace) REQUIRED str in path
 
+        user_id: (userId) REQUIRED str in path
+
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
+
     Responses:
-        204: No Content - (No Content)
+        200: OK - ModelListUserRewardsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - ResponseError (20029: not found)
-
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = AdminEvaluateProgress.create(
-        body=body,
+    request = AdminGetUserRewards.create(
+        user_id=user_id,
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(EvaluateMyProgress)
-def evaluate_my_progress(
+@same_doc_as(PublicClaimUserRewards)
+def public_claim_user_rewards(
+    body: ModelClaimUserRewardsReq,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Evaluate User's Challenge Progressions (EvaluateMyProgress)
+    """Claim User's Rewards (publicClaimUserRewards)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim
 
         method: POST
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelClaimUserRewardsReq in body
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (No Content)
+        200: OK - List[ModelUserReward] (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - IamErrorResponse (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = EvaluateMyProgress.create(
+    request = PublicClaimUserRewards.create(
+        body=body,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(EvaluateMyProgress)
-async def evaluate_my_progress_async(
+@same_doc_as(PublicClaimUserRewards)
+async def public_claim_user_rewards_async(
+    body: ModelClaimUserRewardsReq,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """Evaluate User's Challenge Progressions (EvaluateMyProgress)
+    """Claim User's Rewards (publicClaimUserRewards)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [UPDATE]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [UPDATE]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/evaluate
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards/claim
 
         method: POST
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
-        consumes: []
+        consumes: ["application/json"]
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
+        body: (body) REQUIRED ModelClaimUserRewardsReq in body
+
         namespace: (namespace) REQUIRED str in path
 
     Responses:
-        204: No Content - (No Content)
+        200: OK - List[ModelUserReward] (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
+        404: Not Found - IamErrorResponse (20029: not found)
+
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = EvaluateMyProgress.create(
+    request = PublicClaimUserRewards.create(
+        body=body,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
 
 
-@same_doc_as(PublicGetUserProgression)
-def public_get_user_progression(
-    challenge_code: str,
-    goal_code: Optional[str] = None,
+@same_doc_as(PublicGetUserRewards)
+def public_get_user_rewards(
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, PublicGetUserRewardsStatusEnum]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List User's Progressions (publicGetUserProgression)
+    """List User's Rewards (publicGetUserRewards)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards
 
         method: GET
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        challenge_code: (challengeCode) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
-        goal_code: (goalCode) OPTIONAL str in query
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
 
     Responses:
-        200: OK - ModelUserProgressionResponse (OK)
+        200: OK - ModelListUserRewardsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - IamErrorResponse (20029: not found)
-
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = PublicGetUserProgression.create(
-        challenge_code=challenge_code,
-        goal_code=goal_code,
+    request = PublicGetUserRewards.create(
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
         namespace=namespace,
     )
     return run_request(request, additional_headers=x_additional_headers, **kwargs)
 
 
-@same_doc_as(PublicGetUserProgression)
-async def public_get_user_progression_async(
-    challenge_code: str,
-    goal_code: Optional[str] = None,
+@same_doc_as(PublicGetUserRewards)
+async def public_get_user_rewards_async(
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    sort_by: Optional[str] = None,
+    status: Optional[Union[str, PublicGetUserRewardsStatusEnum]] = None,
     namespace: Optional[str] = None,
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
-    """List User's Progressions (publicGetUserProgression)
+    """List User's Rewards (publicGetUserRewards)
 
-    * Required permission: NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+    * Required permission: NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Required Permission(s):
-        - NAMESPACE:{namespace}:CHALLENGE:PROGRESSION [READ]
+        - NAMESPACE:{namespace}:CHALLENGE:REWARD [READ]
 
     Properties:
-        url: /challenge/v1/public/namespaces/{namespace}/users/me/progress/{challengeCode}
+        url: /challenge/v1/public/namespaces/{namespace}/users/me/rewards
 
         method: GET
 
-        tags: ["Challenge Progression"]
+        tags: ["Player Reward"]
 
         consumes: []
 
         produces: ["application/json"]
 
         securities: [BEARER_AUTH]
 
-        challenge_code: (challengeCode) REQUIRED str in path
-
         namespace: (namespace) REQUIRED str in path
 
-        goal_code: (goalCode) OPTIONAL str in query
+        limit: (limit) OPTIONAL int in query
+
+        offset: (offset) OPTIONAL int in query
+
+        sort_by: (sortBy) OPTIONAL str in query
+
+        status: (status) OPTIONAL Union[str, StatusEnum] in query
 
     Responses:
-        200: OK - ModelUserProgressionResponse (OK)
+        200: OK - ModelListUserRewardsResponse (OK)
 
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
-        404: Not Found - IamErrorResponse (20029: not found)
-
         500: Internal Server Error - ResponseError (20000: internal server error: {{message}})
     """
     if namespace is None:
         namespace, error = get_services_namespace()
         if error:
             return None, error
-    request = PublicGetUserProgression.create(
-        challenge_code=challenge_code,
-        goal_code=goal_code,
+    request = PublicGetUserRewards.create(
+        limit=limit,
+        offset=offset,
+        sort_by=sort_by,
+        status=status,
         namespace=namespace,
     )
     return await run_request_async(
         request, additional_headers=x_additional_headers, **kwargs
     )
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk/api/challenge/wrappers/_goal_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         * code: unique within a challenge
         * name: name of the goal
         * description: text describing the goal (optional)
         * schedule: a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
         * requirementGroups: list of conditions that conform with the goal progressions.
         * rewards: list of rewards that will be claimable once a goal is complete
         * tag: goal's labels
+        * isActive: when goal is in a schedule, isActive determine whether goal is active to progress or not
     Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
 
     Properties:
         url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals
@@ -86,14 +87,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelGoalResponse (Created)
 
+        400: Bad Request - IamErrorResponse (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         404: Not Found - ResponseError (20029: not found)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
@@ -128,14 +131,15 @@
         * code: unique within a challenge
         * name: name of the goal
         * description: text describing the goal (optional)
         * schedule: a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
         * requirementGroups: list of conditions that conform with the goal progressions.
         * rewards: list of rewards that will be claimable once a goal is complete
         * tag: goal's labels
+        * isActive: when goal is in a schedule, isActive determine whether goal is active to progress or not
     Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
 
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [CREATE]
 
     Properties:
         url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals
@@ -155,14 +159,16 @@
         challenge_code: (challengeCode) REQUIRED str in path
 
         namespace: (namespace) REQUIRED str in path
 
     Responses:
         201: Created - ModelGoalResponse (Created)
 
+        400: Bad Request - IamErrorResponse (20018: bad request: {{message}})
+
         401: Unauthorized - IamErrorResponse (20001: unauthorized access)
 
         403: Forbidden - IamErrorResponse (20013: insufficient permission)
 
         404: Not Found - ResponseError (20029: not found)
 
         409: Conflict - ResponseError (99002: duplicate key error: {{message}})
@@ -552,14 +558,24 @@
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Goal (adminUpdateGoals)
 
     * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
 
+    Request body:
+        * name: name of the goal
+        * description: text describing the goal (optional)
+        * schedule (optional): a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
+        * requirementGroups: list of conditions that conform with the goal progressions.
+        * rewards: list of rewards that will be claimable once a goal is complete
+        * tag: goal's labels
+        * isActive (optional): when goal is in a schedule, isActive determine whether goal is active to progress or not
+    Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
+
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
 
     Properties:
         url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
 
         method: PUT
@@ -609,14 +625,24 @@
     x_additional_headers: Optional[Dict[str, str]] = None,
     **kwargs
 ):
     """Update Goal (adminUpdateGoals)
 
     * Required permission: ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
 
+    Request body:
+        * name: name of the goal
+        * description: text describing the goal (optional)
+        * schedule (optional): a time range that indicated the availability of a goal within a timeframe. used in fixed assignment rule
+        * requirementGroups: list of conditions that conform with the goal progressions.
+        * rewards: list of rewards that will be claimable once a goal is complete
+        * tag: goal's labels
+        * isActive (optional): when goal is in a schedule, isActive determine whether goal is active to progress or not
+    Goal describe set of requirements that need to be fulfilled by players in order to complete it and describe what is the rewards given to player when they complete the goal.The requirement will have target value and a operator that will evaluate that against an observable playerâs attribute (e.g. statistic, entitlement). Goal belongs to a challenge.
+
     Required Permission(s):
         - ADMIN:NAMESPACE:{namespace}:CHALLENGE [UPDATE]
 
     Properties:
         url: /challenge/v1/admin/namespaces/{namespace}/challenges/{challengeCode}/goals/{code}
 
         method: PUT
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelbyte-py-sdk-service-challenge
-Version: 0.2.0
+Version: 0.3.0
 Summary: AccelByte Python SDK - AccelByte Gaming Services Challenge Service
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: accelbyte-py-sdk-core
 
 [//]: # (Code generated. DO NOT EDIT!)
```

### Comparing `accelbyte-py-sdk-service-challenge-0.2.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt` & `accelbyte_py_sdk_service_challenge-0.3.0/accelbyte_py_sdk_service_challenge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 accelbyte_py_sdk/api/challenge/models/iam_error_response.py
 accelbyte_py_sdk/api/challenge/models/model_challenge_response.py
 accelbyte_py_sdk/api/challenge/models/model_claim_user_rewards_req.py
 accelbyte_py_sdk/api/challenge/models/model_create_challenge_request.py
 accelbyte_py_sdk/api/challenge/models/model_create_goal_request.py
 accelbyte_py_sdk/api/challenge/models/model_evaluate_player_progression_request.py
 accelbyte_py_sdk/api/challenge/models/model_get_goals_response.py
+accelbyte_py_sdk/api/challenge/models/model_goal_meta.py
 accelbyte_py_sdk/api/challenge/models/model_goal_order.py
 accelbyte_py_sdk/api/challenge/models/model_goal_progression_response.py
 accelbyte_py_sdk/api/challenge/models/model_goal_response.py
 accelbyte_py_sdk/api/challenge/models/model_goal_schedule.py
 accelbyte_py_sdk/api/challenge/models/model_list_challenge_response.py
 accelbyte_py_sdk/api/challenge/models/model_list_periods_response.py
 accelbyte_py_sdk/api/challenge/models/model_list_user_rewards_response.py
```

